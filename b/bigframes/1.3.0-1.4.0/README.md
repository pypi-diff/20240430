# Comparing `tmp/bigframes-1.3.0.tar.gz` & `tmp/bigframes-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigframes-1.3.0.tar", last modified: Mon Apr 22 23:20:04 2024, max compression
+gzip compressed data, was "bigframes-1.4.0.tar", last modified: Tue Apr 30 00:15:00 2024, max compression
```

## Comparing `bigframes-1.3.0.tar` & `bigframes-1.4.0.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.639690 bigframes-1.3.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-22 23:17:27.000000 bigframes-1.3.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      914 2024-04-22 23:17:27.000000 bigframes-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4650 2024-04-22 23:20:04.639690 bigframes-1.3.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2256 2024-04-22 23:17:27.000000 bigframes-1.3.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.563684 bigframes-1.3.0/bigframes/
--rw-rw-r--   0 root         (0)     1003     1111 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.563684 bigframes-1.3.0/bigframes/_config/
--rw-rw-r--   0 root         (0)     1003     2453 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     8953 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/bigquery_options.py
--rw-rw-r--   0 root         (0)     1003     2141 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/compute_options.py
--rw-rw-r--   0 root         (0)     1003     1661 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/display_options.py
--rw-rw-r--   0 root         (0)     1003     1892 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/sampling_options.py
--rw-rw-r--   0 root         (0)     1003     7152 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/clients.py
--rw-rw-r--   0 root         (0)     1003     2709 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/constants.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/
--rw-rw-r--   0 root         (0)     1003    18183 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/__init__.py
--rw-rw-r--   0 root         (0)     1003    30768 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/block_transforms.py
--rw-rw-r--   0 root         (0)     1003    91562 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/blocks.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/compile/
--rw-rw-r--   0 root         (0)     1003      832 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/__init__.py
--rw-rw-r--   0 root         (0)     1003    17475 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/aggregate_compiler.py
--rw-rw-r--   0 root         (0)     1003    51565 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/compiled.py
--rw-rw-r--   0 root         (0)     1003     6341 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/compiler.py
--rw-rw-r--   0 root         (0)     1003     3356 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/concat.py
--rw-rw-r--   0 root         (0)     1003    48952 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/scalar_op_compiler.py
--rw-rw-r--   0 root         (0)     1003     7121 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/single_column.py
--rw-rw-r--   0 root         (0)     1003     2369 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/convert.py
--rw-rw-r--   0 root         (0)     1003     2495 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/eval.py
--rw-rw-r--   0 root         (0)     1003     6685 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/expression.py
--rw-rw-r--   0 root         (0)     1003     1846 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/global_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/groupby/
--rw-rw-r--   0 root         (0)     1003    23982 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/groupby/__init__.py
--rw-rw-r--   0 root         (0)     1003      716 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/guid.py
--rw-rw-r--   0 root         (0)     1003    18056 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/indexes/
--rw-rw-r--   0 root         (0)     1003      719 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003    16223 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     1720 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexes/multi.py
--rw-rw-r--   0 root         (0)     1003     1730 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/join_def.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/joins/
--rw-rw-r--   0 root         (0)     1003      691 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/joins/__init__.py
--rw-rw-r--   0 root         (0)     1003     2132 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/joins/merge.py
--rw-rw-r--   0 root         (0)     1003     2218 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/local_data.py
--rw-rw-r--   0 root         (0)     1003     2255 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/log_adapter.py
--rw-rw-r--   0 root         (0)     1003    18515 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/nodes.py
--rw-rw-r--   0 root         (0)     1003     9392 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/ordering.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/reshape/
--rw-rw-r--   0 root         (0)     1003     6872 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003    10722 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/rewrite.py
--rw-rw-r--   0 root         (0)     1003      746 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/scalar.py
--rw-rw-r--   0 root         (0)     1003     2144 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/schema.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/tools/
--rw-rw-r--   0 root         (0)     1003      664 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2515 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/tools/datetimes.py
--rw-rw-r--   0 root         (0)     1003     3002 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/tree_properties.py
--rw-rw-r--   0 root         (0)     1003     5483 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/window/
--rw-rw-r--   0 root         (0)     1003     3075 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1286 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/window_spec.py
--rw-rw-r--   0 root         (0)     1003   131677 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/dataframe.py
--rw-rw-r--   0 root         (0)     1003    27474 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/dtypes.py
--rw-rw-r--   0 root         (0)     1003      666 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/exceptions.py
--rw-rw-r--   0 root         (0)     1003     1273 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/features.py
--rw-rw-r--   0 root         (0)     1003    11179 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/formatting_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/functions/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/functions/__init__.py
--rw-rw-r--   0 root         (0)     1003    40641 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/functions/remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.579686 bigframes-1.3.0/bigframes/ml/
--rw-rw-r--   0 root         (0)     1003      877 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     8542 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/base.py
--rw-rw-r--   0 root         (0)     1003     6659 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/cluster.py
--rw-rw-r--   0 root         (0)     1003     7984 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/compose.py
--rw-rw-r--   0 root         (0)     1003    17608 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/core.py
--rw-rw-r--   0 root         (0)     1003     6807 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/decomposition.py
--rw-rw-r--   0 root         (0)     1003    24746 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/ensemble.py
--rw-rw-r--   0 root         (0)     1003    15998 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/forecasting.py
--rw-rw-r--   0 root         (0)     1003     1141 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/globals.py
--rw-rw-r--   0 root         (0)     1003    10844 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/imported.py
--rw-rw-r--   0 root         (0)     1003    13818 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/linear_model.py
--rw-rw-r--   0 root         (0)     1003    29649 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/llm.py
--rw-rw-r--   0 root         (0)     1003     4899 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/loader.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.579686 bigframes-1.3.0/bigframes/ml/metrics/
--rw-rw-r--   0 root         (0)     1003     1066 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/metrics/__init__.py
--rw-rw-r--   0 root         (0)     1003    11096 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/metrics/_metrics.py
--rw-rw-r--   0 root         (0)     1003     2373 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     3748 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/model_selection.py
--rw-rw-r--   0 root         (0)     1003     5067 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/pipeline.py
--rw-rw-r--   0 root         (0)     1003    22667 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/preprocessing.py
--rw-rw-r--   0 root         (0)     1003     5754 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/remote.py
--rw-rw-r--   0 root         (0)     1003    13949 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/sql.py
--rw-rw-r--   0 root         (0)     1003     2403 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/operations/
--rw-rw-r--   0 root         (0)     1003    23377 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/operations/_matplotlib/
--rw-rw-r--   0 root         (0)     1003     1022 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/_matplotlib/__init__.py
--rw-rw-r--   0 root         (0)     1003     4477 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/_matplotlib/core.py
--rw-rw-r--   0 root         (0)     1003     5970 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/_matplotlib/hist.py
--rw-rw-r--   0 root         (0)     1003    13202 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/aggregations.py
--rw-rw-r--   0 root         (0)     1003     8273 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/base.py
--rw-rw-r--   0 root         (0)     1003     3079 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/datetimes.py
--rw-rw-r--   0 root         (0)     1003     2814 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/plotting.py
--rw-rw-r--   0 root         (0)     1003     9009 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/strings.py
--rw-rw-r--   0 root         (0)     1003     2089 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/structs.py
--rw-rw-r--   0 root         (0)     1003     7613 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/type.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/pandas/
--rw-rw-r--   0 root         (0)     1003    23314 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/pandas/__init__.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/py.typed
--rw-rw-r--   0 root         (0)     1003    64553 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/session/
--rw-rw-r--   0 root         (0)     1003    82333 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/session/_io/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/_io/__init__.py
--rw-rw-r--   0 root         (0)     1003     9139 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/_io/bigquery.py
--rw-rw-r--   0 root         (0)     1003     4345 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/_io/pandas.py
--rw-rw-r--   0 root         (0)     1003     8043 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/clients.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/typing.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.635690 bigframes-1.3.0/bigframes.egg-info/
--rw-r--r--   0 root         (0)     1003     4650 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    12307 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      732 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       29 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       81 2024-04-22 23:17:27.000000 bigframes-1.3.0/pyproject.toml
--rw-rw-r--   0 root         (0)     1003       67 2024-04-22 23:20:04.639690 bigframes-1.3.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     4428 2024-04-22 23:17:27.000000 bigframes-1.3.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.587686 bigframes-1.3.0/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.587686 bigframes-1.3.0/tests/data/
--rw-rw-r--   0 root         (0)     1003      619 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/hockey_players.json
--rw-rw-r--   0 root         (0)     1003     1250 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/hockey_players.jsonl
--rw-rw-r--   0 root         (0)     1003      340 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_2by3.json
--rw-rw-r--   0 root         (0)     1003       80 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_2by3.jsonl
--rw-rw-r--   0 root         (0)     1003      421 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_3by4.json
--rw-rw-r--   0 root         (0)     1003      154 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_3by4.jsonl
--rw-rw-r--   0 root         (0)     1003    33350 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/nested.jsonl
--rw-rw-r--   0 root         (0)     1003      966 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/nested_schema.json
--rw-rw-r--   0 root         (0)     1003    58869 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/penguins.jsonl
--rw-rw-r--   0 root         (0)     1003      636 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/penguins_schema.json
--rw-rw-r--   0 root         (0)     1003     3909 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/scalars.jsonl
--rw-rw-r--   0 root         (0)     1003     1458 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/scalars_schema.json
--rw-rw-r--   0 root         (0)     1003    23424 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/time_series.jsonl
--rw-rw-r--   0 root         (0)     1003      192 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/time_series_schema.json
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.591686 bigframes-1.3.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003    37000 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.591686 bigframes-1.3.0/tests/system/large/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.591686 bigframes-1.3.0/tests/system/large/ml/
--rw-rw-r--   0 root         (0)     1003     5411 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003     5391 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     6401 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6487 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    14451 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     4366 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     8408 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    30362 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003     4079 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/test_location.py
--rw-rw-r--   0 root         (0)     1003    50275 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003     1908 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/test_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.595687 bigframes-1.3.0/tests/system/load/
--rw-rw-r--   0 root         (0)     1003     2664 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/load/test_large_tables.py
--rw-rw-r--   0 root         (0)     1003     2970 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/load/test_llm.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.599687 bigframes-1.3.0/tests/system/small/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.603687 bigframes-1.3.0/tests/system/small/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003    11773 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/conftest.py
--rw-rw-r--   0 root         (0)     1003     7074 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003    13810 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6764 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    17015 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     6859 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     4983 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_imported.py
--rw-rw-r--   0 root         (0)     1003     8788 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    11541 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_llm.py
--rw-rw-r--   0 root         (0)     1003    25138 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_metrics.py
--rw-rw-r--   0 root         (0)     1003     2224 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_metrics_pairwise.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_model_selection.py
--rw-rw-r--   0 root         (0)     1003    27150 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_preprocessing.py
--rw-rw-r--   0 root         (0)     1003     2570 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_register.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_remote.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.603687 bigframes-1.3.0/tests/system/small/operations/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003    10399 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/test_datetimes.py
--rw-rw-r--   0 root         (0)     1003    12453 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/test_plotting.py
--rw-rw-r--   0 root         (0)     1003    15770 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/test_strings.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.603687 bigframes-1.3.0/tests/system/small/regression/
--rw-rw-r--   0 root         (0)     1003     1999 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/regression/test_issue355_merge_after_filter.py
--rw-rw-r--   0 root         (0)     1003   140298 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003    18961 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_dataframe_io.py
--rw-rw-r--   0 root         (0)     1003    10570 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_encryption.py
--rw-rw-r--   0 root         (0)     1003    13974 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_groupby.py
--rw-rw-r--   0 root         (0)     1003     1558 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_ibis.py
--rw-rw-r--   0 root         (0)     1003    13328 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_index.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_ipython.py
--rw-rw-r--   0 root         (0)     1003    41010 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_multiindex.py
--rw-rw-r--   0 root         (0)     1003     4190 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_numpy.py
--rw-rw-r--   0 root         (0)     1003    19608 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     9533 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_pandas_options.py
--rw-rw-r--   0 root         (0)     1003     4126 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_progress_bar.py
--rw-rw-r--   0 root         (0)     1003    26485 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003      913 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_scalar.py
--rw-rw-r--   0 root         (0)     1003   108974 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_series.py
--rw-rw-r--   0 root         (0)     1003    40386 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_session.py
--rw-rw-r--   0 root         (0)     1003     3343 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_window.py
--rw-rw-r--   0 root         (0)     1003    12113 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.607688 bigframes-1.3.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.607688 bigframes-1.3.0/tests/unit/_config/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     4218 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/_config/test_bigquery_options.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.607688 bigframes-1.3.0/tests/unit/core/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/__init__.py
--rw-rw-r--   0 root         (0)     1003     1619 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_bf_utils.py
--rw-rw-r--   0 root         (0)     1003     2966 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_blocks.py
--rw-rw-r--   0 root         (0)     1003     1553 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_expression.py
--rw-rw-r--   0 root         (0)     1003     1813 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_log_adapter.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/tests/unit/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     2323 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_api_primitives.py
--rw-rw-r--   0 root         (0)     1003     6555 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     7426 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_golden_sql.py
--rw-rw-r--   0 root         (0)     1003     4058 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003    13789 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_sql.py
--rw-rw-r--   0 root         (0)     1003     4931 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/tests/unit/session/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/__init__.py
--rw-rw-r--   0 root         (0)     1003     4347 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_clients.py
--rw-rw-r--   0 root         (0)     1003     7809 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_io_bigquery.py
--rw-rw-r--   0 root         (0)     1003    18664 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_io_pandas.py
--rw-rw-r--   0 root         (0)     1003     8099 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_session.py
--rw-rw-r--   0 root         (0)     1003     1744 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_clients.py
--rw-rw-r--   0 root         (0)     1003     1056 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_compute_options.py
--rw-rw-r--   0 root         (0)     1003     6648 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_core.py
--rw-rw-r--   0 root         (0)     1003     2136 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003     8819 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_dtypes.py
--rw-rw-r--   0 root         (0)     1003     1577 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_features.py
--rw-rw-r--   0 root         (0)     1003      528 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_formatting_helper.py
--rw-rw-r--   0 root         (0)     1003     1655 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_formatting_helpers.py
--rw-rw-r--   0 root         (0)     1003     4055 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     1207 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.551684 bigframes-1.3.0/third_party/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/cpython/
--rw-rw-r--   0 root         (0)     1003     2339 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/cpython/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/cpython/__init__.py
--rw-rw-r--   0 root         (0)     1003    18854 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/cpython/_pprint.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     5290 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003    14045 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/LICENSE.txt
--rw-rw-r--   0 root         (0)     1003    11663 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/
--rw-rw-r--   0 root         (0)     1003      184 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     2091 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
--rw-rw-r--   0 root         (0)     1003     6600 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
--rw-rw-r--   0 root         (0)     1003     1892 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/
--rw-rw-r--   0 root         (0)     1003      464 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003      536 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
--rw-rw-r--   0 root         (0)     1003      276 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
--rw-rw-r--   0 root         (0)     1003      263 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
--rw-rw-r--   0 root         (0)     1003      690 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/
--rw-rw-r--   0 root         (0)     1003     2284 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/AUTHORS.md
--rw-rw-r--   0 root         (0)     1003     1634 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/LICENSE
--rw-rw-r--   0 root         (0)     1003    10620 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/_config/
--rw-rw-r--   0 root         (0)     1003     1347 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/_config/config.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
--rw-rw-r--   0 root         (0)     1003     3831 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
--rw-rw-r--   0 root         (0)     1003     3689 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
--rw-rw-r--   0 root         (0)     1003     2086 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/common.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/
--rw-rw-r--   0 root         (0)     1003     6944 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/align.py
--rw-rw-r--   0 root         (0)     1003     1543 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/common.py
--rw-rw-r--   0 root         (0)     1003     2295 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
--rw-rw-r--   0 root         (0)     1003    12685 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
--rw-rw-r--   0 root         (0)     1003    25132 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
--rw-rw-r--   0 root         (0)     1003    16244 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
--rw-rw-r--   0 root         (0)     1003     6477 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
--rw-rw-r--   0 root         (0)     1003    10303 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
--rw-rw-r--   0 root         (0)     1003     4394 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/config_init.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/dtypes/
--rw-rw-r--   0 root         (0)     1003      707 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
--rw-rw-r--   0 root         (0)     1003   225813 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/frame.py
--rw-rw-r--   0 root         (0)     1003    40215 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/generic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/groupby/
--rw-rw-r--   0 root         (0)     1003    14023 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003     9589 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
--rw-rw-r--   0 root         (0)     1003    11461 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     2941 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
--rw-rw-r--   0 root         (0)     1003     2909 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003     4372 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
--rw-rw-r--   0 root         (0)     1003     3804 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
--rw-rw-r--   0 root         (0)     1003     3220 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
--rw-rw-r--   0 root         (0)     1003     5844 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
--rw-rw-r--   0 root         (0)     1003   131185 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/strings/
--rw-rw-r--   0 root         (0)     1003    37771 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2964 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1350 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/__init__.py
--rw-rw-r--   0 root         (0)     1003     1269 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/common.py
--rw-rw-r--   0 root         (0)     1003     7071 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/gbq.py
--rw-rw-r--   0 root         (0)     1003     1428 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parquet.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
--rw-rw-r--   0 root         (0)     1003    10553 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
--rw-rw-r--   0 root         (0)     1003     3130 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/pickle.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/pandas/
--rw-rw-r--   0 root         (0)     1003    12353 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/plotting/
--rw-rw-r--   0 root         (0)     1003    11348 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/plotting/_core.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/
--rw-rw-r--   0 root         (0)     1003      765 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
--rw-rw-r--   0 root         (0)     1003     1573 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_validators.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/
--rw-rw-r--   0 root         (0)     1003     1532 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/COPYING
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/__init__.py
--rw-rw-r--   0 root         (0)     1003     6212 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/base.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/cluster/
--rw-rw-r--   0 root         (0)     1003     5924 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/compose/
--rw-rw-r--   0 root         (0)     1003     2014 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/decomposition/
--rw-rw-r--   0 root         (0)     1003     5387 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
--rw-rw-r--   0 root         (0)     1003     8979 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/
--rw-rw-r--   0 root         (0)     1003     5417 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
--rw-rw-r--   0 root         (0)     1003     4348 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/
--rw-rw-r--   0 root         (0)     1003     9783 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
--rw-rw-r--   0 root         (0)     1003     6347 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
--rw-rw-r--   0 root         (0)     1003     3550 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
--rw-rw-r--   0 root         (0)     1003     2121 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     2980 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/pipeline.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.635690 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/
--rw-rw-r--   0 root         (0)     1003     4980 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
--rw-rw-r--   0 root         (0)     1003     1523 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
--rw-rw-r--   0 root         (0)     1003     4064 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
--rw-rw-r--   0 root         (0)     1003     2085 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.635690 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/
--rw-rw-r--   0 root         (0)     1003    11348 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/__init__.py
--rw-rw-r--   0 root         (0)     1003     6921 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/sklearn.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.395885 bigframes-1.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-30 00:12:25.000000 bigframes-1.4.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      914 2024-04-30 00:12:25.000000 bigframes-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4785 2024-04-30 00:15:00.395885 bigframes-1.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2391 2024-04-30 00:12:25.000000 bigframes-1.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.315864 bigframes-1.4.0/bigframes/
+-rw-rw-r--   0 root         (0)     1003     1111 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.319865 bigframes-1.4.0/bigframes/_config/
+-rw-rw-r--   0 root         (0)     1003     2453 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8953 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/bigquery_options.py
+-rw-rw-r--   0 root         (0)     1003     2141 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/compute_options.py
+-rw-rw-r--   0 root         (0)     1003     1661 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/display_options.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/sampling_options.py
+-rw-rw-r--   0 root         (0)     1003     7152 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/clients.py
+-rw-rw-r--   0 root         (0)     1003     2709 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/constants.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.323866 bigframes-1.4.0/bigframes/core/
+-rw-rw-r--   0 root         (0)     1003    17931 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30768 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/block_transforms.py
+-rw-rw-r--   0 root         (0)     1003    95393 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/blocks.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/compile/
+-rw-rw-r--   0 root         (0)     1003      832 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17475 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/aggregate_compiler.py
+-rw-rw-r--   0 root         (0)     1003    52133 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/compiled.py
+-rw-rw-r--   0 root         (0)     1003     6341 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/compiler.py
+-rw-rw-r--   0 root         (0)     1003     3356 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/concat.py
+-rw-rw-r--   0 root         (0)     1003    48955 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/scalar_op_compiler.py
+-rw-rw-r--   0 root         (0)     1003     7121 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/single_column.py
+-rw-rw-r--   0 root         (0)     1003     2962 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/convert.py
+-rw-rw-r--   0 root         (0)     1003     2495 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/eval.py
+-rw-rw-r--   0 root         (0)     1003     6685 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/expression.py
+-rw-rw-r--   0 root         (0)     1003     1846 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/global_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    23982 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/groupby/__init__.py
+-rw-rw-r--   0 root         (0)     1003      716 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/guid.py
+-rw-rw-r--   0 root         (0)     1003    18056 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/indexes/
+-rw-rw-r--   0 root         (0)     1003      719 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16223 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     1720 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     1730 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/join_def.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/joins/
+-rw-rw-r--   0 root         (0)     1003      691 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/joins/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2132 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/joins/merge.py
+-rw-rw-r--   0 root         (0)     1003     2218 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/local_data.py
+-rw-rw-r--   0 root         (0)     1003     2255 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/log_adapter.py
+-rw-rw-r--   0 root         (0)     1003    18515 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/nodes.py
+-rw-rw-r--   0 root         (0)     1003     9445 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/ordering.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/reshape/
+-rw-rw-r--   0 root         (0)     1003     6872 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11714 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/rewrite.py
+-rw-rw-r--   0 root         (0)     1003      746 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/scalar.py
+-rw-rw-r--   0 root         (0)     1003     2144 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/schema.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/tools/
+-rw-rw-r--   0 root         (0)     1003      664 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2515 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/tools/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     3002 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/tree_properties.py
+-rw-rw-r--   0 root         (0)     1003     5483 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/window/
+-rw-rw-r--   0 root         (0)     1003     3075 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1286 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/window_spec.py
+-rw-rw-r--   0 root         (0)     1003   132040 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/dataframe.py
+-rw-rw-r--   0 root         (0)     1003    27597 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/dtypes.py
+-rw-rw-r--   0 root         (0)     1003      666 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1273 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/features.py
+-rw-rw-r--   0 root         (0)     1003    11179 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/formatting_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/functions/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/functions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42108 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/functions/remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/ml/
+-rw-rw-r--   0 root         (0)     1003      877 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8542 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/base.py
+-rw-rw-r--   0 root         (0)     1003     6659 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/cluster.py
+-rw-rw-r--   0 root         (0)     1003     7984 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/compose.py
+-rw-rw-r--   0 root         (0)     1003    17724 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/core.py
+-rw-rw-r--   0 root         (0)     1003     6807 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/decomposition.py
+-rw-rw-r--   0 root         (0)     1003    24746 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/ensemble.py
+-rw-rw-r--   0 root         (0)     1003    15998 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/forecasting.py
+-rw-rw-r--   0 root         (0)     1003     1141 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/globals.py
+-rw-rw-r--   0 root         (0)     1003    10844 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/imported.py
+-rw-rw-r--   0 root         (0)     1003    13818 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/linear_model.py
+-rw-rw-r--   0 root         (0)     1003    32246 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/llm.py
+-rw-rw-r--   0 root         (0)     1003     4899 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/loader.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/ml/metrics/
+-rw-rw-r--   0 root         (0)     1003     1066 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/metrics/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11096 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/metrics/_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2373 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     3748 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/model_selection.py
+-rw-rw-r--   0 root         (0)     1003     5067 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/pipeline.py
+-rw-rw-r--   0 root         (0)     1003    22667 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     5773 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/remote.py
+-rw-rw-r--   0 root         (0)     1003    14405 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/sql.py
+-rw-rw-r--   0 root         (0)     1003     2403 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/operations/
+-rw-rw-r--   0 root         (0)     1003    23377 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/operations/_matplotlib/
+-rw-rw-r--   0 root         (0)     1003     1022 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/_matplotlib/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4477 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/_matplotlib/core.py
+-rw-rw-r--   0 root         (0)     1003     5970 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/_matplotlib/hist.py
+-rw-rw-r--   0 root         (0)     1003    13202 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/aggregations.py
+-rw-rw-r--   0 root         (0)     1003     9321 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/base.py
+-rw-rw-r--   0 root         (0)     1003     3079 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     2814 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/plotting.py
+-rw-rw-r--   0 root         (0)     1003     9009 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/strings.py
+-rw-rw-r--   0 root         (0)     1003     2089 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/structs.py
+-rw-rw-r--   0 root         (0)     1003     7613 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/type.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/bigframes/pandas/
+-rw-rw-r--   0 root         (0)     1003    23435 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/pandas/__init__.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/py.typed
+-rw-rw-r--   0 root         (0)     1003    64464 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/bigframes/session/
+-rw-rw-r--   0 root         (0)     1003    83061 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/bigframes/session/_io/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/_io/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11305 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/_io/bigquery.py
+-rw-rw-r--   0 root         (0)     1003     4345 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/_io/pandas.py
+-rw-rw-r--   0 root         (0)     1003     8043 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/clients.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/typing.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.391884 bigframes-1.4.0/bigframes.egg-info/
+-rw-r--r--   0 root         (0)     1003     4785 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    12307 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      732 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       29 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       81 2024-04-30 00:12:25.000000 bigframes-1.4.0/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003       67 2024-04-30 00:15:00.395885 bigframes-1.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     4428 2024-04-30 00:12:25.000000 bigframes-1.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.343871 bigframes-1.4.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003      619 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/hockey_players.json
+-rw-rw-r--   0 root         (0)     1003     1250 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/hockey_players.jsonl
+-rw-rw-r--   0 root         (0)     1003      340 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_2by3.json
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_2by3.jsonl
+-rw-rw-r--   0 root         (0)     1003      421 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_3by4.json
+-rw-rw-r--   0 root         (0)     1003      154 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_3by4.jsonl
+-rw-rw-r--   0 root         (0)     1003    33350 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/nested.jsonl
+-rw-rw-r--   0 root         (0)     1003      966 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/nested_schema.json
+-rw-rw-r--   0 root         (0)     1003    58869 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/penguins.jsonl
+-rw-rw-r--   0 root         (0)     1003      636 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/penguins_schema.json
+-rw-rw-r--   0 root         (0)     1003     3909 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/scalars.jsonl
+-rw-rw-r--   0 root         (0)     1003     1458 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/scalars_schema.json
+-rw-rw-r--   0 root         (0)     1003    23424 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/time_series.jsonl
+-rw-rw-r--   0 root         (0)     1003      192 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/time_series_schema.json
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.343871 bigframes-1.4.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37000 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.343871 bigframes-1.4.0/tests/system/large/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.347872 bigframes-1.4.0/tests/system/large/ml/
+-rw-rw-r--   0 root         (0)     1003     5411 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003     5391 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     6401 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6487 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    14451 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     4366 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     8408 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    30362 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003     4079 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/test_location.py
+-rw-rw-r--   0 root         (0)     1003    52808 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003     1908 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/test_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.347872 bigframes-1.4.0/tests/system/load/
+-rw-rw-r--   0 root         (0)     1003     3000 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/load/test_large_tables.py
+-rw-rw-r--   0 root         (0)     1003     4559 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/load/test_llm.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.351873 bigframes-1.4.0/tests/system/small/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.355874 bigframes-1.4.0/tests/system/small/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11773 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/conftest.py
+-rw-rw-r--   0 root         (0)     1003     7074 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003    13810 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6764 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    17015 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     6859 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     4983 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_imported.py
+-rw-rw-r--   0 root         (0)     1003     8788 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    11541 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_llm.py
+-rw-rw-r--   0 root         (0)     1003    25138 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2224 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_metrics_pairwise.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_model_selection.py
+-rw-rw-r--   0 root         (0)     1003    27150 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     2570 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_register.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_remote.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/system/small/operations/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10399 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/test_datetimes.py
+-rw-rw-r--   0 root         (0)     1003    12453 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/test_plotting.py
+-rw-rw-r--   0 root         (0)     1003    15770 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/test_strings.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/system/small/regression/
+-rw-rw-r--   0 root         (0)     1003     1999 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/regression/test_issue355_merge_after_filter.py
+-rw-rw-r--   0 root         (0)     1003   145083 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003    18961 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_dataframe_io.py
+-rw-rw-r--   0 root         (0)     1003    10570 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_encryption.py
+-rw-rw-r--   0 root         (0)     1003    13974 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_groupby.py
+-rw-rw-r--   0 root         (0)     1003     1558 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_ibis.py
+-rw-rw-r--   0 root         (0)     1003    13328 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_index.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_ipython.py
+-rw-rw-r--   0 root         (0)     1003    41010 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_multiindex.py
+-rw-rw-r--   0 root         (0)     1003     4190 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_numpy.py
+-rw-rw-r--   0 root         (0)     1003    19608 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     9533 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_pandas_options.py
+-rw-rw-r--   0 root         (0)     1003     4126 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_progress_bar.py
+-rw-rw-r--   0 root         (0)     1003    26485 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003      913 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_scalar.py
+-rw-rw-r--   0 root         (0)     1003   111197 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_series.py
+-rw-rw-r--   0 root         (0)     1003    40386 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_session.py
+-rw-rw-r--   0 root         (0)     1003     3343 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_window.py
+-rw-rw-r--   0 root         (0)     1003    12113 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/unit/_config/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4218 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/_config/test_bigquery_options.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.363877 bigframes-1.4.0/tests/unit/core/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1619 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_bf_utils.py
+-rw-rw-r--   0 root         (0)     1003     2966 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_blocks.py
+-rw-rw-r--   0 root         (0)     1003     1553 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_expression.py
+-rw-rw-r--   0 root         (0)     1003     1813 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_log_adapter.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.363877 bigframes-1.4.0/tests/unit/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2323 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_api_primitives.py
+-rw-rw-r--   0 root         (0)     1003     6555 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     7422 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_golden_sql.py
+-rw-rw-r--   0 root         (0)     1003     4058 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003    14241 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_sql.py
+-rw-rw-r--   0 root         (0)     1003     5298 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.363877 bigframes-1.4.0/tests/unit/session/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4347 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     7809 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_io_bigquery.py
+-rw-rw-r--   0 root         (0)     1003    18664 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_io_pandas.py
+-rw-rw-r--   0 root         (0)     1003     8702 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_session.py
+-rw-rw-r--   0 root         (0)     1003     1744 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     1056 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_compute_options.py
+-rw-rw-r--   0 root         (0)     1003     6648 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_core.py
+-rw-rw-r--   0 root         (0)     1003     2136 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003     8819 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_dtypes.py
+-rw-rw-r--   0 root         (0)     1003     1577 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_features.py
+-rw-rw-r--   0 root         (0)     1003      528 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_formatting_helper.py
+-rw-rw-r--   0 root         (0)     1003     1655 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_formatting_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4055 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     1207 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.303861 bigframes-1.4.0/third_party/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/cpython/
+-rw-rw-r--   0 root         (0)     1003     2339 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/cpython/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/cpython/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18854 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/cpython/_pprint.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5290 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14045 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/ibis/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/LICENSE.txt
+-rw-rw-r--   0 root         (0)     1003    11663 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/
+-rw-rw-r--   0 root         (0)     1003      184 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2091 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
+-rw-rw-r--   0 root         (0)     1003     6600 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/
+-rw-rw-r--   0 root         (0)     1003      464 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      536 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
+-rw-rw-r--   0 root         (0)     1003      276 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
+-rw-rw-r--   0 root         (0)     1003      263 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
+-rw-rw-r--   0 root         (0)     1003      690 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/pandas/
+-rw-rw-r--   0 root         (0)     1003     2284 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/AUTHORS.md
+-rw-rw-r--   0 root         (0)     1003     1634 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/LICENSE
+-rw-rw-r--   0 root         (0)     1003    10620 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/pandas/_config/
+-rw-rw-r--   0 root         (0)     1003     1347 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/_config/config.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.375880 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.375880 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.375880 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3831 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
+-rw-rw-r--   0 root         (0)     1003     3689 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
+-rw-rw-r--   0 root         (0)     1003     2086 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/common.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/
+-rw-rw-r--   0 root         (0)     1003     6944 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/align.py
+-rw-rw-r--   0 root         (0)     1003     1543 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/common.py
+-rw-rw-r--   0 root         (0)     1003     2295 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
+-rw-rw-r--   0 root         (0)     1003    12685 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
+-rw-rw-r--   0 root         (0)     1003    25132 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
+-rw-rw-r--   0 root         (0)     1003    16244 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
+-rw-rw-r--   0 root         (0)     1003     6477 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
+-rw-rw-r--   0 root         (0)     1003    10303 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
+-rw-rw-r--   0 root         (0)     1003     4394 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/config_init.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/dtypes/
+-rw-rw-r--   0 root         (0)     1003      707 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
+-rw-rw-r--   0 root         (0)     1003   228180 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/frame.py
+-rw-rw-r--   0 root         (0)     1003    40215 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/generic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    14023 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9589 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
+-rw-rw-r--   0 root         (0)     1003    11461 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     2941 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     2909 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4372 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
+-rw-rw-r--   0 root         (0)     1003     3804 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
+-rw-rw-r--   0 root         (0)     1003     3220 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
+-rw-rw-r--   0 root         (0)     1003     5844 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
+-rw-rw-r--   0 root         (0)     1003   131177 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/strings/
+-rw-rw-r--   0 root         (0)     1003    37771 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2964 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1350 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1269 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/common.py
+-rw-rw-r--   0 root         (0)     1003     7071 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/gbq.py
+-rw-rw-r--   0 root         (0)     1003     1428 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parquet.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10553 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
+-rw-rw-r--   0 root         (0)     1003     3130 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/pickle.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/pandas/
+-rw-rw-r--   0 root         (0)     1003    12353 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/plotting/
+-rw-rw-r--   0 root         (0)     1003    11348 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/plotting/_core.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/
+-rw-rw-r--   0 root         (0)     1003      765 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1573 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_validators.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/
+-rw-rw-r--   0 root         (0)     1003     1532 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/COPYING
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6212 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/base.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/cluster/
+-rw-rw-r--   0 root         (0)     1003     5924 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/compose/
+-rw-rw-r--   0 root         (0)     1003     2014 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/decomposition/
+-rw-rw-r--   0 root         (0)     1003     5387 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8977 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/
+-rw-rw-r--   0 root         (0)     1003     5417 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
+-rw-rw-r--   0 root         (0)     1003     4348 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/
+-rw-rw-r--   0 root         (0)     1003     9783 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
+-rw-rw-r--   0 root         (0)     1003     6347 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
+-rw-rw-r--   0 root         (0)     1003     3550 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
+-rw-rw-r--   0 root         (0)     1003     2124 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     2977 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/pipeline.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.391884 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/
+-rw-rw-r--   0 root         (0)     1003     4980 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
+-rw-rw-r--   0 root         (0)     1003     1523 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
+-rw-rw-r--   0 root         (0)     1003     4059 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
+-rw-rw-r--   0 root         (0)     1003     2085 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.391884 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/
+-rw-rw-r--   0 root         (0)     1003    11348 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6919 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/sklearn.py
```

### Comparing `bigframes-1.3.0/LICENSE` & `bigframes-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/MANIFEST.in` & `bigframes-1.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/PKG-INFO` & `bigframes-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.3.0
+Version: 1.4.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -82,14 +82,15 @@
 
 Documentation
 -------------
 
 * `BigQuery DataFrames source code (GitHub) <https://github.com/googleapis/python-bigquery-dataframes>`_
 * `BigQuery DataFrames sample notebooks <https://github.com/googleapis/python-bigquery-dataframes/tree/main/notebooks>`_
 * `BigQuery DataFrames API reference <https://cloud.google.com/python/docs/reference/bigframes/latest/summary_overview>`_
+* `BigQuery DataFrames supported pandas APIs <https://cloud.google.com/python/docs/reference/bigframes/latest/supported_pandas_apis>`_
 
 
 Getting started with BigQuery DataFrames
 ----------------------------------------
 Try the `BigQuery DataFrames quickstart <https://cloud.google.com/bigquery/docs/dataframes-quickstart>`_
 to get up and running in just a few minutes.
```

### Comparing `bigframes-1.3.0/README.rst` & `bigframes-1.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 Documentation
 -------------
 
 * `BigQuery DataFrames source code (GitHub) <https://github.com/googleapis/python-bigquery-dataframes>`_
 * `BigQuery DataFrames sample notebooks <https://github.com/googleapis/python-bigquery-dataframes/tree/main/notebooks>`_
 * `BigQuery DataFrames API reference <https://cloud.google.com/python/docs/reference/bigframes/latest/summary_overview>`_
+* `BigQuery DataFrames supported pandas APIs <https://cloud.google.com/python/docs/reference/bigframes/latest/supported_pandas_apis>`_
 
 
 Getting started with BigQuery DataFrames
 ----------------------------------------
 Try the `BigQuery DataFrames quickstart <https://cloud.google.com/bigquery/docs/dataframes-quickstart>`_
 to get up and running in just a few minutes.
```

### Comparing `bigframes-1.3.0/bigframes/__init__.py` & `bigframes-1.4.0/bigframes/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/_config/__init__.py` & `bigframes-1.4.0/bigframes/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/_config/bigquery_options.py` & `bigframes-1.4.0/bigframes/_config/bigquery_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/_config/compute_options.py` & `bigframes-1.4.0/bigframes/_config/compute_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/_config/display_options.py` & `bigframes-1.4.0/bigframes/_config/display_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/_config/sampling_options.py` & `bigframes-1.4.0/bigframes/_config/sampling_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/clients.py` & `bigframes-1.4.0/bigframes/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/constants.py` & `bigframes-1.4.0/bigframes/constants.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/__init__.py` & `bigframes-1.4.0/bigframes/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,26 +113,14 @@
         compiled = self._compile_unordered()
         items = tuple(
             schemata.SchemaItem(id, compiled.get_column_type(id))
             for id in compiled.column_ids
         )
         return schemata.ArraySchema(items)
 
-    def validate_schema(self):
-        tree_derived = self.node.schema
-        ibis_derived = self._compiled_schema
-        if tree_derived.names != ibis_derived.names:
-            raise ValueError(
-                f"Unexpected names internal {tree_derived.names} vs compiled {ibis_derived.names}"
-            )
-        if tree_derived.dtypes != ibis_derived.dtypes:
-            raise ValueError(
-                f"Unexpected types internal {tree_derived.dtypes} vs compiled {ibis_derived.dtypes}"
-            )
-
     def _try_evaluate_local(self):
         """Use only for unit testing paths - not fully featured. Will throw exception if fails."""
         import ibis
 
         return ibis.pandas.connect({}).execute(
             self._compile_ordered()._to_ibis_expr(ordering_mode="unordered")
         )
@@ -191,15 +179,15 @@
             )
             exprs = [*self_projection, (expression, output_id)]
         return ArrayValue(
             nodes.ProjectionNode(
                 child=self.node,
                 assignments=tuple(exprs),
             )
-        )
+        ).merge_projections()
 
     def assign(self, source_id: str, destination_id: str) -> ArrayValue:
         if destination_id in self.column_ids:  # Mutate case
             exprs = [
                 (
                     (
                         ex.free_var(source_id)
@@ -216,15 +204,15 @@
             )
             exprs = [*self_projection, (ex.free_var(source_id), destination_id)]
         return ArrayValue(
             nodes.ProjectionNode(
                 child=self.node,
                 assignments=tuple(exprs),
             )
-        )
+        ).merge_projections()
 
     def assign_constant(
         self,
         destination_id: str,
         value: typing.Any,
         dtype: typing.Optional[bigframes.dtypes.Dtype],
     ) -> ArrayValue:
@@ -250,37 +238,37 @@
             )
             exprs = [*self_projection, (ex.const(value, dtype), destination_id)]
         return ArrayValue(
             nodes.ProjectionNode(
                 child=self.node,
                 assignments=tuple(exprs),
             )
-        )
+        ).merge_projections()
 
     def select_columns(self, column_ids: typing.Sequence[str]) -> ArrayValue:
         selections = ((ex.free_var(col_id), col_id) for col_id in column_ids)
         return ArrayValue(
             nodes.ProjectionNode(
                 child=self.node,
                 assignments=tuple(selections),
             )
-        )
+        ).merge_projections()
 
     def drop_columns(self, columns: Iterable[str]) -> ArrayValue:
         new_projection = (
             (ex.free_var(col_id), col_id)
             for col_id in self.column_ids
             if col_id not in columns
         )
         return ArrayValue(
             nodes.ProjectionNode(
                 child=self.node,
                 assignments=tuple(new_projection),
             )
-        )
+        ).merge_projections()
 
     def aggregate(
         self,
         aggregations: typing.Sequence[typing.Tuple[ex.Aggregation, str]],
         by_column_ids: typing.Sequence[str] = (),
         dropna: bool = True,
     ) -> ArrayValue:
@@ -474,7 +462,11 @@
     def _uniform_sampling(self, fraction: float) -> ArrayValue:
         """Sampling the table on given fraction.
 
         .. warning::
             The row numbers of result is non-deterministic, avoid to use.
         """
         return ArrayValue(nodes.RandomSampleNode(self.node, fraction))
+
+    def merge_projections(self) -> ArrayValue:
+        new_node = bigframes.core.rewrite.maybe_squash_projection(self.node)
+        return ArrayValue(new_node)
```

### Comparing `bigframes-1.3.0/bigframes/core/block_transforms.py` & `bigframes-1.4.0/bigframes/core/block_transforms.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/blocks.py` & `bigframes-1.4.0/bigframes/core/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 
 import dataclasses
 import functools
 import itertools
 import os
 import random
 import typing
-from typing import Iterable, List, Literal, Mapping, Optional, Sequence, Tuple
+from typing import Iterable, List, Literal, Mapping, Optional, Sequence, Tuple, Union
 import warnings
 
 import google.cloud.bigquery as bigquery
 import pandas as pd
 import pyarrow as pa
 
 import bigframes._config.sampling_options as sampling_options
+import bigframes.constants
 import bigframes.constants as constants
 import bigframes.core as core
 import bigframes.core.expression as ex
 import bigframes.core.expression as scalars
 import bigframes.core.guid as guid
 import bigframes.core.join_def as join_defs
 import bigframes.core.ordering as ordering
@@ -100,14 +101,16 @@
 
     def __init__(
         self,
         expr: core.ArrayValue,
         index_columns: Iterable[str],
         column_labels: typing.Union[pd.Index, typing.Iterable[Label]],
         index_labels: typing.Union[pd.Index, typing.Iterable[Label], None] = None,
+        *,
+        transpose_cache: Optional[Block] = None,
     ):
         """Construct a block object, will create default index if no index columns specified."""
         index_columns = list(index_columns)
         if index_labels is not None:
             index_labels = list(index_labels)
             if len(index_labels) != len(index_columns):
                 raise ValueError(
@@ -139,14 +142,15 @@
         # TODO: Preserve cache under safe transforms (eg. drop column, reorder)
         self._stats_cache: dict[str, dict[str, typing.Any]] = {
             col_id: {} for col_id in self.value_columns
         }
         # TODO(kemppeterson) Add a cache for corr to parallel the single-column stats.
 
         self._stats_cache[" ".join(self.index_columns)] = {}
+        self._transpose_cache: Optional[Block] = transpose_cache
 
     @classmethod
     def from_local(cls, data: pd.DataFrame, session: bigframes.Session) -> Block:
         # Assumes caller has already converted datatypes to bigframes ones.
         pd_data = data
         column_labels = pd_data.columns
         index_labels = list(pd_data.index.names)
@@ -509,17 +513,22 @@
         df.columns = self.column_labels
 
     def _materialize_local(
         self, materialize_options: MaterializationOptions = MaterializationOptions()
     ) -> Tuple[pd.DataFrame, bigquery.QueryJob]:
         """Run query and download results as a pandas DataFrame. Return the total number of results as well."""
         # TODO(swast): Allow for dry run and timeout.
-        results_iterator, query_job = self.session._execute(
-            self.expr, sorted=materialize_options.ordered
+        _, query_job = self.session._query_to_destination(
+            self.session._to_sql(self.expr, sorted=True),
+            list(self.index_columns),
+            api_name="cached",
+            do_clustering=False,
         )
+        results_iterator = query_job.result()
+
         table_size = (
             self.session._get_table_size(query_job.destination) / _BYTES_TO_MEGABYTES
         )
         sample_config = materialize_options.downsampling
         max_download_size = sample_config.max_download_size
         fraction = (
             max_download_size / table_size
@@ -711,14 +720,23 @@
         return Block(
             self._expr,
             index_columns=self.index_columns,
             column_labels=label_list,
             index_labels=self.index.names,
         )
 
+    def with_transpose_cache(self, transposed: Block):
+        return Block(
+            self._expr,
+            index_columns=self.index_columns,
+            column_labels=self._column_labels,
+            index_labels=self.index.names,
+            transpose_cache=transposed,
+        )
+
     def with_index_labels(self, value: typing.Sequence[Label]) -> Block:
         if len(value) != len(self.index_columns):
             raise ValueError(
                 f"The index labels size `{len(value)} ` should equal to the index "
                 + f"columns size: {len(self.index_columns)}."
             )
         return Block(
@@ -799,26 +817,43 @@
             )
             result_ids.append(result_id)
         return block, result_ids
 
     def multi_apply_unary_op(
         self,
         columns: typing.Sequence[str],
-        op: ops.UnaryOp,
+        op: Union[ops.UnaryOp, ex.Expression],
     ) -> Block:
+        if isinstance(op, ops.UnaryOp):
+            input_varname = guid.generate_guid()
+            expr = op.as_expr(input_varname)
+        else:
+            input_varnames = op.unbound_variables
+            assert len(input_varnames) == 1
+            expr = op
+            input_varname = input_varnames[0]
+
         block = self
-        for i, col_id in enumerate(columns):
+        for col_id in columns:
             label = self.col_id_to_label[col_id]
-            block, result_id = block.apply_unary_op(
-                col_id,
-                op,
-                result_label=label,
+            block, result_id = block.project_expr(
+                expr.bind_all_variables({input_varname: ex.free_var(col_id)}),
+                label=label,
             )
             block = block.copy_values(result_id, col_id)
             block = block.drop_columns([result_id])
+        # Special case, we can preserve transpose cache for full-frame unary ops
+        if (self._transpose_cache is not None) and set(self.value_columns) == set(
+            columns
+        ):
+            transpose_columns = self._transpose_cache.value_columns
+            new_transpose_cache = self._transpose_cache.multi_apply_unary_op(
+                transpose_columns, op
+            )
+            block = block.with_transpose_cache(new_transpose_cache)
         return block
 
     def apply_window_op(
         self,
         column: str,
         op: agg_ops.WindowOp,
         window_spec: core.WindowSpec,
@@ -917,28 +952,25 @@
     ) -> Block:
         axis_n = utils.get_axis_number(axis)
         if axis_n == 0:
             aggregations = [
                 (ex.UnaryAggregation(operation, ex.free_var(col_id)), col_id)
                 for col_id in self.value_columns
             ]
-            index_col_ids = [
-                guid.generate_guid() for i in range(self.column_labels.nlevels)
-            ]
-            result_expr = self.expr.aggregate(aggregations, dropna=dropna).unpivot(
-                row_labels=self.column_labels.to_list(),
-                index_col_ids=index_col_ids,
-                unpivot_columns=tuple([(value_col_id, tuple(self.value_columns))]),
-            )
+            index_id = guid.generate_guid()
+            result_expr = self.expr.aggregate(
+                aggregations, dropna=dropna
+            ).assign_constant(index_id, None, None)
+            # Transpose as last operation so that final block has valid transpose cache
             return Block(
                 result_expr,
-                index_columns=index_col_ids,
-                column_labels=[None],
-                index_labels=self.column_labels.names,
-            )
+                index_columns=[index_id],
+                column_labels=self.column_labels,
+                index_labels=[None],
+            ).transpose(original_row_index=pd.Index([None]))
         else:  # axis_n == 1
             # using offsets as identity to group on.
             # TODO: Allow to promote identity/total_order columns instead for better perf
             offset_col = guid.generate_guid()
             expr_with_offsets = self.expr.promote_offsets(offset_col)
             stacked_expr = expr_with_offsets.unpivot(
                 row_labels=self.column_labels.to_list(),
@@ -1538,14 +1570,18 @@
     def melt(
         self,
         id_vars=typing.Sequence[str],
         value_vars=typing.Sequence[str],
         var_names=typing.Sequence[typing.Hashable],
         value_name: typing.Hashable = "value",
     ):
+        """
+        Unpivot columns to produce longer, narrower dataframe.
+        Arguments correspond to pandas.melt arguments.
+        """
         # TODO: Implement col_level and ignore_index
         unpivot_col_id = guid.generate_guid()
         var_col_ids = tuple([guid.generate_guid() for _ in var_names])
         # single unpivot col
         unpivot_col = (unpivot_col_id, tuple(value_vars))
         value_labels = [self.col_id_to_label[col_id] for col_id in value_vars]
         id_labels = [self.col_id_to_label[col_id] for col_id in id_vars]
@@ -1566,14 +1602,70 @@
 
         return Block(
             unpivot_expr,
             column_labels=[*id_labels, *var_names, value_name],
             index_columns=[index_id],
         )
 
+    def transpose(self, *, original_row_index: Optional[pd.Index] = None) -> Block:
+        """Transpose the block. Will fail if dtypes aren't coercible to a common type or too many rows.
+        Can provide the original_row_index directly if it is already known, otherwise a query is needed.
+        """
+        if self._transpose_cache is not None:
+            return self._transpose_cache.with_transpose_cache(self)
+
+        original_col_index = self.column_labels
+        original_row_index = (
+            original_row_index
+            if original_row_index is not None
+            else self.index.to_pandas()
+        )
+        original_row_count = len(original_row_index)
+        if original_row_count > bigframes.constants.MAX_COLUMNS:
+            raise NotImplementedError(
+                f"Object has {original_row_count} rows and is too large to transpose."
+            )
+
+        # Add row numbers to both axes to disambiguate, clean them up later
+        block = self
+        numbered_block = block.with_column_labels(
+            utils.combine_indices(
+                block.column_labels, pd.Index(range(len(block.column_labels)))
+            )
+        )
+        numbered_block, offsets = numbered_block.promote_offsets()
+
+        stacked_block = numbered_block.melt(
+            id_vars=(offsets,),
+            var_names=(
+                *[name for name in original_col_index.names],
+                "col_offset",
+            ),
+            value_vars=block.value_columns,
+        )
+        col_labels = stacked_block.value_columns[-2 - original_col_index.nlevels : -2]
+        col_offset = stacked_block.value_columns[-2]  # disambiguator we created earlier
+        cell_values = stacked_block.value_columns[-1]
+        # Groupby source column
+        stacked_block = stacked_block.set_index(
+            [*col_labels, col_offset]
+        )  # col index is now row index
+        result = stacked_block.pivot(
+            columns=[offsets],
+            values=[cell_values],
+            columns_unique_values=tuple(range(original_row_count)),
+        )
+        # Drop the offsets from both axes before returning
+        return (
+            result.with_column_labels(original_row_index)
+            .order_by([ordering.ascending_over(result.index_columns[-1])])
+            .drop_levels([result.index_columns[-1]])
+            .with_transpose_cache(self)
+        )
+
     def _create_stack_column(
         self, col_label: typing.Tuple, stack_labels: typing.Sequence[typing.Tuple]
     ):
         dtype = None
         input_columns: list[Optional[str]] = []
         for uvalue in stack_labels:
             label_to_match = (*col_label, *uvalue)
```

### Comparing `bigframes-1.3.0/bigframes/core/compile/__init__.py` & `bigframes-1.4.0/bigframes/core/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/compile/aggregate_compiler.py` & `bigframes-1.4.0/bigframes/core/compile/aggregate_compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/compile/compiled.py` & `bigframes-1.4.0/bigframes/core/compile/compiled.py`

 * *Files 1% similar despite different names*

```diff
@@ -819,25 +819,22 @@
                 )
             )
             output_columns = [
                 col_id_overrides.get(col) if (col in col_id_overrides) else col
                 for col in baked_ir.column_ids
             ]
             selection = ", ".join(map(lambda col_id: f"`{col_id}`", output_columns))
-            order_by_clause = baked_ir._ordering_clause(
-                baked_ir._ordering.all_ordering_columns
-            )
 
-            sql = textwrap.dedent(
-                f"SELECT {selection}\n"
-                "FROM (\n"
-                f"{sql}\n"
-                ")\n"
-                f"{order_by_clause}\n"
-            )
+            sql = textwrap.dedent(f"SELECT {selection}\n" "FROM (\n" f"{sql}\n" ")\n")
+            # Single row frames may not have any ordering columns
+            if len(baked_ir._ordering.all_ordering_columns) > 0:
+                order_by_clause = baked_ir._ordering_clause(
+                    baked_ir._ordering.all_ordering_columns
+                )
+                sql += f"{order_by_clause}\n"
         else:
             sql = ibis_bigquery.Backend().compile(
                 self._to_ibis_expr(
                     ordering_mode="unordered",
                     col_id_overrides=col_id_overrides,
                     expose_hidden_cols=False,
                 )
@@ -1049,35 +1046,45 @@
         ]
         expr_builder.ordering = self._ordering.with_column_remap({column_id: new_name})
         return expr_builder.build()
 
     def _bake_ordering(self) -> OrderedIR:
         """Bakes ordering expression into the selection, maybe creating hidden columns."""
         ordering_expressions = self._ordering.all_ordering_columns
-        new_exprs = []
-        new_baked_cols = []
+        new_exprs: list[OrderingExpression] = []
+        new_baked_cols: list[ibis_types.Value] = []
         for expr in ordering_expressions:
             if isinstance(expr.scalar_expression, ex.OpExpression):
                 baked_column = self._compile_expression(expr.scalar_expression).name(
                     bigframes.core.guid.generate_guid()
                 )
                 new_baked_cols.append(baked_column)
                 new_expr = OrderingExpression(
-                    ex.free_var(baked_column.name), expr.direction, expr.na_last
+                    ex.free_var(baked_column.get_name()), expr.direction, expr.na_last
                 )
                 new_exprs.append(new_expr)
-            else:
+            elif isinstance(expr.scalar_expression, ex.UnboundVariableExpression):
+                order_col = expr.scalar_expression.id
                 new_exprs.append(expr)
-
-        ordering = self._ordering.with_ordering_columns(new_exprs)
+                if order_col not in self.column_ids:
+                    new_baked_cols.append(
+                        self._ibis_bindings[expr.scalar_expression.id]
+                    )
+
+        new_ordering = ExpressionOrdering(
+            tuple(new_exprs),
+            self._ordering.integer_encoding,
+            self._ordering.string_encoding,
+            self._ordering.total_ordering_columns,
+        )
         return OrderedIR(
             self._table,
             columns=self.columns,
-            hidden_ordering_columns=[*self._hidden_ordering_columns, *new_baked_cols],
-            ordering=ordering,
+            hidden_ordering_columns=tuple(new_baked_cols),
+            ordering=new_ordering,
             predicates=self._predicates,
         )
 
     def _project_offsets(self) -> OrderedIR:
         """Create a new expression that contains offsets. Should only be executed when offsets are needed for an operations. Has no effect on expression semantics."""
         if self._ordering.is_sequential:
             return self
```

### Comparing `bigframes-1.3.0/bigframes/core/compile/compiler.py` & `bigframes-1.4.0/bigframes/core/compile/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/compile/concat.py` & `bigframes-1.4.0/bigframes/core/compile/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/compile/scalar_op_compiler.py` & `bigframes-1.4.0/bigframes/core/compile/scalar_op_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1362,15 +1362,15 @@
             .when(upper.isnull() | (original > upper), upper)
             .else_(original)
             .end()
         )
 
 
 @scalar_op_compiler.register_nary_op(ops.case_when_op)
-def switch_op(*cases_and_outputs: ibis_types.Value) -> ibis_types.Value:
+def case_when_op(*cases_and_outputs: ibis_types.Value) -> ibis_types.Value:
     # ibis can handle most type coercions, but we need to force bool -> int
     # TODO: dispatch coercion depending on bigframes dtype schema
     result_values = cases_and_outputs[1::2]
     do_upcast_bool = any(t.type().is_numeric() for t in result_values)
     if do_upcast_bool:
         # Just need to upcast to int, ibis can handle further coercion
         result_values = tuple(
```

### Comparing `bigframes-1.3.0/bigframes/core/compile/single_column.py` & `bigframes-1.4.0/bigframes/core/compile/single_column.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/convert.py` & `bigframes-1.4.0/bigframes/core/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,30 @@
 
 import pandas as pd
 
 import bigframes.core.indexes as index
 import bigframes.series as series
 
 
-def to_bf_series(obj, default_index: Optional[index.Index]) -> series.Series:
+def is_series_convertible(obj) -> bool:
+    if isinstance(obj, series.Series):
+        return True
+    if isinstance(obj, pd.Series):
+        return True
+    if isinstance(obj, index.Index):
+        return True
+    if isinstance(obj, pd.Index):
+        return True
+    if pd.api.types.is_list_like(obj):
+        return True
+    else:
+        return False
+
+
+def to_bf_series(obj, default_index: Optional[index.Index], session) -> series.Series:
     """
     Convert a an object to a bigframes series
 
     Args:
         obj (list-like or Series):
             Object to convert to bigframes Series
         default_index (list-like or Index or None):
@@ -33,21 +48,23 @@
 
     Returns
         bigframes.pandas.Series
     """
     if isinstance(obj, series.Series):
         return obj
     if isinstance(obj, pd.Series):
-        return series.Series(obj)
+        return series.Series(obj, session=session)
     if isinstance(obj, index.Index):
-        return series.Series(obj, default_index)
+        return series.Series(obj, default_index, session=session)
     if isinstance(obj, pd.Index):
-        return series.Series(obj, default_index)
+        return series.Series(obj, default_index, session=session)
+    if pd.api.types.is_dict_like(obj):
+        return series.Series(obj, session=session)
     if pd.api.types.is_list_like(obj):
-        return series.Series(obj, default_index)
+        return series.Series(obj, default_index, session=session)
     else:
         raise TypeError(f"Cannot interpret {obj} as series.")
 
 
 def to_pd_series(obj, default_index: pd.Index) -> pd.Series:
     """
     Convert a an object to a pandas series
@@ -65,11 +82,13 @@
         return obj.to_pandas()
     if isinstance(obj, pd.Series):
         return obj
     if isinstance(obj, index.Index):
         return pd.Series(obj.to_pandas(), default_index)
     if isinstance(obj, pd.Index):
         return pd.Series(obj, default_index)
+    if pd.api.types.is_dict_like(obj):
+        return pd.Series(obj)
     if pd.api.types.is_list_like(obj):
         return pd.Series(obj, default_index)
     else:
         raise TypeError(f"Cannot interpret {obj} as series.")
```

### Comparing `bigframes-1.3.0/bigframes/core/eval.py` & `bigframes-1.4.0/bigframes/core/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/expression.py` & `bigframes-1.4.0/bigframes/core/expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/global_session.py` & `bigframes-1.4.0/bigframes/core/global_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/groupby/__init__.py` & `bigframes-1.4.0/bigframes/core/groupby/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/guid.py` & `bigframes-1.4.0/bigframes/core/guid.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/indexers.py` & `bigframes-1.4.0/bigframes/core/indexers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/indexes/__init__.py` & `bigframes-1.4.0/bigframes/core/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/indexes/base.py` & `bigframes-1.4.0/bigframes/core/indexes/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/indexes/multi.py` & `bigframes-1.4.0/bigframes/core/indexes/multi.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/join_def.py` & `bigframes-1.4.0/bigframes/core/join_def.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/joins/__init__.py` & `bigframes-1.4.0/bigframes/core/joins/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/joins/merge.py` & `bigframes-1.4.0/bigframes/core/joins/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/local_data.py` & `bigframes-1.4.0/bigframes/core/local_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/log_adapter.py` & `bigframes-1.4.0/bigframes/core/log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/nodes.py` & `bigframes-1.4.0/bigframes/core/nodes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/ordering.py` & `bigframes-1.4.0/bigframes/core/ordering.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,16 @@
             expr = order_part.scalar_expression
             if not set(expr.unbound_variables).issubset(columns_seen):
                 if expr.is_bijective:
                     columns_seen.update(expr.unbound_variables)
                 truncated_refs.append(order_part)
                 if columns_seen.issuperset(must_see):
                     return tuple(truncated_refs)
+        if len(must_see) == 0:
+            return ()
         raise ValueError("Ordering did not contain all total_order_cols")
 
     def with_reverse(self):
         """Reverses the ordering."""
         return ExpressionOrdering(
             tuple([col.with_reverse() for col in self.ordering_value_columns]),
             total_ordering_columns=self.total_ordering_columns,
```

### Comparing `bigframes-1.3.0/bigframes/core/reshape/__init__.py` & `bigframes-1.4.0/bigframes/core/reshape/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/rewrite.py` & `bigframes-1.4.0/bigframes/core/rewrite.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,24 +31,29 @@
 class SquashedSelect:
     """Squash together as many nodes as possible, separating out the projection, filter and reordering expressions."""
 
     root: nodes.BigFrameNode
     columns: Tuple[Tuple[scalar_exprs.Expression, str], ...]
     predicate: Optional[scalar_exprs.Expression]
     ordering: Tuple[order.OrderingExpression, ...]
+    reverse_root: bool = False
 
     @classmethod
-    def from_node(cls, node: nodes.BigFrameNode) -> SquashedSelect:
+    def from_node(
+        cls, node: nodes.BigFrameNode, projections_only: bool = False
+    ) -> SquashedSelect:
         if isinstance(node, nodes.ProjectionNode):
-            return cls.from_node(node.child).project(node.assignments)
-        elif isinstance(node, nodes.FilterNode):
+            return cls.from_node(node.child, projections_only=projections_only).project(
+                node.assignments
+            )
+        elif not projections_only and isinstance(node, nodes.FilterNode):
             return cls.from_node(node.child).filter(node.predicate)
-        elif isinstance(node, nodes.ReversedNode):
+        elif not projections_only and isinstance(node, nodes.ReversedNode):
             return cls.from_node(node.child).reverse()
-        elif isinstance(node, nodes.OrderByNode):
+        elif not projections_only and isinstance(node, nodes.OrderByNode):
             return cls.from_node(node.child).order_with(node.by)
         else:
             selection = tuple(
                 (scalar_exprs.UnboundVariableExpression(id), id)
                 for id in get_node_column_ids(node)
             )
             return cls(node, selection, None, ())
@@ -59,35 +64,43 @@
 
     def project(
         self, projection: Tuple[Tuple[scalar_exprs.Expression, str], ...]
     ) -> SquashedSelect:
         new_columns = tuple(
             (expr.bind_all_variables(self.column_lookup), id) for expr, id in projection
         )
-        return SquashedSelect(self.root, new_columns, self.predicate, self.ordering)
+        return SquashedSelect(
+            self.root, new_columns, self.predicate, self.ordering, self.reverse_root
+        )
 
     def filter(self, predicate: scalar_exprs.Expression) -> SquashedSelect:
         if self.predicate is None:
             new_predicate = predicate.bind_all_variables(self.column_lookup)
         else:
             new_predicate = ops.and_op.as_expr(
                 self.predicate, predicate.bind_all_variables(self.column_lookup)
             )
-        return SquashedSelect(self.root, self.columns, new_predicate, self.ordering)
+        return SquashedSelect(
+            self.root, self.columns, new_predicate, self.ordering, self.reverse_root
+        )
 
     def reverse(self) -> SquashedSelect:
         new_ordering = tuple(expr.with_reverse() for expr in self.ordering)
-        return SquashedSelect(self.root, self.columns, self.predicate, new_ordering)
+        return SquashedSelect(
+            self.root, self.columns, self.predicate, new_ordering, not self.reverse_root
+        )
 
     def order_with(self, by: Tuple[order.OrderingExpression, ...]):
         adjusted_orderings = [
             order_part.bind_variables(self.column_lookup) for order_part in by
         ]
         new_ordering = (*adjusted_orderings, *self.ordering)
-        return SquashedSelect(self.root, self.columns, self.predicate, new_ordering)
+        return SquashedSelect(
+            self.root, self.columns, self.predicate, new_ordering, self.reverse_root
+        )
 
     def maybe_join(
         self, right: SquashedSelect, join_def: join_defs.JoinDefinition
     ) -> Optional[SquashedSelect]:
         if join_def.type == "cross":
             # Cannot convert cross join to projection
             return None
@@ -122,16 +135,18 @@
         if lmask is not None:
             lselection = tuple((apply_mask(expr, lmask), id) for expr, id in lselection)
         if rmask is not None:
             rselection = tuple((apply_mask(expr, rmask), id) for expr, id in rselection)
         new_columns = remap_names(join_def, lselection, rselection)
 
         # Reconstruct ordering
+        reverse_root = self.reverse_root
         if join_type == "right":
             new_ordering = right.ordering
+            reverse_root = right.reverse_root
         elif join_type == "outer":
             if lmask is not None:
                 prefix = order.OrderingExpression(lmask, order.OrderingDirection.DESC)
                 left_ordering = tuple(
                     order.OrderingExpression(
                         apply_mask(ref.scalar_expression, lmask),
                         ref.direction,
@@ -154,26 +169,39 @@
                 new_ordering = (prefix, *left_ordering, *right_ordering)
             else:
                 new_ordering = self.ordering
         elif join_type in {"inner", "left"}:
             new_ordering = self.ordering
         else:
             raise ValueError(f"Unexpected join type {join_type}")
-        return SquashedSelect(self.root, new_columns, new_predicate, new_ordering)
+        return SquashedSelect(
+            self.root, new_columns, new_predicate, new_ordering, reverse_root
+        )
 
     def expand(self) -> nodes.BigFrameNode:
         # Safest to apply predicates first, as it may filter out inputs that cannot be handled by other expressions
         root = self.root
+        if self.reverse_root:
+            root = nodes.ReversedNode(child=root)
         if self.predicate:
             root = nodes.FilterNode(child=root, predicate=self.predicate)
         if self.ordering:
             root = nodes.OrderByNode(child=root, by=self.ordering)
         return nodes.ProjectionNode(child=root, assignments=self.columns)
 
 
+def maybe_squash_projection(node: nodes.BigFrameNode) -> nodes.BigFrameNode:
+    if isinstance(node, nodes.ProjectionNode) and isinstance(
+        node.child, nodes.ProjectionNode
+    ):
+        # Conservative approach, only squash consecutive projections, even though could also squash filters, reorderings
+        return SquashedSelect.from_node(node, projections_only=True).expand()
+    return node
+
+
 def maybe_rewrite_join(join_node: nodes.JoinNode) -> nodes.BigFrameNode:
     left_side = SquashedSelect.from_node(join_node.left_child)
     right_side = SquashedSelect.from_node(join_node.right_child)
     joined = left_side.maybe_join(right_side, join_node.join)
     if joined is not None:
         return joined.expand()
     else:
```

### Comparing `bigframes-1.3.0/bigframes/core/scalar.py` & `bigframes-1.4.0/bigframes/core/scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/schema.py` & `bigframes-1.4.0/bigframes/core/schema.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/tools/__init__.py` & `bigframes-1.4.0/bigframes/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/tools/datetimes.py` & `bigframes-1.4.0/bigframes/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/tree_properties.py` & `bigframes-1.4.0/bigframes/core/tree_properties.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/utils.py` & `bigframes-1.4.0/bigframes/core/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/window/__init__.py` & `bigframes-1.4.0/bigframes/core/window/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/core/window_spec.py` & `bigframes-1.4.0/bigframes/core/window_spec.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/dataframe.py` & `bigframes-1.4.0/bigframes/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,17 @@
         *,
         session: typing.Optional[bigframes.session.Session] = None,
     ):
         if copy is not None and not copy:
             raise ValueError(
                 f"DataFrame constructor only supports copy=True. {constants.FEEDBACK_LINK}"
             )
+        # just ignore object dtype if provided
+        if dtype in {numpy.dtypes.ObjectDType, "object"}:
+            dtype = None
 
         # Check to see if constructing from BigQuery-backed objects before
         # falling back to pandas constructor
         block = None
         if isinstance(data, blocks.Block):
             block = data
 
@@ -307,14 +310,21 @@
         """BigQuery REST API Client the DataFrame uses for operations."""
         return self._session.bqclient
 
     @property
     def _session(self) -> bigframes.Session:
         return self._get_block().expr.session
 
+    @property
+    def T(self) -> DataFrame:
+        return DataFrame(self._get_block().transpose())
+
+    def transpose(self) -> DataFrame:
+        return self.T
+
     def __len__(self):
         rows, _ = self.shape
         return rows
 
     __len__.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.__len__)
 
     def __iter__(self):
@@ -664,39 +674,42 @@
         elif isinstance(other, DataFrame):
             return self._apply_dataframe_binop(other, op, how=how, reverse=reverse)
         elif isinstance(other, pandas.DataFrame):
             return self._apply_dataframe_binop(
                 DataFrame(other), op, how=how, reverse=reverse
             )
         elif utils.get_axis_number(axis) == 0:
-            bf_series = bigframes.core.convert.to_bf_series(other, self.index)
+            bf_series = bigframes.core.convert.to_bf_series(
+                other, self.index, self._session
+            )
             return self._apply_series_binop_axis_0(bf_series, op, how, reverse)
         elif utils.get_axis_number(axis) == 1:
             pd_series = bigframes.core.convert.to_pd_series(other, self.columns)
             return self._apply_series_binop_axis_1(pd_series, op, how, reverse)
         raise NotImplementedError(
             f"binary operation is not implemented on the second operand of type {type(other).__name__}."
             f"{constants.FEEDBACK_LINK}"
         )
 
     def _apply_scalar_binop(
         self, other: float | int, op: ops.BinaryOp, reverse: bool = False
     ) -> DataFrame:
-        block = self._block
-        for column_id, label in zip(
-            self._block.value_columns, self._block.column_labels
-        ):
-            expr = (
-                op.as_expr(ex.const(other), column_id)
-                if reverse
-                else op.as_expr(column_id, ex.const(other))
+        if reverse:
+            expr = op.as_expr(
+                left_input=ex.const(other),
+                right_input=bigframes.core.guid.generate_guid(),
             )
-            block, _ = block.project_expr(expr, label)
-            block = block.drop_columns([column_id])
-        return DataFrame(block)
+        else:
+            expr = op.as_expr(
+                left_input=bigframes.core.guid.generate_guid(),
+                right_input=ex.const(other),
+            )
+        return DataFrame(
+            self._block.multi_apply_unary_op(self._block.value_columns, expr)
+        )
 
     def _apply_series_binop_axis_0(
         self,
         other: bigframes.series.Series,
         op: ops.BinaryOp,
         how: str = "outer",
         reverse: bool = False,
@@ -1958,60 +1971,60 @@
         bool_only: bool = False,
     ) -> bigframes.series.Series:
         if not bool_only:
             frame = self._raise_on_non_boolean("any")
         else:
             frame = self._drop_non_bool()
         block = frame._block.aggregate_all_and_stack(agg_ops.any_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def all(
         self, axis: typing.Union[str, int] = 0, *, bool_only: bool = False
     ) -> bigframes.series.Series:
         if not bool_only:
             frame = self._raise_on_non_boolean("all")
         else:
             frame = self._drop_non_bool()
         block = frame._block.aggregate_all_and_stack(agg_ops.all_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def sum(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("sum")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.sum_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def mean(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("mean")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.mean_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def median(
         self, *, numeric_only: bool = False, exact: bool = True
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("median")
         else:
             frame = self._drop_non_numeric()
         if exact:
             result = frame.quantile()
             result.name = None
             return result
         else:
             block = frame._block.aggregate_all_and_stack(agg_ops.median_op)
-            return bigframes.series.Series(block.select_column("values"))
+            return bigframes.series.Series(block)
 
     def quantile(
         self, q: Union[float, Sequence[float]] = 0.5, *, numeric_only: bool = False
     ):
         if not numeric_only:
             frame = self._raise_on_non_numeric("median")
         else:
@@ -2036,70 +2049,70 @@
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("std")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.std_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def var(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("var")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.var_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def min(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("min")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.min_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def max(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("max")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.max_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def prod(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("prod")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.product_op, axis=axis)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     product = prod
     product.__doc__ = inspect.getdoc(vendored_pandas_frame.DataFrame.prod)
 
     def count(self, *, numeric_only: bool = False) -> bigframes.series.Series:
         if not numeric_only:
             frame = self
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.count_op)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def nunique(self) -> bigframes.series.Series:
         block = self._block.aggregate_all_and_stack(agg_ops.nunique_op)
-        return bigframes.series.Series(block.select_column("values"))
+        return bigframes.series.Series(block)
 
     def agg(
         self, func: str | typing.Sequence[str]
     ) -> DataFrame | bigframes.series.Series:
         if utils.is_list_like(func):
             if any(
                 dtype not in bigframes.dtypes.NUMERIC_BIGFRAMES_TYPES_PERMISSIVE
@@ -3380,14 +3393,25 @@
 
     def _set_block(self, block: blocks.Block):
         self._block = block
 
     def _get_block(self) -> blocks.Block:
         return self._block
 
+    def cache(self):
+        """
+        Materializes the DataFrame to a temporary table.
+
+        Useful if the dataframe will be used multiple times, as this will avoid recomputating the shared intermediate value.
+
+        Returns:
+            DataFrame: Self
+        """
+        return self._cached(force=True)
+
     def _cached(self, *, force: bool = False) -> DataFrame:
         """Materialize dataframe to a temporary table.
         No-op if the dataframe represents a trivial transformation of an existing materialization.
         Force=True is used for BQML integration where need to copy data rather than use snapshot.
         """
         self._set_block(self._block.cached(force=force))
         return self
```

### Comparing `bigframes-1.3.0/bigframes/dtypes.py` & `bigframes-1.4.0/bigframes/dtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,29 +654,33 @@
             return lcd_type(pd.Int64Dtype(), dtype)
         if isinstance(scalar, decimal.Decimal):
             # TODO: Check context to see if can use NUMERIC instead of BIGNUMERIC
             return lcd_type(pd.ArrowDtype(pa.decimal256(76, 38)), dtype)
     return None
 
 
-def lcd_type(dtype1: Dtype, dtype2: Dtype) -> Dtype:
-    """Get the supertype of the two types."""
-    if dtype1 == dtype2:
-        return dtype1
+def lcd_type(*dtypes: Dtype) -> Dtype:
+    if len(dtypes) < 1:
+        raise ValueError("at least one dypes should be provided")
+    if len(dtypes) == 1:
+        return dtypes[0]
+    unique_dtypes = set(dtypes)
+    if len(unique_dtypes) == 1:
+        return unique_dtypes.pop()
     # Implicit conversion currently only supported for numeric types
     hierarchy: list[Dtype] = [
         pd.BooleanDtype(),
         pd.Int64Dtype(),
         pd.ArrowDtype(pa.decimal128(38, 9)),
         pd.ArrowDtype(pa.decimal256(76, 38)),
         pd.Float64Dtype(),
     ]
-    if (dtype1 not in hierarchy) or (dtype2 not in hierarchy):
+    if any([dtype not in hierarchy for dtype in dtypes]):
         return None
-    lcd_index = max(hierarchy.index(dtype1), hierarchy.index(dtype2))
+    lcd_index = max([hierarchy.index(dtype) for dtype in dtypes])
     return hierarchy[lcd_index]
 
 
 def coerce_to_common(etype1: ExpressionType, etype2: ExpressionType) -> ExpressionType:
     """Coerce types to a common type or throw a TypeError"""
     if etype1 is not None and etype2 is not None:
         common_supertype = lcd_type(etype1, etype2)
```

### Comparing `bigframes-1.3.0/bigframes/exceptions.py` & `bigframes-1.4.0/bigframes/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/features.py` & `bigframes-1.4.0/bigframes/features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/formatting_helpers.py` & `bigframes-1.4.0/bigframes/formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/functions/__init__.py` & `bigframes-1.4.0/bigframes/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/functions/remote_function.py` & `bigframes-1.4.0/bigframes/functions/remote_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import random
 import shutil
 import string
 import sys
 import tempfile
 import textwrap
-from typing import List, NamedTuple, Optional, Sequence, TYPE_CHECKING
+from typing import List, NamedTuple, Optional, Sequence, TYPE_CHECKING, Union
 
 import ibis
 import requests
 
 if TYPE_CHECKING:
     from bigframes.session import Session
 
@@ -337,15 +337,17 @@
         with open(requirements_txt, "w") as f:
             f.write("\n".join(requirements))
 
         # main.py
         entry_point = self.generate_cloud_function_main_code(def_, dir)
         return entry_point
 
-    def create_cloud_function(self, def_, cf_name, package_requirements=None):
+    def create_cloud_function(
+        self, def_, cf_name, package_requirements=None, cloud_function_timeout=600
+    ):
         """Create a cloud function from the given user defined function."""
 
         # Build and deploy folder structure containing cloud function
         with tempfile.TemporaryDirectory() as dir:
             entry_point = self.generate_cloud_function_code(
                 def_, dir, package_requirements
             )
@@ -405,15 +407,22 @@
                 upload_url_response.storage_source.object_
             )
             function.build_config.docker_repository = (
                 self._cloud_function_docker_repository
             )
             function.service_config = functions_v2.ServiceConfig()
             function.service_config.available_memory = "1024M"
-            function.service_config.timeout_seconds = 600
+            if cloud_function_timeout is not None:
+                if cloud_function_timeout > 1200:
+                    raise ValueError(
+                        "BigQuery remote function can wait only up to 20 minutes"
+                        ", see for more details "
+                        "https://cloud.google.com/bigquery/quotas#remote_function_limits."
+                    )
+                function.service_config.timeout_seconds = cloud_function_timeout
             function.service_config.service_account_email = (
                 self._cloud_function_service_account
             )
             function.kms_key_name = self._cloud_function_kms_key_name
             create_function_request.function = function
 
             # Create the cloud function and wait for it to be ready to use
@@ -452,14 +461,15 @@
         def_,
         input_types,
         output_type,
         reuse,
         name,
         package_requirements,
         max_batching_rows,
+        cloud_function_timeout,
     ):
         """Provision a BigQuery remote function."""
         # If reuse of any existing function with the same name (indicated by the
         # same hash of its source code) is not intended, then attach a unique
         # suffix to the intended function name to make it unique.
         uniq_suffix = None
         if not reuse:
@@ -473,15 +483,15 @@
             def_, uniq_suffix, package_requirements
         )
         cf_endpoint = self.get_cloud_function_endpoint(cloud_function_name)
 
         # Create the cloud function if it does not exist
         if not cf_endpoint:
             cf_endpoint = self.create_cloud_function(
-                def_, cloud_function_name, package_requirements
+                def_, cloud_function_name, package_requirements, cloud_function_timeout
             )
         else:
             logger.info(f"Cloud function {cloud_function_name} already exists.")
 
         # Derive the name of the remote function
         remote_function_name = name
         if not remote_function_name:
@@ -609,15 +619,15 @@
 
 
 # Inspired by @udf decorator implemented in ibis-bigquery package
 # https://github.com/ibis-project/ibis-bigquery/blob/main/ibis_bigquery/udf/__init__.py
 # which has moved as @js to the ibis package
 # https://github.com/ibis-project/ibis/blob/master/ibis/backends/bigquery/udf/__init__.py
 def remote_function(
-    input_types: Sequence[type],
+    input_types: Union[type, Sequence[type]],
     output_type: type,
     session: Optional[Session] = None,
     bigquery_client: Optional[bigquery.Client] = None,
     bigquery_connection_client: Optional[
         bigquery_connection_v1.ConnectionServiceClient
     ] = None,
     cloud_functions_client: Optional[functions_v2.FunctionServiceClient] = None,
@@ -627,14 +637,15 @@
     reuse: bool = True,
     name: Optional[str] = None,
     packages: Optional[Sequence[str]] = None,
     cloud_function_service_account: Optional[str] = None,
     cloud_function_kms_key_name: Optional[str] = None,
     cloud_function_docker_repository: Optional[str] = None,
     max_batching_rows: Optional[int] = 1000,
+    cloud_function_timeout: Optional[int] = 600,
 ):
     """Decorator to turn a user defined function into a BigQuery remote function.
 
     .. deprecated:: 0.0.1
        This is an internal method. Please use :func:`bigframes.pandas.remote_function` instead.
 
     .. note::
@@ -671,17 +682,18 @@
             2. To set up IAM, follow https://cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions#grant_permission_on_function
 
                Alternatively, the IAM could also be setup via the gcloud CLI:
 
                `$ gcloud projects add-iam-policy-binding PROJECT_ID --member="serviceAccount:CONNECTION_SERVICE_ACCOUNT_ID" --role="roles/run.invoker"`.
 
     Args:
-        input_types list(type):
-            List of input data types in the user defined function.
-        output_type type:
+        input_types (type or sequence(type)):
+            Input data type, or sequence of input data types in the user
+            defined function.
+        output_type (type):
             Data type of the output in the user defined function.
         session (bigframes.Session, Optional):
             BigQuery DataFrames session to use for getting default project,
             dataset and BigQuery connection.
         bigquery_client (google.cloud.bigquery.Client, Optional):
             Client to use for BigQuery operations. If this param is not provided
             then bigquery client from the session would be used.
@@ -752,15 +764,28 @@
             BQ remote function. Default value is 1000. A lower number can be
             passed to avoid timeouts in case the user code is too complex to
             process large number of rows fast enough. A higher number can be
             used to increase throughput in case the user code is fast enough.
             `None` can be passed to let BQ remote functions service apply
             default batching. See for more details
             https://cloud.google.com/bigquery/docs/remote-functions#limiting_number_of_rows_in_a_batch_request.
+        cloud_function_timeout (int, Optional):
+            The maximum amount of time (in seconds) BigQuery should wait for
+            the cloud function to return a response. See for more details
+            https://cloud.google.com/functions/docs/configuring/timeout.
+            Please note that even though the cloud function (2nd gen) itself
+            allows seeting up to 60 minutes of timeout, BigQuery remote
+            function can wait only up to 20 minutes, see for more details
+            https://cloud.google.com/bigquery/quotas#remote_function_limits.
+            By default BigQuery DataFrames uses a 10 minute timeout. `None`
+            can be passed to let the cloud functions default timeout take effect.
     """
+    if isinstance(input_types, type):
+        input_types = [input_types]
+
     import bigframes.pandas as bpd
 
     session = session or bpd.get_global_session()
 
     # A BigQuery client is required to perform BQ operations
     if not bigquery_client:
         bigquery_client = session.bqclient
@@ -876,14 +901,15 @@
             f,
             ibis_signature.input_types,
             ibis_signature.output_type,
             reuse,
             name,
             packages,
             max_batching_rows,
+            cloud_function_timeout,
         )
 
         # TODO: Move ibis logic to compiler step
         node = ibis.udf.scalar.builtin(
             f,
             name=rf_name,
             schema=f"{dataset_ref.project}.{dataset_ref.dataset_id}",
```

### Comparing `bigframes-1.3.0/bigframes/ml/__init__.py` & `bigframes-1.4.0/bigframes/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/base.py` & `bigframes-1.4.0/bigframes/ml/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/cluster.py` & `bigframes-1.4.0/bigframes/ml/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,20 +171,20 @@
         )
 
     def to_gbq(self, model_name: str, replace: bool = False) -> KMeans:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            KMeans: saved model."""
+            KMeans: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
     def score(
```

### Comparing `bigframes-1.3.0/bigframes/ml/compose.py` & `bigframes-1.4.0/bigframes/ml/compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/core.py` & `bigframes-1.4.0/bigframes/ml/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             type:
                 Distance types, accept values are  "EUCLIDEAN", "MANHATTAN", "COSINE".
             name:
                 name of the output result column
         """
         assert len(x.columns) == 1 and len(y.columns) == 1
 
-        input_data = x._cached().join(y._cached(), how="outer")
+        input_data = x.cache().join(y.cache(), how="outer")
         x_column_id, y_column_id = x._block.value_columns[0], y._block.value_columns[0]
 
         return self._apply_sql(
             input_data,
             lambda source_df: self._base_sql_generator.ml_distance(
                 x_column_id,
                 y_column_id,
@@ -183,14 +183,25 @@
         return self._session.read_gbq(sql, index_col="forecast_timestamp").reset_index()
 
     def evaluate(self, input_data: Optional[bpd.DataFrame] = None):
         sql = self._model_manipulation_sql_generator.ml_evaluate(input_data)
 
         return self._session.read_gbq(sql)
 
+    def llm_evaluate(
+        self,
+        input_data: bpd.DataFrame,
+        task_type: Optional[str] = None,
+    ):
+        sql = self._model_manipulation_sql_generator.ml_llm_evaluate(
+            input_data, task_type
+        )
+
+        return self._session.read_gbq(sql)
+
     def arima_evaluate(self, show_all_candidate_models: bool = False):
         sql = self._model_manipulation_sql_generator.ml_arima_evaluate(
             show_all_candidate_models
         )
 
         return self._session.read_gbq(sql)
 
@@ -295,19 +306,17 @@
 
         Returns: a BqmlModel, wrapping a trained model in BigQuery
         """
         options = dict(options)
         # Cache dataframes to make sure base table is not a snapshot
         # cached dataframe creates a full copy, never uses snapshot
         if y_train is None:
-            input_data = X_train._cached(force=True)
+            input_data = X_train.cache()
         else:
-            input_data = X_train._cached(force=True).join(
-                y_train._cached(force=True), how="outer"
-            )
+            input_data = X_train.cache().join(y_train.cache(), how="outer")
             options.update({"INPUT_LABEL_COLS": y_train.columns.tolist()})
 
         session = X_train._session
         if session._bq_kms_key_name:
             options.update({"kms_key_name": session._bq_kms_key_name})
 
         model_ref = self._create_model_ref(session._anonymous_dataset)
@@ -339,17 +348,15 @@
                 a BQ connection to talk with Vertex AI, of the format <PROJECT_NUMBER>.<REGION>.<CONNECTION_NAME>. https://cloud.google.com/bigquery/docs/create-cloud-resource-connection
 
         Returns: a BqmlModel, wrapping a trained model in BigQuery
         """
         options = dict(options)
         # Cache dataframes to make sure base table is not a snapshot
         # cached dataframe creates a full copy, never uses snapshot
-        input_data = X_train._cached(force=True).join(
-            y_train._cached(force=True), how="outer"
-        )
+        input_data = X_train.cache().join(y_train.cache(), how="outer")
         options.update({"INPUT_LABEL_COLS": y_train.columns.tolist()})
 
         session = X_train._session
 
         model_ref = self._create_model_ref(session._anonymous_dataset)
 
         sql = self._model_creation_sql_generator.create_llm_remote_model(
@@ -374,17 +381,15 @@
         assert (
             y_train.columns.size == 1
         ), "Time stamp data input must only contain 1 column."
 
         options = dict(options)
         # Cache dataframes to make sure base table is not a snapshot
         # cached dataframe creates a full copy, never uses snapshot
-        input_data = X_train._cached(force=True).join(
-            y_train._cached(force=True), how="outer"
-        )
+        input_data = X_train.cache().join(y_train.cache(), how="outer")
         options.update({"TIME_SERIES_TIMESTAMP_COL": X_train.columns.tolist()[0]})
         options.update({"TIME_SERIES_DATA_COL": y_train.columns.tolist()[0]})
 
         session = X_train._session
         model_ref = self._create_model_ref(session._anonymous_dataset)
 
         sql = self._model_creation_sql_generator.create_model(
```

### Comparing `bigframes-1.3.0/bigframes/ml/decomposition.py` & `bigframes-1.4.0/bigframes/ml/decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,20 +165,20 @@
         )
 
     def to_gbq(self, model_name: str, replace: bool = False) -> PCA:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            PCA: saved model."""
+            PCA: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
     def score(
```

### Comparing `bigframes-1.3.0/bigframes/ml/ensemble.py` & `bigframes-1.4.0/bigframes/ml/ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/forecasting.py` & `bigframes-1.4.0/bigframes/ml/forecasting.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         return self._bqml_model.arima_evaluate(show_all_candidate_models)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> ARIMAPlus:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             ARIMAPlus: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
```

### Comparing `bigframes-1.3.0/bigframes/ml/globals.py` & `bigframes-1.4.0/bigframes/ml/globals.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/imported.py` & `bigframes-1.4.0/bigframes/ml/imported.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         return self._bqml_model.predict(X)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> TensorFlowModel:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                  Default to False.
 
         Returns:
             TensorFlowModel: Saved model."""
         if not self._bqml_model:
             if self.model_path is None:
@@ -162,15 +162,15 @@
         return self._bqml_model.predict(X)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> ONNXModel:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             ONNXModel: Saved model."""
         if not self._bqml_model:
             if self.model_path is None:
@@ -278,15 +278,15 @@
         return self._bqml_model.predict(X)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> XGBoostModel:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
             XGBoostModel: Saved model."""
         if not self._bqml_model:
             if self.model_path is None:
```

### Comparing `bigframes-1.3.0/bigframes/ml/linear_model.py` & `bigframes-1.4.0/bigframes/ml/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,20 +178,20 @@
         return self._bqml_model.evaluate(input_data)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> LinearRegression:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            LinearRegression: saved model."""
+            LinearRegression: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
 
@@ -343,20 +343,20 @@
         return self._bqml_model.evaluate(input_data)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> LogisticRegression:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            LogisticRegression: saved model."""
+            LogisticRegression: Saved model."""
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         # TODO(ashleyxu): support class_weight (struct array as dict in our API)
         if self.class_weight not in (None, "balanced"):
             raise NotImplementedError(
                 f"class_weight is not supported yet. {constants.FEEDBACK_LINK}"
```

### Comparing `bigframes-1.3.0/bigframes/ml/llm.py` & `bigframes-1.4.0/bigframes/ml/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             The model for natural language tasks. “text-bison” returns model fine-tuned to follow natural language instructions
             and is suitable for a variety of language tasks. "text-bison-32k" supports up to 32k tokens per request.
             Default to "text-bison".
         session (bigframes.Session or None):
             BQ session to create the model. If None, use the global default session.
         connection_name (str or None):
             Connection to connect with remote service. str of the format <PROJECT_NUMBER/PROJECT_ID>.<LOCATION>.<CONNECTION_ID>.
-            if None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
-            permission if the connection isn't fully setup.
+            If None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
+            permission if the connection isn't fully set up.
         max_iterations (Optional[int], Default to 300):
             The number of steps to run when performing supervised tuning.
     """
 
     def __init__(
         self,
         *,
@@ -187,15 +187,15 @@
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 DataFrame of shape (n_samples, n_features). Training data.
             y (bigframes.dataframe.DataFrame or bigframes.series.Series:
                 Training labels.
 
         Returns:
-            PaLM2TextGenerator: Fitted Estimator.
+            PaLM2TextGenerator: Fitted estimator.
         """
         X, y = utils.convert_to_dataframe(X, y)
 
         options = self._bqml_options
         options["endpoint"] = self.model_name + "@001"
         options["prompt_col"] = X.columns.tolist()[0]
 
@@ -216,15 +216,15 @@
         top_k: int = 40,
         top_p: float = 0.95,
     ) -> bpd.DataFrame:
         """Predict the result from input DataFrame.
 
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
-                Input DataFrame or Series, which needs to contain a column with name "prompt". Only the column will be used as input.
+                Input DataFrame or Series, which contains only one column of prompts.
                 Prompts can include preamble, questions, suggestions, instructions, or examples.
 
             temperature (float, default 0.0):
                 The temperature is used for sampling during the response generation, which occurs when topP and topK are applied.
                 Temperature controls the degree of randomness in token selection. Lower temperatures are good for prompts that expect a true or correct response,
                 while higher temperatures can lead to more diverse or unexpected results. A temperature of 0 is deterministic:
                 the highest probability token is always selected. For most use cases, try starting with a temperature of 0.2.
@@ -306,47 +306,104 @@
             warnings.warn(
                 f"Some predictions failed. Check column {_ML_GENERATE_TEXT_STATUS} for detailed status. You may want to filter the failed rows and retry.",
                 RuntimeWarning,
             )
 
         return df
 
+    def score(
+        self,
+        X: Union[bpd.DataFrame, bpd.Series],
+        y: Union[bpd.DataFrame, bpd.Series],
+        task_type: Literal[
+            "text_generation", "classification", "summarization", "question_answering"
+        ] = "text_generation",
+    ) -> bpd.DataFrame:
+        """Calculate evaluation metrics of the model.
+
+        .. note::
+
+            This product or feature is subject to the "Pre-GA Offerings Terms" in the General Service Terms section of the
+            Service Specific Terms(https://cloud.google.com/terms/service-terms#1). Pre-GA products and features are available "as is"
+            and might have limited support. For more information, see the launch stage descriptions
+            (https://cloud.google.com/products#product-launch-stages).
+
+        .. note::
+
+            Output matches that of the BigQuery ML.EVALUTE function.
+            See: https://cloud.google.com/bigquery/docs/reference/standard-sql/bigqueryml-syntax-evaluate#remote-model-llm
+            for the outputs relevant to this model type.
+
+        Args:
+            X (bigframes.dataframe.DataFrame or bigframes.series.Series):
+                A BigQuery DataFrame as evaluation data, which contains only one column of input_text
+                that contains the prompt text to use when evaluating the model.
+            y (bigframes.dataframe.DataFrame or bigframes.series.Series):
+                A BigQuery DataFrame as evaluation labels, which contains only one column of output_text
+                that you would expect to be returned by the model.
+            task_type (str):
+                The type of the task for LLM model. Default to "text_generation".
+                Possible values: "text_generation", "classification", "summarization", and "question_answering".
+
+        Returns:
+            bigframes.dataframe.DataFrame: The DataFrame as evaluation result.
+        """
+        if not self._bqml_model:
+            raise RuntimeError("A model must be fitted before score")
+
+        X, y = utils.convert_to_dataframe(X, y)
+
+        if len(X.columns) != 1 or len(y.columns) != 1:
+            raise ValueError(
+                f"Only support one column as input for X and y. {constants.FEEDBACK_LINK}"
+            )
+
+        # BQML identified the column by name
+        X_col_label = cast(blocks.Label, X.columns[0])
+        y_col_label = cast(blocks.Label, y.columns[0])
+        X = X.rename(columns={X_col_label: "input_text"})
+        y = y.rename(columns={y_col_label: "output_text"})
+
+        input_data = X.join(y, how="outer")
+
+        return self._bqml_model.llm_evaluate(input_data, task_type)
+
     def to_gbq(self, model_name: str, replace: bool = False) -> PaLM2TextGenerator:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            PaLM2TextGenerator: saved model."""
+            PaLM2TextGenerator: Saved model."""
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
 
 @log_adapter.class_logger
 class PaLM2TextEmbeddingGenerator(base.BaseEstimator):
     """PaLM2 text embedding generator LLM model.
 
     Args:
         model_name (str, Default to "textembedding-gecko"):
             The model for text embedding. “textembedding-gecko” returns model embeddings for text inputs.
-            "textembedding-gecko-multilingual" returns model embeddings for text inputs which support over 100 languages
+            "textembedding-gecko-multilingual" returns model embeddings for text inputs which support over 100 languages.
             Default to "textembedding-gecko".
         version (str or None):
             Model version. Accepted values are "001", "002", "003", "latest" etc. Will use the default version if unset.
             See https://cloud.google.com/vertex-ai/docs/generative-ai/learn/model-versioning for details.
         session (bigframes.Session or None):
             BQ session to create the model. If None, use the global default session.
         connection_name (str or None):
-            connection to connect with remote service. str of the format <PROJECT_NUMBER/PROJECT_ID>.<LOCATION>.<CONNECTION_ID>.
-            if None, use default connection in session context.
+            Connection to connect with remote service. str of the format <PROJECT_NUMBER/PROJECT_ID>.<LOCATION>.<CONNECTION_ID>.
+            If None, use default connection in session context.
     """
 
     def __init__(
         self,
         *,
         model_name: Literal[
             "textembedding-gecko", "textembedding-gecko-multilingual"
@@ -478,20 +535,20 @@
     def to_gbq(
         self, model_name: str, replace: bool = False
     ) -> PaLM2TextEmbeddingGenerator:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            PaLM2TextEmbeddingGenerator: saved model."""
+            PaLM2TextEmbeddingGenerator: Saved model."""
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
 
 
 @log_adapter.class_logger
 class GeminiTextGenerator(base.BaseEstimator):
@@ -504,16 +561,16 @@
         (https://cloud.google.com/products#product-launch-stages).
 
     Args:
         session (bigframes.Session or None):
             BQ session to create the model. If None, use the global default session.
         connection_name (str or None):
             Connection to connect with remote service. str of the format <PROJECT_NUMBER/PROJECT_ID>.<LOCATION>.<CONNECTION_ID>.
-            if None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
-            permission if the connection isn't fully setup.
+            If None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
+            permission if the connection isn't fully set up.
     """
 
     def __init__(
         self,
         *,
         session: Optional[bigframes.Session] = None,
         connection_name: Optional[str] = None,
@@ -658,16 +715,16 @@
         return df
 
     def to_gbq(self, model_name: str, replace: bool = False) -> GeminiTextGenerator:
         """Save the model to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model.
+                The name of the model.
             replace (bool, default False):
                 Determine whether to replace if the model already exists. Default to False.
 
         Returns:
-            GeminiTextGenerator: saved model."""
+            GeminiTextGenerator: Saved model."""
 
         new_model = self._bqml_model.copy(model_name, replace)
         return new_model.session.read_gbq_model(model_name)
```

### Comparing `bigframes-1.3.0/bigframes/ml/loader.py` & `bigframes-1.4.0/bigframes/ml/loader.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/metrics/__init__.py` & `bigframes-1.4.0/bigframes/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/metrics/_metrics.py` & `bigframes-1.4.0/bigframes/ml/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/metrics/pairwise.py` & `bigframes-1.4.0/bigframes/ml/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/model_selection.py` & `bigframes-1.4.0/bigframes/ml/model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/pipeline.py` & `bigframes-1.4.0/bigframes/ml/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,19 +122,19 @@
         return self._estimator.score(X=X, y=y)
 
     def to_gbq(self, model_name: str, replace: bool = False) -> Pipeline:
         """Save the pipeline to BigQuery.
 
         Args:
             model_name (str):
-                the name of the model(pipeline).
+                The name of the model(pipeline).
             replace (bool, default False):
-                whether to replace if the model(pipeline) already exists. Default to False.
+                Whether to replace if the model(pipeline) already exists. Default to False.
 
         Returns:
-            Pipeline: saved model(pipeline)."""
+            Pipeline: Saved model(pipeline)."""
         if not self._estimator._bqml_model:
             raise RuntimeError("A model must be fitted before it can be saved")
 
         new_model = self._estimator._bqml_model.copy(model_name, replace)
 
         return new_model.session.read_gbq_model(model_name)
```

### Comparing `bigframes-1.3.0/bigframes/ml/preprocessing.py` & `bigframes-1.4.0/bigframes/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/ml/remote.py` & `bigframes-1.4.0/bigframes/ml/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,30 +26,30 @@
 import bigframes.pandas as bpd
 
 _REMOTE_MODEL_STATUS = "remote_model_status"
 
 
 @log_adapter.class_logger
 class VertexAIModel(base.BaseEstimator):
-    """Remote model from a Vertex AI https endpoint. User must specify https endpoint, input schema and output schema.
-    How to deploy a model in Vertex AI https://cloud.google.com/bigquery/docs/bigquery-ml-remote-model-tutorial#Deploy-Model-on-Vertex-AI.
+    """Remote model from a Vertex AI HTTPS endpoint. User must specify HTTPS endpoint, input schema and output schema.
+    For more information, see Deploy model on Vertex AI: https://cloud.google.com/bigquery/docs/bigquery-ml-remote-model-tutorial#Deploy-Model-on-Vertex-AI.
 
     Args:
         endpoint (str):
-            Vertex AI https endpoint.
+            Vertex AI HTTPS endpoint.
         input (Mapping):
             Input schema: `{column_name: column_type}`. Supported types are "bool", "string", "int64", "float64", "array<bool>", "array<string>", "array<int64>", "array<float64>".
         output (Mapping):
             Output label schema: `{column_name: column_type}`. Supported the same types as the input.
         session (bigframes.Session or None):
             BQ session to create the model. If None, use the global default session.
         connection_name (str or None):
             Connection to connect with remote service. str of the format <PROJECT_NUMBER/PROJECT_ID>.<LOCATION>.<CONNECTION_ID>.
-            if None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
-            permission if the connection isn't fully setup.
+            If None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
+            permission if the connection isn't fully set up.
     """
 
     def __init__(
         self,
         endpoint: str,
         input: Mapping[str, str],
         output: Mapping[str, str],
```

### Comparing `bigframes-1.3.0/bigframes/ml/sql.py` & `bigframes-1.4.0/bigframes/ml/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,24 @@
         if source_sql is None:
             return f"""SELECT * FROM ML.EVALUATE(MODEL `{self._model_name}`)"""
         else:
             return f"""SELECT * FROM ML.EVALUATE(MODEL `{self._model_name}`,
   ({source_sql}))"""
 
     # ML evaluation TVFs
+    def ml_llm_evaluate(
+        self, source_df: bpd.DataFrame, task_type: Optional[str] = None
+    ) -> str:
+        """Encode ML.EVALUATE for BQML"""
+        # Note: don't need index as evaluate returns a new table
+        source_sql, _, _ = source_df._to_sql_query(include_index=False)
+        return f"""SELECT * FROM ML.EVALUATE(MODEL `{self._model_name}`,
+            ({source_sql}), STRUCT("{task_type}" AS task_type))"""
+
+    # ML evaluation TVFs
     def ml_arima_evaluate(self, show_all_candidate_models: bool = False) -> str:
         """Encode ML.ARMIA_EVALUATE for BQML"""
         return f"""SELECT * FROM ML.ARIMA_EVALUATE(MODEL `{self._model_name}`,
             STRUCT({show_all_candidate_models} AS show_all_candidate_models))"""
 
     def ml_centroids(self) -> str:
         """Encode ML.CENTROIDS for BQML"""
```

### Comparing `bigframes-1.3.0/bigframes/ml/utils.py` & `bigframes-1.4.0/bigframes/ml/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/__init__.py` & `bigframes-1.4.0/bigframes/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/_matplotlib/__init__.py` & `bigframes-1.4.0/bigframes/operations/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/_matplotlib/core.py` & `bigframes-1.4.0/bigframes/operations/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/_matplotlib/hist.py` & `bigframes-1.4.0/bigframes/operations/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/aggregations.py` & `bigframes-1.4.0/bigframes/operations/aggregations.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/base.py` & `bigframes-1.4.0/bigframes/operations/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing
 
 import bigframes_vendored.pandas.pandas._typing as vendored_pandas_typing
+import numpy
 import pandas as pd
 
 import bigframes.constants as constants
 import bigframes.core.blocks as blocks
+import bigframes.core.convert
 import bigframes.core.expression as ex
 import bigframes.core.indexes as indexes
 import bigframes.core.scalar as scalars
 import bigframes.dtypes
 import bigframes.operations as ops
 import bigframes.operations.aggregations as agg_ops
 import bigframes.series as series
@@ -40,77 +42,106 @@
             bigframes.dtypes.DtypeString | bigframes.dtypes.Dtype
         ] = None,
         name: str | None = None,
         copy: typing.Optional[bool] = None,
         *,
         session: typing.Optional[bigframes.session.Session] = None,
     ):
-        block = None
+        import bigframes.pandas
+
+        # just ignore object dtype if provided
+        if dtype in {numpy.dtypes.ObjectDType, "object"}:
+            dtype = None
+
+        read_pandas_func = (
+            session.read_pandas
+            if (session is not None)
+            else (lambda x: bigframes.pandas.read_pandas(x))
+        )
+
+        block: typing.Optional[blocks.Block] = None
         if copy is not None and not copy:
             raise ValueError(
                 f"Series constructor only supports copy=True. {constants.FEEDBACK_LINK}"
             )
         if isinstance(data, blocks.Block):
             assert len(data.value_columns) == 1
             assert len(data.column_labels) == 1
             assert index is None
             block = data
 
-        elif isinstance(data, SeriesMethods):
-            block = data._block
+        # interpret these cases as both index and data
+        elif (
+            isinstance(data, SeriesMethods)
+            or isinstance(data, pd.Series)
+            or pd.api.types.is_dict_like(data)
+        ):
+            if isinstance(data, pd.Series):
+                data = read_pandas_func(data)
+            elif pd.api.types.is_dict_like(data):
+                data = read_pandas_func(pd.Series(data, dtype=dtype))  # type: ignore
+                dtype = None
+            data_block = data._block
             if index is not None:
                 # reindex
-                bf_index = indexes.Index(index)
+                bf_index = indexes.Index(index, session=session)
                 idx_block = bf_index._block
                 idx_cols = idx_block.value_columns
-                block_idx, _ = idx_block.join(block, how="left")
-                block = block_idx.with_index_labels(bf_index.names)
-
-        elif isinstance(data, indexes.Index):
+                block_idx, _ = idx_block.join(data_block, how="left")
+                data_block = block_idx.with_index_labels(bf_index.names)
+            block = data_block
+
+        # list-like data that will get default index
+        elif isinstance(data, indexes.Index) or pd.api.types.is_list_like(data):
+            data = indexes.Index(data, dtype=dtype, session=session)
+            dtype = (
+                None  # set to none as it has already been applied, avoid re-cast later
+            )
             if data.nlevels != 1:
                 raise NotImplementedError("Cannot interpret multi-index as Series.")
             # Reset index to promote index columns to value columns, set default index
-            block = data._block.reset_index(drop=False)
+            data_block = data._block.reset_index(drop=False).with_column_labels(
+                data.names
+            )
             if index is not None:
                 # Align by offset
-                bf_index = indexes.Index(index)
-                idx_block = bf_index._block.reset_index(drop=False)
+                bf_index = indexes.Index(index, session=session)
+                idx_block = bf_index._block.reset_index(
+                    drop=False
+                )  # reset to align by offsets, and then reset back
                 idx_cols = idx_block.value_columns
-                block, (l_mapping, _) = idx_block.join(block, how="left")
-                block = block.set_index([l_mapping[col] for col in idx_cols])
-                block = block.with_index_labels(bf_index.names)
-
-        if block:
-            if name:
-                if not isinstance(name, typing.Hashable):
-                    raise ValueError(
-                        f"BigQuery DataFrames only supports hashable series names. {constants.FEEDBACK_LINK}"
-                    )
-                block = block.with_column_labels([name])
-            if dtype:
-                block = block.multi_apply_unary_op(
-                    block.value_columns, ops.AsTypeOp(to_type=dtype)
-                )
-        else:
-            import bigframes.pandas
+                data_block, (l_mapping, _) = idx_block.join(data_block, how="left")
+                data_block = data_block.set_index([l_mapping[col] for col in idx_cols])
+                data_block = data_block.with_index_labels(bf_index.names)
+            block = data_block
 
-            pd_series = pd.Series(
-                data=data, index=index, dtype=dtype, name=name  # type:ignore
-            )
-            pd_dataframe = pd_series.to_frame()
-            if pd_series.name is None:
-                # to_frame will set default numeric column label if unnamed, but we do not support int column label, so must rename
-                pd_dataframe = pd_dataframe.set_axis(["unnamed_col"], axis=1)
-            if session:
-                block = session.read_pandas(pd_dataframe)._get_block()
+        else:  # Scalar case
+            if index is not None:
+                bf_index = indexes.Index(index, session=session)
             else:
-                # Uses default global session
-                block = bigframes.pandas.read_pandas(pd_dataframe)._get_block()
-            if pd_series.name is None:
-                block = block.with_column_labels([None])
+                bf_index = indexes.Index(
+                    [] if (data is None) else [0],
+                    session=session,
+                    dtype=bigframes.dtypes.INT_DTYPE,
+                )
+            block, _ = bf_index._block.create_constant(data, dtype)
+            dtype = None
+            block = block.with_column_labels([name])
+
+        assert block is not None
+        if name:
+            if not isinstance(name, typing.Hashable):
+                raise ValueError(
+                    f"BigQuery DataFrames only supports hashable series names. {constants.FEEDBACK_LINK}"
+                )
+            block = block.with_column_labels([name])
+        if dtype:
+            block = block.multi_apply_unary_op(
+                block.value_columns, ops.AsTypeOp(to_type=dtype)
+            )
         self._block: blocks.Block = block
 
     @property
     def _value_column(self) -> str:
         return self._block.value_columns[0]
 
     @property
@@ -141,36 +172,35 @@
         self,
         other: typing.Any,
         op: ops.BinaryOp,
         alignment: typing.Literal["outer", "left"] = "outer",
         reverse: bool = False,
     ) -> series.Series:
         """Applies a binary operator to the series and other."""
-        if isinstance(other, pd.Series):
-            # TODO: Convert to BigQuery DataFrames series
-            raise NotImplementedError(
-                f"Pandas series not supported as operand. {constants.FEEDBACK_LINK}"
+        if bigframes.core.convert.is_series_convertible(other):
+            self_index = indexes.Index(self._block)
+            other_series = bigframes.core.convert.to_bf_series(
+                other, self_index, self._block.session
             )
-        if isinstance(other, series.Series):
-            (self_col, other_col, block) = self._align(other, how=alignment)
+            (self_col, other_col, block) = self._align(other_series, how=alignment)
 
             name = self._name
             if (
-                isinstance(other, series.Series)
+                hasattr(other, "name")
                 and other.name != self._name
                 and alignment == "outer"
             ):
                 name = None
             expr = op.as_expr(
                 other_col if reverse else self_col, self_col if reverse else other_col
             )
             block, result_id = block.project_expr(expr, name)
             return series.Series(block.select_column(result_id))
 
-        else:
+        else:  # Scalar binop
             name = self._name
             expr = op.as_expr(
                 ex.const(other) if reverse else self._value_column,
                 self._value_column if reverse else ex.const(other),
             )
             block, result_id = self._block.project_expr(expr, name)
             return series.Series(block.select_column(result_id))
```

### Comparing `bigframes-1.3.0/bigframes/operations/datetimes.py` & `bigframes-1.4.0/bigframes/operations/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/plotting.py` & `bigframes-1.4.0/bigframes/operations/plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/strings.py` & `bigframes-1.4.0/bigframes/operations/strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/structs.py` & `bigframes-1.4.0/bigframes/operations/structs.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/operations/type.py` & `bigframes-1.4.0/bigframes/operations/type.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/pandas/__init__.py` & `bigframes-1.4.0/bigframes/pandas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -629,39 +629,41 @@
     )
 
 
 read_parquet.__doc__ = inspect.getdoc(bigframes.session.Session.read_parquet)
 
 
 def remote_function(
-    input_types: List[type],
+    input_types: Union[type, Sequence[type]],
     output_type: type,
     dataset: Optional[str] = None,
     bigquery_connection: Optional[str] = None,
     reuse: bool = True,
     name: Optional[str] = None,
     packages: Optional[Sequence[str]] = None,
     cloud_function_service_account: Optional[str] = None,
     cloud_function_kms_key_name: Optional[str] = None,
     cloud_function_docker_repository: Optional[str] = None,
     max_batching_rows: Optional[int] = 1000,
+    cloud_function_timeout: Optional[int] = 600,
 ):
     return global_session.with_default_session(
         bigframes.session.Session.remote_function,
         input_types=input_types,
         output_type=output_type,
         dataset=dataset,
         bigquery_connection=bigquery_connection,
         reuse=reuse,
         name=name,
         packages=packages,
         cloud_function_service_account=cloud_function_service_account,
         cloud_function_kms_key_name=cloud_function_kms_key_name,
         cloud_function_docker_repository=cloud_function_docker_repository,
         max_batching_rows=max_batching_rows,
+        cloud_function_timeout=cloud_function_timeout,
     )
 
 
 remote_function.__doc__ = inspect.getdoc(bigframes.session.Session.remote_function)
 
 
 def read_gbq_function(function_name: str):
```

### Comparing `bigframes-1.3.0/bigframes/series.py` & `bigframes-1.4.0/bigframes/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from __future__ import annotations
 
 import functools
 import inspect
 import itertools
 import numbers
-import os
 import textwrap
 import typing
 from typing import Any, cast, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import bigframes_vendored.pandas.core.series as vendored_pandas_series
 import google.cloud.bigquery as bigquery
 import numpy
@@ -69,19 +68,14 @@
 
 @log_adapter.class_logger
 class Series(bigframes.operations.base.SeriesMethods, vendored_pandas_series.Series):
     def __init__(self, *args, **kwargs):
         self._query_job: Optional[bigquery.QueryJob] = None
         super().__init__(*args, **kwargs)
 
-        # Runs strict validations to ensure internal type predictions and ibis are completely in sync
-        # Do not execute these validations outside of testing suite.
-        if "PYTEST_CURRENT_TEST" in os.environ:
-            self._block.expr.validate_schema()
-
     @property
     def dt(self) -> dt.DatetimeMethods:
         return dt.DatetimeMethods(self._block)
 
     @property
     def dtype(self):
         return self._dtype
@@ -808,17 +802,14 @@
 
     def combine_first(self, other: Series) -> Series:
         result = self._apply_binary_op(other, ops.coalesce_op)
         result.name = self.name
         return result
 
     def update(self, other: Union[Series, Sequence, Mapping]) -> None:
-        import bigframes.core.convert
-
-        other = bigframes.core.convert.to_bf_series(other, default_index=None)
         result = self._apply_binary_op(
             other, ops.coalesce_op, reverse=True, alignment="left"
         )
         self._set_block(result._get_block())
 
     def abs(self) -> Series:
         return self._apply_unary_op(ops.abs_op)
@@ -1687,14 +1678,25 @@
     ) -> bigframes.series.Series:
         return bigframes.series.Series(
             self._block.slice(start=start, stop=stop, step=step).select_column(
                 self._value_column
             ),
         )
 
+    def cache(self):
+        """
+        Materializes the Series to a temporary table.
+
+        Useful if the series will be used multiple times, as this will avoid recomputating the shared intermediate value.
+
+        Returns:
+            Series: Self
+        """
+        return self._cached(force=True)
+
     def _cached(self, *, force: bool = True) -> Series:
         self._set_block(self._block.cached(force=force))
         return self
 
     def _optimize_query_complexity(self):
         """Reduce query complexity by caching repeated subtrees and recursively materializing maximum-complexity subtrees.
         May generate many queries and take substantial time to execute.
```

### Comparing `bigframes-1.3.0/bigframes/session/__init__.py` & `bigframes-1.4.0/bigframes/session/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,5043 +104,5089 @@
 00000670: 6761 7069 635f 7631 2e63 6c69 656e 745f  gapic_v1.client_
 00000680: 696e 666f 0a69 6d70 6f72 7420 676f 6f67  info.import goog
 00000690: 6c65 2e61 7574 682e 6372 6564 656e 7469  le.auth.credenti
 000006a0: 616c 730a 696d 706f 7274 2067 6f6f 676c  als.import googl
 000006b0: 652e 636c 6f75 642e 6269 6771 7565 7279  e.cloud.bigquery
 000006c0: 2061 7320 6269 6771 7565 7279 0a69 6d70   as bigquery.imp
 000006d0: 6f72 7420 676f 6f67 6c65 2e63 6c6f 7564  ort google.cloud
-000006e0: 2e62 6967 7175 6572 795f 636f 6e6e 6563  .bigquery_connec
-000006f0: 7469 6f6e 5f76 310a 696d 706f 7274 2067  tion_v1.import g
-00000700: 6f6f 676c 652e 636c 6f75 642e 6269 6771  oogle.cloud.bigq
-00000710: 7565 7279 5f73 746f 7261 6765 5f76 310a  uery_storage_v1.
-00000720: 696d 706f 7274 2067 6f6f 676c 652e 636c  import google.cl
-00000730: 6f75 642e 6675 6e63 7469 6f6e 735f 7632  oud.functions_v2
-00000740: 0a69 6d70 6f72 7420 676f 6f67 6c65 2e63  .import google.c
-00000750: 6c6f 7564 2e72 6573 6f75 7263 656d 616e  loud.resourceman
-00000760: 6167 6572 5f76 330a 696d 706f 7274 2067  ager_v3.import g
-00000770: 6f6f 676c 652e 636c 6f75 642e 7374 6f72  oogle.cloud.stor
-00000780: 6167 6520 6173 2073 746f 7261 6765 2020  age as storage  
-00000790: 2320 7479 7065 3a20 6967 6e6f 7265 0a69  # type: ignore.i
-000007a0: 6d70 6f72 7420 6962 6973 0a69 6d70 6f72  mport ibis.impor
-000007b0: 7420 6962 6973 2e62 6163 6b65 6e64 732e  t ibis.backends.
-000007c0: 6269 6771 7565 7279 2061 7320 6962 6973  bigquery as ibis
-000007d0: 5f62 6967 7175 6572 790a 696d 706f 7274  _bigquery.import
-000007e0: 2069 6269 732e 6578 7072 2e64 6174 6174   ibis.expr.datat
-000007f0: 7970 6573 2061 7320 6962 6973 5f64 7479  ypes as ibis_dty
-00000800: 7065 730a 696d 706f 7274 2069 6269 732e  pes.import ibis.
-00000810: 6578 7072 2e74 7970 6573 2061 7320 6962  expr.types as ib
-00000820: 6973 5f74 7970 6573 0a69 6d70 6f72 7420  is_types.import 
-00000830: 6e75 6d70 7920 6173 206e 700a 696d 706f  numpy as np.impo
-00000840: 7274 2070 616e 6461 730a 6672 6f6d 2070  rt pandas.from p
-00000850: 616e 6461 732e 5f74 7970 696e 6720 696d  andas._typing im
-00000860: 706f 7274 2028 0a20 2020 2043 6f6d 7072  port (.    Compr
-00000870: 6573 7369 6f6e 4f70 7469 6f6e 732c 0a20  essionOptions,. 
-00000880: 2020 2046 696c 6550 6174 682c 0a20 2020     FilePath,.   
-00000890: 2052 6561 6450 6963 6b6c 6542 7566 6665   ReadPickleBuffe
-000008a0: 722c 0a20 2020 2053 746f 7261 6765 4f70  r,.    StorageOp
-000008b0: 7469 6f6e 732c 0a29 0a69 6d70 6f72 7420  tions,.).import 
-000008c0: 7079 6172 726f 7720 6173 2070 610a 0a69  pyarrow as pa..i
-000008d0: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
-000008e0: 5f63 6f6e 6669 672e 6269 6771 7565 7279  _config.bigquery
-000008f0: 5f6f 7074 696f 6e73 2061 7320 6269 6771  _options as bigq
-00000900: 7565 7279 5f6f 7074 696f 6e73 0a69 6d70  uery_options.imp
-00000910: 6f72 7420 6269 6766 7261 6d65 732e 636c  ort bigframes.cl
-00000920: 6965 6e74 730a 696d 706f 7274 2062 6967  ients.import big
-00000930: 6672 616d 6573 2e63 6f6e 7374 616e 7473  frames.constants
-00000940: 2061 7320 636f 6e73 7461 6e74 730a 696d   as constants.im
-00000950: 706f 7274 2062 6967 6672 616d 6573 2e63  port bigframes.c
-00000960: 6f72 6520 6173 2063 6f72 650a 696d 706f  ore as core.impo
-00000970: 7274 2062 6967 6672 616d 6573 2e63 6f72  rt bigframes.cor
-00000980: 652e 626c 6f63 6b73 2061 7320 626c 6f63  e.blocks as bloc
-00000990: 6b73 0a69 6d70 6f72 7420 6269 6766 7261  ks.import bigfra
-000009a0: 6d65 732e 636f 7265 2e63 6f6d 7069 6c65  mes.core.compile
-000009b0: 0a69 6d70 6f72 7420 6269 6766 7261 6d65  .import bigframe
-000009c0: 732e 636f 7265 2e67 7569 6420 6173 2067  s.core.guid as g
-000009d0: 7569 640a 696d 706f 7274 2062 6967 6672  uid.import bigfr
-000009e0: 616d 6573 2e63 6f72 652e 6e6f 6465 7320  ames.core.nodes 
-000009f0: 6173 206e 6f64 6573 0a66 726f 6d20 6269  as nodes.from bi
-00000a00: 6766 7261 6d65 732e 636f 7265 2e6f 7264  gframes.core.ord
-00000a10: 6572 696e 6720 696d 706f 7274 2049 6e74  ering import Int
-00000a20: 6567 6572 456e 636f 6469 6e67 0a69 6d70  egerEncoding.imp
-00000a30: 6f72 7420 6269 6766 7261 6d65 732e 636f  ort bigframes.co
-00000a40: 7265 2e6f 7264 6572 696e 6720 6173 206f  re.ordering as o
-00000a50: 7264 6572 0a69 6d70 6f72 7420 6269 6766  rder.import bigf
-00000a60: 7261 6d65 732e 636f 7265 2e74 7265 655f  rames.core.tree_
-00000a70: 7072 6f70 6572 7469 6573 2061 7320 7472  properties as tr
-00000a80: 6176 6572 7361 6c73 0a69 6d70 6f72 7420  aversals.import 
-00000a90: 6269 6766 7261 6d65 732e 636f 7265 2e74  bigframes.core.t
-00000aa0: 7265 655f 7072 6f70 6572 7469 6573 2061  ree_properties a
-00000ab0: 7320 7472 6565 5f70 726f 7065 7274 6965  s tree_propertie
-00000ac0: 730a 696d 706f 7274 2062 6967 6672 616d  s.import bigfram
-00000ad0: 6573 2e63 6f72 652e 7574 696c 7320 6173  es.core.utils as
-00000ae0: 2075 7469 6c73 0a69 6d70 6f72 7420 6269   utils.import bi
-00000af0: 6766 7261 6d65 732e 6474 7970 6573 0a69  gframes.dtypes.i
-00000b00: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
-00000b10: 666f 726d 6174 7469 6e67 5f68 656c 7065  formatting_helpe
-00000b20: 7273 2061 7320 666f 726d 6174 7469 6e67  rs as formatting
-00000b30: 5f68 656c 7065 7273 0a66 726f 6d20 6269  _helpers.from bi
-00000b40: 6766 7261 6d65 732e 6675 6e63 7469 6f6e  gframes.function
-00000b50: 732e 7265 6d6f 7465 5f66 756e 6374 696f  s.remote_functio
-00000b60: 6e20 696d 706f 7274 2072 6561 645f 6762  n import read_gb
-00000b70: 715f 6675 6e63 7469 6f6e 2061 7320 6269  q_function as bi
-00000b80: 6766 7261 6d65 735f 7267 660a 6672 6f6d  gframes_rgf.from
-00000b90: 2062 6967 6672 616d 6573 2e66 756e 6374   bigframes.funct
-00000ba0: 696f 6e73 2e72 656d 6f74 655f 6675 6e63  ions.remote_func
-00000bb0: 7469 6f6e 2069 6d70 6f72 7420 7265 6d6f  tion import remo
-00000bc0: 7465 5f66 756e 6374 696f 6e20 6173 2062  te_function as b
-00000bd0: 6967 6672 616d 6573 5f72 660a 696d 706f  igframes_rf.impo
-00000be0: 7274 2062 6967 6672 616d 6573 2e73 6573  rt bigframes.ses
-00000bf0: 7369 6f6e 2e5f 696f 2e62 6967 7175 6572  sion._io.bigquer
-00000c00: 7920 6173 2062 6967 6672 616d 6573 5f69  y as bigframes_i
-00000c10: 6f0a 696d 706f 7274 2062 6967 6672 616d  o.import bigfram
-00000c20: 6573 2e73 6573 7369 6f6e 2e63 6c69 656e  es.session.clien
-00000c30: 7473 0a69 6d70 6f72 7420 6269 6766 7261  ts.import bigfra
-00000c40: 6d65 732e 7665 7273 696f 6e0a 0a23 2041  mes.version..# A
-00000c50: 766f 6964 2063 6972 6375 6c61 7220 696d  void circular im
-00000c60: 706f 7274 732e 0a69 6620 7479 7069 6e67  ports..if typing
-00000c70: 2e54 5950 455f 4348 4543 4b49 4e47 3a0a  .TYPE_CHECKING:.
-00000c80: 2020 2020 696d 706f 7274 2062 6967 6672      import bigfr
-00000c90: 616d 6573 2e63 6f72 652e 696e 6465 7865  ames.core.indexe
-00000ca0: 730a 2020 2020 696d 706f 7274 2062 6967  s.    import big
-00000cb0: 6672 616d 6573 2e64 6174 6166 7261 6d65  frames.dataframe
-00000cc0: 2061 7320 6461 7461 6672 616d 650a 2020   as dataframe.  
-00000cd0: 2020 696d 706f 7274 2062 6967 6672 616d    import bigfram
-00000ce0: 6573 2e73 6572 6965 730a 0a5f 4249 4746  es.series.._BIGF
-00000cf0: 5241 4d45 535f 4445 4641 554c 545f 434f  RAMES_DEFAULT_CO
-00000d00: 4e4e 4543 5449 4f4e 5f49 4420 3d20 2262  NNECTION_ID = "b
-00000d10: 6967 6672 616d 6573 2d64 6566 6175 6c74  igframes-default
-00000d20: 2d63 6f6e 6e65 6374 696f 6e22 0a0a 5f4d  -connection".._M
-00000d30: 4158 5f43 4c55 5354 4552 5f43 4f4c 554d  AX_CLUSTER_COLUM
-00000d40: 4e53 203d 2034 0a0a 2320 544f 444f 2873  NS = 4..# TODO(s
-00000d50: 7761 7374 293a 204e 6565 6420 746f 2063  wast): Need to c
-00000d60: 6f6e 6e65 6374 2074 6f20 7265 6769 6f6e  onnect to region
-00000d70: 616c 2065 6e64 706f 696e 7473 2077 6865  al endpoints whe
-00000d80: 6e20 7065 7266 6f72 6d69 6e67 2072 656d  n performing rem
-00000d90: 6f74 650a 2320 6675 6e63 7469 6f6e 7320  ote.# functions 
-00000da0: 6f70 6572 6174 696f 6e73 2028 4251 2043  operations (BQ C
-00000db0: 6f6e 6e65 6374 696f 6e20 4941 4d2c 2043  onnection IAM, C
-00000dc0: 6c6f 7564 2052 756e 202f 2043 6c6f 7564  loud Run / Cloud
-00000dd0: 2046 756e 6374 696f 6e73 292e 0a23 2041   Functions)..# A
-00000de0: 6c73 6f20 7365 6520 6966 2072 6573 6f75  lso see if resou
-00000df0: 7263 6520 6d61 6e61 6765 7220 636c 6965  rce manager clie
-00000e00: 6e74 206c 6962 7261 7279 2073 7570 706f  nt library suppo
-00000e10: 7274 7320 7265 6769 6f6e 616c 2065 6e64  rts regional end
-00000e20: 706f 696e 7473 2e0a 0a5f 5641 4c49 445f  points..._VALID_
-00000e30: 454e 434f 4449 4e47 5320 3d20 7b0a 2020  ENCODINGS = {.  
-00000e40: 2020 2255 5446 2d38 222c 0a20 2020 2022    "UTF-8",.    "
-00000e50: 4953 4f2d 3838 3539 2d31 222c 0a20 2020  ISO-8859-1",.   
-00000e60: 2022 5554 462d 3136 4245 222c 0a20 2020   "UTF-16BE",.   
-00000e70: 2022 5554 462d 3136 4c45 222c 0a20 2020   "UTF-16LE",.   
-00000e80: 2022 5554 462d 3332 4245 222c 0a20 2020   "UTF-32BE",.   
-00000e90: 2022 5554 462d 3332 4c45 222c 0a7d 0a0a   "UTF-32LE",.}..
-00000ea0: 2320 4269 6751 7565 7279 2068 6173 2031  # BigQuery has 1
-00000eb0: 204d 4220 7175 6572 7920 7369 7a65 206c   MB query size l
-00000ec0: 696d 6974 2e20 446f 6e27 7420 7761 6e74  imit. Don't want
-00000ed0: 2074 6f20 7461 6b65 2075 7020 6d6f 7265   to take up more
-00000ee0: 2074 6861 6e20 6120 6665 7720 2520 6f66   than a few % of
-00000ef0: 2074 6861 7420 696e 6c69 6e69 6e67 2061   that inlining a
-00000f00: 2074 6162 6c65 2e0a 2320 416c 736f 206d   table..# Also m
-00000f10: 7573 7420 6173 7375 6d65 2074 6861 7420  ust assume that 
-00000f20: 7465 7874 2065 6e63 6f64 696e 6720 6173  text encoding as
-00000f30: 206c 6974 6572 616c 7320 6973 206d 7563   literals is muc
-00000f40: 6820 6c65 7373 2065 6666 6963 6965 6e74  h less efficient
-00000f50: 2074 6861 6e20 696e 2d6d 656d 6f72 7920   than in-memory 
-00000f60: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
-00000f70: 4d41 585f 494e 4c49 4e45 5f44 465f 4259  MAX_INLINE_DF_BY
-00000f80: 5445 5320 3d20 3530 3030 0a0a 2320 4d61  TES = 5000..# Ma
-00000f90: 7820 636f 6d70 6c65 7869 7479 2074 6861  x complexity tha
-00000fa0: 7420 7368 6f75 6c64 2062 6520 6578 6563  t should be exec
-00000fb0: 7574 6564 2061 7320 6120 7369 6e67 6c65  uted as a single
-00000fc0: 2071 7565 7279 0a51 5545 5259 5f43 4f4d   query.QUERY_COM
-00000fd0: 504c 4558 4954 595f 4c49 4d49 5420 3d20  PLEXITY_LIMIT = 
-00000fe0: 3165 370a 2320 4e75 6d62 6572 206f 6620  1e7.# Number of 
-00000ff0: 7469 6d65 7320 746f 2066 6163 746f 7220  times to factor 
-00001000: 6f75 7420 7375 6271 7565 7269 6573 2062  out subqueries b
-00001010: 6566 6f72 6520 6769 7669 6e67 2075 702e  efore giving up.
-00001020: 0a4d 4158 5f53 5542 5452 4545 5f46 4143  .MAX_SUBTREE_FAC
-00001030: 544f 5249 4e47 5320 3d20 350a 0a6c 6f67  TORINGS = 5..log
-00001040: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-00001050: 744c 6f67 6765 7228 5f5f 6e61 6d65 5f5f  tLogger(__name__
-00001060: 290a 0a23 2045 7863 6c75 6465 7320 6765  )..# Excludes ge
-00001070: 6f67 7261 7068 792c 2062 7974 6573 2c20  ography, bytes, 
-00001080: 616e 6420 6e65 7374 6564 2028 6172 7261  and nested (arra
-00001090: 792c 2073 7472 7563 7429 2064 6174 6174  y, struct) datat
-000010a0: 7970 6573 0a49 4e4c 494e 4142 4c45 5f44  ypes.INLINABLE_D
-000010b0: 5459 5045 533a 2053 6571 7565 6e63 655b  TYPES: Sequence[
-000010c0: 6269 6766 7261 6d65 732e 6474 7970 6573  bigframes.dtypes
-000010d0: 2e44 7479 7065 5d20 3d20 280a 2020 2020  .Dtype] = (.    
-000010e0: 7061 6e64 6173 2e42 6f6f 6c65 616e 4474  pandas.BooleanDt
-000010f0: 7970 6528 292c 0a20 2020 2070 616e 6461  ype(),.    panda
-00001100: 732e 466c 6f61 7436 3444 7479 7065 2829  s.Float64Dtype()
-00001110: 2c0a 2020 2020 7061 6e64 6173 2e49 6e74  ,.    pandas.Int
-00001120: 3634 4474 7970 6528 292c 0a20 2020 2070  64Dtype(),.    p
-00001130: 616e 6461 732e 5374 7269 6e67 4474 7970  andas.StringDtyp
-00001140: 6528 7374 6f72 6167 653d 2270 7961 7272  e(storage="pyarr
-00001150: 6f77 2229 2c0a 2020 2020 7061 6e64 6173  ow"),.    pandas
-00001160: 2e41 7272 6f77 4474 7970 6528 7061 2e64  .ArrowDtype(pa.d
-00001170: 6174 6533 3228 2929 2c0a 2020 2020 7061  ate32()),.    pa
-00001180: 6e64 6173 2e41 7272 6f77 4474 7970 6528  ndas.ArrowDtype(
-00001190: 7061 2e74 696d 6536 3428 2275 7322 2929  pa.time64("us"))
-000011a0: 2c0a 2020 2020 7061 6e64 6173 2e41 7272  ,.    pandas.Arr
-000011b0: 6f77 4474 7970 6528 7061 2e74 696d 6573  owDtype(pa.times
-000011c0: 7461 6d70 2822 7573 2229 292c 0a20 2020  tamp("us")),.   
-000011d0: 2070 616e 6461 732e 4172 726f 7744 7479   pandas.ArrowDty
-000011e0: 7065 2870 612e 7469 6d65 7374 616d 7028  pe(pa.timestamp(
-000011f0: 2275 7322 2c20 747a 3d22 5554 4322 2929  "us", tz="UTC"))
-00001200: 2c0a 2020 2020 7061 6e64 6173 2e41 7272  ,.    pandas.Arr
-00001210: 6f77 4474 7970 6528 7061 2e64 6563 696d  owDtype(pa.decim
-00001220: 616c 3132 3828 3338 2c20 3929 292c 0a20  al128(38, 9)),. 
-00001230: 2020 2070 616e 6461 732e 4172 726f 7744     pandas.ArrowD
-00001240: 7479 7065 2870 612e 6465 6369 6d61 6c32  type(pa.decimal2
-00001250: 3536 2837 362c 2033 3829 292c 0a29 0a0a  56(76, 38)),.)..
-00001260: 0a64 6566 205f 6973 5f71 7565 7279 2871  .def _is_query(q
-00001270: 7565 7279 5f6f 725f 7461 626c 653a 2073  uery_or_table: s
-00001280: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
-00001290: 2022 2222 4465 7465 726d 696e 6520 6966   """Determine if
-000012a0: 2060 7175 6572 795f 6f72 5f74 6162 6c65   `query_or_table
-000012b0: 6020 6973 2061 2074 6162 6c65 2049 4420  ` is a table ID 
-000012c0: 6f72 2061 2053 514c 2073 7472 696e 6722  or a SQL string"
-000012d0: 2222 0a20 2020 2072 6574 7572 6e20 7265  "".    return re
-000012e0: 2e73 6561 7263 6828 7222 5c73 222c 2071  .search(r"\s", q
-000012f0: 7565 7279 5f6f 725f 7461 626c 652e 7374  uery_or_table.st
-00001300: 7269 7028 292c 2072 652e 4d55 4c54 494c  rip(), re.MULTIL
-00001310: 494e 4529 2069 7320 6e6f 7420 4e6f 6e65  INE) is not None
-00001320: 0a0a 0a64 6566 205f 6973 5f74 6162 6c65  ...def _is_table
-00001330: 5f77 6974 685f 7769 6c64 6361 7264 5f73  _with_wildcard_s
-00001340: 7566 6669 7828 7175 6572 795f 6f72 5f74  uffix(query_or_t
-00001350: 6162 6c65 3a20 7374 7229 202d 3e20 626f  able: str) -> bo
-00001360: 6f6c 3a0a 2020 2020 2222 2244 6574 6572  ol:.    """Deter
-00001370: 6d69 6e65 2069 6620 6071 7565 7279 5f6f  mine if `query_o
-00001380: 725f 7461 626c 6560 2069 7320 6120 7461  r_table` is a ta
-00001390: 626c 6520 616e 6420 636f 6e74 6169 6e73  ble and contains
-000013a0: 2061 2077 696c 6463 6172 6420 7375 6666   a wildcard suff
-000013b0: 6978 2e22 2222 0a20 2020 2072 6574 7572  ix.""".    retur
-000013c0: 6e20 6e6f 7420 5f69 735f 7175 6572 7928  n not _is_query(
-000013d0: 7175 6572 795f 6f72 5f74 6162 6c65 2920  query_or_table) 
-000013e0: 616e 6420 7175 6572 795f 6f72 5f74 6162  and query_or_tab
-000013f0: 6c65 2e65 6e64 7377 6974 6828 222a 2229  le.endswith("*")
-00001400: 0a0a 0a63 6c61 7373 2053 6573 7369 6f6e  ...class Session
-00001410: 280a 2020 2020 7468 6972 645f 7061 7274  (.    third_part
-00001420: 795f 7061 6e64 6173 5f67 6271 2e47 4251  y_pandas_gbq.GBQ
-00001430: 494f 4d69 7869 6e2c 0a20 2020 2074 6869  IOMixin,.    thi
-00001440: 7264 5f70 6172 7479 5f70 616e 6461 735f  rd_party_pandas_
-00001450: 7061 7271 7565 742e 5061 7271 7565 7449  parquet.ParquetI
-00001460: 4f4d 6978 696e 2c0a 2020 2020 7468 6972  OMixin,.    thir
-00001470: 645f 7061 7274 795f 7061 6e64 6173 5f70  d_party_pandas_p
-00001480: 6963 6b6c 652e 5069 636b 6c65 494f 4d69  ickle.PickleIOMi
-00001490: 7869 6e2c 0a20 2020 2074 6869 7264 5f70  xin,.    third_p
-000014a0: 6172 7479 5f70 616e 6461 735f 7265 6164  arty_pandas_read
-000014b0: 6572 732e 5265 6164 6572 494f 4d69 7869  ers.ReaderIOMixi
-000014c0: 6e2c 0a29 3a0a 2020 2020 2222 2245 7374  n,.):.    """Est
-000014d0: 6162 6c69 7368 6573 2061 2042 6967 5175  ablishes a BigQu
-000014e0: 6572 7920 636f 6e6e 6563 7469 6f6e 2074  ery connection t
-000014f0: 6f20 6361 7074 7572 6520 6120 6772 6f75  o capture a grou
-00001500: 7020 6f66 206a 6f62 2061 6374 6976 6974  p of job activit
-00001510: 6965 7320 7265 6c61 7465 6420 746f 0a20  ies related to. 
-00001520: 2020 2044 6174 6146 7261 6d65 732e 0a0a     DataFrames...
-00001530: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00001540: 2020 636f 6e74 6578 7420 2862 6967 6672    context (bigfr
-00001550: 616d 6573 2e5f 636f 6e66 6967 2e62 6967  ames._config.big
-00001560: 7175 6572 795f 6f70 7469 6f6e 732e 4269  query_options.Bi
-00001570: 6751 7565 7279 4f70 7469 6f6e 7329 3a0a  gQueryOptions):.
-00001580: 2020 2020 2020 2020 2020 2020 436f 6e66              Conf
-00001590: 6967 7572 6174 696f 6e20 6164 6a75 7374  iguration adjust
-000015a0: 696e 6720 686f 7720 746f 2063 6f6e 6e65  ing how to conne
-000015b0: 6374 2074 6f20 4269 6751 7565 7279 2061  ct to BigQuery a
-000015c0: 6e64 2072 656c 6174 6564 0a20 2020 2020  nd related.     
-000015d0: 2020 2020 2020 2041 5049 732e 204e 6f74         APIs. Not
-000015e0: 6520 7468 6174 2073 6f6d 6520 6f70 7469  e that some opti
-000015f0: 6f6e 7320 6172 6520 6967 6e6f 7265 6420  ons are ignored 
-00001600: 6966 2060 6063 6c69 656e 7473 5f70 726f  if ``clients_pro
-00001610: 7669 6465 7260 6020 6973 0a20 2020 2020  vider`` is.     
-00001620: 2020 2020 2020 2073 6574 2e0a 2020 2020         set..    
-00001630: 2020 2020 636c 6965 6e74 735f 7072 6f76      clients_prov
-00001640: 6964 6572 2028 6269 6766 7261 6d65 732e  ider (bigframes.
-00001650: 7365 7373 696f 6e2e 636c 6965 6e74 732e  session.clients.
-00001660: 436c 6965 6e74 7350 726f 7669 6465 7229  ClientsProvider)
-00001670: 3a0a 2020 2020 2020 2020 2020 2020 416e  :.            An
-00001680: 206f 626a 6563 7420 7072 6f76 6964 696e   object providin
-00001690: 6720 636c 6965 6e74 206c 6962 7261 7279  g client library
-000016a0: 206f 626a 6563 7473 2e0a 2020 2020 2222   objects..    ""
-000016b0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-000016c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000016d0: 662c 0a20 2020 2020 2020 2063 6f6e 7465  f,.        conte
-000016e0: 7874 3a20 4f70 7469 6f6e 616c 5b62 6967  xt: Optional[big
-000016f0: 7175 6572 795f 6f70 7469 6f6e 732e 4269  query_options.Bi
-00001700: 6751 7565 7279 4f70 7469 6f6e 735d 203d  gQueryOptions] =
-00001710: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00001720: 6c69 656e 7473 5f70 726f 7669 6465 723a  lients_provider:
-00001730: 204f 7074 696f 6e61 6c5b 6269 6766 7261   Optional[bigfra
-00001740: 6d65 732e 7365 7373 696f 6e2e 636c 6965  mes.session.clie
-00001750: 6e74 732e 436c 6965 6e74 7350 726f 7669  nts.ClientsProvi
-00001760: 6465 725d 203d 204e 6f6e 652c 0a20 2020  der] = None,.   
-00001770: 2029 3a0a 2020 2020 2020 2020 6966 2063   ):.        if c
-00001780: 6f6e 7465 7874 2069 7320 4e6f 6e65 3a0a  ontext is None:.
-00001790: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000017a0: 6578 7420 3d20 6269 6771 7565 7279 5f6f  ext = bigquery_o
-000017b0: 7074 696f 6e73 2e42 6967 5175 6572 794f  ptions.BigQueryO
-000017c0: 7074 696f 6e73 2829 0a0a 2020 2020 2020  ptions()..      
-000017d0: 2020 2320 544f 444f 2873 7761 7374 293a    # TODO(swast):
-000017e0: 2047 6574 206c 6f63 6174 696f 6e20 6672   Get location fr
-000017f0: 6f6d 2074 6865 2065 6e76 6972 6f6e 6d65  om the environme
-00001800: 6e74 2e0a 2020 2020 2020 2020 6966 2063  nt..        if c
-00001810: 6f6e 7465 7874 2e6c 6f63 6174 696f 6e20  ontext.location 
-00001820: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00001830: 2020 2020 2073 656c 662e 5f6c 6f63 6174       self._locat
-00001840: 696f 6e20 3d20 2255 5322 0a20 2020 2020  ion = "US".     
-00001850: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-00001860: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
-00001870: 2020 2020 2020 6622 4e6f 2065 7870 6c69        f"No expli
-00001880: 6369 7420 6c6f 6361 7469 6f6e 2069 7320  cit location is 
-00001890: 7365 742c 2073 6f20 7573 696e 6720 6c6f  set, so using lo
-000018a0: 6361 7469 6f6e 207b 7365 6c66 2e5f 6c6f  cation {self._lo
-000018b0: 6361 7469 6f6e 7d20 666f 7220 7468 6520  cation} for the 
-000018c0: 7365 7373 696f 6e2e 222c 0a20 2020 2020  session.",.     
-000018d0: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-000018e0: 6c65 7665 6c3d 322c 0a20 2020 2020 2020  level=2,.       
-000018f0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00001900: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00001910: 2073 656c 662e 5f6c 6f63 6174 696f 6e20   self._location 
-00001920: 3d20 636f 6e74 6578 742e 6c6f 6361 7469  = context.locati
-00001930: 6f6e 0a0a 2020 2020 2020 2020 7365 6c66  on..        self
-00001940: 2e5f 6271 5f6b 6d73 5f6b 6579 5f6e 616d  ._bq_kms_key_nam
-00001950: 6520 3d20 636f 6e74 6578 742e 6b6d 735f  e = context.kms_
-00001960: 6b65 795f 6e61 6d65 0a0a 2020 2020 2020  key_name..      
-00001970: 2020 2320 496e 7374 616e 7469 6174 6520    # Instantiate 
-00001980: 6120 636c 6965 6e74 7320 7072 6f76 6964  a clients provid
-00001990: 6572 2074 6f20 6865 6c70 2077 6974 6820  er to help with 
-000019a0: 636c 6f75 6420 636c 6965 6e74 7320 7468  cloud clients th
-000019b0: 6174 2077 696c 6c20 6265 0a20 2020 2020  at will be.     
-000019c0: 2020 2023 2075 7365 6420 696e 2074 6865     # used in the
-000019d0: 2066 7574 7572 6520 6f70 6572 6174 696f   future operatio
-000019e0: 6e73 2069 6e20 7468 6520 7365 7373 696f  ns in the sessio
-000019f0: 6e0a 2020 2020 2020 2020 6966 2063 6c69  n.        if cli
-00001a00: 656e 7473 5f70 726f 7669 6465 723a 0a20  ents_provider:. 
-00001a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001a20: 5f63 6c69 656e 7473 5f70 726f 7669 6465  _clients_provide
-00001a30: 7220 3d20 636c 6965 6e74 735f 7072 6f76  r = clients_prov
-00001a40: 6964 6572 0a20 2020 2020 2020 2065 6c73  ider.        els
-00001a50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00001a60: 656c 662e 5f63 6c69 656e 7473 5f70 726f  elf._clients_pro
-00001a70: 7669 6465 7220 3d20 6269 6766 7261 6d65  vider = bigframe
-00001a80: 732e 7365 7373 696f 6e2e 636c 6965 6e74  s.session.client
-00001a90: 732e 436c 6965 6e74 7350 726f 7669 6465  s.ClientsProvide
-00001aa0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00001ab0: 2020 2070 726f 6a65 6374 3d63 6f6e 7465     project=conte
-00001ac0: 7874 2e70 726f 6a65 6374 2c0a 2020 2020  xt.project,.    
-00001ad0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001ae0: 7469 6f6e 3d73 656c 662e 5f6c 6f63 6174  tion=self._locat
-00001af0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00001b00: 2020 2020 2075 7365 5f72 6567 696f 6e61       use_regiona
-00001b10: 6c5f 656e 6470 6f69 6e74 733d 636f 6e74  l_endpoints=cont
-00001b20: 6578 742e 7573 655f 7265 6769 6f6e 616c  ext.use_regional
-00001b30: 5f65 6e64 706f 696e 7473 2c0a 2020 2020  _endpoints,.    
-00001b40: 2020 2020 2020 2020 2020 2020 6372 6564              cred
-00001b50: 656e 7469 616c 733d 636f 6e74 6578 742e  entials=context.
-00001b60: 6372 6564 656e 7469 616c 732c 0a20 2020  credentials,.   
-00001b70: 2020 2020 2020 2020 2020 2020 2061 7070               app
-00001b80: 6c69 6361 7469 6f6e 5f6e 616d 653d 636f  lication_name=co
-00001b90: 6e74 6578 742e 6170 706c 6963 6174 696f  ntext.applicatio
-00001ba0: 6e5f 6e61 6d65 2c0a 2020 2020 2020 2020  n_name,.        
-00001bb0: 2020 2020 2020 2020 6271 5f6b 6d73 5f6b          bq_kms_k
-00001bc0: 6579 5f6e 616d 653d 7365 6c66 2e5f 6271  ey_name=self._bq
-00001bd0: 5f6b 6d73 5f6b 6579 5f6e 616d 652c 0a20  _kms_key_name,. 
-00001be0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00001bf0: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
-00001c00: 7465 5f62 715f 6461 7461 7365 7473 2829  te_bq_datasets()
-00001c10: 0a0a 2020 2020 2020 2020 2320 544f 444f  ..        # TODO
-00001c20: 2873 686f 6273 293a 2052 656d 6f76 6520  (shobs): Remove 
-00001c30: 7468 6973 206c 6f67 6963 2061 6674 6572  this logic after
-00001c40: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00001c50: 636f 6d2f 6962 6973 2d70 726f 6a65 6374  com/ibis-project
-00001c60: 2f69 6269 732f 6973 7375 6573 2f38 3439  /ibis/issues/849
-00001c70: 340a 2020 2020 2020 2020 2320 6861 7320  4.        # has 
-00001c80: 6265 656e 2066 6978 6564 2e20 5468 6520  been fixed. The 
-00001c90: 6962 6973 2063 6c69 656e 7420 6368 616e  ibis client chan
-00001ca0: 6765 7320 7468 6520 6465 6661 756c 7420  ges the default 
-00001cb0: 7175 6572 7920 6a6f 6220 636f 6e66 6967  query job config
-00001cc0: 0a20 2020 2020 2020 2023 2073 6f20 7765  .        # so we
-00001cd0: 2061 7265 2067 6f69 6e67 2074 6f20 7265   are going to re
-00001ce0: 6d65 6d62 6572 2074 6865 2063 7572 7265  member the curre
-00001cf0: 6e74 2063 6f6e 6669 6720 616e 6420 7265  nt config and re
-00001d00: 7374 6f72 6520 6974 2061 6674 6572 0a20  store it after. 
-00001d10: 2020 2020 2020 2023 2074 6865 2069 6269         # the ibi
-00001d20: 7320 636c 6965 6e74 2068 6173 2062 6565  s client has bee
-00001d30: 6e20 6372 6561 7465 640a 2020 2020 2020  n created.      
-00001d40: 2020 6f72 6967 696e 616c 5f64 6566 6175    original_defau
-00001d50: 6c74 5f71 7565 7279 5f6a 6f62 5f63 6f6e  lt_query_job_con
-00001d60: 6669 6720 3d20 7365 6c66 2e62 7163 6c69  fig = self.bqcli
-00001d70: 656e 742e 6465 6661 756c 745f 7175 6572  ent.default_quer
-00001d80: 795f 6a6f 625f 636f 6e66 6967 0a0a 2020  y_job_config..  
-00001d90: 2020 2020 2020 7365 6c66 2e69 6269 735f        self.ibis_
-00001da0: 636c 6965 6e74 203d 2074 7970 696e 672e  client = typing.
-00001db0: 6361 7374 280a 2020 2020 2020 2020 2020  cast(.          
-00001dc0: 2020 6962 6973 5f62 6967 7175 6572 792e    ibis_bigquery.
-00001dd0: 4261 636b 656e 642c 0a20 2020 2020 2020  Backend,.       
-00001de0: 2020 2020 2069 6269 732e 6269 6771 7565       ibis.bigque
-00001df0: 7279 2e63 6f6e 6e65 6374 280a 2020 2020  ry.connect(.    
-00001e00: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
-00001e10: 6563 745f 6964 3d63 6f6e 7465 7874 2e70  ect_id=context.p
-00001e20: 726f 6a65 6374 2c0a 2020 2020 2020 2020  roject,.        
-00001e30: 2020 2020 2020 2020 636c 6965 6e74 3d73          client=s
-00001e40: 656c 662e 6271 636c 6965 6e74 2c0a 2020  elf.bqclient,.  
-00001e50: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00001e60: 6f72 6167 655f 636c 6965 6e74 3d73 656c  orage_client=sel
-00001e70: 662e 6271 7374 6f72 6167 6572 6561 6463  f.bqstoragereadc
-00001e80: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
-00001e90: 2020 2029 2c0a 2020 2020 2020 2020 290a     ),.        ).
-00001ea0: 0a20 2020 2020 2020 2073 656c 662e 6271  .        self.bq
-00001eb0: 636c 6965 6e74 2e64 6566 6175 6c74 5f71  client.default_q
-00001ec0: 7565 7279 5f6a 6f62 5f63 6f6e 6669 6720  uery_job_config 
-00001ed0: 3d20 6f72 6967 696e 616c 5f64 6566 6175  = original_defau
-00001ee0: 6c74 5f71 7565 7279 5f6a 6f62 5f63 6f6e  lt_query_job_con
-00001ef0: 6669 670a 0a20 2020 2020 2020 2023 2052  fig..        # R
-00001f00: 6573 6f6c 7665 2074 6865 2042 5120 636f  esolve the BQ co
-00001f10: 6e6e 6563 7469 6f6e 2066 6f72 2072 656d  nnection for rem
-00001f20: 6f74 6520 6675 6e63 7469 6f6e 2061 6e64  ote function and
-00001f30: 2056 6572 7465 7820 4149 2069 6e74 6567   Vertex AI integ
-00001f40: 7261 7469 6f6e 0a20 2020 2020 2020 2073  ration.        s
-00001f50: 656c 662e 5f62 715f 636f 6e6e 6563 7469  elf._bq_connecti
-00001f60: 6f6e 203d 2063 6f6e 7465 7874 2e62 715f  on = context.bq_
-00001f70: 636f 6e6e 6563 7469 6f6e 206f 7220 5f42  connection or _B
-00001f80: 4947 4652 414d 4553 5f44 4546 4155 4c54  IGFRAMES_DEFAULT
-00001f90: 5f43 4f4e 4e45 4354 494f 4e5f 4944 0a20  _CONNECTION_ID. 
-00001fa0: 2020 2020 2020 2073 656c 662e 5f73 6b69         self._ski
-00001fb0: 705f 6271 5f63 6f6e 6e65 6374 696f 6e5f  p_bq_connection_
-00001fc0: 6368 6563 6b20 3d20 636f 6e74 6578 742e  check = context.
-00001fd0: 5f73 6b69 705f 6271 5f63 6f6e 6e65 6374  _skip_bq_connect
-00001fe0: 696f 6e5f 6368 6563 6b0a 0a20 2020 2020  ion_check..     
-00001ff0: 2020 2023 204e 6f77 2074 6861 7420 7765     # Now that we
-00002000: 2772 6520 7374 6172 7469 6e67 2074 6865  're starting the
-00002010: 2073 6573 7369 6f6e 2c20 646f 6e27 7420   session, don't 
-00002020: 616c 6c6f 7720 7468 6520 6f70 7469 6f6e  allow the option
-00002030: 7320 746f 2062 650a 2020 2020 2020 2020  s to be.        
-00002040: 2320 6368 616e 6765 642e 0a20 2020 2020  # changed..     
-00002050: 2020 2063 6f6e 7465 7874 2e5f 7365 7373     context._sess
-00002060: 696f 6e5f 7374 6172 7465 6420 3d20 5472  ion_started = Tr
-00002070: 7565 0a20 2020 2020 2020 2073 656c 662e  ue.        self.
-00002080: 5f64 665f 736e 6170 7368 6f74 3a20 4469  _df_snapshot: Di
-00002090: 6374 5b62 6967 7175 6572 792e 5461 626c  ct[bigquery.Tabl
-000020a0: 6552 6566 6572 656e 6365 2c20 6461 7465  eReference, date
-000020b0: 7469 6d65 2e64 6174 6574 696d 655d 203d  time.datetime] =
-000020c0: 207b 7d0a 0a20 2020 2040 7072 6f70 6572   {}..    @proper
-000020d0: 7479 0a20 2020 2064 6566 2062 7163 6c69  ty.    def bqcli
-000020e0: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
-000020f0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00002100: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
-00002110: 2e62 7163 6c69 656e 740a 0a20 2020 2040  .bqclient..    @
-00002120: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00002130: 2062 7163 6f6e 6e65 6374 696f 6e63 6c69   bqconnectioncli
-00002140: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
-00002150: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00002160: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
-00002170: 2e62 7163 6f6e 6e65 6374 696f 6e63 6c69  .bqconnectioncli
-00002180: 656e 740a 0a20 2020 2040 7072 6f70 6572  ent..    @proper
-00002190: 7479 0a20 2020 2064 6566 2062 7173 746f  ty.    def bqsto
-000021a0: 7261 6765 7265 6164 636c 6965 6e74 2873  ragereadclient(s
-000021b0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-000021c0: 7475 726e 2073 656c 662e 5f63 6c69 656e  turn self._clien
-000021d0: 7473 5f70 726f 7669 6465 722e 6271 7374  ts_provider.bqst
-000021e0: 6f72 6167 6572 6561 6463 6c69 656e 740a  oragereadclient.
-000021f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00002200: 2020 2064 6566 2063 6c6f 7564 6675 6e63     def cloudfunc
-00002210: 7469 6f6e 7363 6c69 656e 7428 7365 6c66  tionsclient(self
-00002220: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00002230: 6e20 7365 6c66 2e5f 636c 6965 6e74 735f  n self._clients_
-00002240: 7072 6f76 6964 6572 2e63 6c6f 7564 6675  provider.cloudfu
-00002250: 6e63 7469 6f6e 7363 6c69 656e 740a 0a20  nctionsclient.. 
-00002260: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00002270: 2064 6566 2072 6573 6f75 7263 656d 616e   def resourceman
-00002280: 6167 6572 636c 6965 6e74 2873 656c 6629  agerclient(self)
-00002290: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000022a0: 2073 656c 662e 5f63 6c69 656e 7473 5f70   self._clients_p
-000022b0: 726f 7669 6465 722e 7265 736f 7572 6365  rovider.resource
-000022c0: 6d61 6e61 6765 7263 6c69 656e 740a 0a20  managerclient.. 
-000022d0: 2020 205f 6271 5f63 6f6e 6e65 6374 696f     _bq_connectio
-000022e0: 6e5f 6d61 6e61 6765 723a 204f 7074 696f  n_manager: Optio
-000022f0: 6e61 6c5b 6269 6766 7261 6d65 732e 636c  nal[bigframes.cl
-00002300: 6965 6e74 732e 4271 436f 6e6e 6563 7469  ients.BqConnecti
-00002310: 6f6e 4d61 6e61 6765 725d 203d 204e 6f6e  onManager] = Non
-00002320: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00002330: 0a20 2020 2064 6566 2062 7163 6f6e 6e65  .    def bqconne
-00002340: 6374 696f 6e6d 616e 6167 6572 2873 656c  ctionmanager(sel
-00002350: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
-00002360: 6f74 2073 656c 662e 5f73 6b69 705f 6271  ot self._skip_bq
-00002370: 5f63 6f6e 6e65 6374 696f 6e5f 6368 6563  _connection_chec
-00002380: 6b20 616e 6420 6e6f 7420 7365 6c66 2e5f  k and not self._
-00002390: 6271 5f63 6f6e 6e65 6374 696f 6e5f 6d61  bq_connection_ma
-000023a0: 6e61 6765 723a 0a20 2020 2020 2020 2020  nager:.         
-000023b0: 2020 2073 656c 662e 5f62 715f 636f 6e6e     self._bq_conn
-000023c0: 6563 7469 6f6e 5f6d 616e 6167 6572 203d  ection_manager =
-000023d0: 2062 6967 6672 616d 6573 2e63 6c69 656e   bigframes.clien
-000023e0: 7473 2e42 7143 6f6e 6e65 6374 696f 6e4d  ts.BqConnectionM
-000023f0: 616e 6167 6572 280a 2020 2020 2020 2020  anager(.        
-00002400: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
-00002410: 6f6e 6e65 6374 696f 6e63 6c69 656e 742c  onnectionclient,
-00002420: 2073 656c 662e 7265 736f 7572 6365 6d61   self.resourcema
-00002430: 6e61 6765 7263 6c69 656e 740a 2020 2020  nagerclient.    
-00002440: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00002450: 2020 7265 7475 726e 2073 656c 662e 5f62    return self._b
-00002460: 715f 636f 6e6e 6563 7469 6f6e 5f6d 616e  q_connection_man
-00002470: 6167 6572 0a0a 2020 2020 4070 726f 7065  ager..    @prope
-00002480: 7274 790a 2020 2020 6465 6620 5f70 726f  rty.    def _pro
-00002490: 6a65 6374 2873 656c 6629 3a0a 2020 2020  ject(self):.    
-000024a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000024b0: 6271 636c 6965 6e74 2e70 726f 6a65 6374  bqclient.project
-000024c0: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
-000024d0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-000024e0: 2020 2320 5374 6162 6c65 2068 6173 6820    # Stable hash 
-000024f0: 6e65 6564 6564 2074 6f20 7573 6520 696e  needed to use in
-00002500: 2065 7870 7265 7373 696f 6e20 7472 6565   expression tree
-00002510: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002520: 6861 7368 2873 7472 2873 656c 662e 5f61  hash(str(self._a
-00002530: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
-00002540: 2929 0a0a 2020 2020 6465 6620 5f63 7265  ))..    def _cre
-00002550: 6174 655f 6271 5f64 6174 6173 6574 7328  ate_bq_datasets(
-00002560: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00002570: 2222 4372 6561 7465 2061 6e64 2069 6465  ""Create and ide
-00002580: 6e74 6966 7920 6461 7461 7365 7428 7329  ntify dataset(s)
-00002590: 2066 6f72 2074 656d 706f 7261 7279 2042   for temporary B
-000025a0: 5120 7265 736f 7572 6365 732e 2222 220a  Q resources.""".
-000025b0: 2020 2020 2020 2020 7175 6572 795f 6a6f          query_jo
-000025c0: 6220 3d20 7365 6c66 2e62 7163 6c69 656e  b = self.bqclien
-000025d0: 742e 7175 6572 7928 2253 454c 4543 5420  t.query("SELECT 
-000025e0: 3122 2c20 6c6f 6361 7469 6f6e 3d73 656c  1", location=sel
-000025f0: 662e 5f6c 6f63 6174 696f 6e29 0a20 2020  f._location).   
-00002600: 2020 2020 2071 7565 7279 5f6a 6f62 2e72       query_job.r
-00002610: 6573 756c 7428 2920 2023 2062 6c6f 636b  esult()  # block
-00002620: 7320 756e 7469 6c20 6669 6e69 7368 6564  s until finished
-00002630: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
-00002640: 616e 6f6e 796d 6f75 7320 6461 7461 7365  anonymous datase
-00002650: 7420 6973 2075 7365 6420 6279 2042 6967  t is used by Big
-00002660: 5175 6572 7920 746f 2077 7269 7465 2071  Query to write q
-00002670: 7565 7279 2072 6573 756c 7473 2061 6e64  uery results and
-00002680: 0a20 2020 2020 2020 2023 2073 6573 7369  .        # sessi
-00002690: 6f6e 2074 6162 6c65 732e 2042 6967 5175  on tables. BigQu
-000026a0: 6572 7920 4461 7461 4672 616d 6573 2061  ery DataFrames a
-000026b0: 6c73 6f20 7772 6974 6573 2074 656d 7020  lso writes temp 
-000026c0: 7461 626c 6573 2064 6972 6563 746c 790a  tables directly.
-000026d0: 2020 2020 2020 2020 2320 746f 2074 6865          # to the
-000026e0: 2064 6174 6173 6574 2c20 6e6f 2042 6967   dataset, no Big
-000026f0: 5175 6572 7920 5365 7373 696f 6e20 7265  Query Session re
-00002700: 7175 6972 6564 2e20 4e6f 7465 3a20 7468  quired. Note: th
-00002710: 6572 6520 6973 2061 0a20 2020 2020 2020  ere is a.       
-00002720: 2023 2064 6966 6665 7265 6e74 2061 6e6f   # different ano
-00002730: 6e79 6d6f 7573 2064 6174 6173 6574 2070  nymous dataset p
-00002740: 6572 206c 6f63 6174 696f 6e2e 2053 6565  er location. See
-00002750: 3a0a 2020 2020 2020 2020 2320 6874 7470  :.        # http
-00002760: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
-00002770: 2e63 6f6d 2f62 6967 7175 6572 792f 646f  .com/bigquery/do
-00002780: 6373 2f63 6163 6865 642d 7265 7375 6c74  cs/cached-result
-00002790: 7323 686f 775f 6361 6368 6564 5f72 6573  s#how_cached_res
-000027a0: 756c 7473 5f61 7265 5f73 746f 7265 640a  ults_are_stored.
-000027b0: 2020 2020 2020 2020 7175 6572 795f 6465          query_de
-000027c0: 7374 696e 6174 696f 6e20 3d20 7175 6572  stination = quer
-000027d0: 795f 6a6f 622e 6465 7374 696e 6174 696f  y_job.destinatio
-000027e0: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
-000027f0: 616e 6f6e 796d 6f75 735f 6461 7461 7365  anonymous_datase
-00002800: 7420 3d20 6269 6771 7565 7279 2e44 6174  t = bigquery.Dat
-00002810: 6173 6574 5265 6665 7265 6e63 6528 0a20  asetReference(. 
-00002820: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00002830: 5f64 6573 7469 6e61 7469 6f6e 2e70 726f  _destination.pro
-00002840: 6a65 6374 2c0a 2020 2020 2020 2020 2020  ject,.          
-00002850: 2020 7175 6572 795f 6465 7374 696e 6174    query_destinat
-00002860: 696f 6e2e 6461 7461 7365 745f 6964 2c0a  ion.dataset_id,.
-00002870: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00002880: 6566 2063 6c6f 7365 2873 656c 6629 3a0a  ef close(self):.
-00002890: 2020 2020 2020 2020 2222 224e 6f2d 6f70          """No-op
-000028a0: 2e20 5465 6d70 6f72 6172 7920 7265 736f  . Temporary reso
-000028b0: 7572 6365 7320 6172 6520 6465 6c65 7465  urces are delete
-000028c0: 6420 6166 7465 7220 3720 6461 7973 2e22  d after 7 days."
-000028d0: 2222 0a0a 2020 2020 6465 6620 7265 6164  ""..    def read
-000028e0: 5f67 6271 280a 2020 2020 2020 2020 7365  _gbq(.        se
-000028f0: 6c66 2c0a 2020 2020 2020 2020 7175 6572  lf,.        quer
-00002900: 795f 6f72 5f74 6162 6c65 3a20 7374 722c  y_or_table: str,
-00002910: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00002920: 2020 2020 696e 6465 785f 636f 6c3a 2049      index_col: I
-00002930: 7465 7261 626c 655b 7374 725d 207c 2073  terable[str] | s
-00002940: 7472 203d 2028 292c 0a20 2020 2020 2020  tr = (),.       
-00002950: 2063 6f6c 756d 6e73 3a20 4974 6572 6162   columns: Iterab
-00002960: 6c65 5b73 7472 5d20 3d20 2829 2c0a 2020  le[str] = (),.  
-00002970: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
-00002980: 696f 6e3a 204f 7074 696f 6e61 6c5b 4469  ion: Optional[Di
-00002990: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
-000029a0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
-000029b0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-000029c0: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
-000029d0: 696c 7465 7273 3a20 7468 6972 645f 7061  ilters: third_pa
-000029e0: 7274 795f 7061 6e64 6173 5f67 6271 2e46  rty_pandas_gbq.F
-000029f0: 696c 7465 7273 5479 7065 203d 2028 292c  iltersType = (),
-00002a00: 0a20 2020 2020 2020 2075 7365 5f63 6163  .        use_cac
-00002a10: 6865 3a20 4f70 7469 6f6e 616c 5b62 6f6f  he: Optional[boo
-00002a20: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
-00002a30: 2020 2063 6f6c 5f6f 7264 6572 3a20 4974     col_order: It
-00002a40: 6572 6162 6c65 5b73 7472 5d20 3d20 2829  erable[str] = ()
-00002a50: 2c0a 2020 2020 2020 2020 2320 4164 6420  ,.        # Add 
-00002a60: 6120 7665 7269 6679 2069 6e64 6578 2061  a verify index a
-00002a70: 7267 756d 656e 7420 7468 6174 2066 6169  rgument that fai
-00002a80: 6c73 2069 6620 7468 6520 696e 6465 7820  ls if the index 
-00002a90: 6973 206e 6f74 2075 6e69 7175 652e 0a20  is not unique.. 
-00002aa0: 2020 2029 202d 3e20 6461 7461 6672 616d     ) -> datafram
-00002ab0: 652e 4461 7461 4672 616d 653a 0a20 2020  e.DataFrame:.   
-00002ac0: 2020 2020 2023 2054 4f44 4f28 622f 3238       # TODO(b/28
-00002ad0: 3135 3731 3231 3429 3a20 4765 6e65 7261  1571214): Genera
-00002ae0: 7465 2070 726f 6d70 7420 746f 2073 686f  te prompt to sho
-00002af0: 7720 7468 6520 7072 6f67 7265 7373 206f  w the progress o
-00002b00: 6620 7265 6164 5f67 6271 2e0a 2020 2020  f read_gbq..    
-00002b10: 2020 2020 6966 2063 6f6c 756d 6e73 2061      if columns a
-00002b20: 6e64 2063 6f6c 5f6f 7264 6572 3a0a 2020  nd col_order:.  
-00002b30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002b40: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00002b50: 2020 2020 2020 2020 2020 2020 224d 7573              "Mus
-00002b60: 7420 7370 6563 6966 7920 6569 7468 6572  t specify either
-00002b70: 2063 6f6c 756d 6e73 2028 7072 6566 6572   columns (prefer
-00002b80: 7265 6429 206f 7220 636f 6c5f 6f72 6465  red) or col_orde
-00002b90: 722c 206e 6f74 2062 6f74 6822 0a20 2020  r, not both".   
-00002ba0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00002bb0: 2020 2065 6c69 6620 636f 6c5f 6f72 6465     elif col_orde
-00002bc0: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
-00002bd0: 6f6c 756d 6e73 203d 2063 6f6c 5f6f 7264  olumns = col_ord
-00002be0: 6572 0a0a 2020 2020 2020 2020 6669 6c74  er..        filt
-00002bf0: 6572 7320 3d20 6c69 7374 2866 696c 7465  ers = list(filte
-00002c00: 7273 290a 2020 2020 2020 2020 6966 206c  rs).        if l
-00002c10: 656e 2866 696c 7465 7273 2920 213d 2030  en(filters) != 0
-00002c20: 206f 7220 5f69 735f 7461 626c 655f 7769   or _is_table_wi
-00002c30: 7468 5f77 696c 6463 6172 645f 7375 6666  th_wildcard_suff
-00002c40: 6978 2871 7565 7279 5f6f 725f 7461 626c  ix(query_or_tabl
-00002c50: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00002c60: 7175 6572 795f 6f72 5f74 6162 6c65 203d  query_or_table =
-00002c70: 2073 656c 662e 5f74 6f5f 7175 6572 7928   self._to_query(
-00002c80: 7175 6572 795f 6f72 5f74 6162 6c65 2c20  query_or_table, 
-00002c90: 636f 6c75 6d6e 732c 2066 696c 7465 7273  columns, filters
-00002ca0: 290a 0a20 2020 2020 2020 2069 6620 5f69  )..        if _i
-00002cb0: 735f 7175 6572 7928 7175 6572 795f 6f72  s_query(query_or
-00002cc0: 5f74 6162 6c65 293a 0a20 2020 2020 2020  _table):.       
-00002cd0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00002ce0: 2e5f 7265 6164 5f67 6271 5f71 7565 7279  ._read_gbq_query
-00002cf0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00002d00: 2020 7175 6572 795f 6f72 5f74 6162 6c65    query_or_table
-00002d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002d20: 2020 696e 6465 785f 636f 6c3d 696e 6465    index_col=inde
-00002d30: 785f 636f 6c2c 0a20 2020 2020 2020 2020  x_col,.         
-00002d40: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
-00002d50: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
-00002d60: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-00002d70: 6174 696f 6e3d 636f 6e66 6967 7572 6174  ation=configurat
-00002d80: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00002d90: 2020 2020 206d 6178 5f72 6573 756c 7473       max_results
-00002da0: 3d6d 6178 5f72 6573 756c 7473 2c0a 2020  =max_results,.  
-00002db0: 2020 2020 2020 2020 2020 2020 2020 6170                ap
-00002dc0: 695f 6e61 6d65 3d22 7265 6164 5f67 6271  i_name="read_gbq
-00002dd0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002de0: 2020 2075 7365 5f63 6163 6865 3d75 7365     use_cache=use
-00002df0: 5f63 6163 6865 2c0a 2020 2020 2020 2020  _cache,.        
-00002e00: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00002e10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00002e20: 2320 544f 444f 2873 7761 7374 293a 2051  # TODO(swast): Q
-00002e30: 7565 7279 2074 6865 2073 6e61 7073 686f  uery the snapsho
-00002e40: 7420 7461 626c 6520 6275 7420 6d61 726b  t table but mark
-00002e50: 2069 7420 6173 2061 0a20 2020 2020 2020   it as a.       
-00002e60: 2020 2020 2023 2064 6574 6572 6d69 6e69       # determini
-00002e70: 7374 6963 2071 7565 7279 2073 6f20 7765  stic query so we
-00002e80: 2063 616e 2061 766f 6964 2073 6572 6961   can avoid seria
-00002e90: 6c69 7a69 6e67 2069 6620 7765 2068 6176  lizing if we hav
-00002ea0: 6520 610a 2020 2020 2020 2020 2020 2020  e a.            
-00002eb0: 2320 756e 6971 7565 2069 6e64 6578 2e0a  # unique index..
-00002ec0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00002ed0: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
-00002ee0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00002ef0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002f00: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2254 6865 2027 636f 6e66 6967 7572 6174  "The 'configurat
-00002f30: 696f 6e27 2061 7267 756d 656e 7420 6973  ion' argument is
-00002f40: 206e 6f74 2061 6c6c 6f77 6564 2077 6865   not allowed whe
-00002f50: 6e20 220a 2020 2020 2020 2020 2020 2020  n ".            
-00002f60: 2020 2020 2020 2020 2264 6972 6563 746c          "directl
-00002f70: 7920 7265 6164 696e 6720 6672 6f6d 2061  y reading from a
-00002f80: 2074 6162 6c65 2e20 506c 6561 7365 2072   table. Please r
-00002f90: 656d 6f76 6520 220a 2020 2020 2020 2020  emove ".        
-00002fa0: 2020 2020 2020 2020 2020 2020 2227 636f              "'co
-00002fb0: 6e66 6967 7572 6174 696f 6e27 206f 7220  nfiguration' or 
-00002fc0: 7573 6520 6120 7175 6572 792e 220a 2020  use a query.".  
-00002fd0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00002fe0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00002ff0: 7572 6e20 7365 6c66 2e5f 7265 6164 5f67  urn self._read_g
-00003000: 6271 5f74 6162 6c65 280a 2020 2020 2020  bq_table(.      
-00003010: 2020 2020 2020 2020 2020 7175 6572 795f            query_
-00003020: 6f72 5f74 6162 6c65 2c0a 2020 2020 2020  or_table,.      
-00003030: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-00003040: 636f 6c3d 696e 6465 785f 636f 6c2c 0a20  col=index_col,. 
-00003050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003060: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 2c0a  olumns=columns,.
-00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003080: 6d61 785f 7265 7375 6c74 733d 6d61 785f  max_results=max_
-00003090: 7265 7375 6c74 732c 0a20 2020 2020 2020  results,.       
-000030a0: 2020 2020 2020 2020 2061 7069 5f6e 616d           api_nam
-000030b0: 653d 2272 6561 645f 6762 7122 2c0a 2020  e="read_gbq",.  
-000030c0: 2020 2020 2020 2020 2020 2020 2020 7573                us
-000030d0: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
-000030e0: 6520 6966 2075 7365 5f63 6163 6865 2069  e if use_cache i
-000030f0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00003100: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00003110: 2020 290a 0a20 2020 2064 6566 205f 746f    )..    def _to
-00003120: 5f71 7565 7279 280a 2020 2020 2020 2020  _query(.        
-00003130: 7365 6c66 2c0a 2020 2020 2020 2020 7175  self,.        qu
-00003140: 6572 795f 6f72 5f74 6162 6c65 3a20 7374  ery_or_table: st
-00003150: 722c 0a20 2020 2020 2020 2063 6f6c 756d  r,.        colum
-00003160: 6e73 3a20 4974 6572 6162 6c65 5b73 7472  ns: Iterable[str
-00003170: 5d2c 0a20 2020 2020 2020 2066 696c 7465  ],.        filte
-00003180: 7273 3a20 7468 6972 645f 7061 7274 795f  rs: third_party_
-00003190: 7061 6e64 6173 5f67 6271 2e46 696c 7465  pandas_gbq.Filte
-000031a0: 7273 5479 7065 2c0a 2020 2020 2920 2d3e  rsType,.    ) ->
-000031b0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-000031c0: 2243 6f6d 7069 6c65 2071 7565 7279 5f6f  "Compile query_o
-000031d0: 725f 7461 626c 6520 7769 7468 2063 6f6e  r_table with con
-000031e0: 6469 7469 6f6e 7328 6669 6c74 6572 732c  ditions(filters,
-000031f0: 2077 696c 6463 6172 6473 2920 746f 2071   wildcards) to q
-00003200: 7565 7279 2e22 2222 0a20 2020 2020 2020  uery.""".       
-00003210: 2066 696c 7465 7273 203d 206c 6973 7428   filters = list(
-00003220: 6669 6c74 6572 7329 0a20 2020 2020 2020  filters).       
-00003230: 2073 7562 5f71 7565 7279 203d 2028 0a20   sub_query = (. 
-00003240: 2020 2020 2020 2020 2020 2066 2228 7b71             f"({q
-00003250: 7565 7279 5f6f 725f 7461 626c 657d 2922  uery_or_table})"
-00003260: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003270: 5f69 735f 7175 6572 7928 7175 6572 795f  _is_query(query_
-00003280: 6f72 5f74 6162 6c65 290a 2020 2020 2020  or_table).      
-00003290: 2020 2020 2020 656c 7365 2066 2260 7b71        else f"`{q
-000032a0: 7565 7279 5f6f 725f 7461 626c 657d 6022  uery_or_table}`"
-000032b0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000032c0: 2020 2020 7365 6c65 6374 5f63 6c61 7573      select_claus
-000032d0: 6520 3d20 2253 454c 4543 5420 2220 2b20  e = "SELECT " + 
-000032e0: 280a 2020 2020 2020 2020 2020 2020 222c  (.            ",
-000032f0: 2022 2e6a 6f69 6e28 6622 607b 636f 6c75   ".join(f"`{colu
-00003300: 6d6e 7d60 2220 666f 7220 636f 6c75 6d6e  mn}`" for column
-00003310: 2069 6e20 636f 6c75 6d6e 7329 2069 6620   in columns) if 
-00003320: 636f 6c75 6d6e 7320 656c 7365 2022 2a22  columns else "*"
-00003330: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00003340: 2020 2020 7768 6572 655f 636c 6175 7365      where_clause
-00003350: 203d 2022 220a 2020 2020 2020 2020 6966   = "".        if
-00003360: 2066 696c 7465 7273 3a0a 2020 2020 2020   filters:.      
-00003370: 2020 2020 2020 7661 6c69 645f 6f70 6572        valid_oper
-00003380: 6174 6f72 733a 204d 6170 7069 6e67 5b74  ators: Mapping[t
-00003390: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
-000033a0: 735f 6762 712e 4669 6c74 6572 4f70 732c  s_gbq.FilterOps,
-000033b0: 2073 7472 5d20 3d20 7b0a 2020 2020 2020   str] = {.      
-000033c0: 2020 2020 2020 2020 2020 2269 6e22 3a20            "in": 
-000033d0: 2249 4e22 2c0a 2020 2020 2020 2020 2020  "IN",.          
-000033e0: 2020 2020 2020 226e 6f74 2069 6e22 3a20        "not in": 
-000033f0: 224e 4f54 2049 4e22 2c0a 2020 2020 2020  "NOT IN",.      
-00003400: 2020 2020 2020 2020 2020 224c 494b 4522            "LIKE"
-00003410: 3a20 224c 494b 4522 2c0a 2020 2020 2020  : "LIKE",.      
-00003420: 2020 2020 2020 2020 2020 223d 3d22 3a20            "==": 
-00003430: 223d 222c 0a20 2020 2020 2020 2020 2020  "=",.           
-00003440: 2020 2020 2022 3e22 3a20 223e 222c 0a20       ">": ">",. 
-00003450: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003460: 3c22 3a20 223c 222c 0a20 2020 2020 2020  <": "<",.       
-00003470: 2020 2020 2020 2020 2022 3e3d 223a 2022           ">=": "
-00003480: 3e3d 222c 0a20 2020 2020 2020 2020 2020  >=",.           
-00003490: 2020 2020 2022 3c3d 223a 2022 3c3d 222c       "<=": "<=",
-000034a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034b0: 2022 213d 223a 2022 213d 222c 0a20 2020   "!=": "!=",.   
-000034c0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-000034d0: 2020 2020 2020 2020 2320 4966 2073 696e          # If sin
-000034e0: 676c 6520 6c61 7965 7220 6669 6c74 6572  gle layer filter
-000034f0: 2c20 6164 6420 616e 6f74 6865 7220 7073  , add another ps
-00003500: 6575 646f 206c 6179 6572 2e20 536f 2074  eudo layer. So t
-00003510: 6865 2073 696e 676c 6520 6c61 7965 7220  he single layer 
-00003520: 7265 7072 6573 656e 7473 2022 616e 6422  represents "and"
-00003530: 206c 6f67 6963 2e0a 2020 2020 2020 2020   logic..        
-00003540: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00003550: 6528 6669 6c74 6572 735b 305d 2c20 7475  e(filters[0], tu
-00003560: 706c 6529 2061 6e64 2028 0a20 2020 2020  ple) and (.     
-00003570: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
-00003580: 696c 7465 7273 5b30 5d29 203d 3d20 3020  ilters[0]) == 0 
-00003590: 6f72 206e 6f74 2069 7369 6e73 7461 6e63  or not isinstanc
-000035a0: 6528 6c69 7374 2866 696c 7465 7273 5b30  e(list(filters[0
-000035b0: 5d29 5b30 5d2c 2074 7570 6c65 290a 2020  ])[0], tuple).  
-000035c0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-000035d0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000035e0: 7465 7273 203d 2074 7970 696e 672e 6361  ters = typing.ca
-000035f0: 7374 2874 6869 7264 5f70 6172 7479 5f70  st(third_party_p
-00003600: 616e 6461 735f 6762 712e 4669 6c74 6572  andas_gbq.Filter
-00003610: 7354 7970 652c 205b 6669 6c74 6572 735d  sType, [filters]
-00003620: 290a 0a20 2020 2020 2020 2020 2020 206f  )..            o
-00003630: 725f 6578 7072 6573 7369 6f6e 7320 3d20  r_expressions = 
-00003640: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-00003650: 6f72 2067 726f 7570 2069 6e20 6669 6c74  or group in filt
-00003660: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00003670: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00003680: 7374 616e 6365 2867 726f 7570 2c20 4974  stance(group, It
-00003690: 6572 6162 6c65 293a 0a20 2020 2020 2020  erable):.       
-000036a0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-000036b0: 7570 203d 205b 6772 6f75 705d 0a0a 2020  up = [group]..  
-000036c0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000036d0: 645f 6578 7072 6573 7369 6f6e 7320 3d20  d_expressions = 
-000036e0: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-000036f0: 2020 2066 6f72 2066 696c 7465 725f 6974     for filter_it
-00003700: 656d 2069 6e20 6772 6f75 703a 0a20 2020  em in group:.   
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00003730: 6365 2866 696c 7465 725f 6974 656d 2c20  ce(filter_item, 
-00003740: 7475 706c 6529 206f 7220 286c 656e 2866  tuple) or (len(f
-00003750: 696c 7465 725f 6974 656d 2920 213d 2033  ilter_item) != 3
-00003760: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00003770: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003780: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037a0: 2020 2020 2020 2020 2066 2246 696c 7465           f"Filte
-000037b0: 7220 636f 6e64 6974 696f 6e20 7368 6f75  r condition shou
-000037c0: 6c64 2062 6520 6120 7475 706c 6520 6f66  ld be a tuple of
-000037d0: 206c 656e 6774 6820 332c 207b 6669 6c74   length 3, {filt
-000037e0: 6572 5f69 7465 6d7d 2069 7320 6e6f 7420  er_item} is not 
-000037f0: 7661 6c69 642e 220a 2020 2020 2020 2020  valid.".        
-00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003810: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003820: 2020 2020 2020 2063 6f6c 756d 6e2c 206f         column, o
-00003830: 7065 7261 746f 722c 2076 616c 7565 203d  perator, value =
-00003840: 2066 696c 7465 725f 6974 656d 0a0a 2020   filter_item..  
+000006e0: 2e62 6967 7175 6572 792e 7461 626c 650a  .bigquery.table.
+000006f0: 696d 706f 7274 2067 6f6f 676c 652e 636c  import google.cl
+00000700: 6f75 642e 6269 6771 7565 7279 5f63 6f6e  oud.bigquery_con
+00000710: 6e65 6374 696f 6e5f 7631 0a69 6d70 6f72  nection_v1.impor
+00000720: 7420 676f 6f67 6c65 2e63 6c6f 7564 2e62  t google.cloud.b
+00000730: 6967 7175 6572 795f 7374 6f72 6167 655f  igquery_storage_
+00000740: 7631 0a69 6d70 6f72 7420 676f 6f67 6c65  v1.import google
+00000750: 2e63 6c6f 7564 2e66 756e 6374 696f 6e73  .cloud.functions
+00000760: 5f76 320a 696d 706f 7274 2067 6f6f 676c  _v2.import googl
+00000770: 652e 636c 6f75 642e 7265 736f 7572 6365  e.cloud.resource
+00000780: 6d61 6e61 6765 725f 7633 0a69 6d70 6f72  manager_v3.impor
+00000790: 7420 676f 6f67 6c65 2e63 6c6f 7564 2e73  t google.cloud.s
+000007a0: 746f 7261 6765 2061 7320 7374 6f72 6167  torage as storag
+000007b0: 6520 2023 2074 7970 653a 2069 676e 6f72  e  # type: ignor
+000007c0: 650a 696d 706f 7274 2069 6269 730a 696d  e.import ibis.im
+000007d0: 706f 7274 2069 6269 732e 6261 636b 656e  port ibis.backen
+000007e0: 6473 2e62 6967 7175 6572 7920 6173 2069  ds.bigquery as i
+000007f0: 6269 735f 6269 6771 7565 7279 0a69 6d70  bis_bigquery.imp
+00000800: 6f72 7420 6962 6973 2e65 7870 722e 6461  ort ibis.expr.da
+00000810: 7461 7479 7065 7320 6173 2069 6269 735f  tatypes as ibis_
+00000820: 6474 7970 6573 0a69 6d70 6f72 7420 6962  dtypes.import ib
+00000830: 6973 2e65 7870 722e 7479 7065 7320 6173  is.expr.types as
+00000840: 2069 6269 735f 7479 7065 730a 696d 706f   ibis_types.impo
+00000850: 7274 206e 756d 7079 2061 7320 6e70 0a69  rt numpy as np.i
+00000860: 6d70 6f72 7420 7061 6e64 6173 0a66 726f  mport pandas.fro
+00000870: 6d20 7061 6e64 6173 2e5f 7479 7069 6e67  m pandas._typing
+00000880: 2069 6d70 6f72 7420 280a 2020 2020 436f   import (.    Co
+00000890: 6d70 7265 7373 696f 6e4f 7074 696f 6e73  mpressionOptions
+000008a0: 2c0a 2020 2020 4669 6c65 5061 7468 2c0a  ,.    FilePath,.
+000008b0: 2020 2020 5265 6164 5069 636b 6c65 4275      ReadPickleBu
+000008c0: 6666 6572 2c0a 2020 2020 5374 6f72 6167  ffer,.    Storag
+000008d0: 654f 7074 696f 6e73 2c0a 290a 696d 706f  eOptions,.).impo
+000008e0: 7274 2070 7961 7272 6f77 2061 7320 7061  rt pyarrow as pa
+000008f0: 0a0a 696d 706f 7274 2062 6967 6672 616d  ..import bigfram
+00000900: 6573 2e5f 636f 6e66 6967 2e62 6967 7175  es._config.bigqu
+00000910: 6572 795f 6f70 7469 6f6e 7320 6173 2062  ery_options as b
+00000920: 6967 7175 6572 795f 6f70 7469 6f6e 730a  igquery_options.
+00000930: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
+00000940: 2e63 6c69 656e 7473 0a69 6d70 6f72 7420  .clients.import 
+00000950: 6269 6766 7261 6d65 732e 636f 6e73 7461  bigframes.consta
+00000960: 6e74 7320 6173 2063 6f6e 7374 616e 7473  nts as constants
+00000970: 0a69 6d70 6f72 7420 6269 6766 7261 6d65  .import bigframe
+00000980: 732e 636f 7265 2061 7320 636f 7265 0a69  s.core as core.i
+00000990: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
+000009a0: 636f 7265 2e62 6c6f 636b 7320 6173 2062  core.blocks as b
+000009b0: 6c6f 636b 730a 696d 706f 7274 2062 6967  locks.import big
+000009c0: 6672 616d 6573 2e63 6f72 652e 636f 6d70  frames.core.comp
+000009d0: 696c 650a 696d 706f 7274 2062 6967 6672  ile.import bigfr
+000009e0: 616d 6573 2e63 6f72 652e 6775 6964 2061  ames.core.guid a
+000009f0: 7320 6775 6964 0a69 6d70 6f72 7420 6269  s guid.import bi
+00000a00: 6766 7261 6d65 732e 636f 7265 2e6e 6f64  gframes.core.nod
+00000a10: 6573 2061 7320 6e6f 6465 730a 6672 6f6d  es as nodes.from
+00000a20: 2062 6967 6672 616d 6573 2e63 6f72 652e   bigframes.core.
+00000a30: 6f72 6465 7269 6e67 2069 6d70 6f72 7420  ordering import 
+00000a40: 496e 7465 6765 7245 6e63 6f64 696e 670a  IntegerEncoding.
+00000a50: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
+00000a60: 2e63 6f72 652e 6f72 6465 7269 6e67 2061  .core.ordering a
+00000a70: 7320 6f72 6465 720a 696d 706f 7274 2062  s order.import b
+00000a80: 6967 6672 616d 6573 2e63 6f72 652e 7472  igframes.core.tr
+00000a90: 6565 5f70 726f 7065 7274 6965 7320 6173  ee_properties as
+00000aa0: 2074 7261 7665 7273 616c 730a 696d 706f   traversals.impo
+00000ab0: 7274 2062 6967 6672 616d 6573 2e63 6f72  rt bigframes.cor
+00000ac0: 652e 7472 6565 5f70 726f 7065 7274 6965  e.tree_propertie
+00000ad0: 7320 6173 2074 7265 655f 7072 6f70 6572  s as tree_proper
+00000ae0: 7469 6573 0a69 6d70 6f72 7420 6269 6766  ties.import bigf
+00000af0: 7261 6d65 732e 636f 7265 2e75 7469 6c73  rames.core.utils
+00000b00: 2061 7320 7574 696c 730a 696d 706f 7274   as utils.import
+00000b10: 2062 6967 6672 616d 6573 2e64 7479 7065   bigframes.dtype
+00000b20: 730a 696d 706f 7274 2062 6967 6672 616d  s.import bigfram
+00000b30: 6573 2e66 6f72 6d61 7474 696e 675f 6865  es.formatting_he
+00000b40: 6c70 6572 7320 6173 2066 6f72 6d61 7474  lpers as formatt
+00000b50: 696e 675f 6865 6c70 6572 730a 6672 6f6d  ing_helpers.from
+00000b60: 2062 6967 6672 616d 6573 2e66 756e 6374   bigframes.funct
+00000b70: 696f 6e73 2e72 656d 6f74 655f 6675 6e63  ions.remote_func
+00000b80: 7469 6f6e 2069 6d70 6f72 7420 7265 6164  tion import read
+00000b90: 5f67 6271 5f66 756e 6374 696f 6e20 6173  _gbq_function as
+00000ba0: 2062 6967 6672 616d 6573 5f72 6766 0a66   bigframes_rgf.f
+00000bb0: 726f 6d20 6269 6766 7261 6d65 732e 6675  rom bigframes.fu
+00000bc0: 6e63 7469 6f6e 732e 7265 6d6f 7465 5f66  nctions.remote_f
+00000bd0: 756e 6374 696f 6e20 696d 706f 7274 2072  unction import r
+00000be0: 656d 6f74 655f 6675 6e63 7469 6f6e 2061  emote_function a
+00000bf0: 7320 6269 6766 7261 6d65 735f 7266 0a69  s bigframes_rf.i
+00000c00: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
+00000c10: 7365 7373 696f 6e2e 5f69 6f2e 6269 6771  session._io.bigq
+00000c20: 7565 7279 2061 7320 6269 6766 7261 6d65  uery as bigframe
+00000c30: 735f 696f 0a69 6d70 6f72 7420 6269 6766  s_io.import bigf
+00000c40: 7261 6d65 732e 7365 7373 696f 6e2e 636c  rames.session.cl
+00000c50: 6965 6e74 730a 696d 706f 7274 2062 6967  ients.import big
+00000c60: 6672 616d 6573 2e76 6572 7369 6f6e 0a0a  frames.version..
+00000c70: 2320 4176 6f69 6420 6369 7263 756c 6172  # Avoid circular
+00000c80: 2069 6d70 6f72 7473 2e0a 6966 2074 7970   imports..if typ
+00000c90: 696e 672e 5459 5045 5f43 4845 434b 494e  ing.TYPE_CHECKIN
+00000ca0: 473a 0a20 2020 2069 6d70 6f72 7420 6269  G:.    import bi
+00000cb0: 6766 7261 6d65 732e 636f 7265 2e69 6e64  gframes.core.ind
+00000cc0: 6578 6573 0a20 2020 2069 6d70 6f72 7420  exes.    import 
+00000cd0: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
+00000ce0: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
+00000cf0: 0a20 2020 2069 6d70 6f72 7420 6269 6766  .    import bigf
+00000d00: 7261 6d65 732e 7365 7269 6573 0a0a 5f42  rames.series.._B
+00000d10: 4947 4652 414d 4553 5f44 4546 4155 4c54  IGFRAMES_DEFAULT
+00000d20: 5f43 4f4e 4e45 4354 494f 4e5f 4944 203d  _CONNECTION_ID =
+00000d30: 2022 6269 6766 7261 6d65 732d 6465 6661   "bigframes-defa
+00000d40: 756c 742d 636f 6e6e 6563 7469 6f6e 220a  ult-connection".
+00000d50: 0a5f 4d41 585f 434c 5553 5445 525f 434f  ._MAX_CLUSTER_CO
+00000d60: 4c55 4d4e 5320 3d20 340a 0a23 2054 4f44  LUMNS = 4..# TOD
+00000d70: 4f28 7377 6173 7429 3a20 4e65 6564 2074  O(swast): Need t
+00000d80: 6f20 636f 6e6e 6563 7420 746f 2072 6567  o connect to reg
+00000d90: 696f 6e61 6c20 656e 6470 6f69 6e74 7320  ional endpoints 
+00000da0: 7768 656e 2070 6572 666f 726d 696e 6720  when performing 
+00000db0: 7265 6d6f 7465 0a23 2066 756e 6374 696f  remote.# functio
+00000dc0: 6e73 206f 7065 7261 7469 6f6e 7320 2842  ns operations (B
+00000dd0: 5120 436f 6e6e 6563 7469 6f6e 2049 414d  Q Connection IAM
+00000de0: 2c20 436c 6f75 6420 5275 6e20 2f20 436c  , Cloud Run / Cl
+00000df0: 6f75 6420 4675 6e63 7469 6f6e 7329 2e0a  oud Functions)..
+00000e00: 2320 416c 736f 2073 6565 2069 6620 7265  # Also see if re
+00000e10: 736f 7572 6365 206d 616e 6167 6572 2063  source manager c
+00000e20: 6c69 656e 7420 6c69 6272 6172 7920 7375  lient library su
+00000e30: 7070 6f72 7473 2072 6567 696f 6e61 6c20  pports regional 
+00000e40: 656e 6470 6f69 6e74 732e 0a0a 5f56 414c  endpoints..._VAL
+00000e50: 4944 5f45 4e43 4f44 494e 4753 203d 207b  ID_ENCODINGS = {
+00000e60: 0a20 2020 2022 5554 462d 3822 2c0a 2020  .    "UTF-8",.  
+00000e70: 2020 2249 534f 2d38 3835 392d 3122 2c0a    "ISO-8859-1",.
+00000e80: 2020 2020 2255 5446 2d31 3642 4522 2c0a      "UTF-16BE",.
+00000e90: 2020 2020 2255 5446 2d31 364c 4522 2c0a      "UTF-16LE",.
+00000ea0: 2020 2020 2255 5446 2d33 3242 4522 2c0a      "UTF-32BE",.
+00000eb0: 2020 2020 2255 5446 2d33 324c 4522 2c0a      "UTF-32LE",.
+00000ec0: 7d0a 0a23 2042 6967 5175 6572 7920 6861  }..# BigQuery ha
+00000ed0: 7320 3120 4d42 2071 7565 7279 2073 697a  s 1 MB query siz
+00000ee0: 6520 6c69 6d69 742e 2044 6f6e 2774 2077  e limit. Don't w
+00000ef0: 616e 7420 746f 2074 616b 6520 7570 206d  ant to take up m
+00000f00: 6f72 6520 7468 616e 2061 2066 6577 2025  ore than a few %
+00000f10: 206f 6620 7468 6174 2069 6e6c 696e 696e   of that inlinin
+00000f20: 6720 6120 7461 626c 652e 0a23 2041 6c73  g a table..# Als
+00000f30: 6f20 6d75 7374 2061 7373 756d 6520 7468  o must assume th
+00000f40: 6174 2074 6578 7420 656e 636f 6469 6e67  at text encoding
+00000f50: 2061 7320 6c69 7465 7261 6c73 2069 7320   as literals is 
+00000f60: 6d75 6368 206c 6573 7320 6566 6669 6369  much less effici
+00000f70: 656e 7420 7468 616e 2069 6e2d 6d65 6d6f  ent than in-memo
+00000f80: 7279 2072 6570 7265 7365 6e74 6174 696f  ry representatio
+00000f90: 6e2e 0a4d 4158 5f49 4e4c 494e 455f 4446  n..MAX_INLINE_DF
+00000fa0: 5f42 5954 4553 203d 2035 3030 300a 0a23  _BYTES = 5000..#
+00000fb0: 204d 6178 2063 6f6d 706c 6578 6974 7920   Max complexity 
+00000fc0: 7468 6174 2073 686f 756c 6420 6265 2065  that should be e
+00000fd0: 7865 6375 7465 6420 6173 2061 2073 696e  xecuted as a sin
+00000fe0: 676c 6520 7175 6572 790a 5155 4552 595f  gle query.QUERY_
+00000ff0: 434f 4d50 4c45 5849 5459 5f4c 494d 4954  COMPLEXITY_LIMIT
+00001000: 203d 2031 6537 0a23 204e 756d 6265 7220   = 1e7.# Number 
+00001010: 6f66 2074 696d 6573 2074 6f20 6661 6374  of times to fact
+00001020: 6f72 206f 7574 2073 7562 7175 6572 6965  or out subquerie
+00001030: 7320 6265 666f 7265 2067 6976 696e 6720  s before giving 
+00001040: 7570 2e0a 4d41 585f 5355 4254 5245 455f  up..MAX_SUBTREE_
+00001050: 4641 4354 4f52 494e 4753 203d 2035 0a0a  FACTORINGS = 5..
+00001060: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
+00001070: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
+00001080: 655f 5f29 0a0a 2320 4578 636c 7564 6573  e__)..# Excludes
+00001090: 2067 656f 6772 6170 6879 2c20 6279 7465   geography, byte
+000010a0: 732c 2061 6e64 206e 6573 7465 6420 2861  s, and nested (a
+000010b0: 7272 6179 2c20 7374 7275 6374 2920 6461  rray, struct) da
+000010c0: 7461 7479 7065 730a 494e 4c49 4e41 424c  tatypes.INLINABL
+000010d0: 455f 4454 5950 4553 3a20 5365 7175 656e  E_DTYPES: Sequen
+000010e0: 6365 5b62 6967 6672 616d 6573 2e64 7479  ce[bigframes.dty
+000010f0: 7065 732e 4474 7970 655d 203d 2028 0a20  pes.Dtype] = (. 
+00001100: 2020 2070 616e 6461 732e 426f 6f6c 6561     pandas.Boolea
+00001110: 6e44 7479 7065 2829 2c0a 2020 2020 7061  nDtype(),.    pa
+00001120: 6e64 6173 2e46 6c6f 6174 3634 4474 7970  ndas.Float64Dtyp
+00001130: 6528 292c 0a20 2020 2070 616e 6461 732e  e(),.    pandas.
+00001140: 496e 7436 3444 7479 7065 2829 2c0a 2020  Int64Dtype(),.  
+00001150: 2020 7061 6e64 6173 2e53 7472 696e 6744    pandas.StringD
+00001160: 7479 7065 2873 746f 7261 6765 3d22 7079  type(storage="py
+00001170: 6172 726f 7722 292c 0a20 2020 2070 616e  arrow"),.    pan
+00001180: 6461 732e 4172 726f 7744 7479 7065 2870  das.ArrowDtype(p
+00001190: 612e 6461 7465 3332 2829 292c 0a20 2020  a.date32()),.   
+000011a0: 2070 616e 6461 732e 4172 726f 7744 7479   pandas.ArrowDty
+000011b0: 7065 2870 612e 7469 6d65 3634 2822 7573  pe(pa.time64("us
+000011c0: 2229 292c 0a20 2020 2070 616e 6461 732e  ")),.    pandas.
+000011d0: 4172 726f 7744 7479 7065 2870 612e 7469  ArrowDtype(pa.ti
+000011e0: 6d65 7374 616d 7028 2275 7322 2929 2c0a  mestamp("us")),.
+000011f0: 2020 2020 7061 6e64 6173 2e41 7272 6f77      pandas.Arrow
+00001200: 4474 7970 6528 7061 2e74 696d 6573 7461  Dtype(pa.timesta
+00001210: 6d70 2822 7573 222c 2074 7a3d 2255 5443  mp("us", tz="UTC
+00001220: 2229 292c 0a20 2020 2070 616e 6461 732e  ")),.    pandas.
+00001230: 4172 726f 7744 7479 7065 2870 612e 6465  ArrowDtype(pa.de
+00001240: 6369 6d61 6c31 3238 2833 382c 2039 2929  cimal128(38, 9))
+00001250: 2c0a 2020 2020 7061 6e64 6173 2e41 7272  ,.    pandas.Arr
+00001260: 6f77 4474 7970 6528 7061 2e64 6563 696d  owDtype(pa.decim
+00001270: 616c 3235 3628 3736 2c20 3338 2929 2c0a  al256(76, 38)),.
+00001280: 290a 0a0a 6465 6620 5f69 735f 7175 6572  )...def _is_quer
+00001290: 7928 7175 6572 795f 6f72 5f74 6162 6c65  y(query_or_table
+000012a0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
+000012b0: 2020 2020 2222 2244 6574 6572 6d69 6e65      """Determine
+000012c0: 2069 6620 6071 7565 7279 5f6f 725f 7461   if `query_or_ta
+000012d0: 626c 6560 2069 7320 6120 7461 626c 6520  ble` is a table 
+000012e0: 4944 206f 7220 6120 5351 4c20 7374 7269  ID or a SQL stri
+000012f0: 6e67 2222 220a 2020 2020 7265 7475 726e  ng""".    return
+00001300: 2072 652e 7365 6172 6368 2872 225c 7322   re.search(r"\s"
+00001310: 2c20 7175 6572 795f 6f72 5f74 6162 6c65  , query_or_table
+00001320: 2e73 7472 6970 2829 2c20 7265 2e4d 554c  .strip(), re.MUL
+00001330: 5449 4c49 4e45 2920 6973 206e 6f74 204e  TILINE) is not N
+00001340: 6f6e 650a 0a0a 6465 6620 5f69 735f 7461  one...def _is_ta
+00001350: 626c 655f 7769 7468 5f77 696c 6463 6172  ble_with_wildcar
+00001360: 645f 7375 6666 6978 2871 7565 7279 5f6f  d_suffix(query_o
+00001370: 725f 7461 626c 653a 2073 7472 2920 2d3e  r_table: str) ->
+00001380: 2062 6f6f 6c3a 0a20 2020 2022 2222 4465   bool:.    """De
+00001390: 7465 726d 696e 6520 6966 2060 7175 6572  termine if `quer
+000013a0: 795f 6f72 5f74 6162 6c65 6020 6973 2061  y_or_table` is a
+000013b0: 2074 6162 6c65 2061 6e64 2063 6f6e 7461   table and conta
+000013c0: 696e 7320 6120 7769 6c64 6361 7264 2073  ins a wildcard s
+000013d0: 7566 6669 782e 2222 220a 2020 2020 7265  uffix.""".    re
+000013e0: 7475 726e 206e 6f74 205f 6973 5f71 7565  turn not _is_que
+000013f0: 7279 2871 7565 7279 5f6f 725f 7461 626c  ry(query_or_tabl
+00001400: 6529 2061 6e64 2071 7565 7279 5f6f 725f  e) and query_or_
+00001410: 7461 626c 652e 656e 6473 7769 7468 2822  table.endswith("
+00001420: 2a22 290a 0a0a 636c 6173 7320 5365 7373  *")...class Sess
+00001430: 696f 6e28 0a20 2020 2074 6869 7264 5f70  ion(.    third_p
+00001440: 6172 7479 5f70 616e 6461 735f 6762 712e  arty_pandas_gbq.
+00001450: 4742 5149 4f4d 6978 696e 2c0a 2020 2020  GBQIOMixin,.    
+00001460: 7468 6972 645f 7061 7274 795f 7061 6e64  third_party_pand
+00001470: 6173 5f70 6172 7175 6574 2e50 6172 7175  as_parquet.Parqu
+00001480: 6574 494f 4d69 7869 6e2c 0a20 2020 2074  etIOMixin,.    t
+00001490: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
+000014a0: 735f 7069 636b 6c65 2e50 6963 6b6c 6549  s_pickle.PickleI
+000014b0: 4f4d 6978 696e 2c0a 2020 2020 7468 6972  OMixin,.    thir
+000014c0: 645f 7061 7274 795f 7061 6e64 6173 5f72  d_party_pandas_r
+000014d0: 6561 6465 7273 2e52 6561 6465 7249 4f4d  eaders.ReaderIOM
+000014e0: 6978 696e 2c0a 293a 0a20 2020 2022 2222  ixin,.):.    """
+000014f0: 4573 7461 626c 6973 6865 7320 6120 4269  Establishes a Bi
+00001500: 6751 7565 7279 2063 6f6e 6e65 6374 696f  gQuery connectio
+00001510: 6e20 746f 2063 6170 7475 7265 2061 2067  n to capture a g
+00001520: 726f 7570 206f 6620 6a6f 6220 6163 7469  roup of job acti
+00001530: 7669 7469 6573 2072 656c 6174 6564 2074  vities related t
+00001540: 6f0a 2020 2020 4461 7461 4672 616d 6573  o.    DataFrames
+00001550: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00001560: 2020 2020 2063 6f6e 7465 7874 2028 6269       context (bi
+00001570: 6766 7261 6d65 732e 5f63 6f6e 6669 672e  gframes._config.
+00001580: 6269 6771 7565 7279 5f6f 7074 696f 6e73  bigquery_options
+00001590: 2e42 6967 5175 6572 794f 7074 696f 6e73  .BigQueryOptions
+000015a0: 293a 0a20 2020 2020 2020 2020 2020 2043  ):.            C
+000015b0: 6f6e 6669 6775 7261 7469 6f6e 2061 646a  onfiguration adj
+000015c0: 7573 7469 6e67 2068 6f77 2074 6f20 636f  usting how to co
+000015d0: 6e6e 6563 7420 746f 2042 6967 5175 6572  nnect to BigQuer
+000015e0: 7920 616e 6420 7265 6c61 7465 640a 2020  y and related.  
+000015f0: 2020 2020 2020 2020 2020 4150 4973 2e20            APIs. 
+00001600: 4e6f 7465 2074 6861 7420 736f 6d65 206f  Note that some o
+00001610: 7074 696f 6e73 2061 7265 2069 676e 6f72  ptions are ignor
+00001620: 6564 2069 6620 6060 636c 6965 6e74 735f  ed if ``clients_
+00001630: 7072 6f76 6964 6572 6060 2069 730a 2020  provider`` is.  
+00001640: 2020 2020 2020 2020 2020 7365 742e 0a20            set.. 
+00001650: 2020 2020 2020 2063 6c69 656e 7473 5f70         clients_p
+00001660: 726f 7669 6465 7220 2862 6967 6672 616d  rovider (bigfram
+00001670: 6573 2e73 6573 7369 6f6e 2e63 6c69 656e  es.session.clien
+00001680: 7473 2e43 6c69 656e 7473 5072 6f76 6964  ts.ClientsProvid
+00001690: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+000016a0: 2041 6e20 6f62 6a65 6374 2070 726f 7669   An object provi
+000016b0: 6469 6e67 2063 6c69 656e 7420 6c69 6272  ding client libr
+000016c0: 6172 7920 6f62 6a65 6374 732e 0a20 2020  ary objects..   
+000016d0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+000016e0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000016f0: 7365 6c66 2c0a 2020 2020 2020 2020 636f  self,.        co
+00001700: 6e74 6578 743a 204f 7074 696f 6e61 6c5b  ntext: Optional[
+00001710: 6269 6771 7565 7279 5f6f 7074 696f 6e73  bigquery_options
+00001720: 2e42 6967 5175 6572 794f 7074 696f 6e73  .BigQueryOptions
+00001730: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00001740: 2020 636c 6965 6e74 735f 7072 6f76 6964    clients_provid
+00001750: 6572 3a20 4f70 7469 6f6e 616c 5b62 6967  er: Optional[big
+00001760: 6672 616d 6573 2e73 6573 7369 6f6e 2e63  frames.session.c
+00001770: 6c69 656e 7473 2e43 6c69 656e 7473 5072  lients.ClientsPr
+00001780: 6f76 6964 6572 5d20 3d20 4e6f 6e65 2c0a  ovider] = None,.
+00001790: 2020 2020 293a 0a20 2020 2020 2020 2069      ):.        i
+000017a0: 6620 636f 6e74 6578 7420 6973 204e 6f6e  f context is Non
+000017b0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+000017c0: 6f6e 7465 7874 203d 2062 6967 7175 6572  ontext = bigquer
+000017d0: 795f 6f70 7469 6f6e 732e 4269 6751 7565  y_options.BigQue
+000017e0: 7279 4f70 7469 6f6e 7328 290a 0a20 2020  ryOptions()..   
+000017f0: 2020 2020 2023 2054 4f44 4f28 7377 6173       # TODO(swas
+00001800: 7429 3a20 4765 7420 6c6f 6361 7469 6f6e  t): Get location
+00001810: 2066 726f 6d20 7468 6520 656e 7669 726f   from the enviro
+00001820: 6e6d 656e 742e 0a20 2020 2020 2020 2069  nment..        i
+00001830: 6620 636f 6e74 6578 742e 6c6f 6361 7469  f context.locati
+00001840: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00001850: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+00001860: 6361 7469 6f6e 203d 2022 5553 220a 2020  cation = "US".  
+00001870: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+00001880: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
+00001890: 2020 2020 2020 2020 2066 224e 6f20 6578           f"No ex
+000018a0: 706c 6963 6974 206c 6f63 6174 696f 6e20  plicit location 
+000018b0: 6973 2073 6574 2c20 736f 2075 7369 6e67  is set, so using
+000018c0: 206c 6f63 6174 696f 6e20 7b73 656c 662e   location {self.
+000018d0: 5f6c 6f63 6174 696f 6e7d 2066 6f72 2074  _location} for t
+000018e0: 6865 2073 6573 7369 6f6e 2e22 2c0a 2020  he session.",.  
+000018f0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00001900: 6163 6b6c 6576 656c 3d32 2c0a 2020 2020  acklevel=2,.    
+00001910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00001920: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001930: 2020 2020 7365 6c66 2e5f 6c6f 6361 7469      self._locati
+00001940: 6f6e 203d 2063 6f6e 7465 7874 2e6c 6f63  on = context.loc
+00001950: 6174 696f 6e0a 0a20 2020 2020 2020 2073  ation..        s
+00001960: 656c 662e 5f62 715f 6b6d 735f 6b65 795f  elf._bq_kms_key_
+00001970: 6e61 6d65 203d 2063 6f6e 7465 7874 2e6b  name = context.k
+00001980: 6d73 5f6b 6579 5f6e 616d 650a 0a20 2020  ms_key_name..   
+00001990: 2020 2020 2023 2049 6e73 7461 6e74 6961       # Instantia
+000019a0: 7465 2061 2063 6c69 656e 7473 2070 726f  te a clients pro
+000019b0: 7669 6465 7220 746f 2068 656c 7020 7769  vider to help wi
+000019c0: 7468 2063 6c6f 7564 2063 6c69 656e 7473  th cloud clients
+000019d0: 2074 6861 7420 7769 6c6c 2062 650a 2020   that will be.  
+000019e0: 2020 2020 2020 2320 7573 6564 2069 6e20        # used in 
+000019f0: 7468 6520 6675 7475 7265 206f 7065 7261  the future opera
+00001a00: 7469 6f6e 7320 696e 2074 6865 2073 6573  tions in the ses
+00001a10: 7369 6f6e 0a20 2020 2020 2020 2069 6620  sion.        if 
+00001a20: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
+00001a30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00001a40: 6c66 2e5f 636c 6965 6e74 735f 7072 6f76  lf._clients_prov
+00001a50: 6964 6572 203d 2063 6c69 656e 7473 5f70  ider = clients_p
+00001a60: 726f 7669 6465 720a 2020 2020 2020 2020  rovider.        
+00001a70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001a80: 2020 7365 6c66 2e5f 636c 6965 6e74 735f    self._clients_
+00001a90: 7072 6f76 6964 6572 203d 2062 6967 6672  provider = bigfr
+00001aa0: 616d 6573 2e73 6573 7369 6f6e 2e63 6c69  ames.session.cli
+00001ab0: 656e 7473 2e43 6c69 656e 7473 5072 6f76  ents.ClientsProv
+00001ac0: 6964 6572 280a 2020 2020 2020 2020 2020  ider(.          
+00001ad0: 2020 2020 2020 7072 6f6a 6563 743d 636f        project=co
+00001ae0: 6e74 6578 742e 7072 6f6a 6563 742c 0a20  ntext.project,. 
+00001af0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00001b00: 6f63 6174 696f 6e3d 7365 6c66 2e5f 6c6f  ocation=self._lo
+00001b10: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
+00001b20: 2020 2020 2020 2020 7573 655f 7265 6769          use_regi
+00001b30: 6f6e 616c 5f65 6e64 706f 696e 7473 3d63  onal_endpoints=c
+00001b40: 6f6e 7465 7874 2e75 7365 5f72 6567 696f  ontext.use_regio
+00001b50: 6e61 6c5f 656e 6470 6f69 6e74 732c 0a20  nal_endpoints,. 
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001b70: 7265 6465 6e74 6961 6c73 3d63 6f6e 7465  redentials=conte
+00001b80: 7874 2e63 7265 6465 6e74 6961 6c73 2c0a  xt.credentials,.
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 6170 706c 6963 6174 696f 6e5f 6e61 6d65  application_name
+00001bb0: 3d63 6f6e 7465 7874 2e61 7070 6c69 6361  =context.applica
+00001bc0: 7469 6f6e 5f6e 616d 652c 0a20 2020 2020  tion_name,.     
+00001bd0: 2020 2020 2020 2020 2020 2062 715f 6b6d             bq_km
+00001be0: 735f 6b65 795f 6e61 6d65 3d73 656c 662e  s_key_name=self.
+00001bf0: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
+00001c00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00001c10: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00001c20: 7265 6174 655f 6271 5f64 6174 6173 6574  reate_bq_dataset
+00001c30: 7328 290a 0a20 2020 2020 2020 2023 2054  s()..        # T
+00001c40: 4f44 4f28 7368 6f62 7329 3a20 5265 6d6f  ODO(shobs): Remo
+00001c50: 7665 2074 6869 7320 6c6f 6769 6320 6166  ve this logic af
+00001c60: 7465 7220 6874 7470 733a 2f2f 6769 7468  ter https://gith
+00001c70: 7562 2e63 6f6d 2f69 6269 732d 7072 6f6a  ub.com/ibis-proj
+00001c80: 6563 742f 6962 6973 2f69 7373 7565 732f  ect/ibis/issues/
+00001c90: 3834 3934 0a20 2020 2020 2020 2023 2068  8494.        # h
+00001ca0: 6173 2062 6565 6e20 6669 7865 642e 2054  as been fixed. T
+00001cb0: 6865 2069 6269 7320 636c 6965 6e74 2063  he ibis client c
+00001cc0: 6861 6e67 6573 2074 6865 2064 6566 6175  hanges the defau
+00001cd0: 6c74 2071 7565 7279 206a 6f62 2063 6f6e  lt query job con
+00001ce0: 6669 670a 2020 2020 2020 2020 2320 736f  fig.        # so
+00001cf0: 2077 6520 6172 6520 676f 696e 6720 746f   we are going to
+00001d00: 2072 656d 656d 6265 7220 7468 6520 6375   remember the cu
+00001d10: 7272 656e 7420 636f 6e66 6967 2061 6e64  rrent config and
+00001d20: 2072 6573 746f 7265 2069 7420 6166 7465   restore it afte
+00001d30: 720a 2020 2020 2020 2020 2320 7468 6520  r.        # the 
+00001d40: 6962 6973 2063 6c69 656e 7420 6861 7320  ibis client has 
+00001d50: 6265 656e 2063 7265 6174 6564 0a20 2020  been created.   
+00001d60: 2020 2020 206f 7269 6769 6e61 6c5f 6465       original_de
+00001d70: 6661 756c 745f 7175 6572 795f 6a6f 625f  fault_query_job_
+00001d80: 636f 6e66 6967 203d 2073 656c 662e 6271  config = self.bq
+00001d90: 636c 6965 6e74 2e64 6566 6175 6c74 5f71  client.default_q
+00001da0: 7565 7279 5f6a 6f62 5f63 6f6e 6669 670a  uery_job_config.
+00001db0: 0a20 2020 2020 2020 2073 656c 662e 6962  .        self.ib
+00001dc0: 6973 5f63 6c69 656e 7420 3d20 7479 7069  is_client = typi
+00001dd0: 6e67 2e63 6173 7428 0a20 2020 2020 2020  ng.cast(.       
+00001de0: 2020 2020 2069 6269 735f 6269 6771 7565       ibis_bigque
+00001df0: 7279 2e42 6163 6b65 6e64 2c0a 2020 2020  ry.Backend,.    
+00001e00: 2020 2020 2020 2020 6962 6973 2e62 6967          ibis.big
+00001e10: 7175 6572 792e 636f 6e6e 6563 7428 0a20  query.connect(. 
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001e30: 726f 6a65 6374 5f69 643d 636f 6e74 6578  roject_id=contex
+00001e40: 742e 7072 6f6a 6563 742c 0a20 2020 2020  t.project,.     
+00001e50: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00001e60: 743d 7365 6c66 2e62 7163 6c69 656e 742c  t=self.bqclient,
+00001e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e80: 2073 746f 7261 6765 5f63 6c69 656e 743d   storage_client=
+00001e90: 7365 6c66 2e62 7173 746f 7261 6765 7265  self.bqstoragere
+00001ea0: 6164 636c 6965 6e74 2c0a 2020 2020 2020  adclient,.      
+00001eb0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00001ec0: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00001ed0: 2e62 7163 6c69 656e 742e 6465 6661 756c  .bqclient.defaul
+00001ee0: 745f 7175 6572 795f 6a6f 625f 636f 6e66  t_query_job_conf
+00001ef0: 6967 203d 206f 7269 6769 6e61 6c5f 6465  ig = original_de
+00001f00: 6661 756c 745f 7175 6572 795f 6a6f 625f  fault_query_job_
+00001f10: 636f 6e66 6967 0a0a 2020 2020 2020 2020  config..        
+00001f20: 2320 5265 736f 6c76 6520 7468 6520 4251  # Resolve the BQ
+00001f30: 2063 6f6e 6e65 6374 696f 6e20 666f 7220   connection for 
+00001f40: 7265 6d6f 7465 2066 756e 6374 696f 6e20  remote function 
+00001f50: 616e 6420 5665 7274 6578 2041 4920 696e  and Vertex AI in
+00001f60: 7465 6772 6174 696f 6e0a 2020 2020 2020  tegration.      
+00001f70: 2020 7365 6c66 2e5f 6271 5f63 6f6e 6e65    self._bq_conne
+00001f80: 6374 696f 6e20 3d20 636f 6e74 6578 742e  ction = context.
+00001f90: 6271 5f63 6f6e 6e65 6374 696f 6e20 6f72  bq_connection or
+00001fa0: 205f 4249 4746 5241 4d45 535f 4445 4641   _BIGFRAMES_DEFA
+00001fb0: 554c 545f 434f 4e4e 4543 5449 4f4e 5f49  ULT_CONNECTION_I
+00001fc0: 440a 2020 2020 2020 2020 7365 6c66 2e5f  D.        self._
+00001fd0: 736b 6970 5f62 715f 636f 6e6e 6563 7469  skip_bq_connecti
+00001fe0: 6f6e 5f63 6865 636b 203d 2063 6f6e 7465  on_check = conte
+00001ff0: 7874 2e5f 736b 6970 5f62 715f 636f 6e6e  xt._skip_bq_conn
+00002000: 6563 7469 6f6e 5f63 6865 636b 0a0a 2020  ection_check..  
+00002010: 2020 2020 2020 2320 4e6f 7720 7468 6174        # Now that
+00002020: 2077 6527 7265 2073 7461 7274 696e 6720   we're starting 
+00002030: 7468 6520 7365 7373 696f 6e2c 2064 6f6e  the session, don
+00002040: 2774 2061 6c6c 6f77 2074 6865 206f 7074  't allow the opt
+00002050: 696f 6e73 2074 6f20 6265 0a20 2020 2020  ions to be.     
+00002060: 2020 2023 2063 6861 6e67 6564 2e0a 2020     # changed..  
+00002070: 2020 2020 2020 636f 6e74 6578 742e 5f73        context._s
+00002080: 6573 7369 6f6e 5f73 7461 7274 6564 203d  ession_started =
+00002090: 2054 7275 650a 2020 2020 2020 2020 7365   True.        se
+000020a0: 6c66 2e5f 6466 5f73 6e61 7073 686f 743a  lf._df_snapshot:
+000020b0: 2044 6963 745b 0a20 2020 2020 2020 2020   Dict[.         
+000020c0: 2020 2062 6967 7175 6572 792e 5461 626c     bigquery.Tabl
+000020d0: 6552 6566 6572 656e 6365 2c20 5475 706c  eReference, Tupl
+000020e0: 655b 6461 7465 7469 6d65 2e64 6174 6574  e[datetime.datet
+000020f0: 696d 652c 2062 6967 7175 6572 792e 5461  ime, bigquery.Ta
+00002100: 626c 655d 0a20 2020 2020 2020 205d 203d  ble].        ] =
+00002110: 207b 7d0a 0a20 2020 2040 7072 6f70 6572   {}..    @proper
+00002120: 7479 0a20 2020 2064 6566 2062 7163 6c69  ty.    def bqcli
+00002130: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
+00002140: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002150: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
+00002160: 2e62 7163 6c69 656e 740a 0a20 2020 2040  .bqclient..    @
+00002170: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00002180: 2062 7163 6f6e 6e65 6374 696f 6e63 6c69   bqconnectioncli
+00002190: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
+000021a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000021b0: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
+000021c0: 2e62 7163 6f6e 6e65 6374 696f 6e63 6c69  .bqconnectioncli
+000021d0: 656e 740a 0a20 2020 2040 7072 6f70 6572  ent..    @proper
+000021e0: 7479 0a20 2020 2064 6566 2062 7173 746f  ty.    def bqsto
+000021f0: 7261 6765 7265 6164 636c 6965 6e74 2873  ragereadclient(s
+00002200: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00002210: 7475 726e 2073 656c 662e 5f63 6c69 656e  turn self._clien
+00002220: 7473 5f70 726f 7669 6465 722e 6271 7374  ts_provider.bqst
+00002230: 6f72 6167 6572 6561 6463 6c69 656e 740a  oragereadclient.
+00002240: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00002250: 2020 2064 6566 2063 6c6f 7564 6675 6e63     def cloudfunc
+00002260: 7469 6f6e 7363 6c69 656e 7428 7365 6c66  tionsclient(self
+00002270: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00002280: 6e20 7365 6c66 2e5f 636c 6965 6e74 735f  n self._clients_
+00002290: 7072 6f76 6964 6572 2e63 6c6f 7564 6675  provider.cloudfu
+000022a0: 6e63 7469 6f6e 7363 6c69 656e 740a 0a20  nctionsclient.. 
+000022b0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000022c0: 2064 6566 2072 6573 6f75 7263 656d 616e   def resourceman
+000022d0: 6167 6572 636c 6965 6e74 2873 656c 6629  agerclient(self)
+000022e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000022f0: 2073 656c 662e 5f63 6c69 656e 7473 5f70   self._clients_p
+00002300: 726f 7669 6465 722e 7265 736f 7572 6365  rovider.resource
+00002310: 6d61 6e61 6765 7263 6c69 656e 740a 0a20  managerclient.. 
+00002320: 2020 205f 6271 5f63 6f6e 6e65 6374 696f     _bq_connectio
+00002330: 6e5f 6d61 6e61 6765 723a 204f 7074 696f  n_manager: Optio
+00002340: 6e61 6c5b 6269 6766 7261 6d65 732e 636c  nal[bigframes.cl
+00002350: 6965 6e74 732e 4271 436f 6e6e 6563 7469  ients.BqConnecti
+00002360: 6f6e 4d61 6e61 6765 725d 203d 204e 6f6e  onManager] = Non
+00002370: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+00002380: 0a20 2020 2064 6566 2062 7163 6f6e 6e65  .    def bqconne
+00002390: 6374 696f 6e6d 616e 6167 6572 2873 656c  ctionmanager(sel
+000023a0: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
+000023b0: 6f74 2073 656c 662e 5f73 6b69 705f 6271  ot self._skip_bq
+000023c0: 5f63 6f6e 6e65 6374 696f 6e5f 6368 6563  _connection_chec
+000023d0: 6b20 616e 6420 6e6f 7420 7365 6c66 2e5f  k and not self._
+000023e0: 6271 5f63 6f6e 6e65 6374 696f 6e5f 6d61  bq_connection_ma
+000023f0: 6e61 6765 723a 0a20 2020 2020 2020 2020  nager:.         
+00002400: 2020 2073 656c 662e 5f62 715f 636f 6e6e     self._bq_conn
+00002410: 6563 7469 6f6e 5f6d 616e 6167 6572 203d  ection_manager =
+00002420: 2062 6967 6672 616d 6573 2e63 6c69 656e   bigframes.clien
+00002430: 7473 2e42 7143 6f6e 6e65 6374 696f 6e4d  ts.BqConnectionM
+00002440: 616e 6167 6572 280a 2020 2020 2020 2020  anager(.        
+00002450: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
+00002460: 6f6e 6e65 6374 696f 6e63 6c69 656e 742c  onnectionclient,
+00002470: 2073 656c 662e 7265 736f 7572 6365 6d61   self.resourcema
+00002480: 6e61 6765 7263 6c69 656e 740a 2020 2020  nagerclient.    
+00002490: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000024a0: 2020 7265 7475 726e 2073 656c 662e 5f62    return self._b
+000024b0: 715f 636f 6e6e 6563 7469 6f6e 5f6d 616e  q_connection_man
+000024c0: 6167 6572 0a0a 2020 2020 4070 726f 7065  ager..    @prope
+000024d0: 7274 790a 2020 2020 6465 6620 5f70 726f  rty.    def _pro
+000024e0: 6a65 6374 2873 656c 6629 3a0a 2020 2020  ject(self):.    
+000024f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002500: 6271 636c 6965 6e74 2e70 726f 6a65 6374  bqclient.project
+00002510: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
+00002520: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00002530: 2020 2320 5374 6162 6c65 2068 6173 6820    # Stable hash 
+00002540: 6e65 6564 6564 2074 6f20 7573 6520 696e  needed to use in
+00002550: 2065 7870 7265 7373 696f 6e20 7472 6565   expression tree
+00002560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002570: 6861 7368 2873 7472 2873 656c 662e 5f61  hash(str(self._a
+00002580: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
+00002590: 2929 0a0a 2020 2020 6465 6620 5f63 7265  ))..    def _cre
+000025a0: 6174 655f 6271 5f64 6174 6173 6574 7328  ate_bq_datasets(
+000025b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000025c0: 2222 4372 6561 7465 2061 6e64 2069 6465  ""Create and ide
+000025d0: 6e74 6966 7920 6461 7461 7365 7428 7329  ntify dataset(s)
+000025e0: 2066 6f72 2074 656d 706f 7261 7279 2042   for temporary B
+000025f0: 5120 7265 736f 7572 6365 732e 2222 220a  Q resources.""".
+00002600: 2020 2020 2020 2020 7175 6572 795f 6a6f          query_jo
+00002610: 6220 3d20 7365 6c66 2e62 7163 6c69 656e  b = self.bqclien
+00002620: 742e 7175 6572 7928 2253 454c 4543 5420  t.query("SELECT 
+00002630: 3122 2c20 6c6f 6361 7469 6f6e 3d73 656c  1", location=sel
+00002640: 662e 5f6c 6f63 6174 696f 6e29 0a20 2020  f._location).   
+00002650: 2020 2020 2071 7565 7279 5f6a 6f62 2e72       query_job.r
+00002660: 6573 756c 7428 2920 2023 2062 6c6f 636b  esult()  # block
+00002670: 7320 756e 7469 6c20 6669 6e69 7368 6564  s until finished
+00002680: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+00002690: 616e 6f6e 796d 6f75 7320 6461 7461 7365  anonymous datase
+000026a0: 7420 6973 2075 7365 6420 6279 2042 6967  t is used by Big
+000026b0: 5175 6572 7920 746f 2077 7269 7465 2071  Query to write q
+000026c0: 7565 7279 2072 6573 756c 7473 2061 6e64  uery results and
+000026d0: 0a20 2020 2020 2020 2023 2073 6573 7369  .        # sessi
+000026e0: 6f6e 2074 6162 6c65 732e 2042 6967 5175  on tables. BigQu
+000026f0: 6572 7920 4461 7461 4672 616d 6573 2061  ery DataFrames a
+00002700: 6c73 6f20 7772 6974 6573 2074 656d 7020  lso writes temp 
+00002710: 7461 626c 6573 2064 6972 6563 746c 790a  tables directly.
+00002720: 2020 2020 2020 2020 2320 746f 2074 6865          # to the
+00002730: 2064 6174 6173 6574 2c20 6e6f 2042 6967   dataset, no Big
+00002740: 5175 6572 7920 5365 7373 696f 6e20 7265  Query Session re
+00002750: 7175 6972 6564 2e20 4e6f 7465 3a20 7468  quired. Note: th
+00002760: 6572 6520 6973 2061 0a20 2020 2020 2020  ere is a.       
+00002770: 2023 2064 6966 6665 7265 6e74 2061 6e6f   # different ano
+00002780: 6e79 6d6f 7573 2064 6174 6173 6574 2070  nymous dataset p
+00002790: 6572 206c 6f63 6174 696f 6e2e 2053 6565  er location. See
+000027a0: 3a0a 2020 2020 2020 2020 2320 6874 7470  :.        # http
+000027b0: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+000027c0: 2e63 6f6d 2f62 6967 7175 6572 792f 646f  .com/bigquery/do
+000027d0: 6373 2f63 6163 6865 642d 7265 7375 6c74  cs/cached-result
+000027e0: 7323 686f 775f 6361 6368 6564 5f72 6573  s#how_cached_res
+000027f0: 756c 7473 5f61 7265 5f73 746f 7265 640a  ults_are_stored.
+00002800: 2020 2020 2020 2020 7175 6572 795f 6465          query_de
+00002810: 7374 696e 6174 696f 6e20 3d20 7175 6572  stination = quer
+00002820: 795f 6a6f 622e 6465 7374 696e 6174 696f  y_job.destinatio
+00002830: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
+00002840: 616e 6f6e 796d 6f75 735f 6461 7461 7365  anonymous_datase
+00002850: 7420 3d20 6269 6771 7565 7279 2e44 6174  t = bigquery.Dat
+00002860: 6173 6574 5265 6665 7265 6e63 6528 0a20  asetReference(. 
+00002870: 2020 2020 2020 2020 2020 2071 7565 7279             query
+00002880: 5f64 6573 7469 6e61 7469 6f6e 2e70 726f  _destination.pro
+00002890: 6a65 6374 2c0a 2020 2020 2020 2020 2020  ject,.          
+000028a0: 2020 7175 6572 795f 6465 7374 696e 6174    query_destinat
+000028b0: 696f 6e2e 6461 7461 7365 745f 6964 2c0a  ion.dataset_id,.
+000028c0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000028d0: 6566 2063 6c6f 7365 2873 656c 6629 3a0a  ef close(self):.
+000028e0: 2020 2020 2020 2020 2222 224e 6f2d 6f70          """No-op
+000028f0: 2e20 5465 6d70 6f72 6172 7920 7265 736f  . Temporary reso
+00002900: 7572 6365 7320 6172 6520 6465 6c65 7465  urces are delete
+00002910: 6420 6166 7465 7220 3720 6461 7973 2e22  d after 7 days."
+00002920: 2222 0a0a 2020 2020 6465 6620 7265 6164  ""..    def read
+00002930: 5f67 6271 280a 2020 2020 2020 2020 7365  _gbq(.        se
+00002940: 6c66 2c0a 2020 2020 2020 2020 7175 6572  lf,.        quer
+00002950: 795f 6f72 5f74 6162 6c65 3a20 7374 722c  y_or_table: str,
+00002960: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+00002970: 2020 2020 696e 6465 785f 636f 6c3a 2049      index_col: I
+00002980: 7465 7261 626c 655b 7374 725d 207c 2073  terable[str] | s
+00002990: 7472 203d 2028 292c 0a20 2020 2020 2020  tr = (),.       
+000029a0: 2063 6f6c 756d 6e73 3a20 4974 6572 6162   columns: Iterab
+000029b0: 6c65 5b73 7472 5d20 3d20 2829 2c0a 2020  le[str] = (),.  
+000029c0: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+000029d0: 696f 6e3a 204f 7074 696f 6e61 6c5b 4469  ion: Optional[Di
+000029e0: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
+000029f0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
+00002a00: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00002a10: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+00002a20: 696c 7465 7273 3a20 7468 6972 645f 7061  ilters: third_pa
+00002a30: 7274 795f 7061 6e64 6173 5f67 6271 2e46  rty_pandas_gbq.F
+00002a40: 696c 7465 7273 5479 7065 203d 2028 292c  iltersType = (),
+00002a50: 0a20 2020 2020 2020 2075 7365 5f63 6163  .        use_cac
+00002a60: 6865 3a20 4f70 7469 6f6e 616c 5b62 6f6f  he: Optional[boo
+00002a70: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
+00002a80: 2020 2063 6f6c 5f6f 7264 6572 3a20 4974     col_order: It
+00002a90: 6572 6162 6c65 5b73 7472 5d20 3d20 2829  erable[str] = ()
+00002aa0: 2c0a 2020 2020 2020 2020 2320 4164 6420  ,.        # Add 
+00002ab0: 6120 7665 7269 6679 2069 6e64 6578 2061  a verify index a
+00002ac0: 7267 756d 656e 7420 7468 6174 2066 6169  rgument that fai
+00002ad0: 6c73 2069 6620 7468 6520 696e 6465 7820  ls if the index 
+00002ae0: 6973 206e 6f74 2075 6e69 7175 652e 0a20  is not unique.. 
+00002af0: 2020 2029 202d 3e20 6461 7461 6672 616d     ) -> datafram
+00002b00: 652e 4461 7461 4672 616d 653a 0a20 2020  e.DataFrame:.   
+00002b10: 2020 2020 2023 2054 4f44 4f28 622f 3238       # TODO(b/28
+00002b20: 3135 3731 3231 3429 3a20 4765 6e65 7261  1571214): Genera
+00002b30: 7465 2070 726f 6d70 7420 746f 2073 686f  te prompt to sho
+00002b40: 7720 7468 6520 7072 6f67 7265 7373 206f  w the progress o
+00002b50: 6620 7265 6164 5f67 6271 2e0a 2020 2020  f read_gbq..    
+00002b60: 2020 2020 6966 2063 6f6c 756d 6e73 2061      if columns a
+00002b70: 6e64 2063 6f6c 5f6f 7264 6572 3a0a 2020  nd col_order:.  
+00002b80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00002b90: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00002ba0: 2020 2020 2020 2020 2020 2020 224d 7573              "Mus
+00002bb0: 7420 7370 6563 6966 7920 6569 7468 6572  t specify either
+00002bc0: 2063 6f6c 756d 6e73 2028 7072 6566 6572   columns (prefer
+00002bd0: 7265 6429 206f 7220 636f 6c5f 6f72 6465  red) or col_orde
+00002be0: 722c 206e 6f74 2062 6f74 6822 0a20 2020  r, not both".   
+00002bf0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00002c00: 2020 2065 6c69 6620 636f 6c5f 6f72 6465     elif col_orde
+00002c10: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
+00002c20: 6f6c 756d 6e73 203d 2063 6f6c 5f6f 7264  olumns = col_ord
+00002c30: 6572 0a0a 2020 2020 2020 2020 6669 6c74  er..        filt
+00002c40: 6572 7320 3d20 6c69 7374 2866 696c 7465  ers = list(filte
+00002c50: 7273 290a 2020 2020 2020 2020 6966 206c  rs).        if l
+00002c60: 656e 2866 696c 7465 7273 2920 213d 2030  en(filters) != 0
+00002c70: 206f 7220 5f69 735f 7461 626c 655f 7769   or _is_table_wi
+00002c80: 7468 5f77 696c 6463 6172 645f 7375 6666  th_wildcard_suff
+00002c90: 6978 2871 7565 7279 5f6f 725f 7461 626c  ix(query_or_tabl
+00002ca0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00002cb0: 7175 6572 795f 6f72 5f74 6162 6c65 203d  query_or_table =
+00002cc0: 2073 656c 662e 5f74 6f5f 7175 6572 7928   self._to_query(
+00002cd0: 7175 6572 795f 6f72 5f74 6162 6c65 2c20  query_or_table, 
+00002ce0: 636f 6c75 6d6e 732c 2066 696c 7465 7273  columns, filters
+00002cf0: 290a 0a20 2020 2020 2020 2069 6620 5f69  )..        if _i
+00002d00: 735f 7175 6572 7928 7175 6572 795f 6f72  s_query(query_or
+00002d10: 5f74 6162 6c65 293a 0a20 2020 2020 2020  _table):.       
+00002d20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002d30: 2e5f 7265 6164 5f67 6271 5f71 7565 7279  ._read_gbq_query
+00002d40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002d50: 2020 7175 6572 795f 6f72 5f74 6162 6c65    query_or_table
+00002d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002d70: 2020 696e 6465 785f 636f 6c3d 696e 6465    index_col=inde
+00002d80: 785f 636f 6c2c 0a20 2020 2020 2020 2020  x_col,.         
+00002d90: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
+00002da0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+00002db0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+00002dc0: 6174 696f 6e3d 636f 6e66 6967 7572 6174  ation=configurat
+00002dd0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00002de0: 2020 2020 206d 6178 5f72 6573 756c 7473       max_results
+00002df0: 3d6d 6178 5f72 6573 756c 7473 2c0a 2020  =max_results,.  
+00002e00: 2020 2020 2020 2020 2020 2020 2020 6170                ap
+00002e10: 695f 6e61 6d65 3d22 7265 6164 5f67 6271  i_name="read_gbq
+00002e20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002e30: 2020 2075 7365 5f63 6163 6865 3d75 7365     use_cache=use
+00002e40: 5f63 6163 6865 2c0a 2020 2020 2020 2020  _cache,.        
+00002e50: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00002e60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00002e70: 2320 544f 444f 2873 7761 7374 293a 2051  # TODO(swast): Q
+00002e80: 7565 7279 2074 6865 2073 6e61 7073 686f  uery the snapsho
+00002e90: 7420 7461 626c 6520 6275 7420 6d61 726b  t table but mark
+00002ea0: 2069 7420 6173 2061 0a20 2020 2020 2020   it as a.       
+00002eb0: 2020 2020 2023 2064 6574 6572 6d69 6e69       # determini
+00002ec0: 7374 6963 2071 7565 7279 2073 6f20 7765  stic query so we
+00002ed0: 2063 616e 2061 766f 6964 2073 6572 6961   can avoid seria
+00002ee0: 6c69 7a69 6e67 2069 6620 7765 2068 6176  lizing if we hav
+00002ef0: 6520 610a 2020 2020 2020 2020 2020 2020  e a.            
+00002f00: 2320 756e 6971 7565 2069 6e64 6578 2e0a  # unique index..
+00002f10: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00002f20: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
+00002f30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002f40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00002f50: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f70: 2254 6865 2027 636f 6e66 6967 7572 6174  "The 'configurat
+00002f80: 696f 6e27 2061 7267 756d 656e 7420 6973  ion' argument is
+00002f90: 206e 6f74 2061 6c6c 6f77 6564 2077 6865   not allowed whe
+00002fa0: 6e20 220a 2020 2020 2020 2020 2020 2020  n ".            
+00002fb0: 2020 2020 2020 2020 2264 6972 6563 746c          "directl
+00002fc0: 7920 7265 6164 696e 6720 6672 6f6d 2061  y reading from a
+00002fd0: 2074 6162 6c65 2e20 506c 6561 7365 2072   table. Please r
+00002fe0: 656d 6f76 6520 220a 2020 2020 2020 2020  emove ".        
+00002ff0: 2020 2020 2020 2020 2020 2020 2227 636f              "'co
+00003000: 6e66 6967 7572 6174 696f 6e27 206f 7220  nfiguration' or 
+00003010: 7573 6520 6120 7175 6572 792e 220a 2020  use a query.".  
+00003020: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00003030: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003040: 7572 6e20 7365 6c66 2e5f 7265 6164 5f67  urn self._read_g
+00003050: 6271 5f74 6162 6c65 280a 2020 2020 2020  bq_table(.      
+00003060: 2020 2020 2020 2020 2020 7175 6572 795f            query_
+00003070: 6f72 5f74 6162 6c65 2c0a 2020 2020 2020  or_table,.      
+00003080: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+00003090: 636f 6c3d 696e 6465 785f 636f 6c2c 0a20  col=index_col,. 
+000030a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000030b0: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 2c0a  olumns=columns,.
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 6d61 785f 7265 7375 6c74 733d 6d61 785f  max_results=max_
+000030e0: 7265 7375 6c74 732c 0a20 2020 2020 2020  results,.       
+000030f0: 2020 2020 2020 2020 2061 7069 5f6e 616d           api_nam
+00003100: 653d 2272 6561 645f 6762 7122 2c0a 2020  e="read_gbq",.  
+00003110: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00003120: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
+00003130: 6520 6966 2075 7365 5f63 6163 6865 2069  e if use_cache i
+00003140: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00003150: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00003160: 2020 290a 0a20 2020 2064 6566 205f 746f    )..    def _to
+00003170: 5f71 7565 7279 280a 2020 2020 2020 2020  _query(.        
+00003180: 7365 6c66 2c0a 2020 2020 2020 2020 7175  self,.        qu
+00003190: 6572 795f 6f72 5f74 6162 6c65 3a20 7374  ery_or_table: st
+000031a0: 722c 0a20 2020 2020 2020 2063 6f6c 756d  r,.        colum
+000031b0: 6e73 3a20 4974 6572 6162 6c65 5b73 7472  ns: Iterable[str
+000031c0: 5d2c 0a20 2020 2020 2020 2066 696c 7465  ],.        filte
+000031d0: 7273 3a20 7468 6972 645f 7061 7274 795f  rs: third_party_
+000031e0: 7061 6e64 6173 5f67 6271 2e46 696c 7465  pandas_gbq.Filte
+000031f0: 7273 5479 7065 2c0a 2020 2020 2920 2d3e  rsType,.    ) ->
+00003200: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
+00003210: 2243 6f6d 7069 6c65 2071 7565 7279 5f6f  "Compile query_o
+00003220: 725f 7461 626c 6520 7769 7468 2063 6f6e  r_table with con
+00003230: 6469 7469 6f6e 7328 6669 6c74 6572 732c  ditions(filters,
+00003240: 2077 696c 6463 6172 6473 2920 746f 2071   wildcards) to q
+00003250: 7565 7279 2e22 2222 0a20 2020 2020 2020  uery.""".       
+00003260: 2066 696c 7465 7273 203d 206c 6973 7428   filters = list(
+00003270: 6669 6c74 6572 7329 0a20 2020 2020 2020  filters).       
+00003280: 2073 7562 5f71 7565 7279 203d 2028 0a20   sub_query = (. 
+00003290: 2020 2020 2020 2020 2020 2066 2228 7b71             f"({q
+000032a0: 7565 7279 5f6f 725f 7461 626c 657d 2922  uery_or_table})"
+000032b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000032c0: 5f69 735f 7175 6572 7928 7175 6572 795f  _is_query(query_
+000032d0: 6f72 5f74 6162 6c65 290a 2020 2020 2020  or_table).      
+000032e0: 2020 2020 2020 656c 7365 2066 2260 7b71        else f"`{q
+000032f0: 7565 7279 5f6f 725f 7461 626c 657d 6022  uery_or_table}`"
+00003300: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00003310: 2020 2020 7365 6c65 6374 5f63 6c61 7573      select_claus
+00003320: 6520 3d20 2253 454c 4543 5420 2220 2b20  e = "SELECT " + 
+00003330: 280a 2020 2020 2020 2020 2020 2020 222c  (.            ",
+00003340: 2022 2e6a 6f69 6e28 6622 607b 636f 6c75   ".join(f"`{colu
+00003350: 6d6e 7d60 2220 666f 7220 636f 6c75 6d6e  mn}`" for column
+00003360: 2069 6e20 636f 6c75 6d6e 7329 2069 6620   in columns) if 
+00003370: 636f 6c75 6d6e 7320 656c 7365 2022 2a22  columns else "*"
+00003380: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00003390: 2020 2020 7768 6572 655f 636c 6175 7365      where_clause
+000033a0: 203d 2022 220a 2020 2020 2020 2020 6966   = "".        if
+000033b0: 2066 696c 7465 7273 3a0a 2020 2020 2020   filters:.      
+000033c0: 2020 2020 2020 7661 6c69 645f 6f70 6572        valid_oper
+000033d0: 6174 6f72 733a 204d 6170 7069 6e67 5b74  ators: Mapping[t
+000033e0: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
+000033f0: 735f 6762 712e 4669 6c74 6572 4f70 732c  s_gbq.FilterOps,
+00003400: 2073 7472 5d20 3d20 7b0a 2020 2020 2020   str] = {.      
+00003410: 2020 2020 2020 2020 2020 2269 6e22 3a20            "in": 
+00003420: 2249 4e22 2c0a 2020 2020 2020 2020 2020  "IN",.          
+00003430: 2020 2020 2020 226e 6f74 2069 6e22 3a20        "not in": 
+00003440: 224e 4f54 2049 4e22 2c0a 2020 2020 2020  "NOT IN",.      
+00003450: 2020 2020 2020 2020 2020 224c 494b 4522            "LIKE"
+00003460: 3a20 224c 494b 4522 2c0a 2020 2020 2020  : "LIKE",.      
+00003470: 2020 2020 2020 2020 2020 223d 3d22 3a20            "==": 
+00003480: 223d 222c 0a20 2020 2020 2020 2020 2020  "=",.           
+00003490: 2020 2020 2022 3e22 3a20 223e 222c 0a20       ">": ">",. 
+000034a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000034b0: 3c22 3a20 223c 222c 0a20 2020 2020 2020  <": "<",.       
+000034c0: 2020 2020 2020 2020 2022 3e3d 223a 2022           ">=": "
+000034d0: 3e3d 222c 0a20 2020 2020 2020 2020 2020  >=",.           
+000034e0: 2020 2020 2022 3c3d 223a 2022 3c3d 222c       "<=": "<=",
+000034f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003500: 2022 213d 223a 2022 213d 222c 0a20 2020   "!=": "!=",.   
+00003510: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+00003520: 2020 2020 2020 2020 2320 4966 2073 696e          # If sin
+00003530: 676c 6520 6c61 7965 7220 6669 6c74 6572  gle layer filter
+00003540: 2c20 6164 6420 616e 6f74 6865 7220 7073  , add another ps
+00003550: 6575 646f 206c 6179 6572 2e20 536f 2074  eudo layer. So t
+00003560: 6865 2073 696e 676c 6520 6c61 7965 7220  he single layer 
+00003570: 7265 7072 6573 656e 7473 2022 616e 6422  represents "and"
+00003580: 206c 6f67 6963 2e0a 2020 2020 2020 2020   logic..        
+00003590: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000035a0: 6528 6669 6c74 6572 735b 305d 2c20 7475  e(filters[0], tu
+000035b0: 706c 6529 2061 6e64 2028 0a20 2020 2020  ple) and (.     
+000035c0: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
+000035d0: 696c 7465 7273 5b30 5d29 203d 3d20 3020  ilters[0]) == 0 
+000035e0: 6f72 206e 6f74 2069 7369 6e73 7461 6e63  or not isinstanc
+000035f0: 6528 6c69 7374 2866 696c 7465 7273 5b30  e(list(filters[0
+00003600: 5d29 5b30 5d2c 2074 7570 6c65 290a 2020  ])[0], tuple).  
+00003610: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00003620: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00003630: 7465 7273 203d 2074 7970 696e 672e 6361  ters = typing.ca
+00003640: 7374 2874 6869 7264 5f70 6172 7479 5f70  st(third_party_p
+00003650: 616e 6461 735f 6762 712e 4669 6c74 6572  andas_gbq.Filter
+00003660: 7354 7970 652c 205b 6669 6c74 6572 735d  sType, [filters]
+00003670: 290a 0a20 2020 2020 2020 2020 2020 206f  )..            o
+00003680: 725f 6578 7072 6573 7369 6f6e 7320 3d20  r_expressions = 
+00003690: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000036a0: 6f72 2067 726f 7570 2069 6e20 6669 6c74  or group in filt
+000036b0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+000036c0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+000036d0: 7374 616e 6365 2867 726f 7570 2c20 4974  stance(group, It
+000036e0: 6572 6162 6c65 293a 0a20 2020 2020 2020  erable):.       
+000036f0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
+00003700: 7570 203d 205b 6772 6f75 705d 0a0a 2020  up = [group]..  
+00003710: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00003720: 645f 6578 7072 6573 7369 6f6e 7320 3d20  d_expressions = 
+00003730: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+00003740: 2020 2066 6f72 2066 696c 7465 725f 6974     for filter_it
+00003750: 656d 2069 6e20 6772 6f75 703a 0a20 2020  em in group:.   
+00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003770: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00003780: 6365 2866 696c 7465 725f 6974 656d 2c20  ce(filter_item, 
+00003790: 7475 706c 6529 206f 7220 286c 656e 2866  tuple) or (len(f
+000037a0: 696c 7465 725f 6974 656d 2920 213d 2033  ilter_item) != 3
+000037b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000037c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000037d0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 2020 2020 2020 2020 2066 2246 696c 7465           f"Filte
+00003800: 7220 636f 6e64 6974 696f 6e20 7368 6f75  r condition shou
+00003810: 6c64 2062 6520 6120 7475 706c 6520 6f66  ld be a tuple of
+00003820: 206c 656e 6774 6820 332c 207b 6669 6c74   length 3, {filt
+00003830: 6572 5f69 7465 6d7d 2069 7320 6e6f 7420  er_item} is not 
+00003840: 7661 6c69 642e 220a 2020 2020 2020 2020  valid.".        
 00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00003870: 6e63 6528 636f 6c75 6d6e 2c20 7374 7229  nce(column, str)
-00003880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003890: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000038a0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2020 2020 2020 2020 6622 436f 6c75 6d6e          f"Column
-000038d0: 206e 616d 6520 7368 6f75 6c64 2062 6520   name should be 
-000038e0: 6120 7374 7269 6e67 2c20 6275 7420 7265  a string, but re
-000038f0: 6365 6976 6564 2027 7b63 6f6c 756d 6e7d  ceived '{column}
-00003900: 2720 6f66 2074 7970 6520 7b74 7970 6528  ' of type {type(
-00003910: 636f 6c75 6d6e 292e 5f5f 6e61 6d65 5f5f  column).__name__
-00003920: 7d2e 220a 2020 2020 2020 2020 2020 2020  }.".            
-00003930: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003950: 2020 2069 6620 6f70 6572 6174 6f72 206e     if operator n
-00003960: 6f74 2069 6e20 7661 6c69 645f 6f70 6572  ot in valid_oper
-00003970: 6174 6f72 733a 0a20 2020 2020 2020 2020  ators:.         
-00003980: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003990: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000039a0: 6622 4f70 6572 6174 6f72 207b 6f70 6572  f"Operator {oper
-000039b0: 6174 6f72 7d20 6973 206e 6f74 2076 616c  ator} is not val
-000039c0: 6964 2e22 290a 0a20 2020 2020 2020 2020  id.")..         
-000039d0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-000039e0: 746f 725f 7374 7220 3d20 7661 6c69 645f  tor_str = valid_
-000039f0: 6f70 6572 6174 6f72 735b 6f70 6572 6174  operators[operat
-00003a00: 6f72 5d0a 0a20 2020 2020 2020 2020 2020  or]..           
-00003a10: 2020 2020 2020 2020 2069 6620 6f70 6572           if oper
-00003a20: 6174 6f72 5f73 7472 2069 6e20 5b22 494e  ator_str in ["IN
-00003a30: 222c 2022 4e4f 5420 494e 225d 3a0a 2020  ", "NOT IN"]:.  
-00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 2020 2020 2020 7661 6c75 655f 6c69 7374        value_list
-00003a60: 203d 2022 2c20 222e 6a6f 696e 285b 7265   = ", ".join([re
-00003a70: 7072 2876 2920 666f 7220 7620 696e 2076  pr(v) for v in v
-00003a80: 616c 7565 5d29 0a20 2020 2020 2020 2020  alue]).         
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003aa0: 7870 7265 7373 696f 6e20 3d20 6622 607b  xpression = f"`{
-00003ab0: 636f 6c75 6d6e 7d60 207b 6f70 6572 6174  column}` {operat
-00003ac0: 6f72 5f73 7472 7d20 287b 7661 6c75 655f  or_str} ({value_
-00003ad0: 6c69 7374 7d29 220a 2020 2020 2020 2020  list})".        
-00003ae0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003af0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003b00: 2020 2020 2020 2020 2020 6578 7072 6573            expres
-00003b10: 7369 6f6e 203d 2066 2260 7b63 6f6c 756d  sion = f"`{colum
-00003b20: 6e7d 6020 7b6f 7065 7261 746f 725f 7374  n}` {operator_st
-00003b30: 727d 207b 7265 7072 2876 616c 7565 297d  r} {repr(value)}
-00003b40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003b50: 2020 2020 2020 616e 645f 6578 7072 6573        and_expres
-00003b60: 7369 6f6e 732e 6170 7065 6e64 2865 7870  sions.append(exp
-00003b70: 7265 7373 696f 6e29 0a0a 2020 2020 2020  ression)..      
-00003b80: 2020 2020 2020 2020 2020 6f72 5f65 7870            or_exp
-00003b90: 7265 7373 696f 6e73 2e61 7070 656e 6428  ressions.append(
-00003ba0: 2220 414e 4420 222e 6a6f 696e 2861 6e64  " AND ".join(and
-00003bb0: 5f65 7870 7265 7373 696f 6e73 2929 0a0a  _expressions))..
-00003bc0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00003bd0: 725f 6578 7072 6573 7369 6f6e 733a 0a20  r_expressions:. 
-00003be0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00003bf0: 6865 7265 5f63 6c61 7573 6520 3d20 2220  here_clause = " 
-00003c00: 5748 4552 4520 2220 2b20 2220 4f52 2022  WHERE " + " OR "
-00003c10: 2e6a 6f69 6e28 6f72 5f65 7870 7265 7373  .join(or_express
-00003c20: 696f 6e73 290a 0a20 2020 2020 2020 2066  ions)..        f
-00003c30: 756c 6c5f 7175 6572 7920 3d20 6622 7b73  ull_query = f"{s
-00003c40: 656c 6563 745f 636c 6175 7365 7d20 4652  elect_clause} FR
-00003c50: 4f4d 207b 7375 625f 7175 6572 797d 2041  OM {sub_query} A
-00003c60: 5320 7375 627b 7768 6572 655f 636c 6175  S sub{where_clau
-00003c70: 7365 7d22 0a20 2020 2020 2020 2072 6574  se}".        ret
-00003c80: 7572 6e20 6675 6c6c 5f71 7565 7279 0a0a  urn full_query..
-00003c90: 2020 2020 6465 6620 5f71 7565 7279 5f74      def _query_t
-00003ca0: 6f5f 6465 7374 696e 6174 696f 6e28 0a20  o_destination(. 
-00003cb0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00003cc0: 2020 2020 2071 7565 7279 3a20 7374 722c       query: str,
-00003cd0: 0a20 2020 2020 2020 2069 6e64 6578 5f63  .        index_c
-00003ce0: 6f6c 733a 204c 6973 745b 7374 725d 2c0a  ols: List[str],.
-00003cf0: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
-00003d00: 3a20 7374 722c 0a20 2020 2020 2020 2063  : str,.        c
-00003d10: 6f6e 6669 6775 7261 7469 6f6e 3a20 6469  onfiguration: di
-00003d20: 6374 203d 207b 2271 7565 7279 223a 207b  ct = {"query": {
-00003d30: 2275 7365 5175 6572 7943 6163 6865 223a  "useQueryCache":
-00003d40: 2054 7275 657d 7d2c 0a20 2020 2029 202d   True}},.    ) -
-00003d50: 3e20 5475 706c 655b 4f70 7469 6f6e 616c  > Tuple[Optional
-00003d60: 5b62 6967 7175 6572 792e 5461 626c 6552  [bigquery.TableR
-00003d70: 6566 6572 656e 6365 5d2c 204f 7074 696f  eference], Optio
-00003d80: 6e61 6c5b 6269 6771 7565 7279 2e51 7565  nal[bigquery.Que
-00003d90: 7279 4a6f 625d 5d3a 0a20 2020 2020 2020  ryJob]]:.       
-00003da0: 2023 2049 6620 6120 6472 795f 7275 6e20   # If a dry_run 
-00003db0: 696e 6469 6361 7465 7320 7468 6973 2069  indicates this i
-00003dc0: 7320 6e6f 7420 6120 7175 6572 7920 7479  s not a query ty
-00003dd0: 7065 206a 6f62 2c20 7468 656e 2064 6f6e  pe job, then don
-00003de0: 2774 0a20 2020 2020 2020 2023 2062 6f74  't.        # bot
-00003df0: 6865 7220 7472 7969 6e67 2074 6f20 646f  her trying to do
-00003e00: 2061 2043 5245 4154 4520 5445 4d50 2054   a CREATE TEMP T
-00003e10: 4142 4c45 202e 2e2e 2041 5320 5345 4c45  ABLE ... AS SELE
-00003e20: 4354 202e 2e2e 2073 7461 7465 6d65 6e74  CT ... statement
-00003e30: 2e0a 2020 2020 2020 2020 6472 795f 7275  ..        dry_ru
-00003e40: 6e5f 636f 6e66 6967 203d 2062 6967 7175  n_config = bigqu
-00003e50: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
-00003e60: 6967 2829 0a20 2020 2020 2020 2064 7279  ig().        dry
-00003e70: 5f72 756e 5f63 6f6e 6669 672e 6472 795f  _run_config.dry_
-00003e80: 7275 6e20 3d20 5472 7565 0a20 2020 2020  run = True.     
-00003e90: 2020 205f 2c20 6472 795f 7275 6e5f 6a6f     _, dry_run_jo
-00003ea0: 6220 3d20 7365 6c66 2e5f 7374 6172 745f  b = self._start_
-00003eb0: 7175 6572 7928 7175 6572 792c 206a 6f62  query(query, job
-00003ec0: 5f63 6f6e 6669 673d 6472 795f 7275 6e5f  _config=dry_run_
-00003ed0: 636f 6e66 6967 290a 2020 2020 2020 2020  config).        
-00003ee0: 6966 2064 7279 5f72 756e 5f6a 6f62 2e73  if dry_run_job.s
-00003ef0: 7461 7465 6d65 6e74 5f74 7970 6520 213d  tatement_type !=
-00003f00: 2022 5345 4c45 4354 223a 0a20 2020 2020   "SELECT":.     
-00003f10: 2020 2020 2020 205f 2c20 7175 6572 795f         _, query_
-00003f20: 6a6f 6220 3d20 7365 6c66 2e5f 7374 6172  job = self._star
-00003f30: 745f 7175 6572 7928 7175 6572 7929 0a20  t_query(query). 
-00003f40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003f50: 6e20 7175 6572 795f 6a6f 622e 6465 7374  n query_job.dest
-00003f60: 696e 6174 696f 6e2c 2071 7565 7279 5f6a  ination, query_j
-00003f70: 6f62 0a0a 2020 2020 2020 2020 2320 4372  ob..        # Cr
-00003f80: 6561 7465 2061 2074 6162 6c65 2074 6f20  eate a table to 
-00003f90: 776f 726b 6172 6f75 6e64 2042 6967 5175  workaround BigQu
-00003fa0: 6572 7920 3130 2047 4220 7175 6572 7920  ery 10 GB query 
-00003fb0: 7265 7375 6c74 7320 6c69 6d69 742e 2053  results limit. S
-00003fc0: 6565 3a0a 2020 2020 2020 2020 2320 696e  ee:.        # in
-00003fd0: 7465 726e 616c 2069 7373 7565 2033 3033  ternal issue 303
-00003fe0: 3035 3733 3336 2e0a 2020 2020 2020 2020  057336..        
-00003ff0: 2320 5369 6e63 6520 7765 2068 6176 6520  # Since we have 
-00004000: 6120 6073 7461 7465 6d65 6e74 5f74 7970  a `statement_typ
-00004010: 6520 3d3d 2027 5345 4c45 4354 2760 2c20  e == 'SELECT'`, 
-00004020: 7363 6865 6d61 2073 686f 756c 6420 6265  schema should be
-00004030: 2070 6f70 756c 6174 6564 2e0a 2020 2020   populated..    
-00004040: 2020 2020 7363 6865 6d61 203d 2074 7970      schema = typ
-00004050: 696e 672e 6361 7374 2849 7465 7261 626c  ing.cast(Iterabl
-00004060: 655b 6269 6771 7565 7279 2e53 6368 656d  e[bigquery.Schem
-00004070: 6146 6965 6c64 5d2c 2064 7279 5f72 756e  aField], dry_run
-00004080: 5f6a 6f62 2e73 6368 656d 6129 0a20 2020  _job.schema).   
-00004090: 2020 2020 2063 6c75 7374 6572 5f63 6f6c       cluster_col
-000040a0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-000040b0: 2020 6974 656d 2e6e 616d 650a 2020 2020    item.name.    
-000040c0: 2020 2020 2020 2020 666f 7220 6974 656d          for item
-000040d0: 2069 6e20 7363 6865 6d61 0a20 2020 2020   in schema.     
-000040e0: 2020 2020 2020 2069 6620 2869 7465 6d2e         if (item.
-000040f0: 6e61 6d65 2069 6e20 696e 6465 785f 636f  name in index_co
-00004100: 6c73 2920 616e 6420 5f63 616e 5f63 6c75  ls) and _can_clu
-00004110: 7374 6572 5f62 7128 6974 656d 290a 2020  ster_bq(item).  
-00004120: 2020 2020 2020 5d5b 3a5f 4d41 585f 434c        ][:_MAX_CL
-00004130: 5553 5445 525f 434f 4c55 4d4e 535d 0a20  USTER_COLUMNS]. 
-00004140: 2020 2020 2020 2074 656d 705f 7461 626c         temp_tabl
-00004150: 6520 3d20 7365 6c66 2e5f 6372 6561 7465  e = self._create
-00004160: 5f65 6d70 7479 5f74 656d 705f 7461 626c  _empty_temp_tabl
-00004170: 6528 7363 6865 6d61 2c20 636c 7573 7465  e(schema, cluste
-00004180: 725f 636f 6c73 290a 0a20 2020 2020 2020  r_cols)..       
-00004190: 2074 696d 656f 7574 5f6d 7320 3d20 636f   timeout_ms = co
-000041a0: 6e66 6967 7572 6174 696f 6e2e 6765 7428  nfiguration.get(
-000041b0: 226a 6f62 5469 6d65 6f75 744d 7322 2920  "jobTimeoutMs") 
-000041c0: 6f72 2063 6f6e 6669 6775 7261 7469 6f6e  or configuration
-000041d0: 5b22 7175 6572 7922 5d2e 6765 7428 0a20  ["query"].get(. 
-000041e0: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
-000041f0: 6f75 744d 7322 0a20 2020 2020 2020 2029  outMs".        )
-00004200: 0a0a 2020 2020 2020 2020 2320 436f 6e76  ..        # Conv
-00004210: 6572 7420 7469 6d65 6f75 745f 6d73 2074  ert timeout_ms t
-00004220: 6f20 7365 636f 6e64 732c 2065 6e73 7572  o seconds, ensur
-00004230: 696e 6720 6120 6d69 6e69 6d75 6d20 6f66  ing a minimum of
-00004240: 2030 2e31 2073 6563 6f6e 6473 2074 6f20   0.1 seconds to 
-00004250: 6176 6f69 640a 2020 2020 2020 2020 2320  avoid.        # 
-00004260: 7468 6520 7072 6f67 7261 6d20 6765 7474  the program gett
-00004270: 696e 6720 7374 7563 6b20 6f6e 2074 6f6f  ing stuck on too
-00004280: 2d73 686f 7274 2074 696d 656f 7574 732e  -short timeouts.
-00004290: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
-000042a0: 203d 206d 6178 2869 6e74 2874 696d 656f   = max(int(timeo
-000042b0: 7574 5f6d 7329 202a 2031 652d 332c 2030  ut_ms) * 1e-3, 0
-000042c0: 2e31 2920 6966 2074 696d 656f 7574 5f6d  .1) if timeout_m
-000042d0: 7320 656c 7365 204e 6f6e 650a 0a20 2020  s else None..   
-000042e0: 2020 2020 206a 6f62 5f63 6f6e 6669 6720       job_config 
-000042f0: 3d20 7479 7069 6e67 2e63 6173 7428 0a20  = typing.cast(. 
-00004300: 2020 2020 2020 2020 2020 2062 6967 7175             bigqu
-00004310: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
-00004320: 6967 2c0a 2020 2020 2020 2020 2020 2020  ig,.            
-00004330: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-00004340: 6243 6f6e 6669 672e 6672 6f6d 5f61 7069  bConfig.from_api
-00004350: 5f72 6570 7228 636f 6e66 6967 7572 6174  _repr(configurat
-00004360: 696f 6e29 2c0a 2020 2020 2020 2020 290a  ion),.        ).
-00004370: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-00004380: 6967 2e6c 6162 656c 735b 2262 6967 6672  ig.labels["bigfr
-00004390: 616d 6573 2d61 7069 225d 203d 2061 7069  ames-api"] = api
-000043a0: 5f6e 616d 650a 2020 2020 2020 2020 6a6f  _name.        jo
-000043b0: 625f 636f 6e66 6967 2e64 6573 7469 6e61  b_config.destina
-000043c0: 7469 6f6e 203d 2074 656d 705f 7461 626c  tion = temp_tabl
-000043d0: 650a 0a20 2020 2020 2020 2074 7279 3a0a  e..        try:.
-000043e0: 2020 2020 2020 2020 2020 2020 2320 5772              # Wr
-000043f0: 6974 6520 746f 2074 656d 7020 7461 626c  ite to temp tabl
-00004400: 6520 746f 2077 6f72 6b61 726f 756e 6420  e to workaround 
-00004410: 4269 6751 7565 7279 2031 3020 4742 2071  BigQuery 10 GB q
-00004420: 7565 7279 2072 6573 756c 7473 0a20 2020  uery results.   
-00004430: 2020 2020 2020 2020 2023 206c 696d 6974           # limit
-00004440: 2e20 5365 653a 2069 6e74 6572 6e61 6c20  . See: internal 
-00004450: 6973 7375 6520 3330 3330 3537 3333 362e  issue 303057336.
-00004460: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-00004470: 5f63 6f6e 6669 672e 6c61 6265 6c73 5b22  _config.labels["
-00004480: 6572 726f 725f 6361 7567 6874 225d 203d  error_caught"] =
-00004490: 2022 7472 7565 220a 2020 2020 2020 2020   "true".        
-000044a0: 2020 2020 5f2c 2071 7565 7279 5f6a 6f62      _, query_job
-000044b0: 203d 2073 656c 662e 5f73 7461 7274 5f71   = self._start_q
-000044c0: 7565 7279 280a 2020 2020 2020 2020 2020  uery(.          
-000044d0: 2020 2020 2020 7175 6572 792c 206a 6f62        query, job
-000044e0: 5f63 6f6e 6669 673d 6a6f 625f 636f 6e66  _config=job_conf
-000044f0: 6967 2c20 7469 6d65 6f75 743d 7469 6d65  ig, timeout=time
-00004500: 6f75 740a 2020 2020 2020 2020 2020 2020  out.            
-00004510: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00004520: 7475 726e 2071 7565 7279 5f6a 6f62 2e64  turn query_job.d
-00004530: 6573 7469 6e61 7469 6f6e 2c20 7175 6572  estination, quer
-00004540: 795f 6a6f 620a 2020 2020 2020 2020 6578  y_job.        ex
-00004550: 6365 7074 2067 6f6f 676c 652e 6170 695f  cept google.api_
-00004560: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
-00004570: 4261 6452 6571 7565 7374 3a0a 2020 2020  BadRequest:.    
-00004580: 2020 2020 2020 2020 2320 536f 6d65 2053          # Some S
-00004590: 454c 4543 5420 7374 6174 656d 656e 7473  ELECT statements
-000045a0: 2073 7469 6c6c 2061 7265 6e27 7420 636f   still aren't co
-000045b0: 6d70 6174 6962 6c65 2077 6974 6820 636c  mpatible with cl
-000045c0: 7573 7465 720a 2020 2020 2020 2020 2020  uster.          
-000045d0: 2020 2320 7461 626c 6573 2061 7320 7468    # tables as th
-000045e0: 6520 6465 7374 696e 6174 696f 6e2e 2046  e destination. F
-000045f0: 6f72 2065 7861 6d70 6c65 2c20 6966 2074  or example, if t
-00004600: 6865 2071 7565 7279 2068 6173 2061 0a20  he query has a. 
-00004610: 2020 2020 2020 2020 2020 2023 2074 6f70             # top
-00004620: 2d6c 6576 656c 204f 5244 4552 2042 592c  -level ORDER BY,
-00004630: 2074 6869 7320 636f 6e66 6c69 6374 7320   this conflicts 
-00004640: 7769 7468 206f 7572 2061 6269 6c69 7479  with our ability
-00004650: 2074 6f20 636c 7573 7465 720a 2020 2020   to cluster.    
-00004660: 2020 2020 2020 2020 2320 7468 6520 7461          # the ta
-00004670: 626c 6520 6279 2074 6865 2069 6e64 6578  ble by the index
-00004680: 2063 6f6c 756d 6e28 7329 2e0a 2020 2020   column(s)..    
-00004690: 2020 2020 2020 2020 5f2c 2071 7565 7279          _, query
-000046a0: 5f6a 6f62 203d 2073 656c 662e 5f73 7461  _job = self._sta
-000046b0: 7274 5f71 7565 7279 2871 7565 7279 2c20  rt_query(query, 
-000046c0: 7469 6d65 6f75 743d 7469 6d65 6f75 7429  timeout=timeout)
-000046d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000046e0: 7572 6e20 7175 6572 795f 6a6f 622e 6465  urn query_job.de
-000046f0: 7374 696e 6174 696f 6e2c 2071 7565 7279  stination, query
-00004700: 5f6a 6f62 0a0a 2020 2020 6465 6620 7265  _job..    def re
-00004710: 6164 5f67 6271 5f71 7565 7279 280a 2020  ad_gbq_query(.  
-00004720: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00004730: 2020 2020 7175 6572 793a 2073 7472 2c0a      query: str,.
-00004740: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-00004750: 2020 2069 6e64 6578 5f63 6f6c 3a20 4974     index_col: It
-00004760: 6572 6162 6c65 5b73 7472 5d20 7c20 7374  erable[str] | st
-00004770: 7220 3d20 2829 2c0a 2020 2020 2020 2020  r = (),.        
-00004780: 636f 6c75 6d6e 733a 2049 7465 7261 626c  columns: Iterabl
-00004790: 655b 7374 725d 203d 2028 292c 0a20 2020  e[str] = (),.   
-000047a0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-000047b0: 6f6e 3a20 4f70 7469 6f6e 616c 5b44 6963  on: Optional[Dic
-000047c0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-000047d0: 2020 206d 6178 5f72 6573 756c 7473 3a20     max_results: 
-000047e0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000047f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7573  None,.        us
-00004800: 655f 6361 6368 653a 204f 7074 696f 6e61  e_cache: Optiona
-00004810: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
-00004820: 2020 2020 2020 2020 636f 6c5f 6f72 6465          col_orde
-00004830: 723a 2049 7465 7261 626c 655b 7374 725d  r: Iterable[str]
-00004840: 203d 2028 292c 0a20 2020 2029 202d 3e20   = (),.    ) -> 
-00004850: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-00004860: 616d 653a 0a20 2020 2020 2020 2022 2222  ame:.        """
-00004870: 5475 726e 2061 2053 514c 2071 7565 7279  Turn a SQL query
-00004880: 2069 6e74 6f20 6120 4461 7461 4672 616d   into a DataFram
-00004890: 652e 0a0a 2020 2020 2020 2020 4e6f 7465  e...        Note
-000048a0: 3a20 4265 6361 7573 6520 7468 6520 7265  : Because the re
-000048b0: 7375 6c74 7320 6172 6520 7772 6974 7465  sults are writte
-000048c0: 6e20 746f 2061 2074 656d 706f 7261 7279  n to a temporary
-000048d0: 2074 6162 6c65 2c20 6f72 6465 7269 6e67   table, ordering
-000048e0: 2062 790a 2020 2020 2020 2020 6060 4f52   by.        ``OR
-000048f0: 4445 5220 4259 6060 2069 7320 6e6f 7420  DER BY`` is not 
-00004900: 7072 6573 6572 7665 642e 2041 2075 6e69  preserved. A uni
-00004910: 7175 6520 6069 6e64 6578 5f63 6f6c 6020  que `index_col` 
-00004920: 6973 2072 6563 6f6d 6d65 6e64 6564 2e20  is recommended. 
-00004930: 5573 650a 2020 2020 2020 2020 6060 726f  Use.        ``ro
-00004940: 775f 6e75 6d62 6572 2829 206f 7665 7220  w_number() over 
-00004950: 2829 6060 2069 6620 7468 6572 6520 6973  ()`` if there is
-00004960: 206e 6f20 6e61 7475 7261 6c20 756e 6971   no natural uniq
-00004970: 7565 2069 6e64 6578 206f 7220 796f 750a  ue index or you.
-00004980: 2020 2020 2020 2020 7761 6e74 2074 6f20          want to 
-00004990: 7072 6573 6572 7665 206f 7264 6572 696e  preserve orderin
-000049a0: 672e 0a0a 2020 2020 2020 2020 2a2a 4578  g...        **Ex
-000049b0: 616d 706c 6573 3a2a 2a0a 0a20 2020 2020  amples:**..     
-000049c0: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-000049d0: 7420 6269 6766 7261 6d65 732e 7061 6e64  t bigframes.pand
-000049e0: 6173 2061 7320 6270 640a 2020 2020 2020  as as bpd.      
-000049f0: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
-00004a00: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
-00004a10: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
-00004a20: 650a 0a20 2020 2020 2020 2053 696d 706c  e..        Simpl
-00004a30: 6520 7175 6572 7920 696e 7075 743a 0a0a  e query input:..
-00004a40: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00004a50: 6466 203d 2062 7064 2e72 6561 645f 6762  df = bpd.read_gb
-00004a60: 715f 7175 6572 7928 2727 270a 2020 2020  q_query('''.    
-00004a70: 2020 2020 2020 2020 2e2e 2e20 2020 2053          ...    S
-00004a80: 454c 4543 540a 2020 2020 2020 2020 2020  ELECT.          
-00004a90: 2020 2e2e 2e20 2020 2020 2020 7069 7463    ...       pitc
-00004aa0: 6865 7246 6972 7374 4e61 6d65 2c0a 2020  herFirstName,.  
-00004ab0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00004ac0: 2020 2020 7069 7463 6865 724c 6173 744e      pitcherLastN
-00004ad0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00004ae0: 202e 2e2e 2020 2020 2020 2070 6974 6368   ...       pitch
-00004af0: 5370 6565 642c 0a20 2020 2020 2020 2020  Speed,.         
-00004b00: 2020 202e 2e2e 2020 2020 4652 4f4d 2060     ...    FROM `
-00004b10: 6269 6771 7565 7279 2d70 7562 6c69 632d  bigquery-public-
-00004b20: 6461 7461 2e62 6173 6562 616c 6c2e 6761  data.baseball.ga
-00004b30: 6d65 735f 7769 6465 600a 2020 2020 2020  mes_wide`.      
-00004b40: 2020 2020 2020 2e2e 2e20 2727 2729 0a0a        ... ''')..
-00004b50: 2020 2020 2020 2020 5072 6573 6572 7665          Preserve
-00004b60: 206f 7264 6572 696e 6720 696e 2061 2071   ordering in a q
-00004b70: 7565 7279 2069 6e70 7574 2e0a 0a20 2020  uery input...   
-00004b80: 2020 2020 2020 2020 203e 3e3e 2064 6620           >>> df 
-00004b90: 3d20 6270 642e 7265 6164 5f67 6271 5f71  = bpd.read_gbq_q
-00004ba0: 7565 7279 2827 2727 0a20 2020 2020 2020  uery('''.       
-00004bb0: 2020 2020 202e 2e2e 2020 2020 5345 4c45       ...    SELE
-00004bc0: 4354 0a20 2020 2020 2020 2020 2020 202e  CT.            .
-00004bd0: 2e2e 2020 2020 2020 202d 2d20 496e 7374  ..       -- Inst
-00004be0: 6561 6420 6f66 2061 6e20 4f52 4445 5220  ead of an ORDER 
-00004bf0: 4259 2063 6c61 7573 6520 6f6e 2074 6865  BY clause on the
-00004c00: 2071 7565 7279 2c20 7573 650a 2020 2020   query, use.    
-00004c10: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00004c20: 2020 2d2d 2052 4f57 5f4e 554d 4245 5228    -- ROW_NUMBER(
-00004c30: 2920 746f 2063 7265 6174 6520 616e 206f  ) to create an o
-00004c40: 7264 6572 6564 2044 6174 6146 7261 6d65  rdered DataFrame
-00004c50: 2e0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00004c60: 2e20 2020 2020 2020 524f 575f 4e55 4d42  .       ROW_NUMB
-00004c70: 4552 2829 204f 5645 5220 284f 5244 4552  ER() OVER (ORDER
-00004c80: 2042 5920 4156 4728 7069 7463 6853 7065   BY AVG(pitchSpe
-00004c90: 6564 2920 4445 5343 290a 2020 2020 2020  ed) DESC).      
-00004ca0: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
-00004cb0: 2020 4153 2072 6f77 696e 6465 782c 0a20    AS rowindex,. 
-00004cc0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
-00004cd0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-00004ce0: 2020 2020 2070 6974 6368 6572 4669 7273       pitcherFirs
-00004cf0: 744e 616d 652c 0a20 2020 2020 2020 2020  tName,.         
-00004d00: 2020 202e 2e2e 2020 2020 2020 2070 6974     ...       pit
-00004d10: 6368 6572 4c61 7374 4e61 6d65 2c0a 2020  cherLastName,.  
-00004d20: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00004d30: 2020 2020 4156 4728 7069 7463 6853 7065      AVG(pitchSpe
-00004d40: 6564 2920 4153 2061 7665 7261 6765 5069  ed) AS averagePi
-00004d50: 7463 6853 7065 6564 0a20 2020 2020 2020  tchSpeed.       
-00004d60: 2020 2020 202e 2e2e 2020 2020 2046 524f       ...     FRO
-00004d70: 4d20 6062 6967 7175 6572 792d 7075 626c  M `bigquery-publ
-00004d80: 6963 2d64 6174 612e 6261 7365 6261 6c6c  ic-data.baseball
-00004d90: 2e67 616d 6573 5f77 6964 6560 0a20 2020  .games_wide`.   
-00004da0: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00004db0: 2057 4845 5245 2079 6561 7220 3d20 3230   WHERE year = 20
-00004dc0: 3136 0a20 2020 2020 2020 2020 2020 202e  16.            .
-00004dd0: 2e2e 2020 2020 2047 524f 5550 2042 5920  ..     GROUP BY 
-00004de0: 7069 7463 6865 7246 6972 7374 4e61 6d65  pitcherFirstName
-00004df0: 2c20 7069 7463 6865 724c 6173 744e 616d  , pitcherLastNam
-00004e00: 650a 2020 2020 2020 2020 2020 2020 2e2e  e.            ..
-00004e10: 2e20 2727 272c 2069 6e64 6578 5f63 6f6c  . ''', index_col
-00004e20: 3d22 726f 7769 6e64 6578 2229 0a20 2020  ="rowindex").   
-00004e30: 2020 2020 2020 2020 203e 3e3e 2064 662e           >>> df.
-00004e40: 6865 6164 2832 290a 2020 2020 2020 2020  head(2).        
-00004e50: 2020 2020 2020 2020 2020 2020 2070 6974               pit
-00004e60: 6368 6572 4669 7273 744e 616d 6520 7069  cherFirstName pi
-00004e70: 7463 6865 724c 6173 744e 616d 6520 2061  tcherLastName  a
-00004e80: 7665 7261 6765 5069 7463 6853 7065 6564  veragePitchSpeed
-00004e90: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
-00004ea0: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
-00004eb0: 2020 3120 2020 2020 2020 2020 2020 2020    1             
-00004ec0: 2020 2041 6c62 6572 7469 6e20 2020 2020     Albertin     
-00004ed0: 2020 2020 4368 6170 6d61 6e20 2020 2020      Chapman     
-00004ee0: 2020 2020 2039 362e 3531 3431 3133 0a20       96.514113. 
-00004ef0: 2020 2020 2020 2020 2020 2032 2020 2020             2    
-00004f00: 2020 2020 2020 2020 2020 2020 205a 6163               Zac
-00004f10: 6861 7279 2020 2020 2020 2020 2042 7269  hary         Bri
-00004f20: 7474 6f6e 2020 2020 2020 2020 2020 3934  tton          94
-00004f30: 2e35 3931 3033 390a 2020 2020 2020 2020  .591039.        
-00004f40: 2020 2020 3c42 4c41 4e4b 4c49 4e45 3e0a      <BLANKLINE>.
-00004f50: 2020 2020 2020 2020 2020 2020 5b32 2072              [2 r
-00004f60: 6f77 7320 7820 3320 636f 6c75 6d6e 735d  ows x 3 columns]
-00004f70: 0a0a 2020 2020 2020 2020 5365 6520 616c  ..        See al
-00004f80: 736f 3a20 3a6d 6574 683a 6053 6573 7369  so: :meth:`Sessi
-00004f90: 6f6e 2e72 6561 645f 6762 7160 2e0a 2020  on.read_gbq`..  
-00004fa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00004fb0: 2020 2320 4e4f 5445 3a20 5468 6973 206d    # NOTE: This m
-00004fc0: 6574 686f 6420 646f 6573 6e27 7420 2879  ethod doesn't (y
-00004fd0: 6574 2920 6578 6973 7420 696e 2070 616e  et) exist in pan
-00004fe0: 6461 7320 6f72 2070 616e 6461 732d 6762  das or pandas-gb
-00004ff0: 712c 2073 6f0a 2020 2020 2020 2020 2320  q, so.        # 
-00005000: 7468 6573 6520 646f 6373 7472 696e 6773  these docstrings
-00005010: 2061 7265 2069 6e6c 696e 652e 0a20 2020   are inline..   
-00005020: 2020 2020 2069 6620 636f 6c75 6d6e 7320       if columns 
-00005030: 616e 6420 636f 6c5f 6f72 6465 723a 0a20  and col_order:. 
-00005040: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00005050: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00005060: 2020 2020 2020 2020 2020 2020 2022 4d75               "Mu
-00005070: 7374 2073 7065 6369 6679 2065 6974 6865  st specify eithe
-00005080: 7220 636f 6c75 6d6e 7320 2870 7265 6665  r columns (prefe
-00005090: 7272 6564 2920 6f72 2063 6f6c 5f6f 7264  rred) or col_ord
-000050a0: 6572 2c20 6e6f 7420 626f 7468 220a 2020  er, not both".  
-000050b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000050c0: 2020 2020 656c 6966 2063 6f6c 5f6f 7264      elif col_ord
-000050d0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-000050e0: 636f 6c75 6d6e 7320 3d20 636f 6c5f 6f72  columns = col_or
-000050f0: 6465 720a 0a20 2020 2020 2020 2072 6574  der..        ret
-00005100: 7572 6e20 7365 6c66 2e5f 7265 6164 5f67  urn self._read_g
-00005110: 6271 5f71 7565 7279 280a 2020 2020 2020  bq_query(.      
-00005120: 2020 2020 2020 7175 6572 793d 7175 6572        query=quer
-00005130: 792c 0a20 2020 2020 2020 2020 2020 2069  y,.            i
-00005140: 6e64 6578 5f63 6f6c 3d69 6e64 6578 5f63  ndex_col=index_c
-00005150: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
-00005160: 636f 6c75 6d6e 733d 636f 6c75 6d6e 732c  columns=columns,
-00005170: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00005180: 6669 6775 7261 7469 6f6e 3d63 6f6e 6669  figuration=confi
-00005190: 6775 7261 7469 6f6e 2c0a 2020 2020 2020  guration,.      
-000051a0: 2020 2020 2020 6d61 785f 7265 7375 6c74        max_result
-000051b0: 733d 6d61 785f 7265 7375 6c74 732c 0a20  s=max_results,. 
-000051c0: 2020 2020 2020 2020 2020 2061 7069 5f6e             api_n
-000051d0: 616d 653d 2272 6561 645f 6762 715f 7175  ame="read_gbq_qu
-000051e0: 6572 7922 2c0a 2020 2020 2020 2020 2020  ery",.          
-000051f0: 2020 7573 655f 6361 6368 653d 7573 655f    use_cache=use_
-00005200: 6361 6368 652c 0a20 2020 2020 2020 2029  cache,.        )
-00005210: 0a0a 2020 2020 6465 6620 5f72 6561 645f  ..    def _read_
-00005220: 6762 715f 7175 6572 7928 0a20 2020 2020  gbq_query(.     
-00005230: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00005240: 2071 7565 7279 3a20 7374 722c 0a20 2020   query: str,.   
-00005250: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00005260: 696e 6465 785f 636f 6c3a 2049 7465 7261  index_col: Itera
-00005270: 626c 655b 7374 725d 207c 2073 7472 203d  ble[str] | str =
-00005280: 2028 292c 0a20 2020 2020 2020 2063 6f6c   (),.        col
-00005290: 756d 6e73 3a20 4974 6572 6162 6c65 5b73  umns: Iterable[s
-000052a0: 7472 5d20 3d20 2829 2c0a 2020 2020 2020  tr] = (),.      
-000052b0: 2020 636f 6e66 6967 7572 6174 696f 6e3a    configuration:
-000052c0: 204f 7074 696f 6e61 6c5b 4469 6374 5d20   Optional[Dict] 
-000052d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000052e0: 6d61 785f 7265 7375 6c74 733a 204f 7074  max_results: Opt
-000052f0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00005300: 652c 0a20 2020 2020 2020 2061 7069 5f6e  e,.        api_n
-00005310: 616d 653a 2073 7472 203d 2022 7265 6164  ame: str = "read
-00005320: 5f67 6271 5f71 7565 7279 222c 0a20 2020  _gbq_query",.   
-00005330: 2020 2020 2075 7365 5f63 6163 6865 3a20       use_cache: 
-00005340: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00005350: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
-00005360: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-00005370: 616d 653a 0a20 2020 2020 2020 2069 6d70  ame:.        imp
-00005380: 6f72 7420 6269 6766 7261 6d65 732e 6461  ort bigframes.da
-00005390: 7461 6672 616d 6520 6173 2064 6174 6166  taframe as dataf
-000053a0: 7261 6d65 0a0a 2020 2020 2020 2020 636f  rame..        co
-000053b0: 6e66 6967 7572 6174 696f 6e20 3d20 5f74  nfiguration = _t
-000053c0: 7261 6e73 666f 726d 5f72 6561 645f 6762  ransform_read_gb
-000053d0: 715f 636f 6e66 6967 7572 6174 696f 6e28  q_configuration(
-000053e0: 636f 6e66 6967 7572 6174 696f 6e29 0a0a  configuration)..
-000053f0: 2020 2020 2020 2020 6966 2022 7175 6572          if "quer
-00005400: 7922 206e 6f74 2069 6e20 636f 6e66 6967  y" not in config
-00005410: 7572 6174 696f 6e3a 0a20 2020 2020 2020  uration:.       
-00005420: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-00005430: 6f6e 5b22 7175 6572 7922 5d20 3d20 7b7d  on["query"] = {}
-00005440: 0a0a 2020 2020 2020 2020 6966 2022 7175  ..        if "qu
-00005450: 6572 7922 2069 6e20 636f 6e66 6967 7572  ery" in configur
-00005460: 6174 696f 6e5b 2271 7565 7279 225d 3a0a  ation["query"]:.
-00005470: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00005480: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00005490: 2020 2020 2020 2020 2020 2020 2020 2254                "T
-000054a0: 6865 2071 7565 7279 2073 7461 7465 6d65  he query stateme
-000054b0: 6e74 206d 7573 7420 6e6f 7420 6265 2069  nt must not be i
-000054c0: 6e63 6c75 6465 6420 696e 2074 6865 2022  ncluded in the "
-000054d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000054e0: 2020 2227 636f 6e66 6967 7572 6174 696f    "'configuratio
-000054f0: 6e27 2062 6563 6175 7365 2069 7420 6973  n' because it is
-00005500: 2061 6c72 6561 6479 2070 726f 7669 6465   already provide
-00005510: 6420 6173 222c 0a20 2020 2020 2020 2020  d as",.         
-00005520: 2020 2020 2020 2022 2061 2073 6570 6172         " a separ
-00005530: 6174 6520 7061 7261 6d65 7465 722e 222c  ate parameter.",
-00005540: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00005550: 2020 2020 2020 2020 6966 2022 7573 6551          if "useQ
-00005560: 7565 7279 4361 6368 6522 2069 6e20 636f  ueryCache" in co
-00005570: 6e66 6967 7572 6174 696f 6e5b 2271 7565  nfiguration["que
-00005580: 7279 225d 3a0a 2020 2020 2020 2020 2020  ry"]:.          
-00005590: 2020 6966 2075 7365 5f63 6163 6865 2069    if use_cache i
-000055a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000055b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000055c0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2227 7573 6551 7565 7279 4361 6368    "'useQueryCach
-000055f0: 6527 2069 6e20 2763 6f6e 6669 6775 7261  e' in 'configura
-00005600: 7469 6f6e 2720 636f 6e66 6c69 6374 7320  tion' conflicts 
-00005610: 7769 7468 220a 2020 2020 2020 2020 2020  with".          
-00005620: 2020 2020 2020 2020 2020 2220 2775 7365            " 'use
-00005630: 5f63 6163 6865 2720 7061 7261 6d65 7465  _cache' paramete
-00005640: 722e 2050 6c65 6173 6520 7370 6563 6966  r. Please specif
-00005650: 7920 6f6e 6c79 206f 6e65 2e22 0a20 2020  y only one.".   
-00005660: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00005670: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005680: 2020 2020 2020 2020 2063 6f6e 6669 6775           configu
-00005690: 7261 7469 6f6e 5b22 7175 6572 7922 5d5b  ration["query"][
-000056a0: 2275 7365 5175 6572 7943 6163 6865 225d  "useQueryCache"]
-000056b0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000056c0: 2020 2020 2054 7275 6520 6966 2075 7365       True if use
-000056d0: 5f63 6163 6865 2069 7320 4e6f 6e65 2065  _cache is None e
-000056e0: 6c73 6520 7573 655f 6361 6368 650a 2020  lse use_cache.  
-000056f0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00005700: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00005710: 6365 2869 6e64 6578 5f63 6f6c 2c20 7374  ce(index_col, st
-00005720: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00005730: 696e 6465 785f 636f 6c73 203d 205b 696e  index_cols = [in
-00005740: 6465 785f 636f 6c5d 0a20 2020 2020 2020  dex_col].       
-00005750: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005760: 2020 2069 6e64 6578 5f63 6f6c 7320 3d20     index_cols = 
-00005770: 6c69 7374 2869 6e64 6578 5f63 6f6c 290a  list(index_col).
-00005780: 0a20 2020 2020 2020 2064 6573 7469 6e61  .        destina
-00005790: 7469 6f6e 2c20 7175 6572 795f 6a6f 6220  tion, query_job 
-000057a0: 3d20 7365 6c66 2e5f 7175 6572 795f 746f  = self._query_to
-000057b0: 5f64 6573 7469 6e61 7469 6f6e 280a 2020  _destination(.  
-000057c0: 2020 2020 2020 2020 2020 7175 6572 792c            query,
-000057d0: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-000057e0: 6578 5f63 6f6c 732c 0a20 2020 2020 2020  ex_cols,.       
-000057f0: 2020 2020 2061 7069 5f6e 616d 653d 6170       api_name=ap
-00005800: 695f 6e61 6d65 2c0a 2020 2020 2020 2020  i_name,.        
-00005810: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
-00005820: 6e3d 636f 6e66 6967 7572 6174 696f 6e2c  n=configuration,
-00005830: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00005840: 2020 2020 2320 4966 2074 6865 7265 2077      # If there w
-00005850: 6173 206e 6f20 6465 7374 696e 6174 696f  as no destinatio
-00005860: 6e20 7461 626c 652c 2074 6861 7420 6d65  n table, that me
-00005870: 616e 7320 7468 6520 7175 6572 7920 6d75  ans the query mu
-00005880: 7374 2068 6176 650a 2020 2020 2020 2020  st have.        
-00005890: 2320 6265 656e 2044 444c 206f 7220 444d  # been DDL or DM
-000058a0: 4c2e 2052 6574 7572 6e20 736f 6d65 206a  L. Return some j
-000058b0: 6f62 206d 6574 6164 6174 612c 2069 6e73  ob metadata, ins
-000058c0: 7465 6164 2e0a 2020 2020 2020 2020 6966  tead..        if
-000058d0: 206e 6f74 2064 6573 7469 6e61 7469 6f6e   not destination
-000058e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000058f0: 7475 726e 2064 6174 6166 7261 6d65 2e44  turn dataframe.D
-00005900: 6174 6146 7261 6d65 280a 2020 2020 2020  ataFrame(.      
-00005910: 2020 2020 2020 2020 2020 6461 7461 3d70            data=p
-00005920: 616e 6461 732e 4461 7461 4672 616d 6528  andas.DataFrame(
-00005930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005940: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00005950: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005960: 7374 6174 656d 656e 745f 7479 7065 223a  statement_type":
-00005970: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00005980: 2020 2020 2020 2020 2020 2020 2020 2071                 q
-00005990: 7565 7279 5f6a 6f62 2e73 7461 7465 6d65  uery_job.stateme
-000059a0: 6e74 5f74 7970 6520 6966 2071 7565 7279  nt_type if query
-000059b0: 5f6a 6f62 2065 6c73 6520 2275 6e6b 6e6f  _job else "unkno
-000059c0: 776e 220a 2020 2020 2020 2020 2020 2020  wn".            
-000059d0: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 2020 2020 2020 2022 6a6f 625f 6964 223a         "job_id":
-00005a00: 205b 7175 6572 795f 6a6f 622e 6a6f 625f   [query_job.job_
-00005a10: 6964 2069 6620 7175 6572 795f 6a6f 6220  id if query_job 
-00005a20: 656c 7365 2022 756e 6b6e 6f77 6e22 5d2c  else "unknown"],
-00005a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a40: 2020 2020 2020 2020 2022 6c6f 6361 7469           "locati
-00005a50: 6f6e 223a 205b 7175 6572 795f 6a6f 622e  on": [query_job.
-00005a60: 6c6f 6361 7469 6f6e 2069 6620 7175 6572  location if quer
-00005a70: 795f 6a6f 6220 656c 7365 2022 756e 6b6e  y_job else "unkn
-00005a80: 6f77 6e22 5d2c 0a20 2020 2020 2020 2020  own"],.         
-00005a90: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00005aa0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ac0: 7365 7373 696f 6e3d 7365 6c66 2c0a 2020  session=self,.  
-00005ad0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00005ae0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00005af0: 2e72 6561 645f 6762 715f 7461 626c 6528  .read_gbq_table(
-00005b00: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
-00005b10: 6465 7374 696e 6174 696f 6e2e 7072 6f6a  destination.proj
-00005b20: 6563 747d 2e7b 6465 7374 696e 6174 696f  ect}.{destinatio
-00005b30: 6e2e 6461 7461 7365 745f 6964 7d2e 7b64  n.dataset_id}.{d
-00005b40: 6573 7469 6e61 7469 6f6e 2e74 6162 6c65  estination.table
-00005b50: 5f69 647d 222c 0a20 2020 2020 2020 2020  _id}",.         
-00005b60: 2020 2069 6e64 6578 5f63 6f6c 3d69 6e64     index_col=ind
-00005b70: 6578 5f63 6f6c 732c 0a20 2020 2020 2020  ex_cols,.       
-00005b80: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
-00005b90: 756d 6e73 2c0a 2020 2020 2020 2020 2020  umns,.          
-00005ba0: 2020 6d61 785f 7265 7375 6c74 733d 6d61    max_results=ma
-00005bb0: 785f 7265 7375 6c74 732c 0a20 2020 2020  x_results,.     
-00005bc0: 2020 2020 2020 2075 7365 5f63 6163 6865         use_cache
-00005bd0: 3d63 6f6e 6669 6775 7261 7469 6f6e 5b22  =configuration["
-00005be0: 7175 6572 7922 5d5b 2275 7365 5175 6572  query"]["useQuer
-00005bf0: 7943 6163 6865 225d 2c0a 2020 2020 2020  yCache"],.      
-00005c00: 2020 290a 0a20 2020 2064 6566 2072 6561    )..    def rea
-00005c10: 645f 6762 715f 7461 626c 6528 0a20 2020  d_gbq_table(.   
-00005c20: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00005c30: 2020 2071 7565 7279 3a20 7374 722c 0a20     query: str,. 
-00005c40: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00005c50: 2020 696e 6465 785f 636f 6c3a 2049 7465    index_col: Ite
-00005c60: 7261 626c 655b 7374 725d 207c 2073 7472  rable[str] | str
-00005c70: 203d 2028 292c 0a20 2020 2020 2020 2063   = (),.        c
-00005c80: 6f6c 756d 6e73 3a20 4974 6572 6162 6c65  olumns: Iterable
-00005c90: 5b73 7472 5d20 3d20 2829 2c0a 2020 2020  [str] = (),.    
-00005ca0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
-00005cb0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00005cc0: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
-00005cd0: 696c 7465 7273 3a20 7468 6972 645f 7061  ilters: third_pa
-00005ce0: 7274 795f 7061 6e64 6173 5f67 6271 2e46  rty_pandas_gbq.F
-00005cf0: 696c 7465 7273 5479 7065 203d 2028 292c  iltersType = (),
-00005d00: 0a20 2020 2020 2020 2075 7365 5f63 6163  .        use_cac
-00005d10: 6865 3a20 626f 6f6c 203d 2054 7275 652c  he: bool = True,
-00005d20: 0a20 2020 2020 2020 2063 6f6c 5f6f 7264  .        col_ord
-00005d30: 6572 3a20 4974 6572 6162 6c65 5b73 7472  er: Iterable[str
-00005d40: 5d20 3d20 2829 2c0a 2020 2020 2920 2d3e  ] = (),.    ) ->
-00005d50: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
-00005d60: 7261 6d65 3a0a 2020 2020 2020 2020 2222  rame:.        ""
-00005d70: 2254 7572 6e20 6120 4269 6751 7565 7279  "Turn a BigQuery
-00005d80: 2074 6162 6c65 2069 6e74 6f20 6120 4461   table into a Da
-00005d90: 7461 4672 616d 652e 0a0a 2020 2020 2020  taFrame...      
-00005da0: 2020 2a2a 4578 616d 706c 6573 3a2a 2a0a    **Examples:**.
-00005db0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00005dc0: 2069 6d70 6f72 7420 6269 6766 7261 6d65   import bigframe
-00005dd0: 732e 7061 6e64 6173 2061 7320 6270 640a  s.pandas as bpd.
-00005de0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00005df0: 6270 642e 6f70 7469 6f6e 732e 6469 7370  bpd.options.disp
-00005e00: 6c61 792e 7072 6f67 7265 7373 5f62 6172  lay.progress_bar
-00005e10: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-00005e20: 2052 6561 6420 6120 7768 6f6c 6520 7461   Read a whole ta
-00005e30: 626c 652c 2077 6974 6820 6172 6269 7472  ble, with arbitr
-00005e40: 6172 7920 6f72 6465 7269 6e67 206f 7220  ary ordering or 
-00005e50: 6f72 6465 7269 6e67 2063 6f72 7265 7370  ordering corresp
-00005e60: 6f6e 6469 6e67 2074 6f20 7468 6520 7072  onding to the pr
-00005e70: 696d 6172 7920 6b65 7928 7329 2e0a 0a20  imary key(s)... 
-00005e80: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
-00005e90: 6620 3d20 6270 642e 7265 6164 5f67 6271  f = bpd.read_gbq
-00005ea0: 5f74 6162 6c65 2822 6269 6771 7565 7279  _table("bigquery
-00005eb0: 2d70 7562 6c69 632d 6461 7461 2e6d 6c5f  -public-data.ml_
-00005ec0: 6461 7461 7365 7473 2e70 656e 6775 696e  datasets.penguin
-00005ed0: 7322 290a 0a20 2020 2020 2020 2053 6565  s")..        See
-00005ee0: 2061 6c73 6f3a 203a 6d65 7468 3a60 5365   also: :meth:`Se
-00005ef0: 7373 696f 6e2e 7265 6164 5f67 6271 602e  ssion.read_gbq`.
-00005f00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00005f10: 2020 2020 2023 204e 4f54 453a 2054 6869       # NOTE: Thi
-00005f20: 7320 6d65 7468 6f64 2064 6f65 736e 2774  s method doesn't
-00005f30: 2028 7965 7429 2065 7869 7374 2069 6e20   (yet) exist in 
-00005f40: 7061 6e64 6173 206f 7220 7061 6e64 6173  pandas or pandas
-00005f50: 2d67 6271 2c20 736f 0a20 2020 2020 2020  -gbq, so.       
-00005f60: 2023 2074 6865 7365 2064 6f63 7374 7269   # these docstri
-00005f70: 6e67 7320 6172 6520 696e 6c69 6e65 2e0a  ngs are inline..
-00005f80: 2020 2020 2020 2020 6966 2063 6f6c 756d          if colum
-00005f90: 6e73 2061 6e64 2063 6f6c 5f6f 7264 6572  ns and col_order
-00005fa0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00005fb0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 224d 7573 7420 7370 6563 6966 7920 6569  "Must specify ei
-00005fe0: 7468 6572 2063 6f6c 756d 6e73 2028 7072  ther columns (pr
-00005ff0: 6566 6572 7265 6429 206f 7220 636f 6c5f  eferred) or col_
-00006000: 6f72 6465 722c 206e 6f74 2062 6f74 6822  order, not both"
-00006010: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00006020: 2020 2020 2020 2065 6c69 6620 636f 6c5f         elif col_
-00006030: 6f72 6465 723a 0a20 2020 2020 2020 2020  order:.         
-00006040: 2020 2063 6f6c 756d 6e73 203d 2063 6f6c     columns = col
-00006050: 5f6f 7264 6572 0a0a 2020 2020 2020 2020  _order..        
-00006060: 6669 6c74 6572 7320 3d20 6c69 7374 2866  filters = list(f
-00006070: 696c 7465 7273 290a 2020 2020 2020 2020  ilters).        
-00006080: 6966 206c 656e 2866 696c 7465 7273 2920  if len(filters) 
-00006090: 213d 2030 206f 7220 5f69 735f 7461 626c  != 0 or _is_tabl
-000060a0: 655f 7769 7468 5f77 696c 6463 6172 645f  e_with_wildcard_
-000060b0: 7375 6666 6978 2871 7565 7279 293a 0a20  suffix(query):. 
-000060c0: 2020 2020 2020 2020 2020 2071 7565 7279             query
-000060d0: 203d 2073 656c 662e 5f74 6f5f 7175 6572   = self._to_quer
-000060e0: 7928 7175 6572 792c 2063 6f6c 756d 6e73  y(query, columns
-000060f0: 2c20 6669 6c74 6572 7329 0a0a 2020 2020  , filters)..    
-00006100: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00006110: 656c 662e 5f72 6561 645f 6762 715f 7175  elf._read_gbq_qu
-00006120: 6572 7928 0a20 2020 2020 2020 2020 2020  ery(.           
-00006130: 2020 2020 2071 7565 7279 2c0a 2020 2020       query,.    
-00006140: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00006150: 785f 636f 6c3d 696e 6465 785f 636f 6c2c  x_col=index_col,
-00006160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006170: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-00006180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006190: 2020 6d61 785f 7265 7375 6c74 733d 6d61    max_results=ma
-000061a0: 785f 7265 7375 6c74 732c 0a20 2020 2020  x_results,.     
-000061b0: 2020 2020 2020 2020 2020 2061 7069 5f6e             api_n
-000061c0: 616d 653d 2272 6561 645f 6762 715f 7461  ame="read_gbq_ta
-000061d0: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-000061e0: 2020 2020 2020 7573 655f 6361 6368 653d        use_cache=
-000061f0: 7573 655f 6361 6368 652c 0a20 2020 2020  use_cache,.     
-00006200: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00006210: 2020 7265 7475 726e 2073 656c 662e 5f72    return self._r
-00006220: 6561 645f 6762 715f 7461 626c 6528 0a20  ead_gbq_table(. 
-00006230: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00006240: 3d71 7565 7279 2c0a 2020 2020 2020 2020  =query,.        
-00006250: 2020 2020 696e 6465 785f 636f 6c3d 696e      index_col=in
-00006260: 6465 785f 636f 6c2c 0a20 2020 2020 2020  dex_col,.       
-00006270: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
-00006280: 756d 6e73 2c0a 2020 2020 2020 2020 2020  umns,.          
-00006290: 2020 6d61 785f 7265 7375 6c74 733d 6d61    max_results=ma
-000062a0: 785f 7265 7375 6c74 732c 0a20 2020 2020  x_results,.     
-000062b0: 2020 2020 2020 2061 7069 5f6e 616d 653d         api_name=
-000062c0: 2272 6561 645f 6762 715f 7461 626c 6522  "read_gbq_table"
-000062d0: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
-000062e0: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
-000062f0: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-00006300: 2020 6465 6620 5f67 6574 5f73 6e61 7073    def _get_snaps
-00006310: 686f 745f 7371 6c5f 616e 645f 7072 696d  hot_sql_and_prim
-00006320: 6172 795f 6b65 7928 0a20 2020 2020 2020  ary_key(.       
-00006330: 2073 656c 662c 0a20 2020 2020 2020 2074   self,.        t
-00006340: 6162 6c65 5f72 6566 3a20 6269 6771 7565  able_ref: bigque
-00006350: 7279 2e74 6162 6c65 2e54 6162 6c65 5265  ry.table.TableRe
-00006360: 6665 7265 6e63 652c 0a20 2020 2020 2020  ference,.       
-00006370: 202a 2c0a 2020 2020 2020 2020 6170 695f   *,.        api_
-00006380: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-00006390: 2020 2075 7365 5f63 6163 6865 3a20 626f     use_cache: bo
-000063a0: 6f6c 203d 2054 7275 652c 0a20 2020 2029  ol = True,.    )
-000063b0: 202d 3e20 5475 706c 655b 6962 6973 5f74   -> Tuple[ibis_t
-000063c0: 7970 6573 2e54 6162 6c65 2c20 4f70 7469  ypes.Table, Opti
-000063d0: 6f6e 616c 5b53 6571 7565 6e63 655b 7374  onal[Sequence[st
-000063e0: 725d 5d5d 3a0a 2020 2020 2020 2020 2222  r]]]:.        ""
-000063f0: 2243 7265 6174 6520 6120 7265 6164 2d6f  "Create a read-o
-00006400: 6e6c 7920 4962 6973 2074 6162 6c65 2065  nly Ibis table e
-00006410: 7870 7265 7373 696f 6e20 7265 7072 6573  xpression repres
-00006420: 656e 7469 6e67 2061 2074 6162 6c65 2e0a  enting a table..
-00006430: 0a20 2020 2020 2020 2049 6620 7765 2063  .        If we c
-00006440: 616e 2067 6574 2061 2074 6f74 616c 206f  an get a total o
-00006450: 7264 6572 696e 6720 6672 6f6d 2074 6865  rdering from the
-00006460: 2074 6162 6c65 2c20 7375 6368 2061 7320   table, such as 
-00006470: 7669 6120 7072 696d 6172 7920 6b65 790a  via primary key.
-00006480: 2020 2020 2020 2020 636f 6c75 6d6e 2873          column(s
-00006490: 292c 2074 6865 6e20 7265 7475 726e 2074  ), then return t
-000064a0: 686f 7365 2074 6f6f 2073 6f20 7468 6174  hose too so that
-000064b0: 206f 7264 6572 696e 6720 6765 6e65 7261   ordering genera
-000064c0: 7469 6f6e 2063 616e 2062 650a 2020 2020  tion can be.    
-000064d0: 2020 2020 6176 6f69 6465 642e 0a20 2020      avoided..   
-000064e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000064f0: 2023 2049 6620 7468 6572 6520 6172 6520   # If there are 
-00006500: 7072 696d 6172 7920 6b65 7973 2064 6566  primary keys def
-00006510: 696e 6564 2c20 7468 6520 7175 6572 7920  ined, the query 
-00006520: 656e 6769 6e65 2061 7373 756d 6573 2074  engine assumes t
-00006530: 6865 7365 0a20 2020 2020 2020 2023 2063  hese.        # c
-00006540: 6f6c 756d 6e73 2061 7265 2075 6e69 7175  olumns are uniqu
-00006550: 652c 2065 7665 6e20 6966 2074 6865 2063  e, even if the c
-00006560: 6f6e 7374 7261 696e 7420 6973 206e 6f74  onstraint is not
-00006570: 2065 6e66 6f72 6365 642e 2057 6520 6d61   enforced. We ma
-00006580: 6b65 0a20 2020 2020 2020 2023 2074 6865  ke.        # the
-00006590: 2073 616d 6520 6173 7375 6d70 7469 6f6e   same assumption
-000065a0: 2061 6e64 2075 7365 2074 6865 7365 2063   and use these c
-000065b0: 6f6c 756d 6e73 2061 7320 7468 6520 746f  olumns as the to
-000065c0: 7461 6c20 6f72 6465 7269 6e67 206b 6579  tal ordering key
-000065d0: 732e 0a20 2020 2020 2020 2074 6162 6c65  s..        table
-000065e0: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
-000065f0: 2e67 6574 5f74 6162 6c65 2874 6162 6c65  .get_table(table
-00006600: 5f72 6566 290a 0a20 2020 2020 2020 2069  _ref)..        i
-00006610: 6620 7461 626c 652e 6c6f 6361 7469 6f6e  f table.location
-00006620: 2e63 6173 6566 6f6c 6428 2920 213d 2073  .casefold() != s
-00006630: 656c 662e 5f6c 6f63 6174 696f 6e2e 6361  elf._location.ca
-00006640: 7365 666f 6c64 2829 3a0a 2020 2020 2020  sefold():.      
-00006650: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00006660: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00006670: 2020 2020 2020 2020 6622 4375 7272 656e          f"Curren
-00006680: 7420 7365 7373 696f 6e20 6973 2069 6e20  t session is in 
-00006690: 7b73 656c 662e 5f6c 6f63 6174 696f 6e7d  {self._location}
-000066a0: 2062 7574 2064 6174 6173 6574 2027 7b74   but dataset '{t
-000066b0: 6162 6c65 2e70 726f 6a65 6374 7d2e 7b74  able.project}.{t
-000066c0: 6162 6c65 2e64 6174 6173 6574 5f69 647d  able.dataset_id}
-000066d0: 2720 6973 206c 6f63 6174 6564 2069 6e20  ' is located in 
-000066e0: 7b74 6162 6c65 2e6c 6f63 6174 696f 6e7d  {table.location}
-000066f0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00006700: 0a20 2020 2020 2020 2070 7269 6d61 7279  .        primary
-00006710: 5f6b 6579 7320 3d20 4e6f 6e65 0a20 2020  _keys = None.   
-00006720: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00006730: 2020 2020 2020 2874 6162 6c65 5f63 6f6e        (table_con
-00006740: 7374 7261 696e 7473 203a 3d20 6765 7461  straints := geta
-00006750: 7474 7228 7461 626c 652c 2022 7461 626c  ttr(table, "tabl
-00006760: 655f 636f 6e73 7472 6169 6e74 7322 2c20  e_constraints", 
-00006770: 4e6f 6e65 2929 2069 7320 6e6f 7420 4e6f  None)) is not No
-00006780: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
-00006790: 6e64 2028 7072 696d 6172 795f 6b65 7920  nd (primary_key 
-000067a0: 3a3d 2074 6162 6c65 5f63 6f6e 7374 7261  := table_constra
-000067b0: 696e 7473 2e70 7269 6d61 7279 5f6b 6579  ints.primary_key
-000067c0: 2920 6973 206e 6f74 204e 6f6e 650a 2020  ) is not None.  
-000067d0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-000067e0: 2077 696c 6c20 6265 2046 616c 7365 2066   will be False f
-000067f0: 6f72 2065 6974 6865 7220 4e6f 6e65 206f  or either None o
-00006800: 7220 656d 7074 7920 6c69 7374 2e0a 2020  r empty list..  
-00006810: 2020 2020 2020 2020 2020 2320 5765 2077            # We w
-00006820: 616e 7420 7072 696d 6172 795f 6b65 7973  ant primary_keys
-00006830: 203d 204e 6f6e 6520 6966 206e 6f20 7072   = None if no pr
-00006840: 696d 6172 7920 6b65 7973 2061 7265 2073  imary keys are s
-00006850: 6574 2e0a 2020 2020 2020 2020 2020 2020  et..            
-00006860: 616e 6420 2863 6f6c 756d 6e73 203a 3d20  and (columns := 
-00006870: 7072 696d 6172 795f 6b65 792e 636f 6c75  primary_key.colu
-00006880: 6d6e 7329 0a20 2020 2020 2020 2029 3a0a  mns).        ):.
-00006890: 2020 2020 2020 2020 2020 2020 7072 696d              prim
-000068a0: 6172 795f 6b65 7973 203d 2063 6f6c 756d  ary_keys = colum
-000068b0: 6e73 0a0a 2020 2020 2020 2020 6a6f 625f  ns..        job_
-000068c0: 636f 6e66 6967 203d 2062 6967 7175 6572  config = bigquer
-000068d0: 792e 5175 6572 794a 6f62 436f 6e66 6967  y.QueryJobConfig
-000068e0: 2829 0a20 2020 2020 2020 206a 6f62 5f63  ().        job_c
-000068f0: 6f6e 6669 672e 6c61 6265 6c73 5b22 6269  onfig.labels["bi
-00006900: 6766 7261 6d65 732d 6170 6922 5d20 3d20  gframes-api"] = 
-00006910: 6170 695f 6e61 6d65 0a20 2020 2020 2020  api_name.       
-00006920: 2069 6620 7573 655f 6361 6368 6520 616e   if use_cache an
-00006930: 6420 7461 626c 655f 7265 6620 696e 2073  d table_ref in s
-00006940: 656c 662e 5f64 665f 736e 6170 7368 6f74  elf._df_snapshot
-00006950: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
-00006960: 2020 2020 2073 6e61 7073 686f 745f 7469       snapshot_ti
-00006970: 6d65 7374 616d 7020 3d20 7365 6c66 2e5f  mestamp = self._
-00006980: 6466 5f73 6e61 7073 686f 745b 7461 626c  df_snapshot[tabl
-00006990: 655f 7265 665d 0a0a 2020 2020 2020 2020  e_ref]..        
-000069a0: 2020 2020 2320 4361 6368 6520 6869 7420      # Cache hit 
-000069b0: 636f 756c 6420 6265 2075 6e65 7870 6563  could be unexpec
-000069c0: 7465 642e 2053 6565 2069 6e74 6572 6e61  ted. See interna
-000069d0: 6c20 6973 7375 6520 3332 3935 3435 3830  l issue 32954580
-000069e0: 352e 0a20 2020 2020 2020 2020 2020 2023  5..            #
-000069f0: 2052 6169 7365 2061 2077 6172 6e69 6e67   Raise a warning
-00006a00: 2077 6974 6820 6d6f 7265 2069 6e66 6f72   with more infor
-00006a10: 6d61 7469 6f6e 2061 626f 7574 2068 6f77  mation about how
-00006a20: 2074 6f20 6176 6f69 6420 7468 650a 2020   to avoid the.  
-00006a30: 2020 2020 2020 2020 2020 2320 7072 6f62            # prob
-00006a40: 6c65 6d73 2077 6974 6820 7468 6520 6361  lems with the ca
-00006a50: 6368 652e 0a20 2020 2020 2020 2020 2020  che..           
-00006a60: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 6622 5265 6164 696e 6720 6361 6368 6564  f"Reading cached
-00006a90: 2074 6162 6c65 2066 726f 6d20 7b73 6e61   table from {sna
-00006aa0: 7073 686f 745f 7469 6d65 7374 616d 707d  pshot_timestamp}
-00006ab0: 2074 6f20 6176 6f69 6420 220a 2020 2020   to avoid ".    
-00006ac0: 2020 2020 2020 2020 2020 2020 2269 6e63              "inc
-00006ad0: 6f6d 7061 7469 6269 6c69 6573 2077 6974  ompatibilies wit
-00006ae0: 6820 7072 6576 696f 7573 2072 6561 6473  h previous reads
-00006af0: 206f 6620 7468 6973 2074 6162 6c65 2e20   of this table. 
-00006b00: 546f 2072 6561 6420 220a 2020 2020 2020  To read ".      
-00006b10: 2020 2020 2020 2020 2020 2274 6865 206c            "the l
-00006b20: 6174 6573 7420 7665 7273 696f 6e2c 2073  atest version, s
-00006b30: 6574 2060 7573 655f 6361 6368 653d 4661  et `use_cache=Fa
-00006b40: 6c73 6560 206f 7220 636c 6f73 6520 7468  lse` or close th
-00006b50: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
-00006b60: 2020 2020 2263 7572 7265 6e74 2073 6573      "current ses
-00006b70: 7369 6f6e 2077 6974 6820 5365 7373 696f  sion with Sessio
-00006b80: 6e2e 636c 6f73 6528 2920 6f72 2022 0a20  n.close() or ". 
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006ba0: 6269 6766 7261 6d65 732e 7061 6e64 6173  bigframes.pandas
-00006bb0: 2e63 6c6f 7365 5f73 6573 7369 6f6e 2829  .close_session()
-00006bc0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00006bd0: 2020 2020 2320 5468 6572 6520 6172 6520      # There are 
-00006be0: 6d61 6e79 206c 6179 6572 7320 6265 666f  many layers befo
-00006bf0: 7265 2077 6520 6765 7420 746f 2028 706f  re we get to (po
-00006c00: 7373 6962 6c79 2920 7468 6520 7573 6572  ssibly) the user
-00006c10: 2773 2063 6f64 653a 0a20 2020 2020 2020  's code:.       
-00006c20: 2020 2020 2020 2020 2023 2070 616e 6461           # panda
-00006c30: 732e 7265 6164 5f67 6271 5f74 6162 6c65  s.read_gbq_table
-00006c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006c50: 2023 202d 3e20 7769 7468 5f64 6566 6175   # -> with_defau
-00006c60: 6c74 5f73 6573 7369 6f6e 0a20 2020 2020  lt_session.     
-00006c70: 2020 2020 2020 2020 2020 2023 202d 3e20             # -> 
-00006c80: 5365 7373 696f 6e2e 7265 6164 5f67 6271  Session.read_gbq
-00006c90: 5f74 6162 6c65 0a20 2020 2020 2020 2020  _table.         
-00006ca0: 2020 2020 2020 2023 202d 3e20 5f72 6561         # -> _rea
-00006cb0: 645f 6762 715f 7461 626c 650a 2020 2020  d_gbq_table.    
-00006cc0: 2020 2020 2020 2020 2020 2020 2320 2d3e              # ->
-00006cd0: 205f 6765 745f 736e 6170 7368 6f74 5f73   _get_snapshot_s
-00006ce0: 716c 5f61 6e64 5f70 7269 6d61 7279 5f6b  ql_and_primary_k
-00006cf0: 6579 0a20 2020 2020 2020 2020 2020 2020  ey.             
-00006d00: 2020 2073 7461 636b 6c65 7665 6c3d 362c     stacklevel=6,
-00006d10: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00006d20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006d30: 2020 2020 2020 2020 2073 6e61 7073 686f           snapsho
-00006d40: 745f 7469 6d65 7374 616d 7020 3d20 6c69  t_timestamp = li
-00006d50: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-00006d60: 2020 2020 7365 6c66 2e62 7163 6c69 656e      self.bqclien
-00006d70: 742e 7175 6572 7928 0a20 2020 2020 2020  t.query(.       
-00006d80: 2020 2020 2020 2020 2020 2020 2022 5345               "SE
-00006d90: 4c45 4354 2043 5552 5245 4e54 5f54 494d  LECT CURRENT_TIM
-00006da0: 4553 5441 4d50 2829 2041 5320 6063 7572  ESTAMP() AS `cur
-00006db0: 7265 6e74 5f74 696d 6573 7461 6d70 6022  rent_timestamp`"
-00006dc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006dd0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00006de0: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
-00006df0: 2020 2020 2020 2020 2020 2020 2029 2e72               ).r
-00006e00: 6573 756c 7428 290a 2020 2020 2020 2020  esult().        
-00006e10: 2020 2020 295b 305d 5b30 5d0a 2020 2020      )[0][0].    
-00006e20: 2020 2020 2020 2020 7365 6c66 2e5f 6466          self._df
-00006e30: 5f73 6e61 7073 686f 745b 7461 626c 655f  _snapshot[table_
-00006e40: 7265 665d 203d 2073 6e61 7073 686f 745f  ref] = snapshot_
-00006e50: 7469 6d65 7374 616d 700a 0a20 2020 2020  timestamp..     
-00006e60: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00006e70: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
-00006e80: 7369 6f6e 203d 2073 656c 662e 6962 6973  sion = self.ibis
-00006e90: 5f63 6c69 656e 742e 7371 6c28 0a20 2020  _client.sql(.   
-00006ea0: 2020 2020 2020 2020 2020 2020 2062 6967               big
-00006eb0: 6672 616d 6573 5f69 6f2e 6372 6561 7465  frames_io.create
-00006ec0: 5f73 6e61 7073 686f 745f 7371 6c28 7461  _snapshot_sql(ta
-00006ed0: 626c 655f 7265 662c 2073 6e61 7073 686f  ble_ref, snapsho
-00006ee0: 745f 7469 6d65 7374 616d 7029 0a20 2020  t_timestamp).   
-00006ef0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00006f00: 2020 2065 7863 6570 7420 676f 6f67 6c65     except google
-00006f10: 2e61 7069 5f63 6f72 652e 6578 6365 7074  .api_core.except
-00006f20: 696f 6e73 2e46 6f72 6269 6464 656e 2061  ions.Forbidden a
-00006f30: 7320 6578 3a0a 2020 2020 2020 2020 2020  s ex:.          
-00006f40: 2020 6966 2022 4472 6976 6520 6372 6564    if "Drive cred
-00006f50: 656e 7469 616c 7322 2069 6e20 6578 2e6d  entials" in ex.m
-00006f60: 6573 7361 6765 3a0a 2020 2020 2020 2020  essage:.        
-00006f70: 2020 2020 2020 2020 6578 2e6d 6573 7361          ex.messa
-00006f80: 6765 202b 3d20 225c 6e43 6865 636b 2068  ge += "\nCheck h
-00006f90: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
-00006fa0: 676c 652e 636f 6d2f 6269 6771 7565 7279  gle.com/bigquery
-00006fb0: 2f64 6f63 732f 7175 6572 792d 6472 6976  /docs/query-driv
-00006fc0: 652d 6461 7461 2347 6f6f 676c 655f 4472  e-data#Google_Dr
-00006fd0: 6976 655f 7065 726d 6973 7369 6f6e 732e  ive_permissions.
-00006fe0: 220a 2020 2020 2020 2020 2020 2020 7261  ".            ra
-00006ff0: 6973 650a 0a20 2020 2020 2020 2072 6574  ise..        ret
-00007000: 7572 6e20 7461 626c 655f 6578 7072 6573  urn table_expres
-00007010: 7369 6f6e 2c20 7072 696d 6172 795f 6b65  sion, primary_ke
-00007020: 7973 0a0a 2020 2020 6465 6620 5f72 6561  ys..    def _rea
-00007030: 645f 6762 715f 7461 626c 6528 0a20 2020  d_gbq_table(.   
-00007040: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00007050: 2020 2071 7565 7279 3a20 7374 722c 0a20     query: str,. 
-00007060: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00007070: 2020 696e 6465 785f 636f 6c3a 2049 7465    index_col: Ite
-00007080: 7261 626c 655b 7374 725d 207c 2073 7472  rable[str] | str
-00007090: 203d 2028 292c 0a20 2020 2020 2020 2063   = (),.        c
-000070a0: 6f6c 756d 6e73 3a20 4974 6572 6162 6c65  olumns: Iterable
-000070b0: 5b73 7472 5d20 3d20 2829 2c0a 2020 2020  [str] = (),.    
-000070c0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
-000070d0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-000070e0: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
-000070f0: 7069 5f6e 616d 653a 2073 7472 2c0a 2020  pi_name: str,.  
-00007100: 2020 2020 2020 7573 655f 6361 6368 653a        use_cache:
-00007110: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-00007120: 2020 2920 2d3e 2064 6174 6166 7261 6d65    ) -> dataframe
-00007130: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
-00007140: 2020 2020 696d 706f 7274 2062 6967 6672      import bigfr
-00007150: 616d 6573 2e64 6174 6166 7261 6d65 2061  ames.dataframe a
-00007160: 7320 6461 7461 6672 616d 650a 0a20 2020  s dataframe..   
-00007170: 2020 2020 2069 6620 6d61 785f 7265 7375       if max_resu
-00007180: 6c74 7320 616e 6420 6d61 785f 7265 7375  lts and max_resu
-00007190: 6c74 7320 3c3d 2030 3a0a 2020 2020 2020  lts <= 0:.      
-000071a0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000071b0: 6545 7272 6f72 2822 606d 6178 5f72 6573  eError("`max_res
-000071c0: 756c 7473 6020 7368 6f75 6c64 2062 6520  ults` should be 
-000071d0: 6120 706f 7369 7469 7665 206e 756d 6265  a positive numbe
-000071e0: 722e 2229 0a0a 2020 2020 2020 2020 7461  r.")..        ta
-000071f0: 626c 655f 7265 6620 3d20 6269 6771 7565  ble_ref = bigque
-00007200: 7279 2e74 6162 6c65 2e54 6162 6c65 5265  ry.table.TableRe
-00007210: 6665 7265 6e63 652e 6672 6f6d 5f73 7472  ference.from_str
-00007220: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-00007230: 2071 7565 7279 2c20 6465 6661 756c 745f   query, default_
-00007240: 7072 6f6a 6563 743d 7365 6c66 2e62 7163  project=self.bqc
-00007250: 6c69 656e 742e 7072 6f6a 6563 740a 2020  lient.project.  
-00007260: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00007270: 2028 7461 626c 655f 6578 7072 6573 7369   (table_expressi
-00007280: 6f6e 2c20 7072 696d 6172 795f 6b65 7973  on, primary_keys
-00007290: 2c29 203d 2073 656c 662e 5f67 6574 5f73  ,) = self._get_s
-000072a0: 6e61 7073 686f 745f 7371 6c5f 616e 645f  napshot_sql_and_
-000072b0: 7072 696d 6172 795f 6b65 7928 0a20 2020  primary_key(.   
-000072c0: 2020 2020 2020 2020 2074 6162 6c65 5f72           table_r
-000072d0: 6566 2c20 6170 695f 6e61 6d65 3d61 7069  ef, api_name=api
-000072e0: 5f6e 616d 652c 2075 7365 5f63 6163 6865  _name, use_cache
-000072f0: 3d75 7365 5f63 6163 6865 0a20 2020 2020  =use_cache.     
-00007300: 2020 2029 0a20 2020 2020 2020 2074 6f74     ).        tot
-00007310: 616c 5f6f 7264 6572 696e 675f 636f 6c73  al_ordering_cols
-00007320: 203d 2070 7269 6d61 7279 5f6b 6579 730a   = primary_keys.
-00007330: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00007340: 696e 6465 785f 636f 6c20 616e 6420 7072  index_col and pr
-00007350: 696d 6172 795f 6b65 7973 2069 7320 6e6f  imary_keys is no
-00007360: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00007370: 2020 2020 696e 6465 785f 636f 6c20 3d20      index_col = 
-00007380: 7072 696d 6172 795f 6b65 7973 0a0a 2020  primary_keys..  
-00007390: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-000073a0: 2063 6f6c 756d 6e73 3a0a 2020 2020 2020   columns:.      
-000073b0: 2020 2020 2020 6966 206b 6579 206e 6f74        if key not
-000073c0: 2069 6e20 7461 626c 655f 6578 7072 6573   in table_expres
-000073d0: 7369 6f6e 2e63 6f6c 756d 6e73 3a0a 2020  sion.columns:.  
-000073e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000073f0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007410: 2020 2020 6622 436f 6c75 6d6e 2027 7b6b      f"Column '{k
-00007420: 6579 7d27 206f 6620 6063 6f6c 756d 6e73  ey}' of `columns
-00007430: 6020 6e6f 7420 666f 756e 6420 696e 2074  ` not found in t
-00007440: 6869 7320 7461 626c 652e 220a 2020 2020  his table.".    
-00007450: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00007460: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00007470: 616e 6365 2869 6e64 6578 5f63 6f6c 2c20  ance(index_col, 
-00007480: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00007490: 2020 696e 6465 785f 636f 6c73 3a20 4c69    index_cols: Li
-000074a0: 7374 5b73 7472 5d20 3d20 5b69 6e64 6578  st[str] = [index
-000074b0: 5f63 6f6c 5d0a 2020 2020 2020 2020 656c  _col].        el
-000074c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000074d0: 696e 6465 785f 636f 6c73 203d 206c 6973  index_cols = lis
-000074e0: 7428 696e 6465 785f 636f 6c29 0a0a 2020  t(index_col)..  
-000074f0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-00007500: 2069 6e64 6578 5f63 6f6c 733a 0a20 2020   index_cols:.   
-00007510: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
-00007520: 6e6f 7420 696e 2074 6162 6c65 5f65 7870  not in table_exp
-00007530: 7265 7373 696f 6e2e 636f 6c75 6d6e 733a  ression.columns:
-00007540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007550: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00007560: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00007570: 2020 2020 2020 2066 2243 6f6c 756d 6e20         f"Column 
-00007580: 607b 6b65 797d 6020 6f66 2060 696e 6465  `{key}` of `inde
-00007590: 785f 636f 6c60 206e 6f74 2066 6f75 6e64  x_col` not found
-000075a0: 2069 6e20 7468 6973 2074 6162 6c65 2e22   in this table."
-000075b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000075c0: 2029 0a0a 2020 2020 2020 2020 6966 2063   )..        if c
-000075d0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
-000075e0: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
-000075f0: 7369 6f6e 203d 2074 6162 6c65 5f65 7870  sion = table_exp
-00007600: 7265 7373 696f 6e2e 7365 6c65 6374 285b  ression.select([
-00007610: 2a69 6e64 6578 5f63 6f6c 732c 202a 636f  *index_cols, *co
-00007620: 6c75 6d6e 735d 290a 0a20 2020 2020 2020  lumns])..       
-00007630: 2023 2049 6620 7468 6520 696e 6465 7820   # If the index 
-00007640: 6973 2075 6e69 7175 6520 616e 6420 736f  is unique and so
-00007650: 7274 6162 6c65 2c20 7468 656e 2077 6520  rtable, then we 
-00007660: 646f 6e27 7420 6e65 6564 2074 6f20 6765  don't need to ge
-00007670: 6e65 7261 7465 0a20 2020 2020 2020 2023  nerate.        #
-00007680: 2061 6e20 6f72 6465 7269 6e67 2063 6f6c   an ordering col
-00007690: 756d 6e2e 0a20 2020 2020 2020 206f 7264  umn..        ord
-000076a0: 6572 696e 6720 3d20 4e6f 6e65 0a20 2020  ering = None.   
-000076b0: 2020 2020 2069 6620 746f 7461 6c5f 6f72       if total_or
-000076c0: 6465 7269 6e67 5f63 6f6c 7320 6973 206e  dering_cols is n
-000076d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000076e0: 2020 2020 2023 204e 6f74 653a 2063 7572       # Note: cur
-000076f0: 7265 6e74 6c79 2c20 6120 7461 626c 6520  rently, a table 
-00007700: 6861 7320 6120 746f 7461 6c20 6f72 6465  has a total orde
-00007710: 7269 6e67 206f 6e6c 7920 7768 656e 2074  ring only when t
-00007720: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
-00007730: 2070 7269 6d61 7279 206b 6579 2873 2920   primary key(s) 
-00007740: 6172 6520 7365 7420 6f6e 2061 2074 6162  are set on a tab
-00007750: 6c65 2e20 5468 6520 7175 6572 7920 656e  le. The query en
-00007760: 6769 6e65 2061 7373 756d 6573 2073 7563  gine assumes suc
-00007770: 680a 2020 2020 2020 2020 2020 2020 2320  h.            # 
-00007780: 636f 6c75 6d6e 7320 6172 6520 756e 6971  columns are uniq
-00007790: 7565 2c20 6576 656e 2069 6620 6e6f 7420  ue, even if not 
-000077a0: 656e 666f 7263 6564 2e0a 2020 2020 2020  enforced..      
-000077b0: 2020 2020 2020 6f72 6465 7269 6e67 203d        ordering =
-000077c0: 206f 7264 6572 2e45 7870 7265 7373 696f   order.Expressio
-000077d0: 6e4f 7264 6572 696e 6728 0a20 2020 2020  nOrdering(.     
-000077e0: 2020 2020 2020 2020 2020 206f 7264 6572             order
-000077f0: 696e 675f 7661 6c75 655f 636f 6c75 6d6e  ing_value_column
-00007800: 733d 7475 706c 6528 0a20 2020 2020 2020  s=tuple(.       
-00007810: 2020 2020 2020 2020 2020 2020 206f 7264               ord
-00007820: 6572 2e61 7363 656e 6469 6e67 5f6f 7665  er.ascending_ove
-00007830: 7228 636f 6c75 6d6e 5f69 6429 2066 6f72  r(column_id) for
-00007840: 2063 6f6c 756d 6e5f 6964 2069 6e20 746f   column_id in to
-00007850: 7461 6c5f 6f72 6465 7269 6e67 5f63 6f6c  tal_ordering_col
-00007860: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00007870: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00007880: 2020 2020 2074 6f74 616c 5f6f 7264 6572       total_order
-00007890: 696e 675f 636f 6c75 6d6e 733d 6672 6f7a  ing_columns=froz
-000078a0: 656e 7365 7428 746f 7461 6c5f 6f72 6465  enset(total_orde
-000078b0: 7269 6e67 5f63 6f6c 7329 2c0a 2020 2020  ring_cols),.    
-000078c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000078d0: 2020 2020 2020 636f 6c75 6d6e 5f76 616c        column_val
-000078e0: 7565 7320 3d20 5b74 6162 6c65 5f65 7870  ues = [table_exp
-000078f0: 7265 7373 696f 6e5b 636f 6c5d 2066 6f72  ression[col] for
-00007900: 2063 6f6c 2069 6e20 7461 626c 655f 6578   col in table_ex
-00007910: 7072 6573 7369 6f6e 2e63 6f6c 756d 6e73  pression.columns
-00007920: 5d0a 2020 2020 2020 2020 2020 2020 6172  ].            ar
-00007930: 7261 795f 7661 6c75 6520 3d20 636f 7265  ray_value = core
-00007940: 2e41 7272 6179 5661 6c75 652e 6672 6f6d  .ArrayValue.from
-00007950: 5f69 6269 7328 0a20 2020 2020 2020 2020  _ibis(.         
-00007960: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00007970: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-00007980: 6c65 5f65 7870 7265 7373 696f 6e2c 0a20  le_expression,. 
-00007990: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000079a0: 6f6c 756d 6e73 3d63 6f6c 756d 6e5f 7661  olumns=column_va
-000079b0: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
-000079c0: 2020 2020 2020 6869 6464 656e 5f6f 7264        hidden_ord
-000079d0: 6572 696e 675f 636f 6c75 6d6e 733d 5b5d  ering_columns=[]
-000079e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000079f0: 2020 6f72 6465 7269 6e67 3d6f 7264 6572    ordering=order
-00007a00: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-00007a10: 2029 0a0a 2020 2020 2020 2020 656c 6966   )..        elif
-00007a20: 206c 656e 2869 6e64 6578 5f63 6f6c 7329   len(index_cols)
-00007a30: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
-00007a40: 2020 2023 2057 6520 6861 7665 2069 6e64     # We have ind
-00007a50: 6578 2063 6f6c 756d 6e73 2c20 6c65 7473  ex columns, lets
-00007a60: 2073 6565 2069 6620 7468 6f73 6520 6172   see if those ar
-00007a70: 6520 6163 7475 616c 6c79 2074 6f74 616c  e actually total
-00007a80: 5f6f 7264 6572 5f63 6f6c 756d 6e73 0a20  _order_columns. 
-00007a90: 2020 2020 2020 2020 2020 206f 7264 6572             order
-00007aa0: 696e 6720 3d20 6f72 6465 722e 4578 7072  ing = order.Expr
-00007ab0: 6573 7369 6f6e 4f72 6465 7269 6e67 280a  essionOrdering(.
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 6f72 6465 7269 6e67 5f76 616c 7565 5f63  ordering_value_c
-00007ae0: 6f6c 756d 6e73 3d74 7570 6c65 280a 2020  olumns=tuple(.  
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 5b6f 7264 6572 2e61 7363 656e 6469    [order.ascendi
-00007b10: 6e67 5f6f 7665 7228 636f 6c75 6d6e 5f69  ng_over(column_i
-00007b20: 6429 2066 6f72 2063 6f6c 756d 6e5f 6964  d) for column_id
-00007b30: 2069 6e20 696e 6465 785f 636f 6c73 5d0a   in index_cols].
-00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00007b60: 2020 2074 6f74 616c 5f6f 7264 6572 696e     total_orderin
-00007b70: 675f 636f 6c75 6d6e 733d 6672 6f7a 656e  g_columns=frozen
-00007b80: 7365 7428 696e 6465 785f 636f 6c73 292c  set(index_cols),
-00007b90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00007ba0: 2020 2020 2020 2020 2020 2069 735f 746f             is_to
-00007bb0: 7461 6c5f 6f72 6465 7269 6e67 203d 2073  tal_ordering = s
-00007bc0: 656c 662e 5f63 6865 636b 5f69 6e64 6578  elf._check_index
-00007bd0: 5f75 6e69 7175 656e 6573 7328 0a20 2020  _uniqueness(.   
-00007be0: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-00007bf0: 6c65 5f65 7870 7265 7373 696f 6e2c 2069  le_expression, i
-00007c00: 6e64 6578 5f63 6f6c 730a 2020 2020 2020  ndex_cols.      
-00007c10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00007c20: 2020 2020 6966 2069 735f 746f 7461 6c5f      if is_total_
-00007c30: 6f72 6465 7269 6e67 3a0a 2020 2020 2020  ordering:.      
-00007c40: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00007c50: 5f76 616c 7565 7320 3d20 5b0a 2020 2020  _values = [.    
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00007c80: 5b63 6f6c 5d20 666f 7220 636f 6c20 696e  [col] for col in
-00007c90: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
-00007ca0: 6e2e 636f 6c75 6d6e 730a 2020 2020 2020  n.columns.      
-00007cb0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00007cc0: 2020 2020 2020 2020 2020 2020 6172 7261              arra
-00007cd0: 795f 7661 6c75 6520 3d20 636f 7265 2e41  y_value = core.A
-00007ce0: 7272 6179 5661 6c75 652e 6672 6f6d 5f69  rrayValue.from_i
-00007cf0: 6269 7328 0a20 2020 2020 2020 2020 2020  bis(.           
-00007d00: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
-00007d30: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00007d40: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-00007d50: 3d63 6f6c 756d 6e5f 7661 6c75 6573 2c0a  =column_values,.
-00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d70: 2020 2020 6869 6464 656e 5f6f 7264 6572      hidden_order
-00007d80: 696e 675f 636f 6c75 6d6e 733d 5b5d 2c0a  ing_columns=[],.
-00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007da0: 2020 2020 6f72 6465 7269 6e67 3d6f 7264      ordering=ord
-00007db0: 6572 696e 672c 0a20 2020 2020 2020 2020  ering,.         
-00007dc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00007dd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00007de0: 2020 2020 2020 2020 2020 2061 7272 6179             array
-00007df0: 5f76 616c 7565 203d 2073 656c 662e 5f63  _value = self._c
-00007e00: 7265 6174 655f 746f 7461 6c5f 6f72 6465  reate_total_orde
-00007e10: 7269 6e67 2874 6162 6c65 5f65 7870 7265  ring(table_expre
-00007e20: 7373 696f 6e29 0a20 2020 2020 2020 2065  ssion).        e
-00007e30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00007e40: 2061 7272 6179 5f76 616c 7565 203d 2073   array_value = s
-00007e50: 656c 662e 5f63 7265 6174 655f 746f 7461  elf._create_tota
-00007e60: 6c5f 6f72 6465 7269 6e67 2874 6162 6c65  l_ordering(table
-00007e70: 5f65 7870 7265 7373 696f 6e29 0a0a 2020  _expression)..  
-00007e80: 2020 2020 2020 7661 6c75 655f 636f 6c75        value_colu
-00007e90: 6d6e 7320 3d20 5b63 6f6c 2066 6f72 2063  mns = [col for c
-00007ea0: 6f6c 2069 6e20 6172 7261 795f 7661 6c75  ol in array_valu
-00007eb0: 652e 636f 6c75 6d6e 5f69 6473 2069 6620  e.column_ids if 
-00007ec0: 636f 6c20 6e6f 7420 696e 2069 6e64 6578  col not in index
-00007ed0: 5f63 6f6c 735d 0a20 2020 2020 2020 2062  _cols].        b
-00007ee0: 6c6f 636b 203d 2062 6c6f 636b 732e 426c  lock = blocks.Bl
-00007ef0: 6f63 6b28 0a20 2020 2020 2020 2020 2020  ock(.           
-00007f00: 2061 7272 6179 5f76 616c 7565 2c0a 2020   array_value,.  
-00007f10: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-00007f20: 636f 6c75 6d6e 733d 696e 6465 785f 636f  columns=index_co
-00007f30: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00007f40: 636f 6c75 6d6e 5f6c 6162 656c 733d 7661  column_labels=va
-00007f50: 6c75 655f 636f 6c75 6d6e 732c 0a20 2020  lue_columns,.   
-00007f60: 2020 2020 2020 2020 2069 6e64 6578 5f6c           index_l
-00007f70: 6162 656c 733d 696e 6465 785f 636f 6c73  abels=index_cols
-00007f80: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00007f90: 2020 2020 6966 206d 6178 5f72 6573 756c      if max_resul
-00007fa0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00007fb0: 626c 6f63 6b20 3d20 626c 6f63 6b2e 736c  block = block.sl
-00007fc0: 6963 6528 7374 6f70 3d6d 6178 5f72 6573  ice(stop=max_res
-00007fd0: 756c 7473 290a 2020 2020 2020 2020 6466  ults).        df
-00007fe0: 203d 2064 6174 6166 7261 6d65 2e44 6174   = dataframe.Dat
-00007ff0: 6146 7261 6d65 2862 6c6f 636b 290a 0a20  aFrame(block).. 
-00008000: 2020 2020 2020 2023 2049 6620 7573 6572         # If user
-00008010: 2070 726f 7669 6465 6420 696e 6465 7820   provided index 
-00008020: 636f 6c75 6d6e 732c 2073 686f 756c 6420  columns, should 
-00008030: 736f 7274 206f 7665 7220 6974 0a20 2020  sort over it.   
-00008040: 2020 2020 2069 6620 6c65 6e28 696e 6465       if len(inde
-00008050: 785f 636f 6c73 2920 3e20 303a 0a20 2020  x_cols) > 0:.   
-00008060: 2020 2020 2020 2020 2064 662e 736f 7274           df.sort
-00008070: 5f69 6e64 6578 2829 0a20 2020 2020 2020  _index().       
-00008080: 2072 6574 7572 6e20 6466 0a0a 2020 2020   return df..    
-00008090: 6465 6620 5f63 6865 636b 5f69 6e64 6578  def _check_index
-000080a0: 5f75 6e69 7175 656e 6573 7328 0a20 2020  _uniqueness(.   
-000080b0: 2020 2020 2073 656c 662c 2074 6162 6c65       self, table
-000080c0: 3a20 6962 6973 5f74 7970 6573 2e54 6162  : ibis_types.Tab
-000080d0: 6c65 2c20 696e 6465 785f 636f 6c73 3a20  le, index_cols: 
-000080e0: 4c69 7374 5b73 7472 5d0a 2020 2020 2920  List[str].    ) 
-000080f0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00008100: 2064 6973 7469 6e63 745f 7461 626c 6520   distinct_table 
-00008110: 3d20 7461 626c 652e 7365 6c65 6374 282a  = table.select(*
-00008120: 696e 6465 785f 636f 6c73 292e 6469 7374  index_cols).dist
-00008130: 696e 6374 2829 0a20 2020 2020 2020 2069  inct().        i
-00008140: 735f 756e 6971 7565 5f73 716c 203d 2066  s_unique_sql = f
-00008150: 2222 2257 4954 4820 6675 6c6c 5f74 6162  """WITH full_tab
-00008160: 6c65 2041 5320 280a 2020 2020 2020 2020  le AS (.        
-00008170: 2020 2020 7b73 656c 662e 6962 6973 5f63      {self.ibis_c
-00008180: 6c69 656e 742e 636f 6d70 696c 6528 7461  lient.compile(ta
-00008190: 626c 6529 7d0a 2020 2020 2020 2020 292c  ble)}.        ),
-000081a0: 0a20 2020 2020 2020 2064 6973 7469 6e63  .        distinc
-000081b0: 745f 7461 626c 6520 4153 2028 0a20 2020  t_table AS (.   
-000081c0: 2020 2020 2020 2020 207b 7365 6c66 2e69           {self.i
-000081d0: 6269 735f 636c 6965 6e74 2e63 6f6d 7069  bis_client.compi
-000081e0: 6c65 2864 6973 7469 6e63 745f 7461 626c  le(distinct_tabl
-000081f0: 6529 7d0a 2020 2020 2020 2020 290a 0a20  e)}.        ).. 
-00008200: 2020 2020 2020 2053 454c 4543 5420 2853         SELECT (S
-00008210: 454c 4543 5420 434f 554e 5428 2a29 2046  ELECT COUNT(*) F
-00008220: 524f 4d20 6675 6c6c 5f74 6162 6c65 2920  ROM full_table) 
-00008230: 4153 2060 746f 7461 6c5f 636f 756e 7460  AS `total_count`
-00008240: 2c0a 2020 2020 2020 2020 2853 454c 4543  ,.        (SELEC
-00008250: 5420 434f 554e 5428 2a29 2046 524f 4d20  T COUNT(*) FROM 
-00008260: 6469 7374 696e 6374 5f74 6162 6c65 2920  distinct_table) 
-00008270: 4153 2060 6469 7374 696e 6374 5f63 6f75  AS `distinct_cou
-00008280: 6e74 600a 2020 2020 2020 2020 2222 220a  nt`.        """.
-00008290: 2020 2020 2020 2020 7265 7375 6c74 732c          results,
-000082a0: 205f 203d 2073 656c 662e 5f73 7461 7274   _ = self._start
-000082b0: 5f71 7565 7279 2869 735f 756e 6971 7565  _query(is_unique
-000082c0: 5f73 716c 290a 2020 2020 2020 2020 726f  _sql).        ro
-000082d0: 7720 3d20 6e65 7874 2869 7465 7228 7265  w = next(iter(re
-000082e0: 7375 6c74 7329 290a 0a20 2020 2020 2020  sults))..       
-000082f0: 2074 6f74 616c 5f63 6f75 6e74 203d 2072   total_count = r
-00008300: 6f77 5b22 746f 7461 6c5f 636f 756e 7422  ow["total_count"
-00008310: 5d0a 2020 2020 2020 2020 6469 7374 696e  ].        distin
-00008320: 6374 5f63 6f75 6e74 203d 2072 6f77 5b22  ct_count = row["
-00008330: 6469 7374 696e 6374 5f63 6f75 6e74 225d  distinct_count"]
-00008340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008350: 746f 7461 6c5f 636f 756e 7420 3d3d 2064  total_count == d
-00008360: 6973 7469 6e63 745f 636f 756e 740a 0a20  istinct_count.. 
-00008370: 2020 2064 6566 205f 7265 6164 5f62 6967     def _read_big
-00008380: 7175 6572 795f 6c6f 6164 5f6a 6f62 280a  query_load_job(.
-00008390: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000083a0: 2020 2020 2020 6669 6c65 7061 7468 5f6f        filepath_o
-000083b0: 725f 6275 6666 6572 3a20 7374 7220 7c20  r_buffer: str | 
-000083c0: 494f 5b22 6279 7465 7322 5d2c 0a20 2020  IO["bytes"],.   
-000083d0: 2020 2020 2074 6162 6c65 3a20 556e 696f       table: Unio
-000083e0: 6e5b 6269 6771 7565 7279 2e54 6162 6c65  n[bigquery.Table
-000083f0: 2c20 6269 6771 7565 7279 2e54 6162 6c65  , bigquery.Table
-00008400: 5265 6665 7265 6e63 655d 2c0a 2020 2020  Reference],.    
-00008410: 2020 2020 2a2c 0a20 2020 2020 2020 206a      *,.        j
-00008420: 6f62 5f63 6f6e 6669 673a 2062 6967 7175  ob_config: bigqu
-00008430: 6572 792e 4c6f 6164 4a6f 6243 6f6e 6669  ery.LoadJobConfi
-00008440: 672c 0a20 2020 2020 2020 2069 6e64 6578  g,.        index
-00008450: 5f63 6f6c 3a20 4974 6572 6162 6c65 5b73  _col: Iterable[s
-00008460: 7472 5d20 7c20 7374 7220 3d20 2829 2c0a  tr] | str = (),.
-00008470: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
-00008480: 2049 7465 7261 626c 655b 7374 725d 203d   Iterable[str] =
-00008490: 2028 292c 0a20 2020 2029 202d 3e20 6461   (),.    ) -> da
-000084a0: 7461 6672 616d 652e 4461 7461 4672 616d  taframe.DataFram
-000084b0: 653a 0a20 2020 2020 2020 2069 6620 6973  e:.        if is
-000084c0: 696e 7374 616e 6365 2869 6e64 6578 5f63  instance(index_c
-000084d0: 6f6c 2c20 7374 7229 3a0a 2020 2020 2020  ol, str):.      
-000084e0: 2020 2020 2020 696e 6465 785f 636f 6c73        index_cols
-000084f0: 203d 205b 696e 6465 785f 636f 6c5d 0a20   = [index_col]. 
-00008500: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008510: 2020 2020 2020 2020 2069 6e64 6578 5f63           index_c
-00008520: 6f6c 7320 3d20 6c69 7374 2869 6e64 6578  ols = list(index
-00008530: 5f63 6f6c 290a 0a20 2020 2020 2020 2069  _col)..        i
-00008540: 6620 6e6f 7420 6a6f 625f 636f 6e66 6967  f not job_config
-00008550: 2e63 6c75 7374 6572 696e 675f 6669 656c  .clustering_fiel
-00008560: 6473 2061 6e64 2069 6e64 6578 5f63 6f6c  ds and index_col
-00008570: 733a 0a20 2020 2020 2020 2020 2020 206a  s:.            j
-00008580: 6f62 5f63 6f6e 6669 672e 636c 7573 7465  ob_config.cluste
-00008590: 7269 6e67 5f66 6965 6c64 7320 3d20 696e  ring_fields = in
-000085a0: 6465 785f 636f 6c73 5b3a 5f4d 4158 5f43  dex_cols[:_MAX_C
-000085b0: 4c55 5354 4552 5f43 4f4c 554d 4e53 5d0a  LUSTER_COLUMNS].
-000085c0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-000085d0: 7374 616e 6365 2866 696c 6570 6174 685f  stance(filepath_
-000085e0: 6f72 5f62 7566 6665 722c 2073 7472 293a  or_buffer, str):
-000085f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00008600: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
-00008610: 6572 2e73 7461 7274 7377 6974 6828 2267  er.startswith("g
-00008620: 733a 2f2f 2229 3a0a 2020 2020 2020 2020  s://"):.        
-00008630: 2020 2020 2020 2020 6c6f 6164 5f6a 6f62          load_job
-00008640: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
-00008650: 2e6c 6f61 645f 7461 626c 655f 6672 6f6d  .load_table_from
-00008660: 5f75 7269 280a 2020 2020 2020 2020 2020  _uri(.          
-00008670: 2020 2020 2020 2020 2020 6669 6c65 7061            filepa
-00008680: 7468 5f6f 725f 6275 6666 6572 2c20 7461  th_or_buffer, ta
-00008690: 626c 652c 206a 6f62 5f63 6f6e 6669 673d  ble, job_config=
-000086a0: 6a6f 625f 636f 6e66 6967 0a20 2020 2020  job_config.     
-000086b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000086c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000086d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000086e0: 6974 6820 6f70 656e 2866 696c 6570 6174  ith open(filepat
-000086f0: 685f 6f72 5f62 7566 6665 722c 2022 7262  h_or_buffer, "rb
-00008700: 2229 2061 7320 736f 7572 6365 5f66 696c  ") as source_fil
-00008710: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00008720: 2020 2020 2020 206c 6f61 645f 6a6f 6220         load_job 
-00008730: 3d20 7365 6c66 2e62 7163 6c69 656e 742e  = self.bqclient.
-00008740: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
-00008750: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
-00008760: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00008770: 7572 6365 5f66 696c 652c 2074 6162 6c65  urce_file, table
-00008780: 2c20 6a6f 625f 636f 6e66 6967 3d6a 6f62  , job_config=job
-00008790: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
-000087a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000087b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000087c0: 2020 2020 2020 2020 6c6f 6164 5f6a 6f62          load_job
-000087d0: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
-000087e0: 2e6c 6f61 645f 7461 626c 655f 6672 6f6d  .load_table_from
-000087f0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
-00008800: 2020 2020 2020 2066 696c 6570 6174 685f         filepath_
-00008810: 6f72 5f62 7566 6665 722c 2074 6162 6c65  or_buffer, table
-00008820: 2c20 6a6f 625f 636f 6e66 6967 3d6a 6f62  , job_config=job
-00008830: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
-00008840: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
-00008850: 656c 662e 5f73 7461 7274 5f67 656e 6572  elf._start_gener
-00008860: 6963 5f6a 6f62 286c 6f61 645f 6a6f 6229  ic_job(load_job)
-00008870: 0a20 2020 2020 2020 2074 6162 6c65 5f69  .        table_i
-00008880: 6420 3d20 6622 7b74 6162 6c65 2e70 726f  d = f"{table.pro
-00008890: 6a65 6374 7d2e 7b74 6162 6c65 2e64 6174  ject}.{table.dat
-000088a0: 6173 6574 5f69 647d 2e7b 7461 626c 652e  aset_id}.{table.
-000088b0: 7461 626c 655f 6964 7d22 0a0a 2020 2020  table_id}"..    
-000088c0: 2020 2020 2320 5570 6461 7465 2074 6865      # Update the
-000088d0: 2074 6162 6c65 2065 7870 6972 6174 696f   table expiratio
-000088e0: 6e20 736f 2077 6520 6172 656e 2774 206c  n so we aren't l
-000088f0: 696d 6974 6564 2074 6f20 7468 6520 6465  imited to the de
-00008900: 6661 756c 7420 3234 0a20 2020 2020 2020  fault 24.       
-00008910: 2023 2068 6f75 7273 206f 6620 7468 6520   # hours of the 
-00008920: 616e 6f6e 796d 6f75 7320 6461 7461 7365  anonymous datase
-00008930: 742e 0a20 2020 2020 2020 2074 6162 6c65  t..        table
-00008940: 5f65 7870 6972 6174 696f 6e20 3d20 6269  _expiration = bi
-00008950: 6771 7565 7279 2e54 6162 6c65 2874 6162  gquery.Table(tab
-00008960: 6c65 5f69 6429 0a20 2020 2020 2020 2074  le_id).        t
-00008970: 6162 6c65 5f65 7870 6972 6174 696f 6e2e  able_expiration.
-00008980: 6578 7069 7265 7320 3d20 280a 2020 2020  expires = (.    
-00008990: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
-000089a0: 2e64 6174 6574 696d 652e 6e6f 7728 6461  .datetime.now(da
-000089b0: 7465 7469 6d65 2e74 696d 657a 6f6e 652e  tetime.timezone.
-000089c0: 7574 6329 202b 2063 6f6e 7374 616e 7473  utc) + constants
-000089d0: 2e44 4546 4155 4c54 5f45 5850 4952 4154  .DEFAULT_EXPIRAT
-000089e0: 494f 4e0a 2020 2020 2020 2020 290a 2020  ION.        ).  
-000089f0: 2020 2020 2020 7365 6c66 2e62 7163 6c69        self.bqcli
-00008a00: 656e 742e 7570 6461 7465 5f74 6162 6c65  ent.update_table
-00008a10: 2874 6162 6c65 5f65 7870 6972 6174 696f  (table_expiratio
-00008a20: 6e2c 205b 2265 7870 6972 6573 225d 290a  n, ["expires"]).
-00008a30: 0a20 2020 2020 2020 2023 2054 6865 2042  .        # The B
-00008a40: 6967 5175 6572 7920 5245 5354 2041 5049  igQuery REST API
-00008a50: 2066 6f72 2074 6162 6c65 732e 6765 7420   for tables.get 
-00008a60: 646f 6573 6e27 7420 7461 6b65 2061 2073  doesn't take a s
-00008a70: 6573 7369 6f6e 2049 442c 2073 6f20 7765  ession ID, so we
-00008a80: 0a20 2020 2020 2020 2023 2063 616e 2774  .        # can't
-00008a90: 2067 6574 2074 6865 2073 6368 656d 6120   get the schema 
-00008aa0: 666f 7220 6120 7465 6d70 2074 6162 6c65  for a temp table
-00008ab0: 2074 6861 7420 7761 792e 0a20 2020 2020   that way..     
-00008ac0: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
-00008ad0: 6561 645f 6762 715f 7461 626c 6528 0a20  ead_gbq_table(. 
-00008ae0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00008af0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00008b00: 2069 6e64 6578 5f63 6f6c 3d69 6e64 6578   index_col=index
-00008b10: 5f63 6f6c 2c0a 2020 2020 2020 2020 2020  _col,.          
-00008b20: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
-00008b30: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
-00008b40: 2020 6465 6620 7265 6164 5f67 6271 5f6d    def read_gbq_m
-00008b50: 6f64 656c 2873 656c 662c 206d 6f64 656c  odel(self, model
-00008b60: 5f6e 616d 653a 2073 7472 293a 0a20 2020  _name: str):.   
-00008b70: 2020 2020 2022 2222 4c6f 6164 7320 6120       """Loads a 
-00008b80: 4269 6751 7565 7279 204d 4c20 6d6f 6465  BigQuery ML mode
-00008b90: 6c20 6672 6f6d 2042 6967 5175 6572 792e  l from BigQuery.
-00008ba0: 0a0a 2020 2020 2020 2020 2a2a 4578 616d  ..        **Exam
-00008bb0: 706c 6573 3a2a 2a0a 0a20 2020 2020 2020  ples:**..       
-00008bc0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-00008bd0: 6269 6766 7261 6d65 732e 7061 6e64 6173  bigframes.pandas
-00008be0: 2061 7320 6270 640a 2020 2020 2020 2020   as bpd.        
-00008bf0: 2020 2020 3e3e 3e20 6270 642e 6f70 7469      >>> bpd.opti
-00008c00: 6f6e 732e 6469 7370 6c61 792e 7072 6f67  ons.display.prog
-00008c10: 7265 7373 5f62 6172 203d 204e 6f6e 650a  ress_bar = None.
-00008c20: 0a20 2020 2020 2020 2052 6561 6420 616e  .        Read an
-00008c30: 2065 7869 7374 696e 6720 4269 6751 7565   existing BigQue
-00008c40: 7279 204d 4c20 6d6f 6465 6c2e 0a0a 2020  ry ML model...  
-00008c50: 2020 2020 2020 2020 2020 3e3e 3e20 6d6f            >>> mo
-00008c60: 6465 6c5f 6e61 6d65 203d 2022 6269 6766  del_name = "bigf
-00008c70: 7261 6d65 732d 6465 762e 6271 6d6c 5f74  rames-dev.bqml_t
-00008c80: 7574 6f72 6961 6c2e 7065 6e67 7569 6e73  utorial.penguins
-00008c90: 5f6d 6f64 656c 220a 2020 2020 2020 2020  _model".        
-00008ca0: 2020 2020 3e3e 3e20 6d6f 6465 6c20 3d20      >>> model = 
-00008cb0: 6270 642e 7265 6164 5f67 6271 5f6d 6f64  bpd.read_gbq_mod
-00008cc0: 656c 286d 6f64 656c 5f6e 616d 6529 0a0a  el(model_name)..
-00008cd0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00008ce0: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
-00008cf0: 6e61 6d65 2028 7374 7229 3a0a 2020 2020  name (str):.    
-00008d00: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00008d10: 6d6f 6465 6c27 7320 6e61 6d65 2069 6e20  model's name in 
-00008d20: 4269 6751 7565 7279 2069 6e20 7468 6520  BigQuery in the 
-00008d30: 666f 726d 6174 0a20 2020 2020 2020 2020  format.         
-00008d40: 2020 2020 2020 2060 7072 6f6a 6563 745f         `project_
-00008d50: 6964 2e64 6174 6173 6574 5f69 642e 6d6f  id.dataset_id.mo
-00008d60: 6465 6c5f 6964 602c 206f 7220 6a75 7374  del_id`, or just
-00008d70: 2060 6461 7461 7365 745f 6964 2e6d 6f64   `dataset_id.mod
-00008d80: 656c 5f69 6460 0a20 2020 2020 2020 2020  el_id`.         
-00008d90: 2020 2020 2020 2074 6f20 6c6f 6164 2066         to load f
-00008da0: 726f 6d20 7468 6520 6465 6661 756c 7420  rom the default 
-00008db0: 7072 6f6a 6563 742e 0a0a 2020 2020 2020  project...      
-00008dc0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00008dd0: 2020 2020 2020 2041 2062 6967 6672 616d         A bigfram
-00008de0: 6573 2e6d 6c20 4d6f 6465 6c2c 2054 7261  es.ml Model, Tra
-00008df0: 6e73 666f 726d 6572 206f 7220 5069 7065  nsformer or Pipe
-00008e00: 6c69 6e65 2077 7261 7070 696e 6720 7468  line wrapping th
-00008e10: 6520 6d6f 6465 6c2e 0a20 2020 2020 2020  e model..       
-00008e20: 2022 2222 0a20 2020 2020 2020 2069 6d70   """.        imp
-00008e30: 6f72 7420 6269 6766 7261 6d65 732e 6d6c  ort bigframes.ml
-00008e40: 2e6c 6f61 6465 720a 0a20 2020 2020 2020  .loader..       
-00008e50: 206d 6f64 656c 5f72 6566 203d 2062 6967   model_ref = big
-00008e60: 7175 6572 792e 4d6f 6465 6c52 6566 6572  query.ModelRefer
-00008e70: 656e 6365 2e66 726f 6d5f 7374 7269 6e67  ence.from_string
-00008e80: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
-00008e90: 6465 6c5f 6e61 6d65 2c20 6465 6661 756c  del_name, defaul
-00008ea0: 745f 7072 6f6a 6563 743d 7365 6c66 2e62  t_project=self.b
-00008eb0: 7163 6c69 656e 742e 7072 6f6a 6563 740a  qclient.project.
-00008ec0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00008ed0: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e62    model = self.b
-00008ee0: 7163 6c69 656e 742e 6765 745f 6d6f 6465  qclient.get_mode
-00008ef0: 6c28 6d6f 6465 6c5f 7265 6629 0a20 2020  l(model_ref).   
-00008f00: 2020 2020 2072 6574 7572 6e20 6269 6766       return bigf
-00008f10: 7261 6d65 732e 6d6c 2e6c 6f61 6465 722e  rames.ml.loader.
-00008f20: 6672 6f6d 5f62 7128 7365 6c66 2c20 6d6f  from_bq(self, mo
-00008f30: 6465 6c29 0a0a 2020 2020 4074 7970 696e  del)..    @typin
-00008f40: 672e 6f76 6572 6c6f 6164 0a20 2020 2064  g.overload.    d
-00008f50: 6566 2072 6561 645f 7061 6e64 6173 280a  ef read_pandas(.
-00008f60: 2020 2020 2020 2020 7365 6c66 2c20 7061          self, pa
-00008f70: 6e64 6173 5f64 6174 6166 7261 6d65 3a20  ndas_dataframe: 
-00008f80: 7061 6e64 6173 2e49 6e64 6578 0a20 2020  pandas.Index.   
-00008f90: 2029 202d 3e20 6269 6766 7261 6d65 732e   ) -> bigframes.
-00008fa0: 636f 7265 2e69 6e64 6578 6573 2e49 6e64  core.indexes.Ind
-00008fb0: 6578 3a0a 2020 2020 2020 2020 2e2e 2e0a  ex:.        ....
-00008fc0: 0a20 2020 2040 7479 7069 6e67 2e6f 7665  .    @typing.ove
-00008fd0: 726c 6f61 640a 2020 2020 6465 6620 7265  rload.    def re
-00008fe0: 6164 5f70 616e 6461 7328 7365 6c66 2c20  ad_pandas(self, 
-00008ff0: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-00009000: 3a20 7061 6e64 6173 2e53 6572 6965 7329  : pandas.Series)
-00009010: 202d 3e20 6269 6766 7261 6d65 732e 7365   -> bigframes.se
-00009020: 7269 6573 2e53 6572 6965 733a 0a20 2020  ries.Series:.   
-00009030: 2020 2020 202e 2e2e 0a0a 2020 2020 4074       .....    @t
-00009040: 7970 696e 672e 6f76 6572 6c6f 6164 0a20  yping.overload. 
-00009050: 2020 2064 6566 2072 6561 645f 7061 6e64     def read_pand
-00009060: 6173 2873 656c 662c 2070 616e 6461 735f  as(self, pandas_
-00009070: 6461 7461 6672 616d 653a 2070 616e 6461  dataframe: panda
-00009080: 732e 4461 7461 4672 616d 6529 202d 3e20  s.DataFrame) -> 
-00009090: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-000090a0: 616d 653a 0a20 2020 2020 2020 202e 2e2e  ame:.        ...
-000090b0: 0a0a 2020 2020 6465 6620 7265 6164 5f70  ..    def read_p
-000090c0: 616e 6461 7328 0a20 2020 2020 2020 2073  andas(.        s
-000090d0: 656c 662c 2070 616e 6461 735f 6461 7461  elf, pandas_data
-000090e0: 6672 616d 653a 2055 6e69 6f6e 5b70 616e  frame: Union[pan
-000090f0: 6461 732e 4461 7461 4672 616d 652c 2070  das.DataFrame, p
-00009100: 616e 6461 732e 5365 7269 6573 2c20 7061  andas.Series, pa
-00009110: 6e64 6173 2e49 6e64 6578 5d0a 2020 2020  ndas.Index].    
-00009120: 293a 0a20 2020 2020 2020 2022 2222 4c6f  ):.        """Lo
-00009130: 6164 7320 4461 7461 4672 616d 6520 6672  ads DataFrame fr
-00009140: 6f6d 2061 2070 616e 6461 7320 4461 7461  om a pandas Data
-00009150: 4672 616d 652e 0a0a 2020 2020 2020 2020  Frame...        
-00009160: 5468 6520 7061 6e64 6173 2044 6174 6146  The pandas DataF
-00009170: 7261 6d65 2077 696c 6c20 6265 2070 6572  rame will be per
-00009180: 7369 7374 6564 2061 7320 6120 7465 6d70  sisted as a temp
-00009190: 6f72 6172 7920 4269 6751 7565 7279 2074  orary BigQuery t
-000091a0: 6162 6c65 2c20 7768 6963 6820 6361 6e20  able, which can 
-000091b0: 6265 0a20 2020 2020 2020 2061 7574 6f6d  be.        autom
-000091c0: 6174 6963 616c 6c79 2072 6563 7963 6c65  atically recycle
-000091d0: 6420 6166 7465 7220 7468 6520 5365 7373  d after the Sess
-000091e0: 696f 6e20 6973 2063 6c6f 7365 642e 0a0a  ion is closed...
-000091f0: 2020 2020 2020 2020 2a2a 4578 616d 706c          **Exampl
-00009200: 6573 3a2a 2a0a 0a20 2020 2020 2020 2020  es:**..         
-00009210: 2020 203e 3e3e 2069 6d70 6f72 7420 6269     >>> import bi
-00009220: 6766 7261 6d65 732e 7061 6e64 6173 2061  gframes.pandas a
-00009230: 7320 6270 640a 2020 2020 2020 2020 2020  s bpd.          
-00009240: 2020 3e3e 3e20 696d 706f 7274 2070 616e    >>> import pan
-00009250: 6461 7320 6173 2070 640a 2020 2020 2020  das as pd.      
-00009260: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
-00009270: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
-00009280: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
-00009290: 650a 0a20 2020 2020 2020 2020 2020 203e  e..            >
-000092a0: 3e3e 2064 203d 207b 2763 6f6c 3127 3a20  >> d = {'col1': 
-000092b0: 5b31 2c20 325d 2c20 2763 6f6c 3227 3a20  [1, 2], 'col2': 
-000092c0: 5b33 2c20 345d 7d0a 2020 2020 2020 2020  [3, 4]}.        
-000092d0: 2020 2020 3e3e 3e20 7061 6e64 6173 5f64      >>> pandas_d
-000092e0: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
-000092f0: 2864 6174 613d 6429 0a20 2020 2020 2020  (data=d).       
-00009300: 2020 2020 203e 3e3e 2064 6620 3d20 6270       >>> df = bp
-00009310: 642e 7265 6164 5f70 616e 6461 7328 7061  d.read_pandas(pa
-00009320: 6e64 6173 5f64 6629 0a20 2020 2020 2020  ndas_df).       
-00009330: 2020 2020 203e 3e3e 2064 660a 2020 2020       >>> df.    
-00009340: 2020 2020 2020 2020 2020 2063 6f6c 3120             col1 
-00009350: 2063 6f6c 320a 2020 2020 2020 2020 2020   col2.          
-00009360: 2020 3020 2020 2020 3120 2020 2020 330a    0     1     3.
-00009370: 2020 2020 2020 2020 2020 2020 3120 2020              1   
-00009380: 2020 3220 2020 2020 340a 2020 2020 2020    2     4.      
-00009390: 2020 2020 2020 3c42 4c41 4e4b 4c49 4e45        <BLANKLINE
-000093a0: 3e0a 2020 2020 2020 2020 2020 2020 5b32  >.            [2
-000093b0: 2072 6f77 7320 7820 3220 636f 6c75 6d6e   rows x 2 column
-000093c0: 735d 0a0a 2020 2020 2020 2020 4172 6773  s]..        Args
-000093d0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-000093e0: 6e64 6173 5f64 6174 6166 7261 6d65 2028  ndas_dataframe (
-000093f0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-00009400: 2c20 7061 6e64 6173 2e53 6572 6965 732c  , pandas.Series,
-00009410: 206f 7220 7061 6e64 6173 2e49 6e64 6578   or pandas.Index
-00009420: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00009430: 2020 2061 2070 616e 6461 7320 4461 7461     a pandas Data
-00009440: 4672 616d 652f 5365 7269 6573 2f49 6e64  Frame/Series/Ind
-00009450: 6578 206f 626a 6563 7420 746f 2062 6520  ex object to be 
-00009460: 6c6f 6164 6564 2e0a 0a20 2020 2020 2020  loaded...       
-00009470: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00009480: 2020 2020 2020 416e 2065 7175 6976 616c        An equival
-00009490: 656e 7420 6269 6766 7261 6d65 732e 7061  ent bigframes.pa
-000094a0: 6e64 6173 2e28 4461 7461 4672 616d 652f  ndas.(DataFrame/
-000094b0: 5365 7269 6573 2f49 6e64 6578 2920 6f62  Series/Index) ob
-000094c0: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-000094d0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-000094e0: 6269 6766 7261 6d65 732e 7365 7269 6573  bigframes.series
-000094f0: 2061 7320 7365 7269 6573 0a0a 2020 2020   as series..    
-00009500: 2020 2020 2320 5472 7920 746f 2068 616e      # Try to han
-00009510: 646c 6520 6e6f 6e2d 6461 7461 6672 616d  dle non-datafram
-00009520: 6520 7061 6e64 6173 206f 626a 6563 7473  e pandas objects
-00009530: 2061 7320 7765 6c6c 0a20 2020 2020 2020   as well.       
-00009540: 2069 6620 6973 696e 7374 616e 6365 2870   if isinstance(p
-00009550: 616e 6461 735f 6461 7461 6672 616d 652c  andas_dataframe,
-00009560: 2070 616e 6461 732e 5365 7269 6573 293a   pandas.Series):
-00009570: 0a20 2020 2020 2020 2020 2020 2062 665f  .            bf_
-00009580: 6466 203d 2073 656c 662e 5f72 6561 645f  df = self._read_
-00009590: 7061 6e64 6173 2870 616e 6461 732e 4461  pandas(pandas.Da
-000095a0: 7461 4672 616d 6528 7061 6e64 6173 5f64  taFrame(pandas_d
-000095b0: 6174 6166 7261 6d65 292c 2022 7265 6164  ataframe), "read
-000095c0: 5f70 616e 6461 7322 290a 2020 2020 2020  _pandas").      
-000095d0: 2020 2020 2020 6266 5f73 6572 6965 7320        bf_series 
-000095e0: 3d20 7479 7069 6e67 2e63 6173 7428 7365  = typing.cast(se
-000095f0: 7269 6573 2e53 6572 6965 732c 2062 665f  ries.Series, bf_
-00009600: 6466 5b62 665f 6466 2e63 6f6c 756d 6e73  df[bf_df.columns
-00009610: 5b30 5d5d 290a 2020 2020 2020 2020 2020  [0]]).          
-00009620: 2020 2320 7772 6170 7069 6e67 2069 6e74    # wrapping int
-00009630: 6f20 6466 2063 616e 2073 6574 206e 616d  o df can set nam
-00009640: 6520 746f 2030 2073 6f20 7265 7365 7420  e to 0 so reset 
-00009650: 746f 206f 7269 6769 6e61 6c20 6f62 6a65  to original obje
-00009660: 6374 206e 616d 650a 2020 2020 2020 2020  ct name.        
-00009670: 2020 2020 6266 5f73 6572 6965 732e 6e61      bf_series.na
-00009680: 6d65 203d 2070 616e 6461 735f 6461 7461  me = pandas_data
-00009690: 6672 616d 652e 6e61 6d65 0a20 2020 2020  frame.name.     
-000096a0: 2020 2020 2020 2072 6574 7572 6e20 6266         return bf
-000096b0: 5f73 6572 6965 730a 2020 2020 2020 2020  _series.        
-000096c0: 6966 2069 7369 6e73 7461 6e63 6528 7061  if isinstance(pa
-000096d0: 6e64 6173 5f64 6174 6166 7261 6d65 2c20  ndas_dataframe, 
-000096e0: 7061 6e64 6173 2e49 6e64 6578 293a 0a20  pandas.Index):. 
-000096f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009700: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
-00009710: 6461 7328 0a20 2020 2020 2020 2020 2020  das(.           
-00009720: 2020 2020 2070 616e 6461 732e 4461 7461       pandas.Data
-00009730: 4672 616d 6528 696e 6465 783d 7061 6e64  Frame(index=pand
-00009740: 6173 5f64 6174 6166 7261 6d65 292c 2022  as_dataframe), "
-00009750: 7265 6164 5f70 616e 6461 7322 0a20 2020  read_pandas".   
-00009760: 2020 2020 2020 2020 2029 2e69 6e64 6578           ).index
-00009770: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00009780: 7374 616e 6365 2870 616e 6461 735f 6461  stance(pandas_da
-00009790: 7461 6672 616d 652c 2070 616e 6461 732e  taframe, pandas.
-000097a0: 4461 7461 4672 616d 6529 3a0a 2020 2020  DataFrame):.    
-000097b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000097c0: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
-000097d0: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
-000097e0: 652c 2022 7265 6164 5f70 616e 6461 7322  e, "read_pandas"
-000097f0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00009800: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009810: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00009820: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00009830: 7265 6164 5f70 616e 6461 7328 2920 6578  read_pandas() ex
-00009840: 7065 6374 7320 6120 7061 6e64 6173 2e44  pects a pandas.D
-00009850: 6174 6146 7261 6d65 2c20 6275 7420 676f  ataFrame, but go
-00009860: 7420 6120 7b74 7970 6528 7061 6e64 6173  t a {type(pandas
-00009870: 5f64 6174 6166 7261 6d65 297d 220a 2020  _dataframe)}".  
-00009880: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00009890: 2064 6566 205f 7265 6164 5f70 616e 6461   def _read_panda
-000098a0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-000098b0: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-000098c0: 653a 2070 616e 6461 732e 4461 7461 4672  e: pandas.DataFr
-000098d0: 616d 652c 2061 7069 5f6e 616d 653a 2073  ame, api_name: s
-000098e0: 7472 0a20 2020 2029 202d 3e20 6461 7461  tr.    ) -> data
-000098f0: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
-00009900: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00009910: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
-00009920: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
-00009930: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
-00009940: 6e73 7461 6e63 6528 7061 6e64 6173 5f64  nstance(pandas_d
-00009950: 6174 6166 7261 6d65 2c20 6461 7461 6672  ataframe, datafr
-00009960: 616d 652e 4461 7461 4672 616d 6529 3a0a  ame.DataFrame):.
-00009970: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009980: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00009990: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000099a0: 6561 645f 7061 6e64 6173 2829 2065 7870  ead_pandas() exp
-000099b0: 6563 7473 2061 2070 616e 6461 732e 4461  ects a pandas.Da
-000099c0: 7461 4672 616d 652c 2062 7574 2067 6f74  taFrame, but got
-000099d0: 2061 2022 0a20 2020 2020 2020 2020 2020   a ".           
-000099e0: 2020 2020 2022 6269 6766 7261 6d65 732e       "bigframes.
-000099f0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-00009a00: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
-00009a10: 0a0a 2020 2020 2020 2020 696e 6c69 6e65  ..        inline
-00009a20: 5f64 6620 3d20 7365 6c66 2e5f 7265 6164  _df = self._read
-00009a30: 5f70 616e 6461 735f 696e 6c69 6e65 2870  _pandas_inline(p
-00009a40: 616e 6461 735f 6461 7461 6672 616d 6529  andas_dataframe)
-00009a50: 0a20 2020 2020 2020 2069 6620 696e 6c69  .        if inli
-00009a60: 6e65 5f64 6620 6973 206e 6f74 204e 6f6e  ne_df is not Non
-00009a70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00009a80: 6574 7572 6e20 696e 6c69 6e65 5f64 660a  eturn inline_df.
-00009a90: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00009aa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009ab0: 7365 6c66 2e5f 7265 6164 5f70 616e 6461  self._read_panda
-00009ac0: 735f 6c6f 6164 5f6a 6f62 2870 616e 6461  s_load_job(panda
-00009ad0: 735f 6461 7461 6672 616d 652c 2061 7069  s_dataframe, api
-00009ae0: 5f6e 616d 6529 0a20 2020 2020 2020 2065  _name).        e
-00009af0: 7863 6570 7420 7061 2e41 7272 6f77 496e  xcept pa.ArrowIn
-00009b00: 7661 6c69 6420 6173 2065 3a0a 2020 2020  valid as e:.    
-00009b10: 2020 2020 2020 2020 7261 6973 6520 7061          raise pa
-00009b20: 2e41 7272 6f77 496e 7661 6c69 6428 0a20  .ArrowInvalid(. 
-00009b30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00009b40: 2243 6f75 6c64 206e 6f74 2063 6f6e 7665  "Could not conve
-00009b50: 7274 2077 6974 6820 6120 4269 6751 7565  rt with a BigQue
-00009b60: 7279 2074 7970 653a 2060 7b65 7d60 2e20  ry type: `{e}`. 
-00009b70: 220a 2020 2020 2020 2020 2020 2020 2920  ".            ) 
-00009b80: 6672 6f6d 2065 0a0a 2020 2020 6465 6620  from e..    def 
-00009b90: 5f72 6561 645f 7061 6e64 6173 5f69 6e6c  _read_pandas_inl
-00009ba0: 696e 6528 0a20 2020 2020 2020 2073 656c  ine(.        sel
-00009bb0: 662c 2070 616e 6461 735f 6461 7461 6672  f, pandas_datafr
-00009bc0: 616d 653a 2070 616e 6461 732e 4461 7461  ame: pandas.Data
-00009bd0: 4672 616d 650a 2020 2020 2920 2d3e 204f  Frame.    ) -> O
-00009be0: 7074 696f 6e61 6c5b 6461 7461 6672 616d  ptional[datafram
-00009bf0: 652e 4461 7461 4672 616d 655d 3a0a 2020  e.DataFrame]:.  
-00009c00: 2020 2020 2020 696d 706f 7274 2062 6967        import big
-00009c10: 6672 616d 6573 2e64 6174 6166 7261 6d65  frames.dataframe
-00009c20: 2061 7320 6461 7461 6672 616d 650a 0a20   as dataframe.. 
-00009c30: 2020 2020 2020 2069 6620 7061 6e64 6173         if pandas
-00009c40: 5f64 6174 6166 7261 6d65 2e6d 656d 6f72  _dataframe.memor
-00009c50: 795f 7573 6167 6528 6465 6570 3d54 7275  y_usage(deep=Tru
-00009c60: 6529 2e73 756d 2829 203e 204d 4158 5f49  e).sum() > MAX_I
-00009c70: 4e4c 494e 455f 4446 5f42 5954 4553 3a0a  NLINE_DF_BYTES:.
-00009c80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009c90: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-00009ca0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00009cb0: 2020 696e 6c69 6e65 5f64 6620 3d20 6461    inline_df = da
-00009cc0: 7461 6672 616d 652e 4461 7461 4672 616d  taframe.DataFram
-00009cd0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00009ce0: 2020 2062 6c6f 636b 732e 426c 6f63 6b2e     blocks.Block.
-00009cf0: 6672 6f6d 5f6c 6f63 616c 2870 616e 6461  from_local(panda
-00009d00: 735f 6461 7461 6672 616d 652c 2073 656c  s_dataframe, sel
-00009d10: 6629 0a20 2020 2020 2020 2020 2020 2029  f).            )
-00009d20: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00009d30: 7061 2e41 7272 6f77 496e 7661 6c69 6420  pa.ArrowInvalid 
-00009d40: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00009d50: 2020 7261 6973 6520 7061 2e41 7272 6f77    raise pa.Arrow
-00009d60: 496e 7661 6c69 6428 0a20 2020 2020 2020  Invalid(.       
-00009d70: 2020 2020 2020 2020 2066 2243 6f75 6c64           f"Could
-00009d80: 206e 6f74 2063 6f6e 7665 7274 2077 6974   not convert wit
-00009d90: 6820 6120 4269 6751 7565 7279 2074 7970  h a BigQuery typ
-00009da0: 653a 2060 7b65 7d60 2e20 220a 2020 2020  e: `{e}`. ".    
-00009db0: 2020 2020 2020 2020 2920 6672 6f6d 2065          ) from e
-00009dc0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00009dd0: 5661 6c75 6545 7272 6f72 3a20 2023 2054  ValueError:  # T
-00009de0: 6872 6f77 6e20 6279 2069 6269 7320 666f  hrown by ibis fo
-00009df0: 7220 736f 6d65 2075 6e68 616e 646c 6564  r some unhandled
-00009e00: 2074 7970 6573 0a20 2020 2020 2020 2020   types.         
-00009e10: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00009e20: 2020 2020 2020 2065 7863 6570 7420 7061         except pa
-00009e30: 2e41 7272 6f77 5479 7065 4572 726f 723a  .ArrowTypeError:
-00009e40: 2020 2320 5468 726f 776e 2062 7920 6172    # Thrown by ar
-00009e50: 726f 7720 666f 7220 7479 7065 7320 7769  row for types wi
-00009e60: 7468 6f75 7420 6d61 7070 696e 6720 2867  thout mapping (g
-00009e70: 656f 292e 0a20 2020 2020 2020 2020 2020  eo)..           
-00009e80: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00009e90: 2020 2020 2020 696e 6c69 6e65 5f74 7970        inline_typ
-00009ea0: 6573 203d 2069 6e6c 696e 655f 6466 2e5f  es = inline_df._
-00009eb0: 626c 6f63 6b2e 6578 7072 2e73 6368 656d  block.expr.schem
-00009ec0: 612e 6474 7970 6573 0a20 2020 2020 2020  a.dtypes.       
-00009ed0: 2023 2049 6269 7320 6861 7320 7072 6f62   # Ibis has prob
-00009ee0: 6c65 6d73 2065 7363 6170 696e 6720 6279  lems escaping by
-00009ef0: 7465 7320 6c69 7465 7261 6c73 2c20 7768  tes literals, wh
-00009f00: 6963 6820 7769 6c6c 2063 6175 7365 2073  ich will cause s
-00009f10: 796e 7461 7820 6572 726f 7273 2073 6572  yntax errors ser
-00009f20: 7665 722d 7369 6465 2e0a 2020 2020 2020  ver-side..      
-00009f30: 2020 6966 2061 6c6c 2864 7479 7065 2069    if all(dtype i
-00009f40: 6e20 494e 4c49 4e41 424c 455f 4454 5950  n INLINABLE_DTYP
-00009f50: 4553 2066 6f72 2064 7479 7065 2069 6e20  ES for dtype in 
-00009f60: 696e 6c69 6e65 5f74 7970 6573 293a 0a20  inline_types):. 
-00009f70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009f80: 6e20 696e 6c69 6e65 5f64 660a 2020 2020  n inline_df.    
-00009f90: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00009fa0: 0a20 2020 2064 6566 205f 7265 6164 5f70  .    def _read_p
-00009fb0: 616e 6461 735f 6c6f 6164 5f6a 6f62 280a  andas_load_job(.
-00009fc0: 2020 2020 2020 2020 7365 6c66 2c20 7061          self, pa
-00009fd0: 6e64 6173 5f64 6174 6166 7261 6d65 3a20  ndas_dataframe: 
-00009fe0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-00009ff0: 2c20 6170 695f 6e61 6d65 3a20 7374 720a  , api_name: str.
-0000a000: 2020 2020 2920 2d3e 2064 6174 6166 7261      ) -> datafra
-0000a010: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
-0000a020: 2020 2020 2020 696d 706f 7274 2062 6967        import big
-0000a030: 6672 616d 6573 2e64 6174 6166 7261 6d65  frames.dataframe
-0000a040: 2061 7320 6461 7461 6672 616d 650a 0a20   as dataframe.. 
-0000a050: 2020 2020 2020 2063 6f6c 5f69 6e64 6578         col_index
-0000a060: 203d 2070 616e 6461 735f 6461 7461 6672   = pandas_datafr
-0000a070: 616d 652e 636f 6c75 6d6e 732e 636f 7079  ame.columns.copy
-0000a080: 2829 0a20 2020 2020 2020 2063 6f6c 5f6c  ().        col_l
-0000a090: 6162 656c 732c 2069 6478 5f6c 6162 656c  abels, idx_label
-0000a0a0: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
-0000a0b0: 2020 636f 6c5f 696e 6465 782e 746f 5f6c    col_index.to_l
-0000a0c0: 6973 7428 292c 0a20 2020 2020 2020 2020  ist(),.         
-0000a0d0: 2020 2070 616e 6461 735f 6461 7461 6672     pandas_datafr
-0000a0e0: 616d 652e 696e 6465 782e 6e61 6d65 732c  ame.index.names,
-0000a0f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000a100: 2020 206e 6577 5f63 6f6c 5f69 6473 2c20     new_col_ids, 
-0000a110: 6e65 775f 6964 785f 6964 7320 3d20 7574  new_idx_ids = ut
-0000a120: 696c 732e 6765 745f 7374 616e 6461 7264  ils.get_standard
-0000a130: 697a 6564 5f69 6473 280a 2020 2020 2020  ized_ids(.      
-0000a140: 2020 2020 2020 636f 6c5f 6c61 6265 6c73        col_labels
-0000a150: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
-0000a160: 785f 6c61 6265 6c73 2c0a 2020 2020 2020  x_labels,.      
-0000a170: 2020 2020 2020 2320 4c6f 6164 696e 6720        # Loading 
-0000a180: 7061 7271 7565 7420 6669 6c65 7320 696e  parquet files in
-0000a190: 746f 2042 6967 5175 6572 7920 7769 7468  to BigQuery with
-0000a1a0: 2073 7065 6369 616c 2063 6f6c 756d 6e20   special column 
-0000a1b0: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
-0000a1c0: 2020 2320 6973 206f 6e6c 7920 7375 7070    # is only supp
-0000a1d0: 6f72 7465 6420 756e 6465 7220 616e 2061  orted under an a
-0000a1e0: 6c6c 6f77 6c69 7374 2e0a 2020 2020 2020  llowlist..      
-0000a1f0: 2020 2020 2020 7374 7269 6374 3d54 7275        strict=Tru
-0000a200: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-0000a210: 2020 2020 2020 2320 4164 6420 6f72 6465        # Add orde
-0000a220: 7220 636f 6c75 6d6e 2074 6f20 7061 6e64  r column to pand
-0000a230: 6173 2044 6174 6146 7261 6d65 2074 6f20  as DataFrame to 
-0000a240: 7072 6573 6572 7665 206f 7264 6572 2069  preserve order i
-0000a250: 6e20 4269 6751 7565 7279 0a20 2020 2020  n BigQuery.     
-0000a260: 2020 206f 7264 6572 696e 675f 636f 6c20     ordering_col 
-0000a270: 3d20 2272 6f77 6964 220a 2020 2020 2020  = "rowid".      
-0000a280: 2020 636f 6c75 6d6e 7320 3d20 6672 6f7a    columns = froz
-0000a290: 656e 7365 7428 636f 6c5f 6c61 6265 6c73  enset(col_labels
-0000a2a0: 202b 2069 6478 5f6c 6162 656c 7329 0a20   + idx_labels). 
-0000a2b0: 2020 2020 2020 2073 7566 6669 7820 3d20         suffix = 
-0000a2c0: 320a 2020 2020 2020 2020 7768 696c 6520  2.        while 
-0000a2d0: 6f72 6465 7269 6e67 5f63 6f6c 2069 6e20  ordering_col in 
-0000a2e0: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
-0000a2f0: 2020 2020 206f 7264 6572 696e 675f 636f       ordering_co
-0000a300: 6c20 3d20 6622 726f 7769 645f 7b73 7566  l = f"rowid_{suf
-0000a310: 6669 787d 220a 2020 2020 2020 2020 2020  fix}".          
-0000a320: 2020 7375 6666 6978 202b 3d20 310a 0a20    suffix += 1.. 
-0000a330: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
-0000a340: 7461 6672 616d 655f 636f 7079 203d 2070  taframe_copy = p
-0000a350: 616e 6461 735f 6461 7461 6672 616d 652e  andas_dataframe.
-0000a360: 636f 7079 2829 0a20 2020 2020 2020 2070  copy().        p
-0000a370: 616e 6461 735f 6461 7461 6672 616d 655f  andas_dataframe_
-0000a380: 636f 7079 2e69 6e64 6578 2e6e 616d 6573  copy.index.names
-0000a390: 203d 206e 6577 5f69 6478 5f69 6473 0a20   = new_idx_ids. 
-0000a3a0: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
-0000a3b0: 7461 6672 616d 655f 636f 7079 2e63 6f6c  taframe_copy.col
-0000a3c0: 756d 6e73 203d 2070 616e 6461 732e 496e  umns = pandas.In
-0000a3d0: 6465 7828 6e65 775f 636f 6c5f 6964 7329  dex(new_col_ids)
-0000a3e0: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
-0000a3f0: 6461 7461 6672 616d 655f 636f 7079 5b6f  dataframe_copy[o
-0000a400: 7264 6572 696e 675f 636f 6c5d 203d 206e  rdering_col] = n
-0000a410: 702e 6172 616e 6765 2870 616e 6461 735f  p.arange(pandas_
-0000a420: 6461 7461 6672 616d 655f 636f 7079 2e73  dataframe_copy.s
-0000a430: 6861 7065 5b30 5d29 0a0a 2020 2020 2020  hape[0])..      
-0000a440: 2020 6a6f 625f 636f 6e66 6967 203d 2073    job_config = s
-0000a450: 656c 662e 5f70 7265 7061 7265 5f6c 6f61  elf._prepare_loa
-0000a460: 645f 6a6f 625f 636f 6e66 6967 2829 0a0a  d_job_config()..
-0000a470: 2020 2020 2020 2020 2320 5370 6563 6966          # Specif
-0000a480: 7920 7468 6520 6461 7465 7469 6d65 2064  y the datetime d
-0000a490: 7479 7065 732c 2077 6869 6368 2069 7320  types, which is 
-0000a4a0: 6175 746f 2d64 6574 6563 7465 6420 6173  auto-detected as
-0000a4b0: 2074 696d 6573 7461 6d70 2074 7970 6573   timestamp types
-0000a4c0: 2e0a 2020 2020 2020 2020 7363 6865 6d61  ..        schema
-0000a4d0: 3a20 6c69 7374 5b62 6967 7175 6572 792e  : list[bigquery.
-0000a4e0: 5363 6865 6d61 4669 656c 645d 203d 205b  SchemaField] = [
-0000a4f0: 5d0a 2020 2020 2020 2020 666f 7220 636f  ].        for co
-0000a500: 6c75 6d6e 2c20 6474 7970 6520 696e 207a  lumn, dtype in z
-0000a510: 6970 286e 6577 5f63 6f6c 5f69 6473 2c20  ip(new_col_ids, 
-0000a520: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-0000a530: 2e64 7479 7065 7329 3a0a 2020 2020 2020  .dtypes):.      
-0000a540: 2020 2020 2020 6966 2064 7479 7065 203d        if dtype =
-0000a550: 3d20 2274 696d 6573 7461 6d70 5b75 735d  = "timestamp[us]
-0000a560: 5b70 7961 7272 6f77 5d22 3a0a 2020 2020  [pyarrow]":.    
-0000a570: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-0000a580: 6d61 2e61 7070 656e 6428 0a20 2020 2020  ma.append(.     
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000a5a0: 6967 7175 6572 792e 5363 6865 6d61 4669  igquery.SchemaFi
-0000a5b0: 656c 6428 636f 6c75 6d6e 2c20 6269 6771  eld(column, bigq
-0000a5c0: 7565 7279 2e65 6e75 6d73 2e53 716c 5479  uery.enums.SqlTy
-0000a5d0: 7065 4e61 6d65 732e 4441 5445 5449 4d45  peNames.DATETIME
-0000a5e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a5f0: 2020 290a 2020 2020 2020 2020 6a6f 625f    ).        job_
-0000a600: 636f 6e66 6967 2e73 6368 656d 6120 3d20  config.schema = 
-0000a610: 7363 6865 6d61 0a0a 2020 2020 2020 2020  schema..        
-0000a620: 2320 436c 7573 7465 7269 6e67 2070 726f  # Clustering pro
-0000a630: 6261 626c 7920 6e6f 7420 6e65 6564 6564  bably not needed
-0000a640: 2061 6e79 7761 7973 2061 7320 7061 6e64   anyways as pand
-0000a650: 6173 2074 6162 6c65 7320 6172 6520 736d  as tables are sm
-0000a660: 616c 6c0a 2020 2020 2020 2020 636c 7573  all.        clus
-0000a670: 7465 725f 636f 6c73 203d 205b 6f72 6465  ter_cols = [orde
-0000a680: 7269 6e67 5f63 6f6c 5d0a 2020 2020 2020  ring_col].      
-0000a690: 2020 6a6f 625f 636f 6e66 6967 2e63 6c75    job_config.clu
-0000a6a0: 7374 6572 696e 675f 6669 656c 6473 203d  stering_fields =
-0000a6b0: 2063 6c75 7374 6572 5f63 6f6c 730a 0a20   cluster_cols.. 
-0000a6c0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-0000a6d0: 672e 6c61 6265 6c73 203d 207b 2262 6967  g.labels = {"big
-0000a6e0: 6672 616d 6573 2d61 7069 223a 2061 7069  frames-api": api
-0000a6f0: 5f6e 616d 657d 0a0a 2020 2020 2020 2020  _name}..        
-0000a700: 6c6f 6164 5f74 6162 6c65 5f64 6573 7469  load_table_desti
-0000a710: 6e61 7469 6f6e 203d 2062 6967 6672 616d  nation = bigfram
-0000a720: 6573 5f69 6f2e 7261 6e64 6f6d 5f74 6162  es_io.random_tab
-0000a730: 6c65 2873 656c 662e 5f61 6e6f 6e79 6d6f  le(self._anonymo
-0000a740: 7573 5f64 6174 6173 6574 290a 2020 2020  us_dataset).    
-0000a750: 2020 2020 6c6f 6164 5f6a 6f62 203d 2073      load_job = s
-0000a760: 656c 662e 6271 636c 6965 6e74 2e6c 6f61  elf.bqclient.loa
-0000a770: 645f 7461 626c 655f 6672 6f6d 5f64 6174  d_table_from_dat
-0000a780: 6166 7261 6d65 280a 2020 2020 2020 2020  aframe(.        
-0000a790: 2020 2020 7061 6e64 6173 5f64 6174 6166      pandas_dataf
-0000a7a0: 7261 6d65 5f63 6f70 792c 0a20 2020 2020  rame_copy,.     
-0000a7b0: 2020 2020 2020 206c 6f61 645f 7461 626c         load_tabl
-0000a7c0: 655f 6465 7374 696e 6174 696f 6e2c 0a20  e_destination,. 
-0000a7d0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000a7e0: 6f6e 6669 673d 6a6f 625f 636f 6e66 6967  onfig=job_config
-0000a7f0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000a800: 2020 2020 7365 6c66 2e5f 7374 6172 745f      self._start_
-0000a810: 6765 6e65 7269 635f 6a6f 6228 6c6f 6164  generic_job(load
-0000a820: 5f6a 6f62 290a 0a20 2020 2020 2020 206f  _job)..        o
-0000a830: 7264 6572 696e 6720 3d20 6f72 6465 722e  rdering = order.
-0000a840: 4578 7072 6573 7369 6f6e 4f72 6465 7269  ExpressionOrderi
-0000a850: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-0000a860: 6f72 6465 7269 6e67 5f76 616c 7565 5f63  ordering_value_c
-0000a870: 6f6c 756d 6e73 3d74 7570 6c65 285b 6f72  olumns=tuple([or
-0000a880: 6465 722e 6173 6365 6e64 696e 675f 6f76  der.ascending_ov
-0000a890: 6572 286f 7264 6572 696e 675f 636f 6c29  er(ordering_col)
-0000a8a0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0000a8b0: 746f 7461 6c5f 6f72 6465 7269 6e67 5f63  total_ordering_c
-0000a8c0: 6f6c 756d 6e73 3d66 726f 7a65 6e73 6574  olumns=frozenset
-0000a8d0: 285b 6f72 6465 7269 6e67 5f63 6f6c 5d29  ([ordering_col])
-0000a8e0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-0000a8f0: 7465 6765 725f 656e 636f 6469 6e67 3d49  teger_encoding=I
-0000a900: 6e74 6567 6572 456e 636f 6469 6e67 2854  ntegerEncoding(T
-0000a910: 7275 652c 2069 735f 7365 7175 656e 7469  rue, is_sequenti
-0000a920: 616c 3d54 7275 6529 2c0a 2020 2020 2020  al=True),.      
-0000a930: 2020 290a 2020 2020 2020 2020 7461 626c    ).        tabl
-0000a940: 655f 6578 7072 6573 7369 6f6e 203d 2073  e_expression = s
-0000a950: 656c 662e 6962 6973 5f63 6c69 656e 742e  elf.ibis_client.
-0000a960: 7461 626c 6528 2020 2320 7479 7065 3a20  table(  # type: 
-0000a970: 6967 6e6f 7265 0a20 2020 2020 2020 2020  ignore.         
-0000a980: 2020 206c 6f61 645f 7461 626c 655f 6465     load_table_de
-0000a990: 7374 696e 6174 696f 6e2e 7461 626c 655f  stination.table_
-0000a9a0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0000a9b0: 7363 6865 6d61 3d6c 6f61 645f 7461 626c  schema=load_tabl
-0000a9c0: 655f 6465 7374 696e 6174 696f 6e2e 6461  e_destination.da
-0000a9d0: 7461 7365 745f 6964 2c0a 2020 2020 2020  taset_id,.      
-0000a9e0: 2020 2020 2020 6461 7461 6261 7365 3d6c        database=l
-0000a9f0: 6f61 645f 7461 626c 655f 6465 7374 696e  oad_table_destin
-0000aa00: 6174 696f 6e2e 7072 6f6a 6563 742c 0a20  ation.project,. 
-0000aa10: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000aa20: 2020 2320 622f 3239 3735 3930 3137 3820    # b/297590178 
-0000aa30: 506f 7465 6e74 6961 6c6c 7920 6120 6275  Potentially a bu
-0000aa40: 6720 696e 2062 7163 6c69 656e 742e 6c6f  g in bqclient.lo
-0000aa50: 6164 5f74 6162 6c65 5f66 726f 6d5f 6461  ad_table_from_da
-0000aa60: 7461 6672 616d 6528 292c 2074 6861 7420  taframe(), that 
-0000aa70: 6f6e 6c79 2077 6865 6e20 7468 6520 4446  only when the DF
-0000aa80: 2069 7320 656d 7074 792c 2074 6865 2069   is empty, the i
-0000aa90: 6e64 6578 2063 6f6c 756d 6e73 2064 6973  ndex columns dis
-0000aaa0: 6170 7065 6172 2069 6e20 7461 626c 655f  appear in table_
-0000aab0: 6578 7072 6573 7369 6f6e 2e0a 2020 2020  expression..    
-0000aac0: 2020 2020 6966 2061 6e79 280a 2020 2020      if any(.    
-0000aad0: 2020 2020 2020 2020 5b6e 6577 5f69 6478          [new_idx
-0000aae0: 5f69 6420 6e6f 7420 696e 2074 6162 6c65  _id not in table
-0000aaf0: 5f65 7870 7265 7373 696f 6e2e 636f 6c75  _expression.colu
-0000ab00: 6d6e 7320 666f 7220 6e65 775f 6964 785f  mns for new_idx_
-0000ab10: 6964 2069 6e20 6e65 775f 6964 785f 6964  id in new_idx_id
-0000ab20: 735d 0a20 2020 2020 2020 2029 3a0a 2020  s].        ):.  
-0000ab30: 2020 2020 2020 2020 2020 6e65 775f 6964            new_id
-0000ab40: 785f 6964 732c 2069 6478 5f6c 6162 656c  x_ids, idx_label
-0000ab50: 7320 3d20 5b5d 2c20 5b5d 0a0a 2020 2020  s = [], []..    
-0000ab60: 2020 2020 636f 6c75 6d6e 5f76 616c 7565      column_value
-0000ab70: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-0000ab80: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
-0000ab90: 6f6e 5b63 6f6c 5d0a 2020 2020 2020 2020  on[col].        
-0000aba0: 2020 2020 666f 7220 636f 6c20 696e 2074      for col in t
-0000abb0: 6162 6c65 5f65 7870 7265 7373 696f 6e2e  able_expression.
-0000abc0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-0000abd0: 2020 2020 6966 2063 6f6c 2021 3d20 6f72      if col != or
-0000abe0: 6465 7269 6e67 5f63 6f6c 0a20 2020 2020  dering_col.     
-0000abf0: 2020 205d 0a20 2020 2020 2020 2061 7272     ].        arr
-0000ac00: 6179 5f76 616c 7565 203d 2063 6f72 652e  ay_value = core.
-0000ac10: 4172 7261 7956 616c 7565 2e66 726f 6d5f  ArrayValue.from_
-0000ac20: 6962 6973 280a 2020 2020 2020 2020 2020  ibis(.          
-0000ac30: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000ac40: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
-0000ac50: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
-0000ac60: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
-0000ac70: 5f76 616c 7565 732c 0a20 2020 2020 2020  _values,.       
-0000ac80: 2020 2020 2068 6964 6465 6e5f 6f72 6465       hidden_orde
-0000ac90: 7269 6e67 5f63 6f6c 756d 6e73 3d5b 7461  ring_columns=[ta
-0000aca0: 626c 655f 6578 7072 6573 7369 6f6e 5b6f  ble_expression[o
-0000acb0: 7264 6572 696e 675f 636f 6c5d 5d2c 0a20  rdering_col]],. 
-0000acc0: 2020 2020 2020 2020 2020 206f 7264 6572             order
-0000acd0: 696e 673d 6f72 6465 7269 6e67 2c0a 2020  ing=ordering,.  
-0000ace0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000acf0: 2062 6c6f 636b 203d 2062 6c6f 636b 732e   block = blocks.
-0000ad00: 426c 6f63 6b28 0a20 2020 2020 2020 2020  Block(.         
-0000ad10: 2020 2061 7272 6179 5f76 616c 7565 2c0a     array_value,.
-0000ad20: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-0000ad30: 785f 636f 6c75 6d6e 733d 6e65 775f 6964  x_columns=new_id
-0000ad40: 785f 6964 732c 0a20 2020 2020 2020 2020  x_ids,.         
-0000ad50: 2020 2063 6f6c 756d 6e5f 6c61 6265 6c73     column_labels
-0000ad60: 3d63 6f6c 5f69 6e64 6578 2c0a 2020 2020  =col_index,.    
-0000ad70: 2020 2020 2020 2020 696e 6465 785f 6c61          index_la
-0000ad80: 6265 6c73 3d69 6478 5f6c 6162 656c 732c  bels=idx_labels,
-0000ad90: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000ada0: 2020 2072 6574 7572 6e20 6461 7461 6672     return datafr
-0000adb0: 616d 652e 4461 7461 4672 616d 6528 626c  ame.DataFrame(bl
-0000adc0: 6f63 6b29 0a0a 2020 2020 6465 6620 7265  ock)..    def re
-0000add0: 6164 5f63 7376 280a 2020 2020 2020 2020  ad_csv(.        
-0000ade0: 7365 6c66 2c0a 2020 2020 2020 2020 6669  self,.        fi
-0000adf0: 6c65 7061 7468 5f6f 725f 6275 6666 6572  lepath_or_buffer
-0000ae00: 3a20 7374 7220 7c20 494f 5b22 6279 7465  : str | IO["byte
-0000ae10: 7322 5d2c 0a20 2020 2020 2020 202a 2c0a  s"],.        *,.
-0000ae20: 2020 2020 2020 2020 7365 703a 204f 7074          sep: Opt
-0000ae30: 696f 6e61 6c5b 7374 725d 203d 2022 2c22  ional[str] = ","
-0000ae40: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-0000ae50: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0000ae60: 3d20 302c 0a20 2020 2020 2020 206e 616d  = 0,.        nam
-0000ae70: 6573 3a20 4f70 7469 6f6e 616c 5b0a 2020  es: Optional[.  
-0000ae80: 2020 2020 2020 2020 2020 556e 696f 6e5b            Union[
-0000ae90: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
-0000aea0: 416e 795d 2c20 6e70 2e6e 6461 7272 6179  Any], np.ndarray
-0000aeb0: 5b41 6e79 2c20 416e 795d 2c20 5475 706c  [Any, Any], Tupl
-0000aec0: 655b 416e 792c 202e 2e2e 5d2c 2072 616e  e[Any, ...], ran
-0000aed0: 6765 5d0a 2020 2020 2020 2020 5d20 3d20  ge].        ] = 
-0000aee0: 4e6f 6e65 2c0a 2020 2020 2020 2020 696e  None,.        in
-0000aef0: 6465 785f 636f 6c3a 204f 7074 696f 6e61  dex_col: Optiona
-0000af00: 6c5b 0a20 2020 2020 2020 2020 2020 2055  l[.            U
-0000af10: 6e69 6f6e 5b69 6e74 2c20 7374 722c 2053  nion[int, str, S
-0000af20: 6571 7565 6e63 655b 556e 696f 6e5b 7374  equence[Union[st
-0000af30: 722c 2069 6e74 5d5d 2c20 4c69 7465 7261  r, int]], Litera
-0000af40: 6c5b 4661 6c73 655d 5d0a 2020 2020 2020  l[False]].      
-0000af50: 2020 5d20 3d20 4e6f 6e65 2c0a 2020 2020    ] = None,.    
-0000af60: 2020 2020 7573 6563 6f6c 733a 204f 7074      usecols: Opt
-0000af70: 696f 6e61 6c5b 0a20 2020 2020 2020 2020  ional[.         
-0000af80: 2020 2055 6e69 6f6e 5b0a 2020 2020 2020     Union[.      
-0000af90: 2020 2020 2020 2020 2020 4d75 7461 626c            Mutabl
-0000afa0: 6553 6571 7565 6e63 655b 7374 725d 2c0a  eSequence[str],.
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 5475 706c 655b 7374 722c 202e 2e2e 5d2c  Tuple[str, ...],
-0000afd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000afe0: 2053 6571 7565 6e63 655b 696e 745d 2c0a   Sequence[int],.
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b000: 7061 6e64 6173 2e53 6572 6965 732c 0a20  pandas.Series,. 
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000b020: 616e 6461 732e 496e 6465 782c 0a20 2020  andas.Index,.   
-0000b030: 2020 2020 2020 2020 2020 2020 206e 702e               np.
-0000b040: 6e64 6172 7261 795b 416e 792c 2041 6e79  ndarray[Any, Any
-0000b050: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000b060: 2020 2043 616c 6c61 626c 655b 5b41 6e79     Callable[[Any
-0000b070: 5d2c 2062 6f6f 6c5d 2c0a 2020 2020 2020  ], bool],.      
-0000b080: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-0000b090: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000b0a0: 2020 6474 7970 653a 204f 7074 696f 6e61    dtype: Optiona
-0000b0b0: 6c5b 4469 6374 5d20 3d20 4e6f 6e65 2c0a  l[Dict] = None,.
-0000b0c0: 2020 2020 2020 2020 656e 6769 6e65 3a20          engine: 
-0000b0d0: 4f70 7469 6f6e 616c 5b0a 2020 2020 2020  Optional[.      
-0000b0e0: 2020 2020 2020 4c69 7465 7261 6c5b 2263        Literal["c
-0000b0f0: 222c 2022 7079 7468 6f6e 222c 2022 7079  ", "python", "py
-0000b100: 6172 726f 7722 2c20 2270 7974 686f 6e2d  arrow", "python-
-0000b110: 6677 6622 2c20 2262 6967 7175 6572 7922  fwf", "bigquery"
-0000b120: 5d0a 2020 2020 2020 2020 5d20 3d20 4e6f  ].        ] = No
-0000b130: 6e65 2c0a 2020 2020 2020 2020 656e 636f  ne,.        enco
-0000b140: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
-0000b150: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0000b160: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
-0000b170: 2020 2920 2d3e 2064 6174 6166 7261 6d65    ) -> dataframe
-0000b180: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
-0000b190: 2020 2020 7461 626c 6520 3d20 6269 6766      table = bigf
-0000b1a0: 7261 6d65 735f 696f 2e72 616e 646f 6d5f  rames_io.random_
-0000b1b0: 7461 626c 6528 7365 6c66 2e5f 616e 6f6e  table(self._anon
-0000b1c0: 796d 6f75 735f 6461 7461 7365 7429 0a0a  ymous_dataset)..
-0000b1d0: 2020 2020 2020 2020 6966 2065 6e67 696e          if engin
-0000b1e0: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-0000b1f0: 6420 656e 6769 6e65 203d 3d20 2262 6967  d engine == "big
-0000b200: 7175 6572 7922 3a0a 2020 2020 2020 2020  query":.        
-0000b210: 2020 2020 6966 2061 6e79 2870 6172 616d      if any(param
-0000b220: 2069 7320 6e6f 7420 4e6f 6e65 2066 6f72   is not None for
-0000b230: 2070 6172 616d 2069 6e20 2864 7479 7065   param in (dtype
-0000b240: 2c20 6e61 6d65 7329 293a 0a20 2020 2020  , names)):.     
-0000b250: 2020 2020 2020 2020 2020 206e 6f74 5f73             not_s
-0000b260: 7570 706f 7274 6564 203d 2028 2264 7479  upported = ("dty
-0000b270: 7065 222c 2022 6e61 6d65 7322 290a 2020  pe", "names").  
-0000b280: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000b290: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-0000b2a0: 6564 4572 726f 7228 0a20 2020 2020 2020  edError(.       
-0000b2b0: 2020 2020 2020 2020 2020 2020 2066 2242               f"B
-0000b2c0: 6967 5175 6572 7920 656e 6769 6e65 2064  igQuery engine d
-0000b2d0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-0000b2e0: 7468 6573 6520 6172 6775 6d65 6e74 733a  these arguments:
-0000b2f0: 207b 6e6f 745f 7375 7070 6f72 7465 647d   {not_supported}
-0000b300: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-0000b310: 2020 2020 2020 2020 6622 7b63 6f6e 7374          f"{const
-0000b320: 616e 7473 2e46 4545 4442 4143 4b5f 4c49  ants.FEEDBACK_LI
-0000b330: 4e4b 7d22 0a20 2020 2020 2020 2020 2020  NK}".           
-0000b340: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b350: 2020 2020 6966 2069 6e64 6578 5f63 6f6c      if index_col
-0000b360: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000b370: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000b380: 2020 206e 6f74 2069 6e64 6578 5f63 6f6c     not index_col
-0000b390: 206f 7220 6e6f 7420 6973 696e 7374 616e   or not isinstan
-0000b3a0: 6365 2869 6e64 6578 5f63 6f6c 2c20 7374  ce(index_col, st
-0000b3b0: 7229 0a20 2020 2020 2020 2020 2020 2029  r).            )
-0000b3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b3d0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000b3e0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2022 4269 6751 7565 7279 2065 6e67 696e   "BigQuery engin
-0000b410: 6520 6f6e 6c79 2073 7570 706f 7274 7320  e only supports 
-0000b420: 6120 7369 6e67 6c65 2063 6f6c 756d 6e20  a single column 
-0000b430: 6e61 6d65 2066 6f72 2060 696e 6465 785f  name for `index_
-0000b440: 636f 6c60 2e20 220a 2020 2020 2020 2020  col`. ".        
-0000b450: 2020 2020 2020 2020 2020 2020 6622 7b63              f"{c
-0000b460: 6f6e 7374 616e 7473 2e46 4545 4442 4143  onstants.FEEDBAC
-0000b470: 4b5f 4c49 4e4b 7d22 0a20 2020 2020 2020  K_LINK}".       
-0000b480: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000b490: 2020 2020 2020 2020 2320 4e6f 6e65 2076          # None v
-0000b4a0: 616c 7565 2066 6f72 2069 6e64 6578 5f63  alue for index_c
-0000b4b0: 6f6c 2063 616e 6e6f 7420 6265 2070 6173  ol cannot be pas
-0000b4c0: 7365 6420 746f 2072 6561 645f 6762 710a  sed to read_gbq.
-0000b4d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000b4e0: 6e64 6578 5f63 6f6c 2069 7320 4e6f 6e65  ndex_col is None
-0000b4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b500: 2020 696e 6465 785f 636f 6c20 3d20 2829    index_col = ()
-0000b510: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000b520: 7573 6563 6f6c 7320 7368 6f75 6c64 206f  usecols should o
-0000b530: 6e6c 7920 6265 2061 6e20 6974 6572 6162  nly be an iterab
-0000b540: 6c65 206f 6620 7374 7269 6e67 7320 2863  le of strings (c
-0000b550: 6f6c 756d 6e20 6e61 6d65 7329 2066 6f72  olumn names) for
-0000b560: 2075 7365 2061 7320 636f 6c75 6d6e 7320   use as columns 
-0000b570: 696e 2072 6561 645f 6762 712e 0a20 2020  in read_gbq..   
-0000b580: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-0000b590: 3a20 5475 706c 655b 416e 792c 202e 2e2e  : Tuple[Any, ...
-0000b5a0: 5d20 3d20 7475 706c 6528 290a 2020 2020  ] = tuple().    
-0000b5b0: 2020 2020 2020 2020 6966 2075 7365 636f          if useco
-0000b5c0: 6c73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ls is not None:.
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 6966 2069 7369 6e73 7461 6e63 6528 7573  if isinstance(us
-0000b5f0: 6563 6f6c 732c 2049 7465 7261 626c 6529  ecols, Iterable)
-0000b600: 2061 6e64 2061 6c6c 280a 2020 2020 2020   and all(.      
-0000b610: 2020 2020 2020 2020 2020 2020 2020 6973                is
-0000b620: 696e 7374 616e 6365 2863 6f6c 2c20 7374  instance(col, st
-0000b630: 7229 2066 6f72 2063 6f6c 2069 6e20 7573  r) for col in us
-0000b640: 6563 6f6c 730a 2020 2020 2020 2020 2020  ecols.          
-0000b650: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-0000b660: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0000b670: 756d 6e73 203d 2074 7570 6c65 2863 6f6c  umns = tuple(col
-0000b680: 2066 6f72 2063 6f6c 2069 6e20 7573 6563   for col in usec
-0000b690: 6f6c 7329 0a20 2020 2020 2020 2020 2020  ols).           
-0000b6a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b6c0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000b6d0: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 2242 6967 5175 6572 7920 656e 6769    "BigQuery engi
-0000b700: 6e65 206f 6e6c 7920 7375 7070 6f72 7473  ne only supports
-0000b710: 2061 6e20 6974 6572 6162 6c65 206f 6620   an iterable of 
-0000b720: 7374 7269 6e67 7320 666f 7220 6075 7365  strings for `use
-0000b730: 636f 6c73 602e 2022 0a20 2020 2020 2020  cols`. ".       
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2066 227b 636f 6e73 7461 6e74 732e 4645   f"{constants.FE
-0000b760: 4544 4241 434b 5f4c 494e 4b7d 220a 2020  EDBACK_LINK}".  
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-0000b790: 2069 6620 656e 636f 6469 6e67 2069 7320   if encoding is 
-0000b7a0: 6e6f 7420 4e6f 6e65 2061 6e64 2065 6e63  not None and enc
-0000b7b0: 6f64 696e 6720 6e6f 7420 696e 205f 5641  oding not in _VA
-0000b7c0: 4c49 445f 454e 434f 4449 4e47 533a 0a20  LID_ENCODINGS:. 
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b7e0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000b7f0: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
-0000b800: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000b810: 4269 6751 7565 7279 2065 6e67 696e 6520  BigQuery engine 
-0000b820: 6f6e 6c79 2073 7570 706f 7274 7320 7468  only supports th
-0000b830: 6520 666f 6c6c 6f77 696e 6720 656e 636f  e following enco
-0000b840: 6469 6e67 733a 207b 5f56 414c 4944 5f45  dings: {_VALID_E
-0000b850: 4e43 4f44 494e 4753 7d2e 2022 0a20 2020  NCODINGS}. ".   
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 2066 227b 636f 6e73 7461 6e74 732e 4645   f"{constants.FE
-0000b880: 4544 4241 434b 5f4c 494e 4b7d 220a 2020  EDBACK_LINK}".  
-0000b890: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000b8a0: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000b8b0: 5f63 6f6e 6669 6720 3d20 7365 6c66 2e5f  _config = self._
-0000b8c0: 7072 6570 6172 655f 6c6f 6164 5f6a 6f62  prepare_load_job
-0000b8d0: 5f63 6f6e 6669 6728 290a 2020 2020 2020  _config().      
-0000b8e0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-0000b8f0: 2e63 7265 6174 655f 6469 7370 6f73 6974  .create_disposit
-0000b900: 696f 6e20 3d20 6269 6771 7565 7279 2e43  ion = bigquery.C
-0000b910: 7265 6174 6544 6973 706f 7369 7469 6f6e  reateDisposition
-0000b920: 2e43 5245 4154 455f 4946 5f4e 4545 4445  .CREATE_IF_NEEDE
-0000b930: 440a 2020 2020 2020 2020 2020 2020 6a6f  D.            jo
-0000b940: 625f 636f 6e66 6967 2e73 6f75 7263 655f  b_config.source_
-0000b950: 666f 726d 6174 203d 2062 6967 7175 6572  format = bigquer
-0000b960: 792e 536f 7572 6365 466f 726d 6174 2e43  y.SourceFormat.C
-0000b970: 5356 0a20 2020 2020 2020 2020 2020 206a  SV.            j
-0000b980: 6f62 5f63 6f6e 6669 672e 7772 6974 655f  ob_config.write_
-0000b990: 6469 7370 6f73 6974 696f 6e20 3d20 6269  disposition = bi
-0000b9a0: 6771 7565 7279 2e57 7269 7465 4469 7370  gquery.WriteDisp
-0000b9b0: 6f73 6974 696f 6e2e 5752 4954 455f 454d  osition.WRITE_EM
-0000b9c0: 5054 590a 2020 2020 2020 2020 2020 2020  PTY.            
-0000b9d0: 6a6f 625f 636f 6e66 6967 2e61 7574 6f64  job_config.autod
-0000b9e0: 6574 6563 7420 3d20 5472 7565 0a20 2020  etect = True.   
-0000b9f0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000ba00: 6669 672e 6669 656c 645f 6465 6c69 6d69  fig.field_delimi
-0000ba10: 7465 7220 3d20 7365 700a 2020 2020 2020  ter = sep.      
-0000ba20: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-0000ba30: 2e65 6e63 6f64 696e 6720 3d20 656e 636f  .encoding = enco
-0000ba40: 6469 6e67 0a20 2020 2020 2020 2020 2020  ding.           
-0000ba50: 206a 6f62 5f63 6f6e 6669 672e 6c61 6265   job_config.labe
-0000ba60: 6c73 203d 207b 2262 6967 6672 616d 6573  ls = {"bigframes
-0000ba70: 2d61 7069 223a 2022 7265 6164 5f63 7376  -api": "read_csv
-0000ba80: 227d 0a0a 2020 2020 2020 2020 2020 2020  "}..            
-0000ba90: 2320 5765 2077 616e 7420 746f 206d 6174  # We want to mat
-0000baa0: 6368 2070 616e 6461 7320 6265 6861 7669  ch pandas behavi
-0000bab0: 6f72 2e20 4966 2068 6561 6465 7220 6973  or. If header is
-0000bac0: 2030 2c20 6e6f 2072 6f77 7320 7368 6f75   0, no rows shou
-0000bad0: 6c64 2062 6520 736b 6970 7065 642c 2073  ld be skipped, s
-0000bae0: 6f20 7765 0a20 2020 2020 2020 2020 2020  o we.           
-0000baf0: 2023 2064 6f20 6e6f 7420 6e65 6564 2074   # do not need t
-0000bb00: 6f20 7365 7420 6073 6b69 705f 6c65 6164  o set `skip_lead
-0000bb10: 696e 675f 726f 7773 602e 2049 6620 6865  ing_rows`. If he
-0000bb20: 6164 6572 2069 7320 4e6f 6e65 2c20 7468  ader is None, th
-0000bb30: 656e 2074 6865 7265 2069 7320 6e6f 2068  en there is no h
-0000bb40: 6561 6465 722e 0a20 2020 2020 2020 2020  eader..         
-0000bb50: 2020 2023 2053 6574 7469 6e67 2073 6b69     # Setting ski
-0000bb60: 705f 6c65 6164 696e 675f 726f 7773 2074  p_leading_rows t
-0000bb70: 6f20 3020 646f 6573 2074 6861 742e 2049  o 0 does that. I
-0000bb80: 6620 6865 6164 6572 3d4e 2061 6e64 204e  f header=N and N
-0000bb90: 3e30 2c20 7765 2077 616e 7420 746f 2073  >0, we want to s
-0000bba0: 6b69 7020 4e20 726f 7773 2e0a 2020 2020  kip N rows..    
-0000bbb0: 2020 2020 2020 2020 6966 2068 6561 6465          if heade
-0000bbc0: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-0000bbd0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000bbe0: 6f6e 6669 672e 736b 6970 5f6c 6561 6469  onfig.skip_leadi
-0000bbf0: 6e67 5f72 6f77 7320 3d20 300a 2020 2020  ng_rows = 0.    
-0000bc00: 2020 2020 2020 2020 656c 6966 2068 6561          elif hea
-0000bc10: 6465 7220 3e20 303a 0a20 2020 2020 2020  der > 0:.       
-0000bc20: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000bc30: 6669 672e 736b 6970 5f6c 6561 6469 6e67  fig.skip_leading
-0000bc40: 5f72 6f77 7320 3d20 6865 6164 6572 0a0a  _rows = header..
-0000bc50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000bc60: 726e 2073 656c 662e 5f72 6561 645f 6269  rn self._read_bi
-0000bc70: 6771 7565 7279 5f6c 6f61 645f 6a6f 6228  gquery_load_job(
-0000bc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc90: 2066 696c 6570 6174 685f 6f72 5f62 7566   filepath_or_buf
-0000bca0: 6665 722c 0a20 2020 2020 2020 2020 2020  fer,.           
-0000bcb0: 2020 2020 2074 6162 6c65 2c0a 2020 2020       table,.    
-0000bcc0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000bcd0: 636f 6e66 6967 3d6a 6f62 5f63 6f6e 6669  config=job_confi
-0000bce0: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
-0000bcf0: 2020 2069 6e64 6578 5f63 6f6c 3d69 6e64     index_col=ind
-0000bd00: 6578 5f63 6f6c 2c0a 2020 2020 2020 2020  ex_col,.        
-0000bd10: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-0000bd20: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
-0000bd30: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-0000bd40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000bd50: 2069 6620 616e 7928 6172 6720 696e 206b   if any(arg in k
-0000bd60: 7761 7267 7320 666f 7220 6172 6720 696e  wargs for arg in
-0000bd70: 2028 2263 6875 6e6b 7369 7a65 222c 2022   ("chunksize", "
-0000bd80: 6974 6572 6174 6f72 2229 293a 0a20 2020  iterator")):.   
-0000bd90: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000bda0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-0000bdb0: 6445 7272 6f72 280a 2020 2020 2020 2020  dError(.        
-0000bdc0: 2020 2020 2020 2020 2020 2020 2227 6368              "'ch
-0000bdd0: 756e 6b73 697a 6527 2061 6e64 2027 6974  unksize' and 'it
-0000bde0: 6572 6174 6f72 2720 6172 6775 6d65 6e74  erator' argument
-0000bdf0: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
-0000be00: 7465 642e 2022 0a20 2020 2020 2020 2020  ted. ".         
-0000be10: 2020 2020 2020 2020 2020 2066 227b 636f             f"{co
-0000be20: 6e73 7461 6e74 732e 4645 4544 4241 434b  nstants.FEEDBACK
-0000be30: 5f4c 494e 4b7d 220a 2020 2020 2020 2020  _LINK}".        
-0000be40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000be50: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0000be60: 616e 6365 2866 696c 6570 6174 685f 6f72  ance(filepath_or
-0000be70: 5f62 7566 6665 722c 2073 7472 293a 0a20  _buffer, str):. 
-0000be80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000be90: 656c 662e 5f63 6865 636b 5f66 696c 655f  elf._check_file_
-0000bea0: 7369 7a65 2866 696c 6570 6174 685f 6f72  size(filepath_or
-0000beb0: 5f62 7566 6665 7229 0a20 2020 2020 2020  _buffer).       
-0000bec0: 2020 2020 2070 616e 6461 735f 6466 203d       pandas_df =
-0000bed0: 2070 616e 6461 732e 7265 6164 5f63 7376   pandas.read_csv
-0000bee0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000bef0: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
-0000bf00: 6666 6572 2c0a 2020 2020 2020 2020 2020  ffer,.          
-0000bf10: 2020 2020 2020 7365 703d 7365 702c 0a20        sep=sep,. 
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000bf30: 6561 6465 723d 6865 6164 6572 2c0a 2020  eader=header,.  
-0000bf40: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0000bf50: 6d65 733d 6e61 6d65 732c 0a20 2020 2020  mes=names,.     
-0000bf60: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-0000bf70: 5f63 6f6c 3d69 6e64 6578 5f63 6f6c 2c0a  _col=index_col,.
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 7573 6563 6f6c 733d 7573 6563 6f6c 732c  usecols=usecols,
-0000bfa0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-0000bfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bfc0: 2064 7479 7065 3d64 7479 7065 2c0a 2020   dtype=dtype,.  
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000bfe0: 6769 6e65 3d65 6e67 696e 652c 0a20 2020  gine=engine,.   
-0000bff0: 2020 2020 2020 2020 2020 2020 2065 6e63               enc
-0000c000: 6f64 696e 673d 656e 636f 6469 6e67 2c0a  oding=encoding,.
-0000c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c020: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
-0000c030: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000c040: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000c050: 5f72 6561 645f 7061 6e64 6173 2870 616e  _read_pandas(pan
-0000c060: 6461 735f 6466 2c20 2272 6561 645f 6373  das_df, "read_cs
-0000c070: 7622 2920 2023 2074 7970 653a 2069 676e  v")  # type: ign
-0000c080: 6f72 650a 0a20 2020 2064 6566 2072 6561  ore..    def rea
-0000c090: 645f 7069 636b 6c65 280a 2020 2020 2020  d_pickle(.      
-0000c0a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000c0b0: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
-0000c0c0: 6572 3a20 4669 6c65 5061 7468 207c 2052  er: FilePath | R
-0000c0d0: 6561 6450 6963 6b6c 6542 7566 6665 722c  eadPickleBuffer,
-0000c0e0: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
-0000c0f0: 7369 6f6e 3a20 436f 6d70 7265 7373 696f  sion: Compressio
-0000c100: 6e4f 7074 696f 6e73 203d 2022 696e 6665  nOptions = "infe
-0000c110: 7222 2c0a 2020 2020 2020 2020 7374 6f72  r",.        stor
-0000c120: 6167 655f 6f70 7469 6f6e 733a 2053 746f  age_options: Sto
-0000c130: 7261 6765 4f70 7469 6f6e 7320 3d20 4e6f  rageOptions = No
-0000c140: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0000c150: 2020 2070 616e 6461 735f 6f62 6a20 3d20     pandas_obj = 
-0000c160: 7061 6e64 6173 2e72 6561 645f 7069 636b  pandas.read_pick
-0000c170: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-0000c180: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
-0000c190: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-0000c1a0: 636f 6d70 7265 7373 696f 6e3d 636f 6d70  compression=comp
-0000c1b0: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
-0000c1c0: 2020 2020 2073 746f 7261 6765 5f6f 7074       storage_opt
-0000c1d0: 696f 6e73 3d73 746f 7261 6765 5f6f 7074  ions=storage_opt
-0000c1e0: 696f 6e73 2c0a 2020 2020 2020 2020 290a  ions,.        ).
-0000c1f0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000c200: 7374 616e 6365 2870 616e 6461 735f 6f62  stance(pandas_ob
-0000c210: 6a2c 2070 616e 6461 732e 5365 7269 6573  j, pandas.Series
-0000c220: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-0000c230: 6620 7061 6e64 6173 5f6f 626a 2e6e 616d  f pandas_obj.nam
-0000c240: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-0000c250: 2020 2020 2020 2020 2020 2070 616e 6461             panda
-0000c260: 735f 6f62 6a2e 6e61 6d65 203d 2022 3022  s_obj.name = "0"
-0000c270: 0a20 2020 2020 2020 2020 2020 2062 6967  .            big
-0000c280: 6672 616d 6573 5f64 6620 3d20 7365 6c66  frames_df = self
-0000c290: 2e5f 7265 6164 5f70 616e 6461 7328 7061  ._read_pandas(pa
-0000c2a0: 6e64 6173 5f6f 626a 2e74 6f5f 6672 616d  ndas_obj.to_fram
-0000c2b0: 6528 292c 2022 7265 6164 5f70 6963 6b6c  e(), "read_pickl
-0000c2c0: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
-0000c2d0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
-0000c2e0: 5f64 665b 6269 6766 7261 6d65 735f 6466  _df[bigframes_df
-0000c2f0: 2e63 6f6c 756d 6e73 5b30 5d5d 0a20 2020  .columns[0]].   
-0000c300: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c310: 2e5f 7265 6164 5f70 616e 6461 7328 7061  ._read_pandas(pa
-0000c320: 6e64 6173 5f6f 626a 2c20 2272 6561 645f  ndas_obj, "read_
-0000c330: 7069 636b 6c65 2229 0a0a 2020 2020 6465  pickle")..    de
-0000c340: 6620 7265 6164 5f70 6172 7175 6574 280a  f read_parquet(.
-0000c350: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000c360: 2020 2020 2020 7061 7468 3a20 7374 7220        path: str 
-0000c370: 7c20 494f 5b22 6279 7465 7322 5d2c 0a20  | IO["bytes"],. 
-0000c380: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-0000c390: 2020 656e 6769 6e65 3a20 7374 7220 3d20    engine: str = 
-0000c3a0: 2261 7574 6f22 2c0a 2020 2020 2920 2d3e  "auto",.    ) ->
-0000c3b0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
-0000c3c0: 7261 6d65 3a0a 2020 2020 2020 2020 7461  rame:.        ta
-0000c3d0: 626c 6520 3d20 6269 6766 7261 6d65 735f  ble = bigframes_
-0000c3e0: 696f 2e72 616e 646f 6d5f 7461 626c 6528  io.random_table(
-0000c3f0: 7365 6c66 2e5f 616e 6f6e 796d 6f75 735f  self._anonymous_
-0000c400: 6461 7461 7365 7429 0a0a 2020 2020 2020  dataset)..      
-0000c410: 2020 6966 2065 6e67 696e 6520 3d3d 2022    if engine == "
-0000c420: 6269 6771 7565 7279 223a 0a20 2020 2020  bigquery":.     
-0000c430: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-0000c440: 6720 3d20 7365 6c66 2e5f 7072 6570 6172  g = self._prepar
-0000c450: 655f 6c6f 6164 5f6a 6f62 5f63 6f6e 6669  e_load_job_confi
-0000c460: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
-0000c470: 6a6f 625f 636f 6e66 6967 2e63 7265 6174  job_config.creat
-0000c480: 655f 6469 7370 6f73 6974 696f 6e20 3d20  e_disposition = 
-0000c490: 6269 6771 7565 7279 2e43 7265 6174 6544  bigquery.CreateD
-0000c4a0: 6973 706f 7369 7469 6f6e 2e43 5245 4154  isposition.CREAT
-0000c4b0: 455f 4946 5f4e 4545 4445 440a 2020 2020  E_IF_NEEDED.    
-0000c4c0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000c4d0: 6967 2e73 6f75 7263 655f 666f 726d 6174  ig.source_format
-0000c4e0: 203d 2062 6967 7175 6572 792e 536f 7572   = bigquery.Sour
-0000c4f0: 6365 466f 726d 6174 2e50 4152 5155 4554  ceFormat.PARQUET
-0000c500: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000c510: 5f63 6f6e 6669 672e 7772 6974 655f 6469  _config.write_di
-0000c520: 7370 6f73 6974 696f 6e20 3d20 6269 6771  sposition = bigq
-0000c530: 7565 7279 2e57 7269 7465 4469 7370 6f73  uery.WriteDispos
-0000c540: 6974 696f 6e2e 5752 4954 455f 454d 5054  ition.WRITE_EMPT
-0000c550: 590a 2020 2020 2020 2020 2020 2020 6a6f  Y.            jo
-0000c560: 625f 636f 6e66 6967 2e6c 6162 656c 7320  b_config.labels 
-0000c570: 3d20 7b22 6269 6766 7261 6d65 732d 6170  = {"bigframes-ap
-0000c580: 6922 3a20 2272 6561 645f 7061 7271 7565  i": "read_parque
-0000c590: 7422 7d0a 0a20 2020 2020 2020 2020 2020  t"}..           
-0000c5a0: 2072 6574 7572 6e20 7365 6c66 2e5f 7265   return self._re
-0000c5b0: 6164 5f62 6967 7175 6572 795f 6c6f 6164  ad_bigquery_load
-0000c5c0: 5f6a 6f62 2870 6174 682c 2074 6162 6c65  _job(path, table
-0000c5d0: 2c20 6a6f 625f 636f 6e66 6967 3d6a 6f62  , job_config=job
-0000c5e0: 5f63 6f6e 6669 6729 0a20 2020 2020 2020  _config).       
-0000c5f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000c600: 2020 2072 6561 645f 7061 7271 7565 745f     read_parquet_
-0000c610: 6b77 6172 6773 3a20 4469 6374 5b73 7472  kwargs: Dict[str
-0000c620: 2c20 416e 795d 203d 207b 7d0a 2020 2020  , Any] = {}.    
-0000c630: 2020 2020 2020 2020 6966 2070 616e 6461          if panda
-0000c640: 732e 5f5f 7665 7273 696f 6e5f 5f2e 7374  s.__version__.st
-0000c650: 6172 7473 7769 7468 2822 312e 2229 3a0a  artswith("1."):.
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c670: 7265 6164 5f70 6172 7175 6574 5f6b 7761  read_parquet_kwa
-0000c680: 7267 735b 2275 7365 5f6e 756c 6c61 626c  rgs["use_nullabl
-0000c690: 655f 6474 7970 6573 225d 203d 2054 7275  e_dtypes"] = Tru
-0000c6a0: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
-0000c6b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000c6c0: 2020 2020 7265 6164 5f70 6172 7175 6574      read_parquet
-0000c6d0: 5f6b 7761 7267 735b 2264 7479 7065 5f62  _kwargs["dtype_b
-0000c6e0: 6163 6b65 6e64 225d 203d 2022 7079 6172  ackend"] = "pyar
-0000c6f0: 726f 7722 0a0a 2020 2020 2020 2020 2020  row"..          
-0000c700: 2020 7061 6e64 6173 5f6f 626a 203d 2070    pandas_obj = p
-0000c710: 616e 6461 732e 7265 6164 5f70 6172 7175  andas.read_parqu
-0000c720: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0000c730: 2020 2020 7061 7468 2c0a 2020 2020 2020      path,.      
-0000c740: 2020 2020 2020 2020 2020 656e 6769 6e65            engine
-0000c750: 3d65 6e67 696e 652c 2020 2320 7479 7065  =engine,  # type
-0000c760: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-0000c770: 2020 2020 2020 2020 202a 2a72 6561 645f           **read_
-0000c780: 7061 7271 7565 745f 6b77 6172 6773 2c0a  parquet_kwargs,.
-0000c790: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000c7a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c7b0: 2073 656c 662e 5f72 6561 645f 7061 6e64   self._read_pand
-0000c7c0: 6173 2870 616e 6461 735f 6f62 6a2c 2022  as(pandas_obj, "
-0000c7d0: 7265 6164 5f70 6172 7175 6574 2229 0a0a  read_parquet")..
-0000c7e0: 2020 2020 6465 6620 7265 6164 5f6a 736f      def read_jso
-0000c7f0: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
-0000c800: 0a20 2020 2020 2020 2070 6174 685f 6f72  .        path_or
-0000c810: 5f62 7566 3a20 7374 7220 7c20 494f 5b22  _buf: str | IO["
-0000c820: 6279 7465 7322 5d2c 0a20 2020 2020 2020  bytes"],.       
-0000c830: 202a 2c0a 2020 2020 2020 2020 6f72 6965   *,.        orie
-0000c840: 6e74 3a20 4c69 7465 7261 6c5b 0a20 2020  nt: Literal[.   
-0000c850: 2020 2020 2020 2020 2022 7370 6c69 7422           "split"
-0000c860: 2c20 2272 6563 6f72 6473 222c 2022 696e  , "records", "in
-0000c870: 6465 7822 2c20 2263 6f6c 756d 6e73 222c  dex", "columns",
-0000c880: 2022 7661 6c75 6573 222c 2022 7461 626c   "values", "tabl
-0000c890: 6522 0a20 2020 2020 2020 205d 203d 2022  e".        ] = "
-0000c8a0: 636f 6c75 6d6e 7322 2c0a 2020 2020 2020  columns",.      
-0000c8b0: 2020 6474 7970 653a 204f 7074 696f 6e61    dtype: Optiona
-0000c8c0: 6c5b 4469 6374 5d20 3d20 4e6f 6e65 2c0a  l[Dict] = None,.
-0000c8d0: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
-0000c8e0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000c8f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000c900: 6c69 6e65 733a 2062 6f6f 6c20 3d20 4661  lines: bool = Fa
-0000c910: 6c73 652c 0a20 2020 2020 2020 2065 6e67  lse,.        eng
-0000c920: 696e 653a 204c 6974 6572 616c 5b22 756a  ine: Literal["uj
-0000c930: 736f 6e22 2c20 2270 7961 7272 6f77 222c  son", "pyarrow",
-0000c940: 2022 6269 6771 7565 7279 225d 203d 2022   "bigquery"] = "
-0000c950: 756a 736f 6e22 2c0a 2020 2020 2020 2020  ujson",.        
-0000c960: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
-0000c970: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
-0000c980: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
-0000c990: 7461 626c 6520 3d20 6269 6766 7261 6d65  table = bigframe
-0000c9a0: 735f 696f 2e72 616e 646f 6d5f 7461 626c  s_io.random_tabl
-0000c9b0: 6528 7365 6c66 2e5f 616e 6f6e 796d 6f75  e(self._anonymou
-0000c9c0: 735f 6461 7461 7365 7429 0a0a 2020 2020  s_dataset)..    
-0000c9d0: 2020 2020 6966 2065 6e67 696e 6520 3d3d      if engine ==
-0000c9e0: 2022 6269 6771 7565 7279 223a 0a0a 2020   "bigquery":..  
-0000c9f0: 2020 2020 2020 2020 2020 6966 2064 7479            if dty
-0000ca00: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca20: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-0000ca30: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000ca50: 4269 6751 7565 7279 2065 6e67 696e 6520  BigQuery engine 
-0000ca60: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
-0000ca70: 2074 6865 2064 7479 7065 2061 7267 756d   the dtype argum
-0000ca80: 656e 7473 2e22 0a20 2020 2020 2020 2020  ents.".         
-0000ca90: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000caa0: 2020 2020 2020 6966 206e 6f74 206c 696e        if not lin
-0000cab0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000cac0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000cad0: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caf0: 2020 2022 4f6e 6c79 206e 6577 6c69 6e65     "Only newline
-0000cb00: 2064 656c 696d 6974 6564 204a 534f 4e20   delimited JSON 
-0000cb10: 666f 726d 6174 2069 7320 7375 7070 6f72  format is suppor
-0000cb20: 7465 642e 220a 2020 2020 2020 2020 2020  ted.".          
-0000cb30: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000cb40: 2020 2020 2069 6620 656e 636f 6469 6e67       if encoding
-0000cb50: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000cb60: 2065 6e63 6f64 696e 6720 6e6f 7420 696e   encoding not in
-0000cb70: 205f 5641 4c49 445f 454e 434f 4449 4e47   _VALID_ENCODING
-0000cb80: 533a 0a20 2020 2020 2020 2020 2020 2020  S:.             
-0000cb90: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-0000cba0: 656d 656e 7465 6445 7272 6f72 280a 2020  ementedError(.  
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbc0: 2020 6622 4269 6751 7565 7279 2065 6e67    f"BigQuery eng
-0000cbd0: 696e 6520 6f6e 6c79 2073 7570 706f 7274  ine only support
-0000cbe0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
-0000cbf0: 656e 636f 6469 6e67 733a 207b 5f56 414c  encodings: {_VAL
-0000cc00: 4944 5f45 4e43 4f44 494e 4753 7d22 0a20  ID_ENCODINGS}". 
-0000cc10: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000cc20: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000cc30: 206c 696e 6573 2061 6e64 206f 7269 656e   lines and orien
-0000cc40: 7420 213d 2022 7265 636f 7264 7322 3a0a  t != "records":.
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc60: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000cc70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000cc80: 2020 2020 2020 2227 6c69 6e65 7327 206b        "'lines' k
-0000cc90: 6579 776f 7264 2069 7320 6f6e 6c79 2076  eyword is only v
-0000cca0: 616c 6964 2077 6865 6e20 276f 7269 656e  alid when 'orien
-0000ccb0: 7427 2069 7320 2772 6563 6f72 6473 272e  t' is 'records'.
-0000ccc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000ccd0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-0000cce0: 206a 6f62 5f63 6f6e 6669 6720 3d20 7365   job_config = se
-0000ccf0: 6c66 2e5f 7072 6570 6172 655f 6c6f 6164  lf._prepare_load
-0000cd00: 5f6a 6f62 5f63 6f6e 6669 6728 290a 2020  _job_config().  
-0000cd10: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-0000cd20: 6e66 6967 2e63 7265 6174 655f 6469 7370  nfig.create_disp
-0000cd30: 6f73 6974 696f 6e20 3d20 6269 6771 7565  osition = bigque
-0000cd40: 7279 2e43 7265 6174 6544 6973 706f 7369  ry.CreateDisposi
-0000cd50: 7469 6f6e 2e43 5245 4154 455f 4946 5f4e  tion.CREATE_IF_N
-0000cd60: 4545 4445 440a 2020 2020 2020 2020 2020  EEDED.          
-0000cd70: 2020 6a6f 625f 636f 6e66 6967 2e73 6f75    job_config.sou
-0000cd80: 7263 655f 666f 726d 6174 203d 2062 6967  rce_format = big
-0000cd90: 7175 6572 792e 536f 7572 6365 466f 726d  query.SourceForm
-0000cda0: 6174 2e4e 4557 4c49 4e45 5f44 454c 494d  at.NEWLINE_DELIM
-0000cdb0: 4954 4544 5f4a 534f 4e0a 2020 2020 2020  ITED_JSON.      
-0000cdc0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-0000cdd0: 2e77 7269 7465 5f64 6973 706f 7369 7469  .write_dispositi
-0000cde0: 6f6e 203d 2062 6967 7175 6572 792e 5772  on = bigquery.Wr
-0000cdf0: 6974 6544 6973 706f 7369 7469 6f6e 2e57  iteDisposition.W
-0000ce00: 5249 5445 5f45 4d50 5459 0a20 2020 2020  RITE_EMPTY.     
-0000ce10: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-0000ce20: 672e 6175 746f 6465 7465 6374 203d 2054  g.autodetect = T
-0000ce30: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000ce40: 6a6f 625f 636f 6e66 6967 2e65 6e63 6f64  job_config.encod
-0000ce50: 696e 6720 3d20 656e 636f 6469 6e67 0a20  ing = encoding. 
-0000ce60: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000ce70: 6f6e 6669 672e 6c61 6265 6c73 203d 207b  onfig.labels = {
-0000ce80: 2262 6967 6672 616d 6573 2d61 7069 223a  "bigframes-api":
-0000ce90: 2022 7265 6164 5f6a 736f 6e22 7d0a 0a20   "read_json"}.. 
-0000cea0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ceb0: 6e20 7365 6c66 2e5f 7265 6164 5f62 6967  n self._read_big
-0000cec0: 7175 6572 795f 6c6f 6164 5f6a 6f62 280a  query_load_job(.
+00003860: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003870: 2020 2020 2020 2063 6f6c 756d 6e2c 206f         column, o
+00003880: 7065 7261 746f 722c 2076 616c 7565 203d  perator, value =
+00003890: 2066 696c 7465 725f 6974 656d 0a0a 2020   filter_item..  
+000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038b0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+000038c0: 6e63 6528 636f 6c75 6d6e 2c20 7374 7229  nce(column, str)
+000038d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000038e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000038f0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003910: 2020 2020 2020 2020 6622 436f 6c75 6d6e          f"Column
+00003920: 206e 616d 6520 7368 6f75 6c64 2062 6520   name should be 
+00003930: 6120 7374 7269 6e67 2c20 6275 7420 7265  a string, but re
+00003940: 6365 6976 6564 2027 7b63 6f6c 756d 6e7d  ceived '{column}
+00003950: 2720 6f66 2074 7970 6520 7b74 7970 6528  ' of type {type(
+00003960: 636f 6c75 6d6e 292e 5f5f 6e61 6d65 5f5f  column).__name__
+00003970: 7d2e 220a 2020 2020 2020 2020 2020 2020  }.".            
+00003980: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 2020 2069 6620 6f70 6572 6174 6f72 206e     if operator n
+000039b0: 6f74 2069 6e20 7661 6c69 645f 6f70 6572  ot in valid_oper
+000039c0: 6174 6f72 733a 0a20 2020 2020 2020 2020  ators:.         
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000039e0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000039f0: 6622 4f70 6572 6174 6f72 207b 6f70 6572  f"Operator {oper
+00003a00: 6174 6f72 7d20 6973 206e 6f74 2076 616c  ator} is not val
+00003a10: 6964 2e22 290a 0a20 2020 2020 2020 2020  id.")..         
+00003a20: 2020 2020 2020 2020 2020 206f 7065 7261             opera
+00003a30: 746f 725f 7374 7220 3d20 7661 6c69 645f  tor_str = valid_
+00003a40: 6f70 6572 6174 6f72 735b 6f70 6572 6174  operators[operat
+00003a50: 6f72 5d0a 0a20 2020 2020 2020 2020 2020  or]..           
+00003a60: 2020 2020 2020 2020 2069 6620 6f70 6572           if oper
+00003a70: 6174 6f72 5f73 7472 2069 6e20 5b22 494e  ator_str in ["IN
+00003a80: 222c 2022 4e4f 5420 494e 225d 3a0a 2020  ", "NOT IN"]:.  
+00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003aa0: 2020 2020 2020 7661 6c75 655f 6c69 7374        value_list
+00003ab0: 203d 2022 2c20 222e 6a6f 696e 285b 7265   = ", ".join([re
+00003ac0: 7072 2876 2920 666f 7220 7620 696e 2076  pr(v) for v in v
+00003ad0: 616c 7565 5d29 0a20 2020 2020 2020 2020  alue]).         
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003af0: 7870 7265 7373 696f 6e20 3d20 6622 607b  xpression = f"`{
+00003b00: 636f 6c75 6d6e 7d60 207b 6f70 6572 6174  column}` {operat
+00003b10: 6f72 5f73 7472 7d20 287b 7661 6c75 655f  or_str} ({value_
+00003b20: 6c69 7374 7d29 220a 2020 2020 2020 2020  list})".        
+00003b30: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003b50: 2020 2020 2020 2020 2020 6578 7072 6573            expres
+00003b60: 7369 6f6e 203d 2066 2260 7b63 6f6c 756d  sion = f"`{colum
+00003b70: 6e7d 6020 7b6f 7065 7261 746f 725f 7374  n}` {operator_st
+00003b80: 727d 207b 7265 7072 2876 616c 7565 297d  r} {repr(value)}
+00003b90: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00003ba0: 2020 2020 2020 616e 645f 6578 7072 6573        and_expres
+00003bb0: 7369 6f6e 732e 6170 7065 6e64 2865 7870  sions.append(exp
+00003bc0: 7265 7373 696f 6e29 0a0a 2020 2020 2020  ression)..      
+00003bd0: 2020 2020 2020 2020 2020 6f72 5f65 7870            or_exp
+00003be0: 7265 7373 696f 6e73 2e61 7070 656e 6428  ressions.append(
+00003bf0: 2220 414e 4420 222e 6a6f 696e 2861 6e64  " AND ".join(and
+00003c00: 5f65 7870 7265 7373 696f 6e73 2929 0a0a  _expressions))..
+00003c10: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00003c20: 725f 6578 7072 6573 7369 6f6e 733a 0a20  r_expressions:. 
+00003c30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00003c40: 6865 7265 5f63 6c61 7573 6520 3d20 2220  here_clause = " 
+00003c50: 5748 4552 4520 2220 2b20 2220 4f52 2022  WHERE " + " OR "
+00003c60: 2e6a 6f69 6e28 6f72 5f65 7870 7265 7373  .join(or_express
+00003c70: 696f 6e73 290a 0a20 2020 2020 2020 2066  ions)..        f
+00003c80: 756c 6c5f 7175 6572 7920 3d20 6622 7b73  ull_query = f"{s
+00003c90: 656c 6563 745f 636c 6175 7365 7d20 4652  elect_clause} FR
+00003ca0: 4f4d 207b 7375 625f 7175 6572 797d 2041  OM {sub_query} A
+00003cb0: 5320 7375 627b 7768 6572 655f 636c 6175  S sub{where_clau
+00003cc0: 7365 7d22 0a20 2020 2020 2020 2072 6574  se}".        ret
+00003cd0: 7572 6e20 6675 6c6c 5f71 7565 7279 0a0a  urn full_query..
+00003ce0: 2020 2020 6465 6620 5f71 7565 7279 5f74      def _query_t
+00003cf0: 6f5f 6465 7374 696e 6174 696f 6e28 0a20  o_destination(. 
+00003d00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00003d10: 2020 2020 2071 7565 7279 3a20 7374 722c       query: str,
+00003d20: 0a20 2020 2020 2020 2069 6e64 6578 5f63  .        index_c
+00003d30: 6f6c 733a 204c 6973 745b 7374 725d 2c0a  ols: List[str],.
+00003d40: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
+00003d50: 3a20 7374 722c 0a20 2020 2020 2020 2063  : str,.        c
+00003d60: 6f6e 6669 6775 7261 7469 6f6e 3a20 6469  onfiguration: di
+00003d70: 6374 203d 207b 2271 7565 7279 223a 207b  ct = {"query": {
+00003d80: 2275 7365 5175 6572 7943 6163 6865 223a  "useQueryCache":
+00003d90: 2054 7275 657d 7d2c 0a20 2020 2020 2020   True}},.       
+00003da0: 2064 6f5f 636c 7573 7465 7269 6e67 3d54   do_clustering=T
+00003db0: 7275 652c 0a20 2020 2029 202d 3e20 5475  rue,.    ) -> Tu
+00003dc0: 706c 655b 4f70 7469 6f6e 616c 5b62 6967  ple[Optional[big
+00003dd0: 7175 6572 792e 5461 626c 6552 6566 6572  query.TableRefer
+00003de0: 656e 6365 5d2c 2062 6967 7175 6572 792e  ence], bigquery.
+00003df0: 5175 6572 794a 6f62 5d3a 0a20 2020 2020  QueryJob]:.     
+00003e00: 2020 2023 2049 6620 6120 6472 795f 7275     # If a dry_ru
+00003e10: 6e20 696e 6469 6361 7465 7320 7468 6973  n indicates this
+00003e20: 2069 7320 6e6f 7420 6120 7175 6572 7920   is not a query 
+00003e30: 7479 7065 206a 6f62 2c20 7468 656e 2064  type job, then d
+00003e40: 6f6e 2774 0a20 2020 2020 2020 2023 2062  on't.        # b
+00003e50: 6f74 6865 7220 7472 7969 6e67 2074 6f20  other trying to 
+00003e60: 646f 2061 2043 5245 4154 4520 5445 4d50  do a CREATE TEMP
+00003e70: 2054 4142 4c45 202e 2e2e 2041 5320 5345   TABLE ... AS SE
+00003e80: 4c45 4354 202e 2e2e 2073 7461 7465 6d65  LECT ... stateme
+00003e90: 6e74 2e0a 2020 2020 2020 2020 6472 795f  nt..        dry_
+00003ea0: 7275 6e5f 636f 6e66 6967 203d 2062 6967  run_config = big
+00003eb0: 7175 6572 792e 5175 6572 794a 6f62 436f  query.QueryJobCo
+00003ec0: 6e66 6967 2829 0a20 2020 2020 2020 2064  nfig().        d
+00003ed0: 7279 5f72 756e 5f63 6f6e 6669 672e 6472  ry_run_config.dr
+00003ee0: 795f 7275 6e20 3d20 5472 7565 0a20 2020  y_run = True.   
+00003ef0: 2020 2020 205f 2c20 6472 795f 7275 6e5f       _, dry_run_
+00003f00: 6a6f 6220 3d20 7365 6c66 2e5f 7374 6172  job = self._star
+00003f10: 745f 7175 6572 7928 7175 6572 792c 206a  t_query(query, j
+00003f20: 6f62 5f63 6f6e 6669 673d 6472 795f 7275  ob_config=dry_ru
+00003f30: 6e5f 636f 6e66 6967 290a 2020 2020 2020  n_config).      
+00003f40: 2020 6966 2064 7279 5f72 756e 5f6a 6f62    if dry_run_job
+00003f50: 2e73 7461 7465 6d65 6e74 5f74 7970 6520  .statement_type 
+00003f60: 213d 2022 5345 4c45 4354 223a 0a20 2020  != "SELECT":.   
+00003f70: 2020 2020 2020 2020 205f 2c20 7175 6572           _, quer
+00003f80: 795f 6a6f 6220 3d20 7365 6c66 2e5f 7374  y_job = self._st
+00003f90: 6172 745f 7175 6572 7928 7175 6572 7929  art_query(query)
+00003fa0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003fb0: 7572 6e20 7175 6572 795f 6a6f 622e 6465  urn query_job.de
+00003fc0: 7374 696e 6174 696f 6e2c 2071 7565 7279  stination, query
+00003fd0: 5f6a 6f62 0a0a 2020 2020 2020 2020 2320  _job..        # 
+00003fe0: 4372 6561 7465 2061 2074 6162 6c65 2074  Create a table t
+00003ff0: 6f20 776f 726b 6172 6f75 6e64 2042 6967  o workaround Big
+00004000: 5175 6572 7920 3130 2047 4220 7175 6572  Query 10 GB quer
+00004010: 7920 7265 7375 6c74 7320 6c69 6d69 742e  y results limit.
+00004020: 2053 6565 3a0a 2020 2020 2020 2020 2320   See:.        # 
+00004030: 696e 7465 726e 616c 2069 7373 7565 2033  internal issue 3
+00004040: 3033 3035 3733 3336 2e0a 2020 2020 2020  03057336..      
+00004050: 2020 2320 5369 6e63 6520 7765 2068 6176    # Since we hav
+00004060: 6520 6120 6073 7461 7465 6d65 6e74 5f74  e a `statement_t
+00004070: 7970 6520 3d3d 2027 5345 4c45 4354 2760  ype == 'SELECT'`
+00004080: 2c20 7363 6865 6d61 2073 686f 756c 6420  , schema should 
+00004090: 6265 2070 6f70 756c 6174 6564 2e0a 2020  be populated..  
+000040a0: 2020 2020 2020 7363 6865 6d61 203d 2074        schema = t
+000040b0: 7970 696e 672e 6361 7374 2849 7465 7261  yping.cast(Itera
+000040c0: 626c 655b 6269 6771 7565 7279 2e53 6368  ble[bigquery.Sch
+000040d0: 656d 6146 6965 6c64 5d2c 2064 7279 5f72  emaField], dry_r
+000040e0: 756e 5f6a 6f62 2e73 6368 656d 6129 0a20  un_job.schema). 
+000040f0: 2020 2020 2020 2069 6620 646f 5f63 6c75         if do_clu
+00004100: 7374 6572 696e 673a 0a20 2020 2020 2020  stering:.       
+00004110: 2020 2020 2063 6c75 7374 6572 5f63 6f6c       cluster_col
+00004120: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+00004130: 2020 2020 2020 6974 656d 2e6e 616d 650a        item.name.
+00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004150: 666f 7220 6974 656d 2069 6e20 7363 6865  for item in sche
+00004160: 6d61 0a20 2020 2020 2020 2020 2020 2020  ma.             
+00004170: 2020 2069 6620 2869 7465 6d2e 6e61 6d65     if (item.name
+00004180: 2069 6e20 696e 6465 785f 636f 6c73 2920   in index_cols) 
+00004190: 616e 6420 5f63 616e 5f63 6c75 7374 6572  and _can_cluster
+000041a0: 5f62 7128 6974 656d 290a 2020 2020 2020  _bq(item).      
+000041b0: 2020 2020 2020 5d5b 3a5f 4d41 585f 434c        ][:_MAX_CL
+000041c0: 5553 5445 525f 434f 4c55 4d4e 535d 0a20  USTER_COLUMNS]. 
+000041d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000041e0: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+000041f0: 5f63 6f6c 7320 3d20 5b5d 0a20 2020 2020  _cols = [].     
+00004200: 2020 2074 656d 705f 7461 626c 6520 3d20     temp_table = 
+00004210: 7365 6c66 2e5f 6372 6561 7465 5f65 6d70  self._create_emp
+00004220: 7479 5f74 656d 705f 7461 626c 6528 7363  ty_temp_table(sc
+00004230: 6865 6d61 2c20 636c 7573 7465 725f 636f  hema, cluster_co
+00004240: 6c73 290a 0a20 2020 2020 2020 2074 696d  ls)..        tim
+00004250: 656f 7574 5f6d 7320 3d20 636f 6e66 6967  eout_ms = config
+00004260: 7572 6174 696f 6e2e 6765 7428 226a 6f62  uration.get("job
+00004270: 5469 6d65 6f75 744d 7322 2920 6f72 2063  TimeoutMs") or c
+00004280: 6f6e 6669 6775 7261 7469 6f6e 5b22 7175  onfiguration["qu
+00004290: 6572 7922 5d2e 6765 7428 0a20 2020 2020  ery"].get(.     
+000042a0: 2020 2020 2020 2022 7469 6d65 6f75 744d         "timeoutM
+000042b0: 7322 0a20 2020 2020 2020 2029 0a0a 2020  s".        )..  
+000042c0: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
+000042d0: 7469 6d65 6f75 745f 6d73 2074 6f20 7365  timeout_ms to se
+000042e0: 636f 6e64 732c 2065 6e73 7572 696e 6720  conds, ensuring 
+000042f0: 6120 6d69 6e69 6d75 6d20 6f66 2030 2e31  a minimum of 0.1
+00004300: 2073 6563 6f6e 6473 2074 6f20 6176 6f69   seconds to avoi
+00004310: 640a 2020 2020 2020 2020 2320 7468 6520  d.        # the 
+00004320: 7072 6f67 7261 6d20 6765 7474 696e 6720  program getting 
+00004330: 7374 7563 6b20 6f6e 2074 6f6f 2d73 686f  stuck on too-sho
+00004340: 7274 2074 696d 656f 7574 732e 0a20 2020  rt timeouts..   
+00004350: 2020 2020 2074 696d 656f 7574 203d 206d       timeout = m
+00004360: 6178 2869 6e74 2874 696d 656f 7574 5f6d  ax(int(timeout_m
+00004370: 7329 202a 2031 652d 332c 2030 2e31 2920  s) * 1e-3, 0.1) 
+00004380: 6966 2074 696d 656f 7574 5f6d 7320 656c  if timeout_ms el
+00004390: 7365 204e 6f6e 650a 0a20 2020 2020 2020  se None..       
+000043a0: 206a 6f62 5f63 6f6e 6669 6720 3d20 7479   job_config = ty
+000043b0: 7069 6e67 2e63 6173 7428 0a20 2020 2020  ping.cast(.     
+000043c0: 2020 2020 2020 2062 6967 7175 6572 792e         bigquery.
+000043d0: 5175 6572 794a 6f62 436f 6e66 6967 2c0a  QueryJobConfig,.
+000043e0: 2020 2020 2020 2020 2020 2020 6269 6771              bigq
+000043f0: 7565 7279 2e51 7565 7279 4a6f 6243 6f6e  uery.QueryJobCon
+00004400: 6669 672e 6672 6f6d 5f61 7069 5f72 6570  fig.from_api_rep
+00004410: 7228 636f 6e66 6967 7572 6174 696f 6e29  r(configuration)
+00004420: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00004430: 2020 2020 6a6f 625f 636f 6e66 6967 2e6c      job_config.l
+00004440: 6162 656c 735b 2262 6967 6672 616d 6573  abels["bigframes
+00004450: 2d61 7069 225d 203d 2061 7069 5f6e 616d  -api"] = api_nam
+00004460: 650a 2020 2020 2020 2020 6a6f 625f 636f  e.        job_co
+00004470: 6e66 6967 2e64 6573 7469 6e61 7469 6f6e  nfig.destination
+00004480: 203d 2074 656d 705f 7461 626c 650a 0a20   = temp_table.. 
+00004490: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000044a0: 2020 2020 2020 2020 2320 5772 6974 6520          # Write 
+000044b0: 746f 2074 656d 7020 7461 626c 6520 746f  to temp table to
+000044c0: 2077 6f72 6b61 726f 756e 6420 4269 6751   workaround BigQ
+000044d0: 7565 7279 2031 3020 4742 2071 7565 7279  uery 10 GB query
+000044e0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+000044f0: 2020 2020 2023 206c 696d 6974 2e20 5365       # limit. Se
+00004500: 653a 2069 6e74 6572 6e61 6c20 6973 7375  e: internal issu
+00004510: 6520 3330 3330 3537 3333 362e 0a20 2020  e 303057336..   
+00004520: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+00004530: 6669 672e 6c61 6265 6c73 5b22 6572 726f  fig.labels["erro
+00004540: 725f 6361 7567 6874 225d 203d 2022 7472  r_caught"] = "tr
+00004550: 7565 220a 2020 2020 2020 2020 2020 2020  ue".            
+00004560: 5f2c 2071 7565 7279 5f6a 6f62 203d 2073  _, query_job = s
+00004570: 656c 662e 5f73 7461 7274 5f71 7565 7279  elf._start_query
+00004580: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004590: 2020 7175 6572 792c 206a 6f62 5f63 6f6e    query, job_con
+000045a0: 6669 673d 6a6f 625f 636f 6e66 6967 2c20  fig=job_config, 
+000045b0: 7469 6d65 6f75 743d 7469 6d65 6f75 740a  timeout=timeout.
+000045c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000045d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000045e0: 2071 7565 7279 5f6a 6f62 2e64 6573 7469   query_job.desti
+000045f0: 6e61 7469 6f6e 2c20 7175 6572 795f 6a6f  nation, query_jo
+00004600: 620a 2020 2020 2020 2020 6578 6365 7074  b.        except
+00004610: 2067 6f6f 676c 652e 6170 695f 636f 7265   google.api_core
+00004620: 2e65 7863 6570 7469 6f6e 732e 4261 6452  .exceptions.BadR
+00004630: 6571 7565 7374 3a0a 2020 2020 2020 2020  equest:.        
+00004640: 2020 2020 2320 536f 6d65 2053 454c 4543      # Some SELEC
+00004650: 5420 7374 6174 656d 656e 7473 2073 7469  T statements sti
+00004660: 6c6c 2061 7265 6e27 7420 636f 6d70 6174  ll aren't compat
+00004670: 6962 6c65 2077 6974 6820 636c 7573 7465  ible with cluste
+00004680: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
+00004690: 7461 626c 6573 2061 7320 7468 6520 6465  tables as the de
+000046a0: 7374 696e 6174 696f 6e2e 2046 6f72 2065  stination. For e
+000046b0: 7861 6d70 6c65 2c20 6966 2074 6865 2071  xample, if the q
+000046c0: 7565 7279 2068 6173 2061 0a20 2020 2020  uery has a.     
+000046d0: 2020 2020 2020 2023 2074 6f70 2d6c 6576         # top-lev
+000046e0: 656c 204f 5244 4552 2042 592c 2074 6869  el ORDER BY, thi
+000046f0: 7320 636f 6e66 6c69 6374 7320 7769 7468  s conflicts with
+00004700: 206f 7572 2061 6269 6c69 7479 2074 6f20   our ability to 
+00004710: 636c 7573 7465 720a 2020 2020 2020 2020  cluster.        
+00004720: 2020 2020 2320 7468 6520 7461 626c 6520      # the table 
+00004730: 6279 2074 6865 2069 6e64 6578 2063 6f6c  by the index col
+00004740: 756d 6e28 7329 2e0a 2020 2020 2020 2020  umn(s)..        
+00004750: 2020 2020 5f2c 2071 7565 7279 5f6a 6f62      _, query_job
+00004760: 203d 2073 656c 662e 5f73 7461 7274 5f71   = self._start_q
+00004770: 7565 7279 2871 7565 7279 2c20 7469 6d65  uery(query, time
+00004780: 6f75 743d 7469 6d65 6f75 7429 0a20 2020  out=timeout).   
+00004790: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000047a0: 7175 6572 795f 6a6f 622e 6465 7374 696e  query_job.destin
+000047b0: 6174 696f 6e2c 2071 7565 7279 5f6a 6f62  ation, query_job
+000047c0: 0a0a 2020 2020 6465 6620 7265 6164 5f67  ..    def read_g
+000047d0: 6271 5f71 7565 7279 280a 2020 2020 2020  bq_query(.      
+000047e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000047f0: 7175 6572 793a 2073 7472 2c0a 2020 2020  query: str,.    
+00004800: 2020 2020 2a2c 0a20 2020 2020 2020 2069      *,.        i
+00004810: 6e64 6578 5f63 6f6c 3a20 4974 6572 6162  ndex_col: Iterab
+00004820: 6c65 5b73 7472 5d20 7c20 7374 7220 3d20  le[str] | str = 
+00004830: 2829 2c0a 2020 2020 2020 2020 636f 6c75  (),.        colu
+00004840: 6d6e 733a 2049 7465 7261 626c 655b 7374  mns: Iterable[st
+00004850: 725d 203d 2028 292c 0a20 2020 2020 2020  r] = (),.       
+00004860: 2063 6f6e 6669 6775 7261 7469 6f6e 3a20   configuration: 
+00004870: 4f70 7469 6f6e 616c 5b44 6963 745d 203d  Optional[Dict] =
+00004880: 204e 6f6e 652c 0a20 2020 2020 2020 206d   None,.        m
+00004890: 6178 5f72 6573 756c 7473 3a20 4f70 7469  ax_results: Opti
+000048a0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000048b0: 2c0a 2020 2020 2020 2020 7573 655f 6361  ,.        use_ca
+000048c0: 6368 653a 204f 7074 696f 6e61 6c5b 626f  che: Optional[bo
+000048d0: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
+000048e0: 2020 2020 636f 6c5f 6f72 6465 723a 2049      col_order: I
+000048f0: 7465 7261 626c 655b 7374 725d 203d 2028  terable[str] = (
+00004900: 292c 0a20 2020 2029 202d 3e20 6461 7461  ),.    ) -> data
+00004910: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
+00004920: 0a20 2020 2020 2020 2022 2222 5475 726e  .        """Turn
+00004930: 2061 2053 514c 2071 7565 7279 2069 6e74   a SQL query int
+00004940: 6f20 6120 4461 7461 4672 616d 652e 0a0a  o a DataFrame...
+00004950: 2020 2020 2020 2020 4e6f 7465 3a20 4265          Note: Be
+00004960: 6361 7573 6520 7468 6520 7265 7375 6c74  cause the result
+00004970: 7320 6172 6520 7772 6974 7465 6e20 746f  s are written to
+00004980: 2061 2074 656d 706f 7261 7279 2074 6162   a temporary tab
+00004990: 6c65 2c20 6f72 6465 7269 6e67 2062 790a  le, ordering by.
+000049a0: 2020 2020 2020 2020 6060 4f52 4445 5220          ``ORDER 
+000049b0: 4259 6060 2069 7320 6e6f 7420 7072 6573  BY`` is not pres
+000049c0: 6572 7665 642e 2041 2075 6e69 7175 6520  erved. A unique 
+000049d0: 6069 6e64 6578 5f63 6f6c 6020 6973 2072  `index_col` is r
+000049e0: 6563 6f6d 6d65 6e64 6564 2e20 5573 650a  ecommended. Use.
+000049f0: 2020 2020 2020 2020 6060 726f 775f 6e75          ``row_nu
+00004a00: 6d62 6572 2829 206f 7665 7220 2829 6060  mber() over ()``
+00004a10: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00004a20: 6e61 7475 7261 6c20 756e 6971 7565 2069  natural unique i
+00004a30: 6e64 6578 206f 7220 796f 750a 2020 2020  ndex or you.    
+00004a40: 2020 2020 7761 6e74 2074 6f20 7072 6573      want to pres
+00004a50: 6572 7665 206f 7264 6572 696e 672e 0a0a  erve ordering...
+00004a60: 2020 2020 2020 2020 2a2a 4578 616d 706c          **Exampl
+00004a70: 6573 3a2a 2a0a 0a20 2020 2020 2020 2020  es:**..         
+00004a80: 2020 203e 3e3e 2069 6d70 6f72 7420 6269     >>> import bi
+00004a90: 6766 7261 6d65 732e 7061 6e64 6173 2061  gframes.pandas a
+00004aa0: 7320 6270 640a 2020 2020 2020 2020 2020  s bpd.          
+00004ab0: 2020 3e3e 3e20 6270 642e 6f70 7469 6f6e    >>> bpd.option
+00004ac0: 732e 6469 7370 6c61 792e 7072 6f67 7265  s.display.progre
+00004ad0: 7373 5f62 6172 203d 204e 6f6e 650a 0a20  ss_bar = None.. 
+00004ae0: 2020 2020 2020 2053 696d 706c 6520 7175         Simple qu
+00004af0: 6572 7920 696e 7075 743a 0a0a 2020 2020  ery input:..    
+00004b00: 2020 2020 2020 2020 3e3e 3e20 6466 203d          >>> df =
+00004b10: 2062 7064 2e72 6561 645f 6762 715f 7175   bpd.read_gbq_qu
+00004b20: 6572 7928 2727 270a 2020 2020 2020 2020  ery('''.        
+00004b30: 2020 2020 2e2e 2e20 2020 2053 454c 4543      ...    SELEC
+00004b40: 540a 2020 2020 2020 2020 2020 2020 2e2e  T.            ..
+00004b50: 2e20 2020 2020 2020 7069 7463 6865 7246  .       pitcherF
+00004b60: 6972 7374 4e61 6d65 2c0a 2020 2020 2020  irstName,.      
+00004b70: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00004b80: 7069 7463 6865 724c 6173 744e 616d 652c  pitcherLastName,
+00004b90: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00004ba0: 2020 2020 2020 2070 6974 6368 5370 6565         pitchSpee
+00004bb0: 642c 0a20 2020 2020 2020 2020 2020 202e  d,.            .
+00004bc0: 2e2e 2020 2020 4652 4f4d 2060 6269 6771  ..    FROM `bigq
+00004bd0: 7565 7279 2d70 7562 6c69 632d 6461 7461  uery-public-data
+00004be0: 2e62 6173 6562 616c 6c2e 6761 6d65 735f  .baseball.games_
+00004bf0: 7769 6465 600a 2020 2020 2020 2020 2020  wide`.          
+00004c00: 2020 2e2e 2e20 2727 2729 0a0a 2020 2020    ... ''')..    
+00004c10: 2020 2020 5072 6573 6572 7665 206f 7264      Preserve ord
+00004c20: 6572 696e 6720 696e 2061 2071 7565 7279  ering in a query
+00004c30: 2069 6e70 7574 2e0a 0a20 2020 2020 2020   input...       
+00004c40: 2020 2020 203e 3e3e 2064 6620 3d20 6270       >>> df = bp
+00004c50: 642e 7265 6164 5f67 6271 5f71 7565 7279  d.read_gbq_query
+00004c60: 2827 2727 0a20 2020 2020 2020 2020 2020  ('''.           
+00004c70: 202e 2e2e 2020 2020 5345 4c45 4354 0a20   ...    SELECT. 
+00004c80: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00004c90: 2020 2020 202d 2d20 496e 7374 6561 6420       -- Instead 
+00004ca0: 6f66 2061 6e20 4f52 4445 5220 4259 2063  of an ORDER BY c
+00004cb0: 6c61 7573 6520 6f6e 2074 6865 2071 7565  lause on the que
+00004cc0: 7279 2c20 7573 650a 2020 2020 2020 2020  ry, use.        
+00004cd0: 2020 2020 2e2e 2e20 2020 2020 2020 2d2d      ...       --
+00004ce0: 2052 4f57 5f4e 554d 4245 5228 2920 746f   ROW_NUMBER() to
+00004cf0: 2063 7265 6174 6520 616e 206f 7264 6572   create an order
+00004d00: 6564 2044 6174 6146 7261 6d65 2e0a 2020  ed DataFrame..  
+00004d10: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004d20: 2020 2020 524f 575f 4e55 4d42 4552 2829      ROW_NUMBER()
+00004d30: 204f 5645 5220 284f 5244 4552 2042 5920   OVER (ORDER BY 
+00004d40: 4156 4728 7069 7463 6853 7065 6564 2920  AVG(pitchSpeed) 
+00004d50: 4445 5343 290a 2020 2020 2020 2020 2020  DESC).          
+00004d60: 2020 2e2e 2e20 2020 2020 2020 2020 4153    ...         AS
+00004d70: 2072 6f77 696e 6465 782c 0a20 2020 2020   rowindex,.     
+00004d80: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+00004d90: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
+00004da0: 2070 6974 6368 6572 4669 7273 744e 616d   pitcherFirstNam
+00004db0: 652c 0a20 2020 2020 2020 2020 2020 202e  e,.            .
+00004dc0: 2e2e 2020 2020 2020 2070 6974 6368 6572  ..       pitcher
+00004dd0: 4c61 7374 4e61 6d65 2c0a 2020 2020 2020  LastName,.      
+00004de0: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00004df0: 4156 4728 7069 7463 6853 7065 6564 2920  AVG(pitchSpeed) 
+00004e00: 4153 2061 7665 7261 6765 5069 7463 6853  AS averagePitchS
+00004e10: 7065 6564 0a20 2020 2020 2020 2020 2020  peed.           
+00004e20: 202e 2e2e 2020 2020 2046 524f 4d20 6062   ...     FROM `b
+00004e30: 6967 7175 6572 792d 7075 626c 6963 2d64  igquery-public-d
+00004e40: 6174 612e 6261 7365 6261 6c6c 2e67 616d  ata.baseball.gam
+00004e50: 6573 5f77 6964 6560 0a20 2020 2020 2020  es_wide`.       
+00004e60: 2020 2020 202e 2e2e 2020 2020 2057 4845       ...     WHE
+00004e70: 5245 2079 6561 7220 3d20 3230 3136 0a20  RE year = 2016. 
+00004e80: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00004e90: 2020 2047 524f 5550 2042 5920 7069 7463     GROUP BY pitc
+00004ea0: 6865 7246 6972 7374 4e61 6d65 2c20 7069  herFirstName, pi
+00004eb0: 7463 6865 724c 6173 744e 616d 650a 2020  tcherLastName.  
+00004ec0: 2020 2020 2020 2020 2020 2e2e 2e20 2727            ... ''
+00004ed0: 272c 2069 6e64 6578 5f63 6f6c 3d22 726f  ', index_col="ro
+00004ee0: 7769 6e64 6578 2229 0a20 2020 2020 2020  windex").       
+00004ef0: 2020 2020 203e 3e3e 2064 662e 6865 6164       >>> df.head
+00004f00: 2832 290a 2020 2020 2020 2020 2020 2020  (2).            
+00004f10: 2020 2020 2020 2020 2070 6974 6368 6572           pitcher
+00004f20: 4669 7273 744e 616d 6520 7069 7463 6865  FirstName pitche
+00004f30: 724c 6173 744e 616d 6520 2061 7665 7261  rLastName  avera
+00004f40: 6765 5069 7463 6853 7065 6564 0a20 2020  gePitchSpeed.   
+00004f50: 2020 2020 2020 2020 2072 6f77 696e 6465           rowinde
+00004f60: 780a 2020 2020 2020 2020 2020 2020 3120  x.            1 
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00004f80: 6c62 6572 7469 6e20 2020 2020 2020 2020  lbertin         
+00004f90: 4368 6170 6d61 6e20 2020 2020 2020 2020  Chapman         
+00004fa0: 2039 362e 3531 3431 3133 0a20 2020 2020   96.514113.     
+00004fb0: 2020 2020 2020 2032 2020 2020 2020 2020         2        
+00004fc0: 2020 2020 2020 2020 205a 6163 6861 7279           Zachary
+00004fd0: 2020 2020 2020 2020 2042 7269 7474 6f6e           Britton
+00004fe0: 2020 2020 2020 2020 2020 3934 2e35 3931            94.591
+00004ff0: 3033 390a 2020 2020 2020 2020 2020 2020  039.            
+00005000: 3c42 4c41 4e4b 4c49 4e45 3e0a 2020 2020  <BLANKLINE>.    
+00005010: 2020 2020 2020 2020 5b32 2072 6f77 7320          [2 rows 
+00005020: 7820 3320 636f 6c75 6d6e 735d 0a0a 2020  x 3 columns]..  
+00005030: 2020 2020 2020 5365 6520 616c 736f 3a20        See also: 
+00005040: 3a6d 6574 683a 6053 6573 7369 6f6e 2e72  :meth:`Session.r
+00005050: 6561 645f 6762 7160 2e0a 2020 2020 2020  ead_gbq`..      
+00005060: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+00005070: 4e4f 5445 3a20 5468 6973 206d 6574 686f  NOTE: This metho
+00005080: 6420 646f 6573 6e27 7420 2879 6574 2920  d doesn't (yet) 
+00005090: 6578 6973 7420 696e 2070 616e 6461 7320  exist in pandas 
+000050a0: 6f72 2070 616e 6461 732d 6762 712c 2073  or pandas-gbq, s
+000050b0: 6f0a 2020 2020 2020 2020 2320 7468 6573  o.        # thes
+000050c0: 6520 646f 6373 7472 696e 6773 2061 7265  e docstrings are
+000050d0: 2069 6e6c 696e 652e 0a20 2020 2020 2020   inline..       
+000050e0: 2069 6620 636f 6c75 6d6e 7320 616e 6420   if columns and 
+000050f0: 636f 6c5f 6f72 6465 723a 0a20 2020 2020  col_order:.     
+00005100: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00005110: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+00005120: 2020 2020 2020 2020 2022 4d75 7374 2073           "Must s
+00005130: 7065 6369 6679 2065 6974 6865 7220 636f  pecify either co
+00005140: 6c75 6d6e 7320 2870 7265 6665 7272 6564  lumns (preferred
+00005150: 2920 6f72 2063 6f6c 5f6f 7264 6572 2c20  ) or col_order, 
+00005160: 6e6f 7420 626f 7468 220a 2020 2020 2020  not both".      
+00005170: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005180: 656c 6966 2063 6f6c 5f6f 7264 6572 3a0a  elif col_order:.
+00005190: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+000051a0: 6d6e 7320 3d20 636f 6c5f 6f72 6465 720a  mns = col_order.
+000051b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000051c0: 7365 6c66 2e5f 7265 6164 5f67 6271 5f71  self._read_gbq_q
+000051d0: 7565 7279 280a 2020 2020 2020 2020 2020  uery(.          
+000051e0: 2020 7175 6572 793d 7175 6572 792c 0a20    query=query,. 
+000051f0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00005200: 5f63 6f6c 3d69 6e64 6578 5f63 6f6c 2c0a  _col=index_col,.
+00005210: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00005220: 6d6e 733d 636f 6c75 6d6e 732c 0a20 2020  mns=columns,.   
+00005230: 2020 2020 2020 2020 2063 6f6e 6669 6775           configu
+00005240: 7261 7469 6f6e 3d63 6f6e 6669 6775 7261  ration=configura
+00005250: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00005260: 2020 6d61 785f 7265 7375 6c74 733d 6d61    max_results=ma
+00005270: 785f 7265 7375 6c74 732c 0a20 2020 2020  x_results,.     
+00005280: 2020 2020 2020 2061 7069 5f6e 616d 653d         api_name=
+00005290: 2272 6561 645f 6762 715f 7175 6572 7922  "read_gbq_query"
+000052a0: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
+000052b0: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
+000052c0: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+000052d0: 2020 6465 6620 5f72 6561 645f 6762 715f    def _read_gbq_
+000052e0: 7175 6572 7928 0a20 2020 2020 2020 2073  query(.        s
+000052f0: 656c 662c 0a20 2020 2020 2020 2071 7565  elf,.        que
+00005300: 7279 3a20 7374 722c 0a20 2020 2020 2020  ry: str,.       
+00005310: 202a 2c0a 2020 2020 2020 2020 696e 6465   *,.        inde
+00005320: 785f 636f 6c3a 2049 7465 7261 626c 655b  x_col: Iterable[
+00005330: 7374 725d 207c 2073 7472 203d 2028 292c  str] | str = (),
+00005340: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
+00005350: 3a20 4974 6572 6162 6c65 5b73 7472 5d20  : Iterable[str] 
+00005360: 3d20 2829 2c0a 2020 2020 2020 2020 636f  = (),.        co
+00005370: 6e66 6967 7572 6174 696f 6e3a 204f 7074  nfiguration: Opt
+00005380: 696f 6e61 6c5b 4469 6374 5d20 3d20 4e6f  ional[Dict] = No
+00005390: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
+000053a0: 7265 7375 6c74 733a 204f 7074 696f 6e61  results: Optiona
+000053b0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+000053c0: 2020 2020 2020 2061 7069 5f6e 616d 653a         api_name:
+000053d0: 2073 7472 203d 2022 7265 6164 5f67 6271   str = "read_gbq
+000053e0: 5f71 7565 7279 222c 0a20 2020 2020 2020  _query",.       
+000053f0: 2075 7365 5f63 6163 6865 3a20 4f70 7469   use_cache: Opti
+00005400: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00005410: 652c 0a20 2020 2029 202d 3e20 6461 7461  e,.    ) -> data
+00005420: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
+00005430: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+00005440: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
+00005450: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
+00005460: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
+00005470: 7572 6174 696f 6e20 3d20 5f74 7261 6e73  uration = _trans
+00005480: 666f 726d 5f72 6561 645f 6762 715f 636f  form_read_gbq_co
+00005490: 6e66 6967 7572 6174 696f 6e28 636f 6e66  nfiguration(conf
+000054a0: 6967 7572 6174 696f 6e29 0a0a 2020 2020  iguration)..    
+000054b0: 2020 2020 6966 2022 7175 6572 7922 206e      if "query" n
+000054c0: 6f74 2069 6e20 636f 6e66 6967 7572 6174  ot in configurat
+000054d0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+000054e0: 2063 6f6e 6669 6775 7261 7469 6f6e 5b22   configuration["
+000054f0: 7175 6572 7922 5d20 3d20 7b7d 0a0a 2020  query"] = {}..  
+00005500: 2020 2020 2020 6966 2022 7175 6572 7922        if "query"
+00005510: 2069 6e20 636f 6e66 6967 7572 6174 696f   in configuratio
+00005520: 6e5b 2271 7565 7279 225d 3a0a 2020 2020  n["query"]:.    
+00005530: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00005540: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00005550: 2020 2020 2020 2020 2020 2254 6865 2071            "The q
+00005560: 7565 7279 2073 7461 7465 6d65 6e74 206d  uery statement m
+00005570: 7573 7420 6e6f 7420 6265 2069 6e63 6c75  ust not be inclu
+00005580: 6465 6420 696e 2074 6865 2022 2c0a 2020  ded in the ",.  
+00005590: 2020 2020 2020 2020 2020 2020 2020 2227                "'
+000055a0: 636f 6e66 6967 7572 6174 696f 6e27 2062  configuration' b
+000055b0: 6563 6175 7365 2069 7420 6973 2061 6c72  ecause it is alr
+000055c0: 6561 6479 2070 726f 7669 6465 6420 6173  eady provided as
+000055d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000055e0: 2020 2022 2061 2073 6570 6172 6174 6520     " a separate 
+000055f0: 7061 7261 6d65 7465 722e 222c 0a20 2020  parameter.",.   
+00005600: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00005610: 2020 2020 6966 2022 7573 6551 7565 7279      if "useQuery
+00005620: 4361 6368 6522 2069 6e20 636f 6e66 6967  Cache" in config
+00005630: 7572 6174 696f 6e5b 2271 7565 7279 225d  uration["query"]
+00005640: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00005650: 2075 7365 5f63 6163 6865 2069 7320 6e6f   use_cache is no
+00005660: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00005670: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00005680: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00005690: 2020 2020 2020 2020 2020 2020 2020 2227                "'
+000056a0: 7573 6551 7565 7279 4361 6368 6527 2069  useQueryCache' i
+000056b0: 6e20 2763 6f6e 6669 6775 7261 7469 6f6e  n 'configuration
+000056c0: 2720 636f 6e66 6c69 6374 7320 7769 7468  ' conflicts with
+000056d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000056e0: 2020 2020 2020 2220 2775 7365 5f63 6163        " 'use_cac
+000056f0: 6865 2720 7061 7261 6d65 7465 722e 2050  he' parameter. P
+00005700: 6c65 6173 6520 7370 6563 6966 7920 6f6e  lease specify on
+00005710: 6c79 206f 6e65 2e22 0a20 2020 2020 2020  ly one.".       
+00005720: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00005730: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005740: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+00005750: 6f6e 5b22 7175 6572 7922 5d5b 2275 7365  on["query"]["use
+00005760: 5175 6572 7943 6163 6865 225d 203d 2028  QueryCache"] = (
+00005770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005780: 2054 7275 6520 6966 2075 7365 5f63 6163   True if use_cac
+00005790: 6865 2069 7320 4e6f 6e65 2065 6c73 6520  he is None else 
+000057a0: 7573 655f 6361 6368 650a 2020 2020 2020  use_cache.      
+000057b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000057c0: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
+000057d0: 6e64 6578 5f63 6f6c 2c20 7374 7229 3a0a  ndex_col, str):.
+000057e0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+000057f0: 785f 636f 6c73 203d 205b 696e 6465 785f  x_cols = [index_
+00005800: 636f 6c5d 0a20 2020 2020 2020 2065 6c73  col].        els
+00005810: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00005820: 6e64 6578 5f63 6f6c 7320 3d20 6c69 7374  ndex_cols = list
+00005830: 2869 6e64 6578 5f63 6f6c 290a 0a20 2020  (index_col)..   
+00005840: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+00005850: 2c20 7175 6572 795f 6a6f 6220 3d20 7365  , query_job = se
+00005860: 6c66 2e5f 7175 6572 795f 746f 5f64 6573  lf._query_to_des
+00005870: 7469 6e61 7469 6f6e 280a 2020 2020 2020  tination(.      
+00005880: 2020 2020 2020 7175 6572 792c 0a20 2020        query,.   
+00005890: 2020 2020 2020 2020 2069 6e64 6578 5f63           index_c
+000058a0: 6f6c 732c 0a20 2020 2020 2020 2020 2020  ols,.           
+000058b0: 2061 7069 5f6e 616d 653d 6170 695f 6e61   api_name=api_na
+000058c0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000058d0: 636f 6e66 6967 7572 6174 696f 6e3d 636f  configuration=co
+000058e0: 6e66 6967 7572 6174 696f 6e2c 0a20 2020  nfiguration,.   
+000058f0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00005900: 2320 4966 2074 6865 7265 2077 6173 206e  # If there was n
+00005910: 6f20 6465 7374 696e 6174 696f 6e20 7461  o destination ta
+00005920: 626c 652c 2074 6861 7420 6d65 616e 7320  ble, that means 
+00005930: 7468 6520 7175 6572 7920 6d75 7374 2068  the query must h
+00005940: 6176 650a 2020 2020 2020 2020 2320 6265  ave.        # be
+00005950: 656e 2044 444c 206f 7220 444d 4c2e 2052  en DDL or DML. R
+00005960: 6574 7572 6e20 736f 6d65 206a 6f62 206d  eturn some job m
+00005970: 6574 6164 6174 612c 2069 6e73 7465 6164  etadata, instead
+00005980: 2e0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00005990: 2064 6573 7469 6e61 7469 6f6e 3a0a 2020   destination:.  
+000059a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000059b0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
+000059c0: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
+000059d0: 2020 2020 2020 6461 7461 3d70 616e 6461        data=panda
+000059e0: 732e 4461 7461 4672 616d 6528 0a20 2020  s.DataFrame(.   
+000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00005a10: 2020 2020 2020 2020 2020 2022 7374 6174             "stat
+00005a20: 656d 656e 745f 7479 7065 223a 205b 0a20  ement_type": [. 
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 2020 2020 2020 2020 2020 2071 7565 7279             query
+00005a50: 5f6a 6f62 2e73 7461 7465 6d65 6e74 5f74  _job.statement_t
+00005a60: 7970 6520 6966 2071 7565 7279 5f6a 6f62  ype if query_job
+00005a70: 2065 6c73 6520 2275 6e6b 6e6f 776e 220a   else "unknown".
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2020 2022 6a6f 625f 6964 223a 205b 7175     "job_id": [qu
+00005ac0: 6572 795f 6a6f 622e 6a6f 625f 6964 2069  ery_job.job_id i
+00005ad0: 6620 7175 6572 795f 6a6f 6220 656c 7365  f query_job else
+00005ae0: 2022 756e 6b6e 6f77 6e22 5d2c 0a20 2020   "unknown"],.   
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b00: 2020 2020 2022 6c6f 6361 7469 6f6e 223a       "location":
+00005b10: 205b 7175 6572 795f 6a6f 622e 6c6f 6361   [query_job.loca
+00005b20: 7469 6f6e 2069 6620 7175 6572 795f 6a6f  tion if query_jo
+00005b30: 6220 656c 7365 2022 756e 6b6e 6f77 6e22  b else "unknown"
+00005b40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00005b50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00005b60: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00005b70: 2020 2020 2020 2020 2020 2020 7365 7373              sess
+00005b80: 696f 6e3d 7365 6c66 2c0a 2020 2020 2020  ion=self,.      
+00005b90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00005ba0: 2072 6574 7572 6e20 7365 6c66 2e72 6561   return self.rea
+00005bb0: 645f 6762 715f 7461 626c 6528 0a20 2020  d_gbq_table(.   
+00005bc0: 2020 2020 2020 2020 2066 227b 6465 7374           f"{dest
+00005bd0: 696e 6174 696f 6e2e 7072 6f6a 6563 747d  ination.project}
+00005be0: 2e7b 6465 7374 696e 6174 696f 6e2e 6461  .{destination.da
+00005bf0: 7461 7365 745f 6964 7d2e 7b64 6573 7469  taset_id}.{desti
+00005c00: 6e61 7469 6f6e 2e74 6162 6c65 5f69 647d  nation.table_id}
+00005c10: 222c 0a20 2020 2020 2020 2020 2020 2069  ",.            i
+00005c20: 6e64 6578 5f63 6f6c 3d69 6e64 6578 5f63  ndex_col=index_c
+00005c30: 6f6c 732c 0a20 2020 2020 2020 2020 2020  ols,.           
+00005c40: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
+00005c50: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+00005c60: 785f 7265 7375 6c74 733d 6d61 785f 7265  x_results=max_re
+00005c70: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
+00005c80: 2020 2075 7365 5f63 6163 6865 3d63 6f6e     use_cache=con
+00005c90: 6669 6775 7261 7469 6f6e 5b22 7175 6572  figuration["quer
+00005ca0: 7922 5d5b 2275 7365 5175 6572 7943 6163  y"]["useQueryCac
+00005cb0: 6865 225d 2c0a 2020 2020 2020 2020 290a  he"],.        ).
+00005cc0: 0a20 2020 2064 6566 2072 6561 645f 6762  .    def read_gb
+00005cd0: 715f 7461 626c 6528 0a20 2020 2020 2020  q_table(.       
+00005ce0: 2073 656c 662c 0a20 2020 2020 2020 2071   self,.        q
+00005cf0: 7565 7279 3a20 7374 722c 0a20 2020 2020  uery: str,.     
+00005d00: 2020 202a 2c0a 2020 2020 2020 2020 696e     *,.        in
+00005d10: 6465 785f 636f 6c3a 2049 7465 7261 626c  dex_col: Iterabl
+00005d20: 655b 7374 725d 207c 2073 7472 203d 2028  e[str] | str = (
+00005d30: 292c 0a20 2020 2020 2020 2063 6f6c 756d  ),.        colum
+00005d40: 6e73 3a20 4974 6572 6162 6c65 5b73 7472  ns: Iterable[str
+00005d50: 5d20 3d20 2829 2c0a 2020 2020 2020 2020  ] = (),.        
+00005d60: 6d61 785f 7265 7375 6c74 733a 204f 7074  max_results: Opt
+00005d70: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00005d80: 652c 0a20 2020 2020 2020 2066 696c 7465  e,.        filte
+00005d90: 7273 3a20 7468 6972 645f 7061 7274 795f  rs: third_party_
+00005da0: 7061 6e64 6173 5f67 6271 2e46 696c 7465  pandas_gbq.Filte
+00005db0: 7273 5479 7065 203d 2028 292c 0a20 2020  rsType = (),.   
+00005dc0: 2020 2020 2075 7365 5f63 6163 6865 3a20       use_cache: 
+00005dd0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+00005de0: 2020 2020 2063 6f6c 5f6f 7264 6572 3a20       col_order: 
+00005df0: 4974 6572 6162 6c65 5b73 7472 5d20 3d20  Iterable[str] = 
+00005e00: 2829 2c0a 2020 2020 2920 2d3e 2064 6174  (),.    ) -> dat
+00005e10: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
+00005e20: 3a0a 2020 2020 2020 2020 2222 2254 7572  :.        """Tur
+00005e30: 6e20 6120 4269 6751 7565 7279 2074 6162  n a BigQuery tab
+00005e40: 6c65 2069 6e74 6f20 6120 4461 7461 4672  le into a DataFr
+00005e50: 616d 652e 0a0a 2020 2020 2020 2020 2a2a  ame...        **
+00005e60: 4578 616d 706c 6573 3a2a 2a0a 0a20 2020  Examples:**..   
+00005e70: 2020 2020 2020 2020 203e 3e3e 2069 6d70           >>> imp
+00005e80: 6f72 7420 6269 6766 7261 6d65 732e 7061  ort bigframes.pa
+00005e90: 6e64 6173 2061 7320 6270 640a 2020 2020  ndas as bpd.    
+00005ea0: 2020 2020 2020 2020 3e3e 3e20 6270 642e          >>> bpd.
+00005eb0: 6f70 7469 6f6e 732e 6469 7370 6c61 792e  options.display.
+00005ec0: 7072 6f67 7265 7373 5f62 6172 203d 204e  progress_bar = N
+00005ed0: 6f6e 650a 0a20 2020 2020 2020 2052 6561  one..        Rea
+00005ee0: 6420 6120 7768 6f6c 6520 7461 626c 652c  d a whole table,
+00005ef0: 2077 6974 6820 6172 6269 7472 6172 7920   with arbitrary 
+00005f00: 6f72 6465 7269 6e67 206f 7220 6f72 6465  ordering or orde
+00005f10: 7269 6e67 2063 6f72 7265 7370 6f6e 6469  ring correspondi
+00005f20: 6e67 2074 6f20 7468 6520 7072 696d 6172  ng to the primar
+00005f30: 7920 6b65 7928 7329 2e0a 0a20 2020 2020  y key(s)...     
+00005f40: 2020 2020 2020 203e 3e3e 2064 6620 3d20         >>> df = 
+00005f50: 6270 642e 7265 6164 5f67 6271 5f74 6162  bpd.read_gbq_tab
+00005f60: 6c65 2822 6269 6771 7565 7279 2d70 7562  le("bigquery-pub
+00005f70: 6c69 632d 6461 7461 2e6d 6c5f 6461 7461  lic-data.ml_data
+00005f80: 7365 7473 2e70 656e 6775 696e 7322 290a  sets.penguins").
+00005f90: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
+00005fa0: 6f3a 203a 6d65 7468 3a60 5365 7373 696f  o: :meth:`Sessio
+00005fb0: 6e2e 7265 6164 5f67 6271 602e 0a20 2020  n.read_gbq`..   
+00005fc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005fd0: 2023 204e 4f54 453a 2054 6869 7320 6d65   # NOTE: This me
+00005fe0: 7468 6f64 2064 6f65 736e 2774 2028 7965  thod doesn't (ye
+00005ff0: 7429 2065 7869 7374 2069 6e20 7061 6e64  t) exist in pand
+00006000: 6173 206f 7220 7061 6e64 6173 2d67 6271  as or pandas-gbq
+00006010: 2c20 736f 0a20 2020 2020 2020 2023 2074  , so.        # t
+00006020: 6865 7365 2064 6f63 7374 7269 6e67 7320  hese docstrings 
+00006030: 6172 6520 696e 6c69 6e65 2e0a 2020 2020  are inline..    
+00006040: 2020 2020 6966 2063 6f6c 756d 6e73 2061      if columns a
+00006050: 6e64 2063 6f6c 5f6f 7264 6572 3a0a 2020  nd col_order:.  
+00006060: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00006070: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00006080: 2020 2020 2020 2020 2020 2020 224d 7573              "Mus
+00006090: 7420 7370 6563 6966 7920 6569 7468 6572  t specify either
+000060a0: 2063 6f6c 756d 6e73 2028 7072 6566 6572   columns (prefer
+000060b0: 7265 6429 206f 7220 636f 6c5f 6f72 6465  red) or col_orde
+000060c0: 722c 206e 6f74 2062 6f74 6822 0a20 2020  r, not both".   
+000060d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000060e0: 2020 2065 6c69 6620 636f 6c5f 6f72 6465     elif col_orde
+000060f0: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
+00006100: 6f6c 756d 6e73 203d 2063 6f6c 5f6f 7264  olumns = col_ord
+00006110: 6572 0a0a 2020 2020 2020 2020 6669 6c74  er..        filt
+00006120: 6572 7320 3d20 6c69 7374 2866 696c 7465  ers = list(filte
+00006130: 7273 290a 2020 2020 2020 2020 6966 206c  rs).        if l
+00006140: 656e 2866 696c 7465 7273 2920 213d 2030  en(filters) != 0
+00006150: 206f 7220 5f69 735f 7461 626c 655f 7769   or _is_table_wi
+00006160: 7468 5f77 696c 6463 6172 645f 7375 6666  th_wildcard_suff
+00006170: 6978 2871 7565 7279 293a 0a20 2020 2020  ix(query):.     
+00006180: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
+00006190: 656c 662e 5f74 6f5f 7175 6572 7928 7175  elf._to_query(qu
+000061a0: 6572 792c 2063 6f6c 756d 6e73 2c20 6669  ery, columns, fi
+000061b0: 6c74 6572 7329 0a0a 2020 2020 2020 2020  lters)..        
+000061c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000061d0: 5f72 6561 645f 6762 715f 7175 6572 7928  _read_gbq_query(
+000061e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000061f0: 2071 7565 7279 2c0a 2020 2020 2020 2020   query,.        
+00006200: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
+00006210: 6c3d 696e 6465 785f 636f 6c2c 0a20 2020  l=index_col,.   
+00006220: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00006230: 756d 6e73 3d63 6f6c 756d 6e73 2c0a 2020  umns=columns,.  
+00006240: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00006250: 785f 7265 7375 6c74 733d 6d61 785f 7265  x_results=max_re
+00006260: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
+00006270: 2020 2020 2020 2061 7069 5f6e 616d 653d         api_name=
+00006280: 2272 6561 645f 6762 715f 7461 626c 6522  "read_gbq_table"
+00006290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000062a0: 2020 7573 655f 6361 6368 653d 7573 655f    use_cache=use_
+000062b0: 6361 6368 652c 0a20 2020 2020 2020 2020  cache,.         
+000062c0: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+000062d0: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
+000062e0: 6762 715f 7461 626c 6528 0a20 2020 2020  gbq_table(.     
+000062f0: 2020 2020 2020 2071 7565 7279 3d71 7565         query=que
+00006300: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+00006310: 696e 6465 785f 636f 6c3d 696e 6465 785f  index_col=index_
+00006320: 636f 6c2c 0a20 2020 2020 2020 2020 2020  col,.           
+00006330: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
+00006340: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+00006350: 785f 7265 7375 6c74 733d 6d61 785f 7265  x_results=max_re
+00006360: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
+00006370: 2020 2061 7069 5f6e 616d 653d 2272 6561     api_name="rea
+00006380: 645f 6762 715f 7461 626c 6522 2c0a 2020  d_gbq_table",.  
+00006390: 2020 2020 2020 2020 2020 7573 655f 6361            use_ca
+000063a0: 6368 653d 7573 655f 6361 6368 652c 0a20  che=use_cache,. 
+000063b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+000063c0: 6620 5f67 6574 5f73 6e61 7073 686f 745f  f _get_snapshot_
+000063d0: 7371 6c5f 616e 645f 7072 696d 6172 795f  sql_and_primary_
+000063e0: 6b65 7928 0a20 2020 2020 2020 2073 656c  key(.        sel
+000063f0: 662c 0a20 2020 2020 2020 2074 6162 6c65  f,.        table
+00006400: 3a20 676f 6f67 6c65 2e63 6c6f 7564 2e62  : google.cloud.b
+00006410: 6967 7175 6572 792e 7461 626c 652e 5461  igquery.table.Ta
+00006420: 626c 652c 0a20 2020 2020 2020 202a 2c0a  ble,.        *,.
+00006430: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
+00006440: 3a20 7374 722c 0a20 2020 2020 2020 2075  : str,.        u
+00006450: 7365 5f63 6163 6865 3a20 626f 6f6c 203d  se_cache: bool =
+00006460: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
+00006470: 5475 706c 655b 6962 6973 5f74 7970 6573  Tuple[ibis_types
+00006480: 2e54 6162 6c65 2c20 4f70 7469 6f6e 616c  .Table, Optional
+00006490: 5b53 6571 7565 6e63 655b 7374 725d 5d5d  [Sequence[str]]]
+000064a0: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
+000064b0: 6174 6520 6120 7265 6164 2d6f 6e6c 7920  ate a read-only 
+000064c0: 4962 6973 2074 6162 6c65 2065 7870 7265  Ibis table expre
+000064d0: 7373 696f 6e20 7265 7072 6573 656e 7469  ssion representi
+000064e0: 6e67 2061 2074 6162 6c65 2e0a 0a20 2020  ng a table...   
+000064f0: 2020 2020 2049 6620 7765 2063 616e 2067       If we can g
+00006500: 6574 2061 2074 6f74 616c 206f 7264 6572  et a total order
+00006510: 696e 6720 6672 6f6d 2074 6865 2074 6162  ing from the tab
+00006520: 6c65 2c20 7375 6368 2061 7320 7669 6120  le, such as via 
+00006530: 7072 696d 6172 7920 6b65 790a 2020 2020  primary key.    
+00006540: 2020 2020 636f 6c75 6d6e 2873 292c 2074      column(s), t
+00006550: 6865 6e20 7265 7475 726e 2074 686f 7365  hen return those
+00006560: 2074 6f6f 2073 6f20 7468 6174 206f 7264   too so that ord
+00006570: 6572 696e 6720 6765 6e65 7261 7469 6f6e  ering generation
+00006580: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
+00006590: 6176 6f69 6465 642e 0a20 2020 2020 2020  avoided..       
+000065a0: 2022 2222 0a20 2020 2020 2020 2028 0a20   """.        (. 
+000065b0: 2020 2020 2020 2020 2020 2073 6e61 7073             snaps
+000065c0: 686f 745f 7469 6d65 7374 616d 702c 0a20  hot_timestamp,. 
+000065d0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000065e0: 2c0a 2020 2020 2020 2020 2920 3d20 6269  ,.        ) = bi
+000065f0: 6766 7261 6d65 735f 696f 2e67 6574 5f73  gframes_io.get_s
+00006600: 6e61 7073 686f 745f 6461 7465 7469 6d65  napshot_datetime
+00006610: 5f61 6e64 5f74 6162 6c65 5f6d 6574 6164  _and_table_metad
+00006620: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
+00006630: 2073 656c 662e 6271 636c 6965 6e74 2c0a   self.bqclient,.
+00006640: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+00006650: 655f 7265 663d 7461 626c 652e 7265 6665  e_ref=table.refe
+00006660: 7265 6e63 652c 0a20 2020 2020 2020 2020  rence,.         
+00006670: 2020 2061 7069 5f6e 616d 653d 6170 695f     api_name=api_
+00006680: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00006690: 2020 6361 6368 653d 7365 6c66 2e5f 6466    cache=self._df
+000066a0: 5f73 6e61 7073 686f 742c 0a20 2020 2020  _snapshot,.     
+000066b0: 2020 2020 2020 2075 7365 5f63 6163 6865         use_cache
+000066c0: 3d75 7365 5f63 6163 6865 2c0a 2020 2020  =use_cache,.    
+000066d0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+000066e0: 6620 7461 626c 652e 6c6f 6361 7469 6f6e  f table.location
+000066f0: 2e63 6173 6566 6f6c 6428 2920 213d 2073  .casefold() != s
+00006700: 656c 662e 5f6c 6f63 6174 696f 6e2e 6361  elf._location.ca
+00006710: 7365 666f 6c64 2829 3a0a 2020 2020 2020  sefold():.      
+00006720: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00006730: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00006740: 2020 2020 2020 2020 6622 4375 7272 656e          f"Curren
+00006750: 7420 7365 7373 696f 6e20 6973 2069 6e20  t session is in 
+00006760: 7b73 656c 662e 5f6c 6f63 6174 696f 6e7d  {self._location}
+00006770: 2062 7574 2064 6174 6173 6574 2027 7b74   but dataset '{t
+00006780: 6162 6c65 2e70 726f 6a65 6374 7d2e 7b74  able.project}.{t
+00006790: 6162 6c65 2e64 6174 6173 6574 5f69 647d  able.dataset_id}
+000067a0: 2720 6973 206c 6f63 6174 6564 2069 6e20  ' is located in 
+000067b0: 7b74 6162 6c65 2e6c 6f63 6174 696f 6e7d  {table.location}
+000067c0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+000067d0: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
+000067e0: 6572 6520 6172 6520 7072 696d 6172 7920  ere are primary 
+000067f0: 6b65 7973 2064 6566 696e 6564 2c20 7468  keys defined, th
+00006800: 6520 7175 6572 7920 656e 6769 6e65 2061  e query engine a
+00006810: 7373 756d 6573 2074 6865 7365 0a20 2020  ssumes these.   
+00006820: 2020 2020 2023 2063 6f6c 756d 6e73 2061       # columns a
+00006830: 7265 2075 6e69 7175 652c 2065 7665 6e20  re unique, even 
+00006840: 6966 2074 6865 2063 6f6e 7374 7261 696e  if the constrain
+00006850: 7420 6973 206e 6f74 2065 6e66 6f72 6365  t is not enforce
+00006860: 642e 2057 6520 6d61 6b65 0a20 2020 2020  d. We make.     
+00006870: 2020 2023 2074 6865 2073 616d 6520 6173     # the same as
+00006880: 7375 6d70 7469 6f6e 2061 6e64 2075 7365  sumption and use
+00006890: 2074 6865 7365 2063 6f6c 756d 6e73 2061   these columns a
+000068a0: 7320 7468 6520 746f 7461 6c20 6f72 6465  s the total orde
+000068b0: 7269 6e67 206b 6579 732e 0a20 2020 2020  ring keys..     
+000068c0: 2020 2070 7269 6d61 7279 5f6b 6579 7320     primary_keys 
+000068d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+000068e0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+000068f0: 2874 6162 6c65 5f63 6f6e 7374 7261 696e  (table_constrain
+00006900: 7473 203a 3d20 6765 7461 7474 7228 7461  ts := getattr(ta
+00006910: 626c 652c 2022 7461 626c 655f 636f 6e73  ble, "table_cons
+00006920: 7472 6169 6e74 7322 2c20 4e6f 6e65 2929  traints", None))
+00006930: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+00006940: 2020 2020 2020 2020 2061 6e64 2028 7072           and (pr
+00006950: 696d 6172 795f 6b65 7920 3a3d 2074 6162  imary_key := tab
+00006960: 6c65 5f63 6f6e 7374 7261 696e 7473 2e70  le_constraints.p
+00006970: 7269 6d61 7279 5f6b 6579 2920 6973 206e  rimary_key) is n
+00006980: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00006990: 2020 2020 2320 5468 6973 2077 696c 6c20      # This will 
+000069a0: 6265 2046 616c 7365 2066 6f72 2065 6974  be False for eit
+000069b0: 6865 7220 4e6f 6e65 206f 7220 656d 7074  her None or empt
+000069c0: 7920 6c69 7374 2e0a 2020 2020 2020 2020  y list..        
+000069d0: 2020 2020 2320 5765 2077 616e 7420 7072      # We want pr
+000069e0: 696d 6172 795f 6b65 7973 203d 204e 6f6e  imary_keys = Non
+000069f0: 6520 6966 206e 6f20 7072 696d 6172 7920  e if no primary 
+00006a00: 6b65 7973 2061 7265 2073 6574 2e0a 2020  keys are set..  
+00006a10: 2020 2020 2020 2020 2020 616e 6420 2863            and (c
+00006a20: 6f6c 756d 6e73 203a 3d20 7072 696d 6172  olumns := primar
+00006a30: 795f 6b65 792e 636f 6c75 6d6e 7329 0a20  y_key.columns). 
+00006a40: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00006a50: 2020 2020 2020 7072 696d 6172 795f 6b65        primary_ke
+00006a60: 7973 203d 2063 6f6c 756d 6e73 0a0a 2020  ys = columns..  
+00006a70: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00006a80: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
+00006a90: 7265 7373 696f 6e20 3d20 7365 6c66 2e69  ression = self.i
+00006aa0: 6269 735f 636c 6965 6e74 2e73 716c 280a  bis_client.sql(.
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 6269 6766 7261 6d65 735f 696f 2e63 7265  bigframes_io.cre
+00006ad0: 6174 655f 736e 6170 7368 6f74 5f73 716c  ate_snapshot_sql
+00006ae0: 2874 6162 6c65 2e72 6566 6572 656e 6365  (table.reference
+00006af0: 2c20 736e 6170 7368 6f74 5f74 696d 6573  , snapshot_times
+00006b00: 7461 6d70 290a 2020 2020 2020 2020 2020  tamp).          
+00006b10: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
+00006b20: 7074 2067 6f6f 676c 652e 6170 695f 636f  pt google.api_co
+00006b30: 7265 2e65 7863 6570 7469 6f6e 732e 466f  re.exceptions.Fo
+00006b40: 7262 6964 6465 6e20 6173 2065 783a 0a20  rbidden as ex:. 
+00006b50: 2020 2020 2020 2020 2020 2069 6620 2244             if "D
+00006b60: 7269 7665 2063 7265 6465 6e74 6961 6c73  rive credentials
+00006b70: 2220 696e 2065 782e 6d65 7373 6167 653a  " in ex.message:
+00006b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006b90: 2065 782e 6d65 7373 6167 6520 2b3d 2022   ex.message += "
+00006ba0: 5c6e 4368 6563 6b20 6874 7470 733a 2f2f  \nCheck https://
+00006bb0: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
+00006bc0: 2f62 6967 7175 6572 792f 646f 6373 2f71  /bigquery/docs/q
+00006bd0: 7565 7279 2d64 7269 7665 2d64 6174 6123  uery-drive-data#
+00006be0: 476f 6f67 6c65 5f44 7269 7665 5f70 6572  Google_Drive_per
+00006bf0: 6d69 7373 696f 6e73 2e22 0a20 2020 2020  missions.".     
+00006c00: 2020 2020 2020 2072 6169 7365 0a0a 2020         raise..  
+00006c10: 2020 2020 2020 7265 7475 726e 2074 6162        return tab
+00006c20: 6c65 5f65 7870 7265 7373 696f 6e2c 2070  le_expression, p
+00006c30: 7269 6d61 7279 5f6b 6579 730a 0a20 2020  rimary_keys..   
+00006c40: 2064 6566 205f 7265 6164 5f67 6271 5f74   def _read_gbq_t
+00006c50: 6162 6c65 280a 2020 2020 2020 2020 7365  able(.        se
+00006c60: 6c66 2c0a 2020 2020 2020 2020 7175 6572  lf,.        quer
+00006c70: 793a 2073 7472 2c0a 2020 2020 2020 2020  y: str,.        
+00006c80: 2a2c 0a20 2020 2020 2020 2069 6e64 6578  *,.        index
+00006c90: 5f63 6f6c 3a20 4974 6572 6162 6c65 5b73  _col: Iterable[s
+00006ca0: 7472 5d20 7c20 7374 7220 3d20 2829 2c0a  tr] | str = (),.
+00006cb0: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+00006cc0: 2049 7465 7261 626c 655b 7374 725d 203d   Iterable[str] =
+00006cd0: 2028 292c 0a20 2020 2020 2020 206d 6178   (),.        max
+00006ce0: 5f72 6573 756c 7473 3a20 4f70 7469 6f6e  _results: Option
+00006cf0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+00006d00: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
+00006d10: 3a20 7374 722c 0a20 2020 2020 2020 2075  : str,.        u
+00006d20: 7365 5f63 6163 6865 3a20 626f 6f6c 203d  se_cache: bool =
+00006d30: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
+00006d40: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
+00006d50: 616d 653a 0a20 2020 2020 2020 2069 6d70  ame:.        imp
+00006d60: 6f72 7420 6269 6766 7261 6d65 732e 6461  ort bigframes.da
+00006d70: 7461 6672 616d 6520 6173 2064 6174 6166  taframe as dataf
+00006d80: 7261 6d65 0a0a 2020 2020 2020 2020 6966  rame..        if
+00006d90: 206d 6178 5f72 6573 756c 7473 2061 6e64   max_results and
+00006da0: 206d 6178 5f72 6573 756c 7473 203c 3d20   max_results <= 
+00006db0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00006dc0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00006dd0: 2260 6d61 785f 7265 7375 6c74 7360 2073  "`max_results` s
+00006de0: 686f 756c 6420 6265 2061 2070 6f73 6974  hould be a posit
+00006df0: 6976 6520 6e75 6d62 6572 2e22 290a 0a20  ive number.").. 
+00006e00: 2020 2020 2020 2074 6162 6c65 5f72 6566         table_ref
+00006e10: 203d 2062 6967 7175 6572 792e 7461 626c   = bigquery.tabl
+00006e20: 652e 5461 626c 6552 6566 6572 656e 6365  e.TableReference
+00006e30: 2e66 726f 6d5f 7374 7269 6e67 280a 2020  .from_string(.  
+00006e40: 2020 2020 2020 2020 2020 7175 6572 792c            query,
+00006e50: 2064 6566 6175 6c74 5f70 726f 6a65 6374   default_project
+00006e60: 3d73 656c 662e 6271 636c 6965 6e74 2e70  =self.bqclient.p
+00006e70: 726f 6a65 6374 0a20 2020 2020 2020 2029  roject.        )
+00006e80: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
+00006e90: 3d20 7365 6c66 2e62 7163 6c69 656e 742e  = self.bqclient.
+00006ea0: 6765 745f 7461 626c 6528 7461 626c 655f  get_table(table_
+00006eb0: 7265 6629 0a20 2020 2020 2020 2028 7461  ref).        (ta
+00006ec0: 626c 655f 6578 7072 6573 7369 6f6e 2c20  ble_expression, 
+00006ed0: 7072 696d 6172 795f 6b65 7973 2c29 203d  primary_keys,) =
+00006ee0: 2073 656c 662e 5f67 6574 5f73 6e61 7073   self._get_snaps
+00006ef0: 686f 745f 7371 6c5f 616e 645f 7072 696d  hot_sql_and_prim
+00006f00: 6172 795f 6b65 7928 0a20 2020 2020 2020  ary_key(.       
+00006f10: 2020 2020 2074 6162 6c65 2c20 6170 695f       table, api_
+00006f20: 6e61 6d65 3d61 7069 5f6e 616d 652c 2075  name=api_name, u
+00006f30: 7365 5f63 6163 6865 3d75 7365 5f63 6163  se_cache=use_cac
+00006f40: 6865 0a20 2020 2020 2020 2029 0a20 2020  he.        ).   
+00006f50: 2020 2020 2074 6f74 616c 5f6f 7264 6572       total_order
+00006f60: 696e 675f 636f 6c73 203d 2070 7269 6d61  ing_cols = prima
+00006f70: 7279 5f6b 6579 730a 0a20 2020 2020 2020  ry_keys..       
+00006f80: 2069 6620 6e6f 7420 696e 6465 785f 636f   if not index_co
+00006f90: 6c20 616e 6420 7072 696d 6172 795f 6b65  l and primary_ke
+00006fa0: 7973 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ys is not None:.
+00006fb0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00006fc0: 785f 636f 6c20 3d20 7072 696d 6172 795f  x_col = primary_
+00006fd0: 6b65 7973 0a0a 2020 2020 2020 2020 666f  keys..        fo
+00006fe0: 7220 6b65 7920 696e 2063 6f6c 756d 6e73  r key in columns
+00006ff0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007000: 206b 6579 206e 6f74 2069 6e20 7461 626c   key not in tabl
+00007010: 655f 6578 7072 6573 7369 6f6e 2e63 6f6c  e_expression.col
+00007020: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
+00007030: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00007040: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00007050: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
+00007060: 6c75 6d6e 2027 7b6b 6579 7d27 206f 6620  lumn '{key}' of 
+00007070: 6063 6f6c 756d 6e73 6020 6e6f 7420 666f  `columns` not fo
+00007080: 756e 6420 696e 2074 6869 7320 7461 626c  und in this tabl
+00007090: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
+000070a0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+000070b0: 6620 6973 696e 7374 616e 6365 2869 6e64  f isinstance(ind
+000070c0: 6578 5f63 6f6c 2c20 7374 7229 3a0a 2020  ex_col, str):.  
+000070d0: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+000070e0: 636f 6c73 3a20 4c69 7374 5b73 7472 5d20  cols: List[str] 
+000070f0: 3d20 5b69 6e64 6578 5f63 6f6c 5d0a 2020  = [index_col].  
+00007100: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00007110: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
+00007120: 6c73 203d 206c 6973 7428 696e 6465 785f  ls = list(index_
+00007130: 636f 6c29 0a0a 2020 2020 2020 2020 666f  col)..        fo
+00007140: 7220 6b65 7920 696e 2069 6e64 6578 5f63  r key in index_c
+00007150: 6f6c 733a 0a20 2020 2020 2020 2020 2020  ols:.           
+00007160: 2069 6620 6b65 7920 6e6f 7420 696e 2074   if key not in t
+00007170: 6162 6c65 5f65 7870 7265 7373 696f 6e2e  able_expression.
+00007180: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
+00007190: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000071a0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000071c0: 2243 6f6c 756d 6e20 607b 6b65 797d 6020  "Column `{key}` 
+000071d0: 6f66 2060 696e 6465 785f 636f 6c60 206e  of `index_col` n
+000071e0: 6f74 2066 6f75 6e64 2069 6e20 7468 6973  ot found in this
+000071f0: 2074 6162 6c65 2e22 0a20 2020 2020 2020   table.".       
+00007200: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00007210: 2020 2020 6966 2063 6f6c 756d 6e73 3a0a      if columns:.
+00007220: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+00007230: 655f 6578 7072 6573 7369 6f6e 203d 2074  e_expression = t
+00007240: 6162 6c65 5f65 7870 7265 7373 696f 6e2e  able_expression.
+00007250: 7365 6c65 6374 285b 2a69 6e64 6578 5f63  select([*index_c
+00007260: 6f6c 732c 202a 636f 6c75 6d6e 735d 290a  ols, *columns]).
+00007270: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
+00007280: 6520 696e 6465 7820 6973 2075 6e69 7175  e index is uniqu
+00007290: 6520 616e 6420 736f 7274 6162 6c65 2c20  e and sortable, 
+000072a0: 7468 656e 2077 6520 646f 6e27 7420 6e65  then we don't ne
+000072b0: 6564 2074 6f20 6765 6e65 7261 7465 0a20  ed to generate. 
+000072c0: 2020 2020 2020 2023 2061 6e20 6f72 6465         # an orde
+000072d0: 7269 6e67 2063 6f6c 756d 6e2e 0a20 2020  ring column..   
+000072e0: 2020 2020 206f 7264 6572 696e 6720 3d20       ordering = 
+000072f0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00007300: 746f 7461 6c5f 6f72 6465 7269 6e67 5f63  total_ordering_c
+00007310: 6f6c 7320 6973 206e 6f74 204e 6f6e 653a  ols is not None:
+00007320: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
+00007330: 6f74 653a 2063 7572 7265 6e74 6c79 2c20  ote: currently, 
+00007340: 6120 7461 626c 6520 6861 7320 6120 746f  a table has a to
+00007350: 7461 6c20 6f72 6465 7269 6e67 206f 6e6c  tal ordering onl
+00007360: 7920 7768 656e 2074 6865 0a20 2020 2020  y when the.     
+00007370: 2020 2020 2020 2023 2070 7269 6d61 7279         # primary
+00007380: 206b 6579 2873 2920 6172 6520 7365 7420   key(s) are set 
+00007390: 6f6e 2061 2074 6162 6c65 2e20 5468 6520  on a table. The 
+000073a0: 7175 6572 7920 656e 6769 6e65 2061 7373  query engine ass
+000073b0: 756d 6573 2073 7563 680a 2020 2020 2020  umes such.      
+000073c0: 2020 2020 2020 2320 636f 6c75 6d6e 7320        # columns 
+000073d0: 6172 6520 756e 6971 7565 2c20 6576 656e  are unique, even
+000073e0: 2069 6620 6e6f 7420 656e 666f 7263 6564   if not enforced
+000073f0: 2e0a 2020 2020 2020 2020 2020 2020 6f72  ..            or
+00007400: 6465 7269 6e67 203d 206f 7264 6572 2e45  dering = order.E
+00007410: 7870 7265 7373 696f 6e4f 7264 6572 696e  xpressionOrderin
+00007420: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+00007430: 2020 206f 7264 6572 696e 675f 7661 6c75     ordering_valu
+00007440: 655f 636f 6c75 6d6e 733d 7475 706c 6528  e_columns=tuple(
+00007450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007460: 2020 2020 206f 7264 6572 2e61 7363 656e       order.ascen
+00007470: 6469 6e67 5f6f 7665 7228 636f 6c75 6d6e  ding_over(column
+00007480: 5f69 6429 2066 6f72 2063 6f6c 756d 6e5f  _id) for column_
+00007490: 6964 2069 6e20 746f 7461 6c5f 6f72 6465  id in total_orde
+000074a0: 7269 6e67 5f63 6f6c 730a 2020 2020 2020  ring_cols.      
+000074b0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+000074c0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
+000074d0: 616c 5f6f 7264 6572 696e 675f 636f 6c75  al_ordering_colu
+000074e0: 6d6e 733d 6672 6f7a 656e 7365 7428 746f  mns=frozenset(to
+000074f0: 7461 6c5f 6f72 6465 7269 6e67 5f63 6f6c  tal_ordering_col
+00007500: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00007510: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+00007520: 6c75 6d6e 5f76 616c 7565 7320 3d20 5b74  lumn_values = [t
+00007530: 6162 6c65 5f65 7870 7265 7373 696f 6e5b  able_expression[
+00007540: 636f 6c5d 2066 6f72 2063 6f6c 2069 6e20  col] for col in 
+00007550: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+00007560: 2e63 6f6c 756d 6e73 5d0a 2020 2020 2020  .columns].      
+00007570: 2020 2020 2020 6172 7261 795f 7661 6c75        array_valu
+00007580: 6520 3d20 636f 7265 2e41 7272 6179 5661  e = core.ArrayVa
+00007590: 6c75 652e 6672 6f6d 5f69 6269 7328 0a20  lue.from_ibis(. 
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000075b0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+000075c0: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
+000075d0: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
+000075e0: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
+000075f0: 6f6c 756d 6e5f 7661 6c75 6573 2c0a 2020  olumn_values,.  
+00007600: 2020 2020 2020 2020 2020 2020 2020 6869                hi
+00007610: 6464 656e 5f6f 7264 6572 696e 675f 636f  dden_ordering_co
+00007620: 6c75 6d6e 733d 5b5d 2c0a 2020 2020 2020  lumns=[],.      
+00007630: 2020 2020 2020 2020 2020 6f72 6465 7269            orderi
+00007640: 6e67 3d6f 7264 6572 696e 672c 0a20 2020  ng=ordering,.   
+00007650: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00007660: 2020 2020 656c 6966 206c 656e 2869 6e64      elif len(ind
+00007670: 6578 5f63 6f6c 7329 2021 3d20 303a 0a20  ex_cols) != 0:. 
+00007680: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+00007690: 6861 7665 2069 6e64 6578 2063 6f6c 756d  have index colum
+000076a0: 6e73 2c20 6c65 7473 2073 6565 2069 6620  ns, lets see if 
+000076b0: 7468 6f73 6520 6172 6520 6163 7475 616c  those are actual
+000076c0: 6c79 2074 6f74 616c 5f6f 7264 6572 5f63  ly total_order_c
+000076d0: 6f6c 756d 6e73 0a20 2020 2020 2020 2020  olumns.         
+000076e0: 2020 206f 7264 6572 696e 6720 3d20 6f72     ordering = or
+000076f0: 6465 722e 4578 7072 6573 7369 6f6e 4f72  der.ExpressionOr
+00007700: 6465 7269 6e67 280a 2020 2020 2020 2020  dering(.        
+00007710: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
+00007720: 5f76 616c 7565 5f63 6f6c 756d 6e73 3d74  _value_columns=t
+00007730: 7570 6c65 280a 2020 2020 2020 2020 2020  uple(.          
+00007740: 2020 2020 2020 2020 2020 5b6f 7264 6572            [order
+00007750: 2e61 7363 656e 6469 6e67 5f6f 7665 7228  .ascending_over(
+00007760: 636f 6c75 6d6e 5f69 6429 2066 6f72 2063  column_id) for c
+00007770: 6f6c 756d 6e5f 6964 2069 6e20 696e 6465  olumn_id in inde
+00007780: 785f 636f 6c73 5d0a 2020 2020 2020 2020  x_cols].        
+00007790: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+000077a0: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+000077b0: 5f6f 7264 6572 696e 675f 636f 6c75 6d6e  _ordering_column
+000077c0: 733d 6672 6f7a 656e 7365 7428 696e 6465  s=frozenset(inde
+000077d0: 785f 636f 6c73 292c 0a20 2020 2020 2020  x_cols),.       
+000077e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000077f0: 2020 2069 735f 746f 7461 6c5f 6f72 6465     is_total_orde
+00007800: 7269 6e67 203d 2073 656c 662e 5f63 6865  ring = self._che
+00007810: 636b 5f69 6e64 6578 5f75 6e69 7175 656e  ck_index_uniquen
+00007820: 6573 7328 0a20 2020 2020 2020 2020 2020  ess(.           
+00007830: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
+00007840: 7373 696f 6e2c 2069 6e64 6578 5f63 6f6c  ssion, index_col
+00007850: 730a 2020 2020 2020 2020 2020 2020 290a  s.            ).
+00007860: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007870: 735f 746f 7461 6c5f 6f72 6465 7269 6e67  s_total_ordering
+00007880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007890: 2020 636f 6c75 6d6e 5f76 616c 7565 7320    column_values 
+000078a0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+000078b0: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
+000078c0: 7072 6573 7369 6f6e 5b63 6f6c 5d20 666f  pression[col] fo
+000078d0: 7220 636f 6c20 696e 2074 6162 6c65 5f65  r col in table_e
+000078e0: 7870 7265 7373 696f 6e2e 636f 6c75 6d6e  xpression.column
+000078f0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00007900: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00007910: 2020 2020 6172 7261 795f 7661 6c75 6520      array_value 
+00007920: 3d20 636f 7265 2e41 7272 6179 5661 6c75  = core.ArrayValu
+00007930: 652e 6672 6f6d 5f69 6269 7328 0a20 2020  e.from_ibis(.   
+00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007950: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00007960: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00007970: 5f65 7870 7265 7373 696f 6e2c 0a20 2020  _expression,.   
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e5f   columns=column_
+000079a0: 7661 6c75 6573 2c0a 2020 2020 2020 2020  values,.        
+000079b0: 2020 2020 2020 2020 2020 2020 6869 6464              hidd
+000079c0: 656e 5f6f 7264 6572 696e 675f 636f 6c75  en_ordering_colu
+000079d0: 6d6e 733d 5b5d 2c0a 2020 2020 2020 2020  mns=[],.        
+000079e0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+000079f0: 7269 6e67 3d6f 7264 6572 696e 672c 0a20  ring=ordering,. 
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007a10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00007a20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007a30: 2020 2061 7272 6179 5f76 616c 7565 203d     array_value =
+00007a40: 2073 656c 662e 5f63 7265 6174 655f 746f   self._create_to
+00007a50: 7461 6c5f 6f72 6465 7269 6e67 280a 2020  tal_ordering(.  
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
+00007a80: 6f6e 2c20 7461 626c 655f 726f 7773 3d74  on, table_rows=t
+00007a90: 6162 6c65 2e6e 756d 5f72 6f77 730a 2020  able.num_rows.  
+00007aa0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00007ab0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00007ac0: 2020 2020 2020 2020 2020 6172 7261 795f            array_
+00007ad0: 7661 6c75 6520 3d20 7365 6c66 2e5f 6372  value = self._cr
+00007ae0: 6561 7465 5f74 6f74 616c 5f6f 7264 6572  eate_total_order
+00007af0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00007b00: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
+00007b10: 7373 696f 6e2c 2074 6162 6c65 5f72 6f77  ssion, table_row
+00007b20: 733d 7461 626c 652e 6e75 6d5f 726f 7773  s=table.num_rows
+00007b30: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00007b40: 2020 2020 2020 2020 7661 6c75 655f 636f          value_co
+00007b50: 6c75 6d6e 7320 3d20 5b63 6f6c 2066 6f72  lumns = [col for
+00007b60: 2063 6f6c 2069 6e20 6172 7261 795f 7661   col in array_va
+00007b70: 6c75 652e 636f 6c75 6d6e 5f69 6473 2069  lue.column_ids i
+00007b80: 6620 636f 6c20 6e6f 7420 696e 2069 6e64  f col not in ind
+00007b90: 6578 5f63 6f6c 735d 0a20 2020 2020 2020  ex_cols].       
+00007ba0: 2062 6c6f 636b 203d 2062 6c6f 636b 732e   block = blocks.
+00007bb0: 426c 6f63 6b28 0a20 2020 2020 2020 2020  Block(.         
+00007bc0: 2020 2061 7272 6179 5f76 616c 7565 2c0a     array_value,.
+00007bd0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00007be0: 785f 636f 6c75 6d6e 733d 696e 6465 785f  x_columns=index_
+00007bf0: 636f 6c73 2c0a 2020 2020 2020 2020 2020  cols,.          
+00007c00: 2020 636f 6c75 6d6e 5f6c 6162 656c 733d    column_labels=
+00007c10: 7661 6c75 655f 636f 6c75 6d6e 732c 0a20  value_columns,. 
+00007c20: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00007c30: 5f6c 6162 656c 733d 696e 6465 785f 636f  _labels=index_co
+00007c40: 6c73 2c0a 2020 2020 2020 2020 290a 2020  ls,.        ).  
+00007c50: 2020 2020 2020 6966 206d 6178 5f72 6573        if max_res
+00007c60: 756c 7473 3a0a 2020 2020 2020 2020 2020  ults:.          
+00007c70: 2020 626c 6f63 6b20 3d20 626c 6f63 6b2e    block = block.
+00007c80: 736c 6963 6528 7374 6f70 3d6d 6178 5f72  slice(stop=max_r
+00007c90: 6573 756c 7473 290a 2020 2020 2020 2020  esults).        
+00007ca0: 6466 203d 2064 6174 6166 7261 6d65 2e44  df = dataframe.D
+00007cb0: 6174 6146 7261 6d65 2862 6c6f 636b 290a  ataFrame(block).
+00007cc0: 0a20 2020 2020 2020 2023 2049 6620 7573  .        # If us
+00007cd0: 6572 2070 726f 7669 6465 6420 696e 6465  er provided inde
+00007ce0: 7820 636f 6c75 6d6e 732c 2073 686f 756c  x columns, shoul
+00007cf0: 6420 736f 7274 206f 7665 7220 6974 0a20  d sort over it. 
+00007d00: 2020 2020 2020 2069 6620 6c65 6e28 696e         if len(in
+00007d10: 6465 785f 636f 6c73 2920 3e20 303a 0a20  dex_cols) > 0:. 
+00007d20: 2020 2020 2020 2020 2020 2064 662e 736f             df.so
+00007d30: 7274 5f69 6e64 6578 2829 0a20 2020 2020  rt_index().     
+00007d40: 2020 2072 6574 7572 6e20 6466 0a0a 2020     return df..  
+00007d50: 2020 6465 6620 5f63 6865 636b 5f69 6e64    def _check_ind
+00007d60: 6578 5f75 6e69 7175 656e 6573 7328 0a20  ex_uniqueness(. 
+00007d70: 2020 2020 2020 2073 656c 662c 2074 6162         self, tab
+00007d80: 6c65 3a20 6962 6973 5f74 7970 6573 2e54  le: ibis_types.T
+00007d90: 6162 6c65 2c20 696e 6465 785f 636f 6c73  able, index_cols
+00007da0: 3a20 4c69 7374 5b73 7472 5d0a 2020 2020  : List[str].    
+00007db0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00007dc0: 2020 2064 6973 7469 6e63 745f 7461 626c     distinct_tabl
+00007dd0: 6520 3d20 7461 626c 652e 7365 6c65 6374  e = table.select
+00007de0: 282a 696e 6465 785f 636f 6c73 292e 6469  (*index_cols).di
+00007df0: 7374 696e 6374 2829 0a20 2020 2020 2020  stinct().       
+00007e00: 2069 735f 756e 6971 7565 5f73 716c 203d   is_unique_sql =
+00007e10: 2066 2222 2257 4954 4820 6675 6c6c 5f74   f"""WITH full_t
+00007e20: 6162 6c65 2041 5320 280a 2020 2020 2020  able AS (.      
+00007e30: 2020 2020 2020 7b73 656c 662e 6962 6973        {self.ibis
+00007e40: 5f63 6c69 656e 742e 636f 6d70 696c 6528  _client.compile(
+00007e50: 7461 626c 6529 7d0a 2020 2020 2020 2020  table)}.        
+00007e60: 292c 0a20 2020 2020 2020 2064 6973 7469  ),.        disti
+00007e70: 6e63 745f 7461 626c 6520 4153 2028 0a20  nct_table AS (. 
+00007e80: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
+00007e90: 2e69 6269 735f 636c 6965 6e74 2e63 6f6d  .ibis_client.com
+00007ea0: 7069 6c65 2864 6973 7469 6e63 745f 7461  pile(distinct_ta
+00007eb0: 626c 6529 7d0a 2020 2020 2020 2020 290a  ble)}.        ).
+00007ec0: 0a20 2020 2020 2020 2053 454c 4543 5420  .        SELECT 
+00007ed0: 2853 454c 4543 5420 434f 554e 5428 2a29  (SELECT COUNT(*)
+00007ee0: 2046 524f 4d20 6675 6c6c 5f74 6162 6c65   FROM full_table
+00007ef0: 2920 4153 2060 746f 7461 6c5f 636f 756e  ) AS `total_coun
+00007f00: 7460 2c0a 2020 2020 2020 2020 2853 454c  t`,.        (SEL
+00007f10: 4543 5420 434f 554e 5428 2a29 2046 524f  ECT COUNT(*) FRO
+00007f20: 4d20 6469 7374 696e 6374 5f74 6162 6c65  M distinct_table
+00007f30: 2920 4153 2060 6469 7374 696e 6374 5f63  ) AS `distinct_c
+00007f40: 6f75 6e74 600a 2020 2020 2020 2020 2222  ount`.        ""
+00007f50: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
+00007f60: 732c 205f 203d 2073 656c 662e 5f73 7461  s, _ = self._sta
+00007f70: 7274 5f71 7565 7279 2869 735f 756e 6971  rt_query(is_uniq
+00007f80: 7565 5f73 716c 290a 2020 2020 2020 2020  ue_sql).        
+00007f90: 726f 7720 3d20 6e65 7874 2869 7465 7228  row = next(iter(
+00007fa0: 7265 7375 6c74 7329 290a 0a20 2020 2020  results))..     
+00007fb0: 2020 2074 6f74 616c 5f63 6f75 6e74 203d     total_count =
+00007fc0: 2072 6f77 5b22 746f 7461 6c5f 636f 756e   row["total_coun
+00007fd0: 7422 5d0a 2020 2020 2020 2020 6469 7374  t"].        dist
+00007fe0: 696e 6374 5f63 6f75 6e74 203d 2072 6f77  inct_count = row
+00007ff0: 5b22 6469 7374 696e 6374 5f63 6f75 6e74  ["distinct_count
+00008000: 225d 0a20 2020 2020 2020 2072 6574 7572  "].        retur
+00008010: 6e20 746f 7461 6c5f 636f 756e 7420 3d3d  n total_count ==
+00008020: 2064 6973 7469 6e63 745f 636f 756e 740a   distinct_count.
+00008030: 0a20 2020 2064 6566 205f 7265 6164 5f62  .    def _read_b
+00008040: 6967 7175 6572 795f 6c6f 6164 5f6a 6f62  igquery_load_job
+00008050: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00008060: 2020 2020 2020 2020 6669 6c65 7061 7468          filepath
+00008070: 5f6f 725f 6275 6666 6572 3a20 7374 7220  _or_buffer: str 
+00008080: 7c20 494f 5b22 6279 7465 7322 5d2c 0a20  | IO["bytes"],. 
+00008090: 2020 2020 2020 2074 6162 6c65 3a20 556e         table: Un
+000080a0: 696f 6e5b 6269 6771 7565 7279 2e54 6162  ion[bigquery.Tab
+000080b0: 6c65 2c20 6269 6771 7565 7279 2e54 6162  le, bigquery.Tab
+000080c0: 6c65 5265 6665 7265 6e63 655d 2c0a 2020  leReference],.  
+000080d0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+000080e0: 206a 6f62 5f63 6f6e 6669 673a 2062 6967   job_config: big
+000080f0: 7175 6572 792e 4c6f 6164 4a6f 6243 6f6e  query.LoadJobCon
+00008100: 6669 672c 0a20 2020 2020 2020 2069 6e64  fig,.        ind
+00008110: 6578 5f63 6f6c 3a20 4974 6572 6162 6c65  ex_col: Iterable
+00008120: 5b73 7472 5d20 7c20 7374 7220 3d20 2829  [str] | str = ()
+00008130: 2c0a 2020 2020 2020 2020 636f 6c75 6d6e  ,.        column
+00008140: 733a 2049 7465 7261 626c 655b 7374 725d  s: Iterable[str]
+00008150: 203d 2028 292c 0a20 2020 2029 202d 3e20   = (),.    ) -> 
+00008160: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
+00008170: 616d 653a 0a20 2020 2020 2020 2069 6620  ame:.        if 
+00008180: 6973 696e 7374 616e 6365 2869 6e64 6578  isinstance(index
+00008190: 5f63 6f6c 2c20 7374 7229 3a0a 2020 2020  _col, str):.    
+000081a0: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
+000081b0: 6c73 203d 205b 696e 6465 785f 636f 6c5d  ls = [index_col]
+000081c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000081d0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+000081e0: 5f63 6f6c 7320 3d20 6c69 7374 2869 6e64  _cols = list(ind
+000081f0: 6578 5f63 6f6c 290a 0a20 2020 2020 2020  ex_col)..       
+00008200: 2069 6620 6e6f 7420 6a6f 625f 636f 6e66   if not job_conf
+00008210: 6967 2e63 6c75 7374 6572 696e 675f 6669  ig.clustering_fi
+00008220: 656c 6473 2061 6e64 2069 6e64 6578 5f63  elds and index_c
+00008230: 6f6c 733a 0a20 2020 2020 2020 2020 2020  ols:.           
+00008240: 206a 6f62 5f63 6f6e 6669 672e 636c 7573   job_config.clus
+00008250: 7465 7269 6e67 5f66 6965 6c64 7320 3d20  tering_fields = 
+00008260: 696e 6465 785f 636f 6c73 5b3a 5f4d 4158  index_cols[:_MAX
+00008270: 5f43 4c55 5354 4552 5f43 4f4c 554d 4e53  _CLUSTER_COLUMNS
+00008280: 5d0a 0a20 2020 2020 2020 2069 6620 6973  ]..        if is
+00008290: 696e 7374 616e 6365 2866 696c 6570 6174  instance(filepat
+000082a0: 685f 6f72 5f62 7566 6665 722c 2073 7472  h_or_buffer, str
+000082b0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+000082c0: 6620 6669 6c65 7061 7468 5f6f 725f 6275  f filepath_or_bu
+000082d0: 6666 6572 2e73 7461 7274 7377 6974 6828  ffer.startswith(
+000082e0: 2267 733a 2f2f 2229 3a0a 2020 2020 2020  "gs://"):.      
+000082f0: 2020 2020 2020 2020 2020 6c6f 6164 5f6a            load_j
+00008300: 6f62 203d 2073 656c 662e 6271 636c 6965  ob = self.bqclie
+00008310: 6e74 2e6c 6f61 645f 7461 626c 655f 6672  nt.load_table_fr
+00008320: 6f6d 5f75 7269 280a 2020 2020 2020 2020  om_uri(.        
+00008330: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00008340: 7061 7468 5f6f 725f 6275 6666 6572 2c20  path_or_buffer, 
+00008350: 7461 626c 652c 206a 6f62 5f63 6f6e 6669  table, job_confi
+00008360: 673d 6a6f 625f 636f 6e66 6967 0a20 2020  g=job_config.   
+00008370: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00008380: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00008390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000083a0: 2077 6974 6820 6f70 656e 2866 696c 6570   with open(filep
+000083b0: 6174 685f 6f72 5f62 7566 6665 722c 2022  ath_or_buffer, "
+000083c0: 7262 2229 2061 7320 736f 7572 6365 5f66  rb") as source_f
+000083d0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
+000083e0: 2020 2020 2020 2020 206c 6f61 645f 6a6f           load_jo
+000083f0: 6220 3d20 7365 6c66 2e62 7163 6c69 656e  b = self.bqclien
+00008400: 742e 6c6f 6164 5f74 6162 6c65 5f66 726f  t.load_table_fro
+00008410: 6d5f 6669 6c65 280a 2020 2020 2020 2020  m_file(.        
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008430: 736f 7572 6365 5f66 696c 652c 2074 6162  source_file, tab
+00008440: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
+00008450: 6f62 5f63 6f6e 6669 670a 2020 2020 2020  ob_config.      
+00008460: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00008470: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008480: 2020 2020 2020 2020 2020 6c6f 6164 5f6a            load_j
+00008490: 6f62 203d 2073 656c 662e 6271 636c 6965  ob = self.bqclie
+000084a0: 6e74 2e6c 6f61 645f 7461 626c 655f 6672  nt.load_table_fr
+000084b0: 6f6d 5f66 696c 6528 0a20 2020 2020 2020  om_file(.       
+000084c0: 2020 2020 2020 2020 2066 696c 6570 6174           filepat
+000084d0: 685f 6f72 5f62 7566 6665 722c 2074 6162  h_or_buffer, tab
+000084e0: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
+000084f0: 6f62 5f63 6f6e 6669 670a 2020 2020 2020  ob_config.      
+00008500: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00008510: 2073 656c 662e 5f73 7461 7274 5f67 656e   self._start_gen
+00008520: 6572 6963 5f6a 6f62 286c 6f61 645f 6a6f  eric_job(load_jo
+00008530: 6229 0a20 2020 2020 2020 2074 6162 6c65  b).        table
+00008540: 5f69 6420 3d20 6622 7b74 6162 6c65 2e70  _id = f"{table.p
+00008550: 726f 6a65 6374 7d2e 7b74 6162 6c65 2e64  roject}.{table.d
+00008560: 6174 6173 6574 5f69 647d 2e7b 7461 626c  ataset_id}.{tabl
+00008570: 652e 7461 626c 655f 6964 7d22 0a0a 2020  e.table_id}"..  
+00008580: 2020 2020 2020 2320 5570 6461 7465 2074        # Update t
+00008590: 6865 2074 6162 6c65 2065 7870 6972 6174  he table expirat
+000085a0: 696f 6e20 736f 2077 6520 6172 656e 2774  ion so we aren't
+000085b0: 206c 696d 6974 6564 2074 6f20 7468 6520   limited to the 
+000085c0: 6465 6661 756c 7420 3234 0a20 2020 2020  default 24.     
+000085d0: 2020 2023 2068 6f75 7273 206f 6620 7468     # hours of th
+000085e0: 6520 616e 6f6e 796d 6f75 7320 6461 7461  e anonymous data
+000085f0: 7365 742e 0a20 2020 2020 2020 2074 6162  set..        tab
+00008600: 6c65 5f65 7870 6972 6174 696f 6e20 3d20  le_expiration = 
+00008610: 6269 6771 7565 7279 2e54 6162 6c65 2874  bigquery.Table(t
+00008620: 6162 6c65 5f69 6429 0a20 2020 2020 2020  able_id).       
+00008630: 2074 6162 6c65 5f65 7870 6972 6174 696f   table_expiratio
+00008640: 6e2e 6578 7069 7265 7320 3d20 280a 2020  n.expires = (.  
+00008650: 2020 2020 2020 2020 2020 6461 7465 7469            dateti
+00008660: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
+00008670: 6461 7465 7469 6d65 2e74 696d 657a 6f6e  datetime.timezon
+00008680: 652e 7574 6329 202b 2063 6f6e 7374 616e  e.utc) + constan
+00008690: 7473 2e44 4546 4155 4c54 5f45 5850 4952  ts.DEFAULT_EXPIR
+000086a0: 4154 494f 4e0a 2020 2020 2020 2020 290a  ATION.        ).
+000086b0: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
+000086c0: 6c69 656e 742e 7570 6461 7465 5f74 6162  lient.update_tab
+000086d0: 6c65 2874 6162 6c65 5f65 7870 6972 6174  le(table_expirat
+000086e0: 696f 6e2c 205b 2265 7870 6972 6573 225d  ion, ["expires"]
+000086f0: 290a 0a20 2020 2020 2020 2023 2054 6865  )..        # The
+00008700: 2042 6967 5175 6572 7920 5245 5354 2041   BigQuery REST A
+00008710: 5049 2066 6f72 2074 6162 6c65 732e 6765  PI for tables.ge
+00008720: 7420 646f 6573 6e27 7420 7461 6b65 2061  t doesn't take a
+00008730: 2073 6573 7369 6f6e 2049 442c 2073 6f20   session ID, so 
+00008740: 7765 0a20 2020 2020 2020 2023 2063 616e  we.        # can
+00008750: 2774 2067 6574 2074 6865 2073 6368 656d  't get the schem
+00008760: 6120 666f 7220 6120 7465 6d70 2074 6162  a for a temp tab
+00008770: 6c65 2074 6861 7420 7761 792e 0a20 2020  le that way..   
+00008780: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00008790: 2e72 6561 645f 6762 715f 7461 626c 6528  .read_gbq_table(
+000087a0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+000087b0: 6c65 5f69 642c 0a20 2020 2020 2020 2020  le_id,.         
+000087c0: 2020 2069 6e64 6578 5f63 6f6c 3d69 6e64     index_col=ind
+000087d0: 6578 5f63 6f6c 2c0a 2020 2020 2020 2020  ex_col,.        
+000087e0: 2020 2020 636f 6c75 6d6e 733d 636f 6c75      columns=colu
+000087f0: 6d6e 732c 0a20 2020 2020 2020 2029 0a0a  mns,.        )..
+00008800: 2020 2020 6465 6620 7265 6164 5f67 6271      def read_gbq
+00008810: 5f6d 6f64 656c 2873 656c 662c 206d 6f64  _model(self, mod
+00008820: 656c 5f6e 616d 653a 2073 7472 293a 0a20  el_name: str):. 
+00008830: 2020 2020 2020 2022 2222 4c6f 6164 7320         """Loads 
+00008840: 6120 4269 6751 7565 7279 204d 4c20 6d6f  a BigQuery ML mo
+00008850: 6465 6c20 6672 6f6d 2042 6967 5175 6572  del from BigQuer
+00008860: 792e 0a0a 2020 2020 2020 2020 2a2a 4578  y...        **Ex
+00008870: 616d 706c 6573 3a2a 2a0a 0a20 2020 2020  amples:**..     
+00008880: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00008890: 7420 6269 6766 7261 6d65 732e 7061 6e64  t bigframes.pand
+000088a0: 6173 2061 7320 6270 640a 2020 2020 2020  as as bpd.      
+000088b0: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
+000088c0: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
+000088d0: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
+000088e0: 650a 0a20 2020 2020 2020 2052 6561 6420  e..        Read 
+000088f0: 616e 2065 7869 7374 696e 6720 4269 6751  an existing BigQ
+00008900: 7565 7279 204d 4c20 6d6f 6465 6c2e 0a0a  uery ML model...
+00008910: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00008920: 6d6f 6465 6c5f 6e61 6d65 203d 2022 6269  model_name = "bi
+00008930: 6766 7261 6d65 732d 6465 762e 6271 6d6c  gframes-dev.bqml
+00008940: 5f74 7574 6f72 6961 6c2e 7065 6e67 7569  _tutorial.pengui
+00008950: 6e73 5f6d 6f64 656c 220a 2020 2020 2020  ns_model".      
+00008960: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c20        >>> model 
+00008970: 3d20 6270 642e 7265 6164 5f67 6271 5f6d  = bpd.read_gbq_m
+00008980: 6f64 656c 286d 6f64 656c 5f6e 616d 6529  odel(model_name)
+00008990: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000089a0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+000089b0: 6c5f 6e61 6d65 2028 7374 7229 3a0a 2020  l_name (str):.  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+000089d0: 6520 6d6f 6465 6c27 7320 6e61 6d65 2069  e model's name i
+000089e0: 6e20 4269 6751 7565 7279 2069 6e20 7468  n BigQuery in th
+000089f0: 6520 666f 726d 6174 0a20 2020 2020 2020  e format.       
+00008a00: 2020 2020 2020 2020 2060 7072 6f6a 6563           `projec
+00008a10: 745f 6964 2e64 6174 6173 6574 5f69 642e  t_id.dataset_id.
+00008a20: 6d6f 6465 6c5f 6964 602c 206f 7220 6a75  model_id`, or ju
+00008a30: 7374 2060 6461 7461 7365 745f 6964 2e6d  st `dataset_id.m
+00008a40: 6f64 656c 5f69 6460 0a20 2020 2020 2020  odel_id`.       
+00008a50: 2020 2020 2020 2020 2074 6f20 6c6f 6164           to load
+00008a60: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
+00008a70: 7420 7072 6f6a 6563 742e 0a0a 2020 2020  t project...    
+00008a80: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00008a90: 2020 2020 2020 2020 2041 2062 6967 6672           A bigfr
+00008aa0: 616d 6573 2e6d 6c20 4d6f 6465 6c2c 2054  ames.ml Model, T
+00008ab0: 7261 6e73 666f 726d 6572 206f 7220 5069  ransformer or Pi
+00008ac0: 7065 6c69 6e65 2077 7261 7070 696e 6720  peline wrapping 
+00008ad0: 7468 6520 6d6f 6465 6c2e 0a20 2020 2020  the model..     
+00008ae0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00008af0: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
+00008b00: 6d6c 2e6c 6f61 6465 720a 0a20 2020 2020  ml.loader..     
+00008b10: 2020 206d 6f64 656c 5f72 6566 203d 2062     model_ref = b
+00008b20: 6967 7175 6572 792e 4d6f 6465 6c52 6566  igquery.ModelRef
+00008b30: 6572 656e 6365 2e66 726f 6d5f 7374 7269  erence.from_stri
+00008b40: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00008b50: 6d6f 6465 6c5f 6e61 6d65 2c20 6465 6661  model_name, defa
+00008b60: 756c 745f 7072 6f6a 6563 743d 7365 6c66  ult_project=self
+00008b70: 2e62 7163 6c69 656e 742e 7072 6f6a 6563  .bqclient.projec
+00008b80: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
+00008b90: 2020 2020 6d6f 6465 6c20 3d20 7365 6c66      model = self
+00008ba0: 2e62 7163 6c69 656e 742e 6765 745f 6d6f  .bqclient.get_mo
+00008bb0: 6465 6c28 6d6f 6465 6c5f 7265 6629 0a20  del(model_ref). 
+00008bc0: 2020 2020 2020 2072 6574 7572 6e20 6269         return bi
+00008bd0: 6766 7261 6d65 732e 6d6c 2e6c 6f61 6465  gframes.ml.loade
+00008be0: 722e 6672 6f6d 5f62 7128 7365 6c66 2c20  r.from_bq(self, 
+00008bf0: 6d6f 6465 6c29 0a0a 2020 2020 4074 7970  model)..    @typ
+00008c00: 696e 672e 6f76 6572 6c6f 6164 0a20 2020  ing.overload.   
+00008c10: 2064 6566 2072 6561 645f 7061 6e64 6173   def read_pandas
+00008c20: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00008c30: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+00008c40: 3a20 7061 6e64 6173 2e49 6e64 6578 0a20  : pandas.Index. 
+00008c50: 2020 2029 202d 3e20 6269 6766 7261 6d65     ) -> bigframe
+00008c60: 732e 636f 7265 2e69 6e64 6578 6573 2e49  s.core.indexes.I
+00008c70: 6e64 6578 3a0a 2020 2020 2020 2020 2e2e  ndex:.        ..
+00008c80: 2e0a 0a20 2020 2040 7479 7069 6e67 2e6f  ...    @typing.o
+00008c90: 7665 726c 6f61 640a 2020 2020 6465 6620  verload.    def 
+00008ca0: 7265 6164 5f70 616e 6461 7328 7365 6c66  read_pandas(self
+00008cb0: 2c20 7061 6e64 6173 5f64 6174 6166 7261  , pandas_datafra
+00008cc0: 6d65 3a20 7061 6e64 6173 2e53 6572 6965  me: pandas.Serie
+00008cd0: 7329 202d 3e20 6269 6766 7261 6d65 732e  s) -> bigframes.
+00008ce0: 7365 7269 6573 2e53 6572 6965 733a 0a20  series.Series:. 
+00008cf0: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
+00008d00: 4074 7970 696e 672e 6f76 6572 6c6f 6164  @typing.overload
+00008d10: 0a20 2020 2064 6566 2072 6561 645f 7061  .    def read_pa
+00008d20: 6e64 6173 2873 656c 662c 2070 616e 6461  ndas(self, panda
+00008d30: 735f 6461 7461 6672 616d 653a 2070 616e  s_dataframe: pan
+00008d40: 6461 732e 4461 7461 4672 616d 6529 202d  das.DataFrame) -
+00008d50: 3e20 6461 7461 6672 616d 652e 4461 7461  > dataframe.Data
+00008d60: 4672 616d 653a 0a20 2020 2020 2020 202e  Frame:.        .
+00008d70: 2e2e 0a0a 2020 2020 6465 6620 7265 6164  ....    def read
+00008d80: 5f70 616e 6461 7328 0a20 2020 2020 2020  _pandas(.       
+00008d90: 2073 656c 662c 2070 616e 6461 735f 6461   self, pandas_da
+00008da0: 7461 6672 616d 653a 2055 6e69 6f6e 5b70  taframe: Union[p
+00008db0: 616e 6461 732e 4461 7461 4672 616d 652c  andas.DataFrame,
+00008dc0: 2070 616e 6461 732e 5365 7269 6573 2c20   pandas.Series, 
+00008dd0: 7061 6e64 6173 2e49 6e64 6578 5d0a 2020  pandas.Index].  
+00008de0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+00008df0: 4c6f 6164 7320 4461 7461 4672 616d 6520  Loads DataFrame 
+00008e00: 6672 6f6d 2061 2070 616e 6461 7320 4461  from a pandas Da
+00008e10: 7461 4672 616d 652e 0a0a 2020 2020 2020  taFrame...      
+00008e20: 2020 5468 6520 7061 6e64 6173 2044 6174    The pandas Dat
+00008e30: 6146 7261 6d65 2077 696c 6c20 6265 2070  aFrame will be p
+00008e40: 6572 7369 7374 6564 2061 7320 6120 7465  ersisted as a te
+00008e50: 6d70 6f72 6172 7920 4269 6751 7565 7279  mporary BigQuery
+00008e60: 2074 6162 6c65 2c20 7768 6963 6820 6361   table, which ca
+00008e70: 6e20 6265 0a20 2020 2020 2020 2061 7574  n be.        aut
+00008e80: 6f6d 6174 6963 616c 6c79 2072 6563 7963  omatically recyc
+00008e90: 6c65 6420 6166 7465 7220 7468 6520 5365  led after the Se
+00008ea0: 7373 696f 6e20 6973 2063 6c6f 7365 642e  ssion is closed.
+00008eb0: 0a0a 2020 2020 2020 2020 2a2a 4578 616d  ..        **Exam
+00008ec0: 706c 6573 3a2a 2a0a 0a20 2020 2020 2020  ples:**..       
+00008ed0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+00008ee0: 6269 6766 7261 6d65 732e 7061 6e64 6173  bigframes.pandas
+00008ef0: 2061 7320 6270 640a 2020 2020 2020 2020   as bpd.        
+00008f00: 2020 2020 3e3e 3e20 696d 706f 7274 2070      >>> import p
+00008f10: 616e 6461 7320 6173 2070 640a 2020 2020  andas as pd.    
+00008f20: 2020 2020 2020 2020 3e3e 3e20 6270 642e          >>> bpd.
+00008f30: 6f70 7469 6f6e 732e 6469 7370 6c61 792e  options.display.
+00008f40: 7072 6f67 7265 7373 5f62 6172 203d 204e  progress_bar = N
+00008f50: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
+00008f60: 203e 3e3e 2064 203d 207b 2763 6f6c 3127   >>> d = {'col1'
+00008f70: 3a20 5b31 2c20 325d 2c20 2763 6f6c 3227  : [1, 2], 'col2'
+00008f80: 3a20 5b33 2c20 345d 7d0a 2020 2020 2020  : [3, 4]}.      
+00008f90: 2020 2020 2020 3e3e 3e20 7061 6e64 6173        >>> pandas
+00008fa0: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
+00008fb0: 6d65 2864 6174 613d 6429 0a20 2020 2020  me(data=d).     
+00008fc0: 2020 2020 2020 203e 3e3e 2064 6620 3d20         >>> df = 
+00008fd0: 6270 642e 7265 6164 5f70 616e 6461 7328  bpd.read_pandas(
+00008fe0: 7061 6e64 6173 5f64 6629 0a20 2020 2020  pandas_df).     
+00008ff0: 2020 2020 2020 203e 3e3e 2064 660a 2020         >>> df.  
+00009000: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00009010: 3120 2063 6f6c 320a 2020 2020 2020 2020  1  col2.        
+00009020: 2020 2020 3020 2020 2020 3120 2020 2020      0     1     
+00009030: 330a 2020 2020 2020 2020 2020 2020 3120  3.            1 
+00009040: 2020 2020 3220 2020 2020 340a 2020 2020      2     4.    
+00009050: 2020 2020 2020 2020 3c42 4c41 4e4b 4c49          <BLANKLI
+00009060: 4e45 3e0a 2020 2020 2020 2020 2020 2020  NE>.            
+00009070: 5b32 2072 6f77 7320 7820 3220 636f 6c75  [2 rows x 2 colu
+00009080: 6d6e 735d 0a0a 2020 2020 2020 2020 4172  mns]..        Ar
+00009090: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000090a0: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+000090b0: 2028 7061 6e64 6173 2e44 6174 6146 7261   (pandas.DataFra
+000090c0: 6d65 2c20 7061 6e64 6173 2e53 6572 6965  me, pandas.Serie
+000090d0: 732c 206f 7220 7061 6e64 6173 2e49 6e64  s, or pandas.Ind
+000090e0: 6578 293a 0a20 2020 2020 2020 2020 2020  ex):.           
+000090f0: 2020 2020 2061 2070 616e 6461 7320 4461       a pandas Da
+00009100: 7461 4672 616d 652f 5365 7269 6573 2f49  taFrame/Series/I
+00009110: 6e64 6578 206f 626a 6563 7420 746f 2062  ndex object to b
+00009120: 6520 6c6f 6164 6564 2e0a 0a20 2020 2020  e loaded...     
+00009130: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00009140: 2020 2020 2020 2020 416e 2065 7175 6976          An equiv
+00009150: 616c 656e 7420 6269 6766 7261 6d65 732e  alent bigframes.
+00009160: 7061 6e64 6173 2e28 4461 7461 4672 616d  pandas.(DataFram
+00009170: 652f 5365 7269 6573 2f49 6e64 6578 2920  e/Series/Index) 
+00009180: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+00009190: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
+000091a0: 7420 6269 6766 7261 6d65 732e 7365 7269  t bigframes.seri
+000091b0: 6573 2061 7320 7365 7269 6573 0a0a 2020  es as series..  
+000091c0: 2020 2020 2020 2320 5472 7920 746f 2068        # Try to h
+000091d0: 616e 646c 6520 6e6f 6e2d 6461 7461 6672  andle non-datafr
+000091e0: 616d 6520 7061 6e64 6173 206f 626a 6563  ame pandas objec
+000091f0: 7473 2061 7320 7765 6c6c 0a20 2020 2020  ts as well.     
+00009200: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00009210: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
+00009220: 652c 2070 616e 6461 732e 5365 7269 6573  e, pandas.Series
+00009230: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
+00009240: 665f 6466 203d 2073 656c 662e 5f72 6561  f_df = self._rea
+00009250: 645f 7061 6e64 6173 2870 616e 6461 732e  d_pandas(pandas.
+00009260: 4461 7461 4672 616d 6528 7061 6e64 6173  DataFrame(pandas
+00009270: 5f64 6174 6166 7261 6d65 292c 2022 7265  _dataframe), "re
+00009280: 6164 5f70 616e 6461 7322 290a 2020 2020  ad_pandas").    
+00009290: 2020 2020 2020 2020 6266 5f73 6572 6965          bf_serie
+000092a0: 7320 3d20 7479 7069 6e67 2e63 6173 7428  s = typing.cast(
+000092b0: 7365 7269 6573 2e53 6572 6965 732c 2062  series.Series, b
+000092c0: 665f 6466 5b62 665f 6466 2e63 6f6c 756d  f_df[bf_df.colum
+000092d0: 6e73 5b30 5d5d 290a 2020 2020 2020 2020  ns[0]]).        
+000092e0: 2020 2020 2320 7772 6170 7069 6e67 2069      # wrapping i
+000092f0: 6e74 6f20 6466 2063 616e 2073 6574 206e  nto df can set n
+00009300: 616d 6520 746f 2030 2073 6f20 7265 7365  ame to 0 so rese
+00009310: 7420 746f 206f 7269 6769 6e61 6c20 6f62  t to original ob
+00009320: 6a65 6374 206e 616d 650a 2020 2020 2020  ject name.      
+00009330: 2020 2020 2020 6266 5f73 6572 6965 732e        bf_series.
+00009340: 6e61 6d65 203d 2070 616e 6461 735f 6461  name = pandas_da
+00009350: 7461 6672 616d 652e 6e61 6d65 0a20 2020  taframe.name.   
+00009360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009370: 6266 5f73 6572 6965 730a 2020 2020 2020  bf_series.      
+00009380: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00009390: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+000093a0: 2c20 7061 6e64 6173 2e49 6e64 6578 293a  , pandas.Index):
+000093b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000093c0: 7572 6e20 7365 6c66 2e5f 7265 6164 5f70  urn self._read_p
+000093d0: 616e 6461 7328 0a20 2020 2020 2020 2020  andas(.         
+000093e0: 2020 2020 2020 2070 616e 6461 732e 4461         pandas.Da
+000093f0: 7461 4672 616d 6528 696e 6465 783d 7061  taFrame(index=pa
+00009400: 6e64 6173 5f64 6174 6166 7261 6d65 292c  ndas_dataframe),
+00009410: 2022 7265 6164 5f70 616e 6461 7322 0a20   "read_pandas". 
+00009420: 2020 2020 2020 2020 2020 2029 2e69 6e64             ).ind
+00009430: 6578 0a20 2020 2020 2020 2069 6620 6973  ex.        if is
+00009440: 696e 7374 616e 6365 2870 616e 6461 735f  instance(pandas_
+00009450: 6461 7461 6672 616d 652c 2070 616e 6461  dataframe, panda
+00009460: 732e 4461 7461 4672 616d 6529 3a0a 2020  s.DataFrame):.  
+00009470: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009480: 2073 656c 662e 5f72 6561 645f 7061 6e64   self._read_pand
+00009490: 6173 2870 616e 6461 735f 6461 7461 6672  as(pandas_datafr
+000094a0: 616d 652c 2022 7265 6164 5f70 616e 6461  ame, "read_panda
+000094b0: 7322 290a 2020 2020 2020 2020 656c 7365  s").        else
+000094c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000094d0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 6622 7265 6164 5f70 616e 6461 7328 2920  f"read_pandas() 
+00009500: 6578 7065 6374 7320 6120 7061 6e64 6173  expects a pandas
+00009510: 2e44 6174 6146 7261 6d65 2c20 6275 7420  .DataFrame, but 
+00009520: 676f 7420 6120 7b74 7970 6528 7061 6e64  got a {type(pand
+00009530: 6173 5f64 6174 6166 7261 6d65 297d 220a  as_dataframe)}".
+00009540: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00009550: 2020 2064 6566 205f 7265 6164 5f70 616e     def _read_pan
+00009560: 6461 7328 0a20 2020 2020 2020 2073 656c  das(.        sel
+00009570: 662c 2070 616e 6461 735f 6461 7461 6672  f, pandas_datafr
+00009580: 616d 653a 2070 616e 6461 732e 4461 7461  ame: pandas.Data
+00009590: 4672 616d 652c 2061 7069 5f6e 616d 653a  Frame, api_name:
+000095a0: 2073 7472 0a20 2020 2029 202d 3e20 6461   str.    ) -> da
+000095b0: 7461 6672 616d 652e 4461 7461 4672 616d  taframe.DataFram
+000095c0: 653a 0a20 2020 2020 2020 2069 6d70 6f72  e:.        impor
+000095d0: 7420 6269 6766 7261 6d65 732e 6461 7461  t bigframes.data
+000095e0: 6672 616d 6520 6173 2064 6174 6166 7261  frame as datafra
+000095f0: 6d65 0a0a 2020 2020 2020 2020 6966 2069  me..        if i
+00009600: 7369 6e73 7461 6e63 6528 7061 6e64 6173  sinstance(pandas
+00009610: 5f64 6174 6166 7261 6d65 2c20 6461 7461  _dataframe, data
+00009620: 6672 616d 652e 4461 7461 4672 616d 6529  frame.DataFrame)
+00009630: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00009640: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009660: 2272 6561 645f 7061 6e64 6173 2829 2065  "read_pandas() e
+00009670: 7870 6563 7473 2061 2070 616e 6461 732e  xpects a pandas.
+00009680: 4461 7461 4672 616d 652c 2062 7574 2067  DataFrame, but g
+00009690: 6f74 2061 2022 0a20 2020 2020 2020 2020  ot a ".         
+000096a0: 2020 2020 2020 2022 6269 6766 7261 6d65         "bigframe
+000096b0: 732e 7061 6e64 6173 2e44 6174 6146 7261  s.pandas.DataFra
+000096c0: 6d65 2e22 0a20 2020 2020 2020 2020 2020  me.".           
+000096d0: 2029 0a0a 2020 2020 2020 2020 696e 6c69   )..        inli
+000096e0: 6e65 5f64 6620 3d20 7365 6c66 2e5f 7265  ne_df = self._re
+000096f0: 6164 5f70 616e 6461 735f 696e 6c69 6e65  ad_pandas_inline
+00009700: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
+00009710: 6529 0a20 2020 2020 2020 2069 6620 696e  e).        if in
+00009720: 6c69 6e65 5f64 6620 6973 206e 6f74 204e  line_df is not N
+00009730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009740: 2072 6574 7572 6e20 696e 6c69 6e65 5f64   return inline_d
+00009750: 660a 2020 2020 2020 2020 7472 793a 0a20  f.        try:. 
+00009760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009770: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
+00009780: 6461 735f 6c6f 6164 5f6a 6f62 2870 616e  das_load_job(pan
+00009790: 6461 735f 6461 7461 6672 616d 652c 2061  das_dataframe, a
+000097a0: 7069 5f6e 616d 6529 0a20 2020 2020 2020  pi_name).       
+000097b0: 2065 7863 6570 7420 7061 2e41 7272 6f77   except pa.Arrow
+000097c0: 496e 7661 6c69 6420 6173 2065 3a0a 2020  Invalid as e:.  
+000097d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000097e0: 7061 2e41 7272 6f77 496e 7661 6c69 6428  pa.ArrowInvalid(
+000097f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009800: 2066 2243 6f75 6c64 206e 6f74 2063 6f6e   f"Could not con
+00009810: 7665 7274 2077 6974 6820 6120 4269 6751  vert with a BigQ
+00009820: 7565 7279 2074 7970 653a 2060 7b65 7d60  uery type: `{e}`
+00009830: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+00009840: 2920 6672 6f6d 2065 0a0a 2020 2020 6465  ) from e..    de
+00009850: 6620 5f72 6561 645f 7061 6e64 6173 5f69  f _read_pandas_i
+00009860: 6e6c 696e 6528 0a20 2020 2020 2020 2073  nline(.        s
+00009870: 656c 662c 2070 616e 6461 735f 6461 7461  elf, pandas_data
+00009880: 6672 616d 653a 2070 616e 6461 732e 4461  frame: pandas.Da
+00009890: 7461 4672 616d 650a 2020 2020 2920 2d3e  taFrame.    ) ->
+000098a0: 204f 7074 696f 6e61 6c5b 6461 7461 6672   Optional[datafr
+000098b0: 616d 652e 4461 7461 4672 616d 655d 3a0a  ame.DataFrame]:.
+000098c0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
+000098d0: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
+000098e0: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
+000098f0: 0a20 2020 2020 2020 2069 6620 7061 6e64  .        if pand
+00009900: 6173 5f64 6174 6166 7261 6d65 2e6d 656d  as_dataframe.mem
+00009910: 6f72 795f 7573 6167 6528 6465 6570 3d54  ory_usage(deep=T
+00009920: 7275 6529 2e73 756d 2829 203e 204d 4158  rue).sum() > MAX
+00009930: 5f49 4e4c 494e 455f 4446 5f42 5954 4553  _INLINE_DF_BYTES
+00009940: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00009950: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
+00009960: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00009970: 2020 2020 696e 6c69 6e65 5f64 6620 3d20      inline_df = 
+00009980: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
+00009990: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
+000099a0: 2020 2020 2062 6c6f 636b 732e 426c 6f63       blocks.Bloc
+000099b0: 6b2e 6672 6f6d 5f6c 6f63 616c 2870 616e  k.from_local(pan
+000099c0: 6461 735f 6461 7461 6672 616d 652c 2073  das_dataframe, s
+000099d0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
+000099e0: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
+000099f0: 7420 7061 2e41 7272 6f77 496e 7661 6c69  t pa.ArrowInvali
+00009a00: 6420 6173 2065 3a0a 2020 2020 2020 2020  d as e:.        
+00009a10: 2020 2020 7261 6973 6520 7061 2e41 7272      raise pa.Arr
+00009a20: 6f77 496e 7661 6c69 6428 0a20 2020 2020  owInvalid(.     
+00009a30: 2020 2020 2020 2020 2020 2066 2243 6f75             f"Cou
+00009a40: 6c64 206e 6f74 2063 6f6e 7665 7274 2077  ld not convert w
+00009a50: 6974 6820 6120 4269 6751 7565 7279 2074  ith a BigQuery t
+00009a60: 7970 653a 2060 7b65 7d60 2e20 220a 2020  ype: `{e}`. ".  
+00009a70: 2020 2020 2020 2020 2020 2920 6672 6f6d            ) from
+00009a80: 2065 0a20 2020 2020 2020 2065 7863 6570   e.        excep
+00009a90: 7420 5661 6c75 6545 7272 6f72 3a20 2023  t ValueError:  #
+00009aa0: 2054 6872 6f77 6e20 6279 2069 6269 7320   Thrown by ibis 
+00009ab0: 666f 7220 736f 6d65 2075 6e68 616e 646c  for some unhandl
+00009ac0: 6564 2074 7970 6573 0a20 2020 2020 2020  ed types.       
+00009ad0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00009ae0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00009af0: 7061 2e41 7272 6f77 5479 7065 4572 726f  pa.ArrowTypeErro
+00009b00: 723a 2020 2320 5468 726f 776e 2062 7920  r:  # Thrown by 
+00009b10: 6172 726f 7720 666f 7220 7479 7065 7320  arrow for types 
+00009b20: 7769 7468 6f75 7420 6d61 7070 696e 6720  without mapping 
+00009b30: 2867 656f 292e 0a20 2020 2020 2020 2020  (geo)..         
+00009b40: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00009b50: 2020 2020 2020 2020 696e 6c69 6e65 5f74          inline_t
+00009b60: 7970 6573 203d 2069 6e6c 696e 655f 6466  ypes = inline_df
+00009b70: 2e5f 626c 6f63 6b2e 6578 7072 2e73 6368  ._block.expr.sch
+00009b80: 656d 612e 6474 7970 6573 0a20 2020 2020  ema.dtypes.     
+00009b90: 2020 2023 2049 6269 7320 6861 7320 7072     # Ibis has pr
+00009ba0: 6f62 6c65 6d73 2065 7363 6170 696e 6720  oblems escaping 
+00009bb0: 6279 7465 7320 6c69 7465 7261 6c73 2c20  bytes literals, 
+00009bc0: 7768 6963 6820 7769 6c6c 2063 6175 7365  which will cause
+00009bd0: 2073 796e 7461 7820 6572 726f 7273 2073   syntax errors s
+00009be0: 6572 7665 722d 7369 6465 2e0a 2020 2020  erver-side..    
+00009bf0: 2020 2020 6966 2061 6c6c 2864 7479 7065      if all(dtype
+00009c00: 2069 6e20 494e 4c49 4e41 424c 455f 4454   in INLINABLE_DT
+00009c10: 5950 4553 2066 6f72 2064 7479 7065 2069  YPES for dtype i
+00009c20: 6e20 696e 6c69 6e65 5f74 7970 6573 293a  n inline_types):
+00009c30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009c40: 7572 6e20 696e 6c69 6e65 5f64 660a 2020  urn inline_df.  
+00009c50: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00009c60: 650a 0a20 2020 2064 6566 205f 7265 6164  e..    def _read
+00009c70: 5f70 616e 6461 735f 6c6f 6164 5f6a 6f62  _pandas_load_job
+00009c80: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00009c90: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+00009ca0: 3a20 7061 6e64 6173 2e44 6174 6146 7261  : pandas.DataFra
+00009cb0: 6d65 2c20 6170 695f 6e61 6d65 3a20 7374  me, api_name: st
+00009cc0: 720a 2020 2020 2920 2d3e 2064 6174 6166  r.    ) -> dataf
+00009cd0: 7261 6d65 2e44 6174 6146 7261 6d65 3a0a  rame.DataFrame:.
+00009ce0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
+00009cf0: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
+00009d00: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
+00009d10: 0a20 2020 2020 2020 2063 6f6c 5f69 6e64  .        col_ind
+00009d20: 6578 203d 2070 616e 6461 735f 6461 7461  ex = pandas_data
+00009d30: 6672 616d 652e 636f 6c75 6d6e 732e 636f  frame.columns.co
+00009d40: 7079 2829 0a20 2020 2020 2020 2063 6f6c  py().        col
+00009d50: 5f6c 6162 656c 732c 2069 6478 5f6c 6162  _labels, idx_lab
+00009d60: 656c 7320 3d20 280a 2020 2020 2020 2020  els = (.        
+00009d70: 2020 2020 636f 6c5f 696e 6465 782e 746f      col_index.to
+00009d80: 5f6c 6973 7428 292c 0a20 2020 2020 2020  _list(),.       
+00009d90: 2020 2020 2070 616e 6461 735f 6461 7461       pandas_data
+00009da0: 6672 616d 652e 696e 6465 782e 6e61 6d65  frame.index.name
+00009db0: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
+00009dc0: 2020 2020 206e 6577 5f63 6f6c 5f69 6473       new_col_ids
+00009dd0: 2c20 6e65 775f 6964 785f 6964 7320 3d20  , new_idx_ids = 
+00009de0: 7574 696c 732e 6765 745f 7374 616e 6461  utils.get_standa
+00009df0: 7264 697a 6564 5f69 6473 280a 2020 2020  rdized_ids(.    
+00009e00: 2020 2020 2020 2020 636f 6c5f 6c61 6265          col_labe
+00009e10: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00009e20: 6964 785f 6c61 6265 6c73 2c0a 2020 2020  idx_labels,.    
+00009e30: 2020 2020 2020 2020 2320 4c6f 6164 696e          # Loadin
+00009e40: 6720 7061 7271 7565 7420 6669 6c65 7320  g parquet files 
+00009e50: 696e 746f 2042 6967 5175 6572 7920 7769  into BigQuery wi
+00009e60: 7468 2073 7065 6369 616c 2063 6f6c 756d  th special colum
+00009e70: 6e20 6e61 6d65 730a 2020 2020 2020 2020  n names.        
+00009e80: 2020 2020 2320 6973 206f 6e6c 7920 7375      # is only su
+00009e90: 7070 6f72 7465 6420 756e 6465 7220 616e  pported under an
+00009ea0: 2061 6c6c 6f77 6c69 7374 2e0a 2020 2020   allowlist..    
+00009eb0: 2020 2020 2020 2020 7374 7269 6374 3d54          strict=T
+00009ec0: 7275 652c 0a20 2020 2020 2020 2029 0a0a  rue,.        )..
+00009ed0: 2020 2020 2020 2020 2320 4164 6420 6f72          # Add or
+00009ee0: 6465 7220 636f 6c75 6d6e 2074 6f20 7061  der column to pa
+00009ef0: 6e64 6173 2044 6174 6146 7261 6d65 2074  ndas DataFrame t
+00009f00: 6f20 7072 6573 6572 7665 206f 7264 6572  o preserve order
+00009f10: 2069 6e20 4269 6751 7565 7279 0a20 2020   in BigQuery.   
+00009f20: 2020 2020 206f 7264 6572 696e 675f 636f       ordering_co
+00009f30: 6c20 3d20 2272 6f77 6964 220a 2020 2020  l = "rowid".    
+00009f40: 2020 2020 636f 6c75 6d6e 7320 3d20 6672      columns = fr
+00009f50: 6f7a 656e 7365 7428 636f 6c5f 6c61 6265  ozenset(col_labe
+00009f60: 6c73 202b 2069 6478 5f6c 6162 656c 7329  ls + idx_labels)
+00009f70: 0a20 2020 2020 2020 2073 7566 6669 7820  .        suffix 
+00009f80: 3d20 320a 2020 2020 2020 2020 7768 696c  = 2.        whil
+00009f90: 6520 6f72 6465 7269 6e67 5f63 6f6c 2069  e ordering_col i
+00009fa0: 6e20 636f 6c75 6d6e 733a 0a20 2020 2020  n columns:.     
+00009fb0: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
+00009fc0: 636f 6c20 3d20 6622 726f 7769 645f 7b73  col = f"rowid_{s
+00009fd0: 7566 6669 787d 220a 2020 2020 2020 2020  uffix}".        
+00009fe0: 2020 2020 7375 6666 6978 202b 3d20 310a      suffix += 1.
+00009ff0: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
+0000a000: 6461 7461 6672 616d 655f 636f 7079 203d  dataframe_copy =
+0000a010: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
+0000a020: 652e 636f 7079 2829 0a20 2020 2020 2020  e.copy().       
+0000a030: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
+0000a040: 655f 636f 7079 2e69 6e64 6578 2e6e 616d  e_copy.index.nam
+0000a050: 6573 203d 206e 6577 5f69 6478 5f69 6473  es = new_idx_ids
+0000a060: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
+0000a070: 6461 7461 6672 616d 655f 636f 7079 2e63  dataframe_copy.c
+0000a080: 6f6c 756d 6e73 203d 2070 616e 6461 732e  olumns = pandas.
+0000a090: 496e 6465 7828 6e65 775f 636f 6c5f 6964  Index(new_col_id
+0000a0a0: 7329 0a20 2020 2020 2020 2070 616e 6461  s).        panda
+0000a0b0: 735f 6461 7461 6672 616d 655f 636f 7079  s_dataframe_copy
+0000a0c0: 5b6f 7264 6572 696e 675f 636f 6c5d 203d  [ordering_col] =
+0000a0d0: 206e 702e 6172 616e 6765 2870 616e 6461   np.arange(panda
+0000a0e0: 735f 6461 7461 6672 616d 655f 636f 7079  s_dataframe_copy
+0000a0f0: 2e73 6861 7065 5b30 5d29 0a0a 2020 2020  .shape[0])..    
+0000a100: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
+0000a110: 2073 656c 662e 5f70 7265 7061 7265 5f6c   self._prepare_l
+0000a120: 6f61 645f 6a6f 625f 636f 6e66 6967 2829  oad_job_config()
+0000a130: 0a0a 2020 2020 2020 2020 2320 5370 6563  ..        # Spec
+0000a140: 6966 7920 7468 6520 6461 7465 7469 6d65  ify the datetime
+0000a150: 2064 7479 7065 732c 2077 6869 6368 2069   dtypes, which i
+0000a160: 7320 6175 746f 2d64 6574 6563 7465 6420  s auto-detected 
+0000a170: 6173 2074 696d 6573 7461 6d70 2074 7970  as timestamp typ
+0000a180: 6573 2e0a 2020 2020 2020 2020 7363 6865  es..        sche
+0000a190: 6d61 3a20 6c69 7374 5b62 6967 7175 6572  ma: list[bigquer
+0000a1a0: 792e 5363 6865 6d61 4669 656c 645d 203d  y.SchemaField] =
+0000a1b0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+0000a1c0: 636f 6c75 6d6e 2c20 6474 7970 6520 696e  column, dtype in
+0000a1d0: 207a 6970 286e 6577 5f63 6f6c 5f69 6473   zip(new_col_ids
+0000a1e0: 2c20 7061 6e64 6173 5f64 6174 6166 7261  , pandas_datafra
+0000a1f0: 6d65 2e64 7479 7065 7329 3a0a 2020 2020  me.dtypes):.    
+0000a200: 2020 2020 2020 2020 6966 2064 7479 7065          if dtype
+0000a210: 203d 3d20 2274 696d 6573 7461 6d70 5b75   == "timestamp[u
+0000a220: 735d 5b70 7961 7272 6f77 5d22 3a0a 2020  s][pyarrow]":.  
+0000a230: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+0000a240: 6865 6d61 2e61 7070 656e 6428 0a20 2020  hema.append(.   
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2062 6967 7175 6572 792e 5363 6865 6d61   bigquery.Schema
+0000a270: 4669 656c 6428 636f 6c75 6d6e 2c20 6269  Field(column, bi
+0000a280: 6771 7565 7279 2e65 6e75 6d73 2e53 716c  gquery.enums.Sql
+0000a290: 5479 7065 4e61 6d65 732e 4441 5445 5449  TypeNames.DATETI
+0000a2a0: 4d45 290a 2020 2020 2020 2020 2020 2020  ME).            
+0000a2b0: 2020 2020 290a 2020 2020 2020 2020 6a6f      ).        jo
+0000a2c0: 625f 636f 6e66 6967 2e73 6368 656d 6120  b_config.schema 
+0000a2d0: 3d20 7363 6865 6d61 0a0a 2020 2020 2020  = schema..      
+0000a2e0: 2020 2320 436c 7573 7465 7269 6e67 2070    # Clustering p
+0000a2f0: 726f 6261 626c 7920 6e6f 7420 6e65 6564  robably not need
+0000a300: 6564 2061 6e79 7761 7973 2061 7320 7061  ed anyways as pa
+0000a310: 6e64 6173 2074 6162 6c65 7320 6172 6520  ndas tables are 
+0000a320: 736d 616c 6c0a 2020 2020 2020 2020 636c  small.        cl
+0000a330: 7573 7465 725f 636f 6c73 203d 205b 6f72  uster_cols = [or
+0000a340: 6465 7269 6e67 5f63 6f6c 5d0a 2020 2020  dering_col].    
+0000a350: 2020 2020 6a6f 625f 636f 6e66 6967 2e63      job_config.c
+0000a360: 6c75 7374 6572 696e 675f 6669 656c 6473  lustering_fields
+0000a370: 203d 2063 6c75 7374 6572 5f63 6f6c 730a   = cluster_cols.
+0000a380: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
+0000a390: 6669 672e 6c61 6265 6c73 203d 207b 2262  fig.labels = {"b
+0000a3a0: 6967 6672 616d 6573 2d61 7069 223a 2061  igframes-api": a
+0000a3b0: 7069 5f6e 616d 657d 0a0a 2020 2020 2020  pi_name}..      
+0000a3c0: 2020 6c6f 6164 5f74 6162 6c65 5f64 6573    load_table_des
+0000a3d0: 7469 6e61 7469 6f6e 203d 2062 6967 6672  tination = bigfr
+0000a3e0: 616d 6573 5f69 6f2e 7261 6e64 6f6d 5f74  ames_io.random_t
+0000a3f0: 6162 6c65 2873 656c 662e 5f61 6e6f 6e79  able(self._anony
+0000a400: 6d6f 7573 5f64 6174 6173 6574 290a 2020  mous_dataset).  
+0000a410: 2020 2020 2020 6c6f 6164 5f6a 6f62 203d        load_job =
+0000a420: 2073 656c 662e 6271 636c 6965 6e74 2e6c   self.bqclient.l
+0000a430: 6f61 645f 7461 626c 655f 6672 6f6d 5f64  oad_table_from_d
+0000a440: 6174 6166 7261 6d65 280a 2020 2020 2020  ataframe(.      
+0000a450: 2020 2020 2020 7061 6e64 6173 5f64 6174        pandas_dat
+0000a460: 6166 7261 6d65 5f63 6f70 792c 0a20 2020  aframe_copy,.   
+0000a470: 2020 2020 2020 2020 206c 6f61 645f 7461           load_ta
+0000a480: 626c 655f 6465 7374 696e 6174 696f 6e2c  ble_destination,
+0000a490: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
+0000a4a0: 5f63 6f6e 6669 673d 6a6f 625f 636f 6e66  _config=job_conf
+0000a4b0: 6967 2c0a 2020 2020 2020 2020 290a 2020  ig,.        ).  
+0000a4c0: 2020 2020 2020 7365 6c66 2e5f 7374 6172        self._star
+0000a4d0: 745f 6765 6e65 7269 635f 6a6f 6228 6c6f  t_generic_job(lo
+0000a4e0: 6164 5f6a 6f62 290a 0a20 2020 2020 2020  ad_job)..       
+0000a4f0: 206f 7264 6572 696e 6720 3d20 6f72 6465   ordering = orde
+0000a500: 722e 4578 7072 6573 7369 6f6e 4f72 6465  r.ExpressionOrde
+0000a510: 7269 6e67 280a 2020 2020 2020 2020 2020  ring(.          
+0000a520: 2020 6f72 6465 7269 6e67 5f76 616c 7565    ordering_value
+0000a530: 5f63 6f6c 756d 6e73 3d74 7570 6c65 285b  _columns=tuple([
+0000a540: 6f72 6465 722e 6173 6365 6e64 696e 675f  order.ascending_
+0000a550: 6f76 6572 286f 7264 6572 696e 675f 636f  over(ordering_co
+0000a560: 6c29 5d29 2c0a 2020 2020 2020 2020 2020  l)]),.          
+0000a570: 2020 746f 7461 6c5f 6f72 6465 7269 6e67    total_ordering
+0000a580: 5f63 6f6c 756d 6e73 3d66 726f 7a65 6e73  _columns=frozens
+0000a590: 6574 285b 6f72 6465 7269 6e67 5f63 6f6c  et([ordering_col
+0000a5a0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0000a5b0: 696e 7465 6765 725f 656e 636f 6469 6e67  integer_encoding
+0000a5c0: 3d49 6e74 6567 6572 456e 636f 6469 6e67  =IntegerEncoding
+0000a5d0: 2854 7275 652c 2069 735f 7365 7175 656e  (True, is_sequen
+0000a5e0: 7469 616c 3d54 7275 6529 2c0a 2020 2020  tial=True),.    
+0000a5f0: 2020 2020 290a 2020 2020 2020 2020 7461      ).        ta
+0000a600: 626c 655f 6578 7072 6573 7369 6f6e 203d  ble_expression =
+0000a610: 2073 656c 662e 6962 6973 5f63 6c69 656e   self.ibis_clien
+0000a620: 742e 7461 626c 6528 2020 2320 7479 7065  t.table(  # type
+0000a630: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+0000a640: 2020 2020 206c 6f61 645f 7461 626c 655f       load_table_
+0000a650: 6465 7374 696e 6174 696f 6e2e 7461 626c  destination.tabl
+0000a660: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+0000a670: 2020 7363 6865 6d61 3d6c 6f61 645f 7461    schema=load_ta
+0000a680: 626c 655f 6465 7374 696e 6174 696f 6e2e  ble_destination.
+0000a690: 6461 7461 7365 745f 6964 2c0a 2020 2020  dataset_id,.    
+0000a6a0: 2020 2020 2020 2020 6461 7461 6261 7365          database
+0000a6b0: 3d6c 6f61 645f 7461 626c 655f 6465 7374  =load_table_dest
+0000a6c0: 696e 6174 696f 6e2e 7072 6f6a 6563 742c  ination.project,
+0000a6d0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000a6e0: 2020 2020 2320 622f 3239 3735 3930 3137      # b/29759017
+0000a6f0: 3820 506f 7465 6e74 6961 6c6c 7920 6120  8 Potentially a 
+0000a700: 6275 6720 696e 2062 7163 6c69 656e 742e  bug in bqclient.
+0000a710: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
+0000a720: 6461 7461 6672 616d 6528 292c 2074 6861  dataframe(), tha
+0000a730: 7420 6f6e 6c79 2077 6865 6e20 7468 6520  t only when the 
+0000a740: 4446 2069 7320 656d 7074 792c 2074 6865  DF is empty, the
+0000a750: 2069 6e64 6578 2063 6f6c 756d 6e73 2064   index columns d
+0000a760: 6973 6170 7065 6172 2069 6e20 7461 626c  isappear in tabl
+0000a770: 655f 6578 7072 6573 7369 6f6e 2e0a 2020  e_expression..  
+0000a780: 2020 2020 2020 6966 2061 6e79 280a 2020        if any(.  
+0000a790: 2020 2020 2020 2020 2020 5b6e 6577 5f69            [new_i
+0000a7a0: 6478 5f69 6420 6e6f 7420 696e 2074 6162  dx_id not in tab
+0000a7b0: 6c65 5f65 7870 7265 7373 696f 6e2e 636f  le_expression.co
+0000a7c0: 6c75 6d6e 7320 666f 7220 6e65 775f 6964  lumns for new_id
+0000a7d0: 785f 6964 2069 6e20 6e65 775f 6964 785f  x_id in new_idx_
+0000a7e0: 6964 735d 0a20 2020 2020 2020 2029 3a0a  ids].        ):.
+0000a7f0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000a800: 6964 785f 6964 732c 2069 6478 5f6c 6162  idx_ids, idx_lab
+0000a810: 656c 7320 3d20 5b5d 2c20 5b5d 0a0a 2020  els = [], []..  
+0000a820: 2020 2020 2020 636f 6c75 6d6e 5f76 616c        column_val
+0000a830: 7565 7320 3d20 5b0a 2020 2020 2020 2020  ues = [.        
+0000a840: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
+0000a850: 7369 6f6e 5b63 6f6c 5d0a 2020 2020 2020  sion[col].      
+0000a860: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
+0000a870: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
+0000a880: 6e2e 636f 6c75 6d6e 730a 2020 2020 2020  n.columns.      
+0000a890: 2020 2020 2020 6966 2063 6f6c 2021 3d20        if col != 
+0000a8a0: 6f72 6465 7269 6e67 5f63 6f6c 0a20 2020  ordering_col.   
+0000a8b0: 2020 2020 205d 0a20 2020 2020 2020 2061       ].        a
+0000a8c0: 7272 6179 5f76 616c 7565 203d 2063 6f72  rray_value = cor
+0000a8d0: 652e 4172 7261 7956 616c 7565 2e66 726f  e.ArrayValue.fro
+0000a8e0: 6d5f 6962 6973 280a 2020 2020 2020 2020  m_ibis(.        
+0000a8f0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000a900: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
+0000a910: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
+0000a920: 2020 2020 636f 6c75 6d6e 733d 636f 6c75      columns=colu
+0000a930: 6d6e 5f76 616c 7565 732c 0a20 2020 2020  mn_values,.     
+0000a940: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
+0000a950: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d5b  dering_columns=[
+0000a960: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+0000a970: 5b6f 7264 6572 696e 675f 636f 6c5d 5d2c  [ordering_col]],
+0000a980: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+0000a990: 6572 696e 673d 6f72 6465 7269 6e67 2c0a  ering=ordering,.
+0000a9a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000a9b0: 2020 2062 6c6f 636b 203d 2062 6c6f 636b     block = block
+0000a9c0: 732e 426c 6f63 6b28 0a20 2020 2020 2020  s.Block(.       
+0000a9d0: 2020 2020 2061 7272 6179 5f76 616c 7565       array_value
+0000a9e0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+0000a9f0: 6465 785f 636f 6c75 6d6e 733d 6e65 775f  dex_columns=new_
+0000aa00: 6964 785f 6964 732c 0a20 2020 2020 2020  idx_ids,.       
+0000aa10: 2020 2020 2063 6f6c 756d 6e5f 6c61 6265       column_labe
+0000aa20: 6c73 3d63 6f6c 5f69 6e64 6578 2c0a 2020  ls=col_index,.  
+0000aa30: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+0000aa40: 6c61 6265 6c73 3d69 6478 5f6c 6162 656c  labels=idx_label
+0000aa50: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
+0000aa60: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
+0000aa70: 6672 616d 652e 4461 7461 4672 616d 6528  frame.DataFrame(
+0000aa80: 626c 6f63 6b29 0a0a 2020 2020 6465 6620  block)..    def 
+0000aa90: 7265 6164 5f63 7376 280a 2020 2020 2020  read_csv(.      
+0000aaa0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000aab0: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
+0000aac0: 6572 3a20 7374 7220 7c20 494f 5b22 6279  er: str | IO["by
+0000aad0: 7465 7322 5d2c 0a20 2020 2020 2020 202a  tes"],.        *
+0000aae0: 2c0a 2020 2020 2020 2020 7365 703a 204f  ,.        sep: O
+0000aaf0: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
+0000ab00: 2c22 2c0a 2020 2020 2020 2020 6865 6164  ,",.        head
+0000ab10: 6572 3a20 4f70 7469 6f6e 616c 5b69 6e74  er: Optional[int
+0000ab20: 5d20 3d20 302c 0a20 2020 2020 2020 206e  ] = 0,.        n
+0000ab30: 616d 6573 3a20 4f70 7469 6f6e 616c 5b0a  ames: Optional[.
+0000ab40: 2020 2020 2020 2020 2020 2020 556e 696f              Unio
+0000ab50: 6e5b 4d75 7461 626c 6553 6571 7565 6e63  n[MutableSequenc
+0000ab60: 655b 416e 795d 2c20 6e70 2e6e 6461 7272  e[Any], np.ndarr
+0000ab70: 6179 5b41 6e79 2c20 416e 795d 2c20 5475  ay[Any, Any], Tu
+0000ab80: 706c 655b 416e 792c 202e 2e2e 5d2c 2072  ple[Any, ...], r
+0000ab90: 616e 6765 5d0a 2020 2020 2020 2020 5d20  ange].        ] 
+0000aba0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000abb0: 696e 6465 785f 636f 6c3a 204f 7074 696f  index_col: Optio
+0000abc0: 6e61 6c5b 0a20 2020 2020 2020 2020 2020  nal[.           
+0000abd0: 2055 6e69 6f6e 5b69 6e74 2c20 7374 722c   Union[int, str,
+0000abe0: 2053 6571 7565 6e63 655b 556e 696f 6e5b   Sequence[Union[
+0000abf0: 7374 722c 2069 6e74 5d5d 2c20 4c69 7465  str, int]], Lite
+0000ac00: 7261 6c5b 4661 6c73 655d 5d0a 2020 2020  ral[False]].    
+0000ac10: 2020 2020 5d20 3d20 4e6f 6e65 2c0a 2020      ] = None,.  
+0000ac20: 2020 2020 2020 7573 6563 6f6c 733a 204f        usecols: O
+0000ac30: 7074 696f 6e61 6c5b 0a20 2020 2020 2020  ptional[.       
+0000ac40: 2020 2020 2055 6e69 6f6e 5b0a 2020 2020       Union[.    
+0000ac50: 2020 2020 2020 2020 2020 2020 4d75 7461              Muta
+0000ac60: 626c 6553 6571 7565 6e63 655b 7374 725d  bleSequence[str]
+0000ac70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ac80: 2020 5475 706c 655b 7374 722c 202e 2e2e    Tuple[str, ...
+0000ac90: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000aca0: 2020 2053 6571 7565 6e63 655b 696e 745d     Sequence[int]
+0000acb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000acc0: 2020 7061 6e64 6173 2e53 6572 6965 732c    pandas.Series,
+0000acd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ace0: 2070 616e 6461 732e 496e 6465 782c 0a20   pandas.Index,. 
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000ad00: 702e 6e64 6172 7261 795b 416e 792c 2041  p.ndarray[Any, A
+0000ad10: 6e79 5d2c 0a20 2020 2020 2020 2020 2020  ny],.           
+0000ad20: 2020 2020 2043 616c 6c61 626c 655b 5b41       Callable[[A
+0000ad30: 6e79 5d2c 2062 6f6f 6c5d 2c0a 2020 2020  ny], bool],.    
+0000ad40: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0000ad50: 2020 5d20 3d20 4e6f 6e65 2c0a 2020 2020    ] = None,.    
+0000ad60: 2020 2020 6474 7970 653a 204f 7074 696f      dtype: Optio
+0000ad70: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
+0000ad80: 2c0a 2020 2020 2020 2020 656e 6769 6e65  ,.        engine
+0000ad90: 3a20 4f70 7469 6f6e 616c 5b0a 2020 2020  : Optional[.    
+0000ada0: 2020 2020 2020 2020 4c69 7465 7261 6c5b          Literal[
+0000adb0: 2263 222c 2022 7079 7468 6f6e 222c 2022  "c", "python", "
+0000adc0: 7079 6172 726f 7722 2c20 2270 7974 686f  pyarrow", "pytho
+0000add0: 6e2d 6677 6622 2c20 2262 6967 7175 6572  n-fwf", "bigquer
+0000ade0: 7922 5d0a 2020 2020 2020 2020 5d20 3d20  y"].        ] = 
+0000adf0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656e  None,.        en
+0000ae00: 636f 6469 6e67 3a20 4f70 7469 6f6e 616c  coding: Optional
+0000ae10: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000ae20: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
+0000ae30: 2020 2020 2920 2d3e 2064 6174 6166 7261      ) -> datafra
+0000ae40: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
+0000ae50: 2020 2020 2020 7461 626c 6520 3d20 6269        table = bi
+0000ae60: 6766 7261 6d65 735f 696f 2e72 616e 646f  gframes_io.rando
+0000ae70: 6d5f 7461 626c 6528 7365 6c66 2e5f 616e  m_table(self._an
+0000ae80: 6f6e 796d 6f75 735f 6461 7461 7365 7429  onymous_dataset)
+0000ae90: 0a0a 2020 2020 2020 2020 6966 2065 6e67  ..        if eng
+0000aea0: 696e 6520 6973 206e 6f74 204e 6f6e 6520  ine is not None 
+0000aeb0: 616e 6420 656e 6769 6e65 203d 3d20 2262  and engine == "b
+0000aec0: 6967 7175 6572 7922 3a0a 2020 2020 2020  igquery":.      
+0000aed0: 2020 2020 2020 6966 2061 6e79 2870 6172        if any(par
+0000aee0: 616d 2069 7320 6e6f 7420 4e6f 6e65 2066  am is not None f
+0000aef0: 6f72 2070 6172 616d 2069 6e20 2864 7479  or param in (dty
+0000af00: 7065 2c20 6e61 6d65 7329 293a 0a20 2020  pe, names)):.   
+0000af10: 2020 2020 2020 2020 2020 2020 206e 6f74               not
+0000af20: 5f73 7570 706f 7274 6564 203d 2028 2264  _supported = ("d
+0000af30: 7479 7065 222c 2022 6e61 6d65 7322 290a  type", "names").
+0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af50: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+0000af60: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000af80: 2242 6967 5175 6572 7920 656e 6769 6e65  "BigQuery engine
+0000af90: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+0000afa0: 7420 7468 6573 6520 6172 6775 6d65 6e74  t these argument
+0000afb0: 733a 207b 6e6f 745f 7375 7070 6f72 7465  s: {not_supporte
+0000afc0: 647d 2e20 220a 2020 2020 2020 2020 2020  d}. ".          
+0000afd0: 2020 2020 2020 2020 2020 6622 7b63 6f6e            f"{con
+0000afe0: 7374 616e 7473 2e46 4545 4442 4143 4b5f  stants.FEEDBACK_
+0000aff0: 4c49 4e4b 7d22 0a20 2020 2020 2020 2020  LINK}".         
+0000b000: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000b010: 2020 2020 2020 6966 2069 6e64 6578 5f63        if index_c
+0000b020: 6f6c 2069 7320 6e6f 7420 4e6f 6e65 2061  ol is not None a
+0000b030: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
+0000b040: 2020 2020 206e 6f74 2069 6e64 6578 5f63       not index_c
+0000b050: 6f6c 206f 7220 6e6f 7420 6973 696e 7374  ol or not isinst
+0000b060: 616e 6365 2869 6e64 6578 5f63 6f6c 2c20  ance(index_col, 
+0000b070: 7374 7229 0a20 2020 2020 2020 2020 2020  str).           
+0000b080: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000b090: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+0000b0a0: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
+0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0c0: 2020 2022 4269 6751 7565 7279 2065 6e67     "BigQuery eng
+0000b0d0: 696e 6520 6f6e 6c79 2073 7570 706f 7274  ine only support
+0000b0e0: 7320 6120 7369 6e67 6c65 2063 6f6c 756d  s a single colum
+0000b0f0: 6e20 6e61 6d65 2066 6f72 2060 696e 6465  n name for `inde
+0000b100: 785f 636f 6c60 2e20 220a 2020 2020 2020  x_col`. ".      
+0000b110: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000b120: 7b63 6f6e 7374 616e 7473 2e46 4545 4442  {constants.FEEDB
+0000b130: 4143 4b5f 4c49 4e4b 7d22 0a20 2020 2020  ACK_LINK}".     
+0000b140: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000b150: 2020 2020 2020 2020 2020 2320 4e6f 6e65            # None
+0000b160: 2076 616c 7565 2066 6f72 2069 6e64 6578   value for index
+0000b170: 5f63 6f6c 2063 616e 6e6f 7420 6265 2070  _col cannot be p
+0000b180: 6173 7365 6420 746f 2072 6561 645f 6762  assed to read_gb
+0000b190: 710a 2020 2020 2020 2020 2020 2020 6966  q.            if
+0000b1a0: 2069 6e64 6578 5f63 6f6c 2069 7320 4e6f   index_col is No
+0000b1b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000b1c0: 2020 2020 696e 6465 785f 636f 6c20 3d20      index_col = 
+0000b1d0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+0000b1e0: 2320 7573 6563 6f6c 7320 7368 6f75 6c64  # usecols should
+0000b1f0: 206f 6e6c 7920 6265 2061 6e20 6974 6572   only be an iter
+0000b200: 6162 6c65 206f 6620 7374 7269 6e67 7320  able of strings 
+0000b210: 2863 6f6c 756d 6e20 6e61 6d65 7329 2066  (column names) f
+0000b220: 6f72 2075 7365 2061 7320 636f 6c75 6d6e  or use as column
+0000b230: 7320 696e 2072 6561 645f 6762 712e 0a20  s in read_gbq.. 
+0000b240: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000b250: 6e73 3a20 5475 706c 655b 416e 792c 202e  ns: Tuple[Any, .
+0000b260: 2e2e 5d20 3d20 7475 706c 6528 290a 2020  ..] = tuple().  
+0000b270: 2020 2020 2020 2020 2020 6966 2075 7365            if use
+0000b280: 636f 6c73 2069 7320 6e6f 7420 4e6f 6e65  cols is not None
+0000b290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b2a0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000b2b0: 7573 6563 6f6c 732c 2049 7465 7261 626c  usecols, Iterabl
+0000b2c0: 6529 2061 6e64 2061 6c6c 280a 2020 2020  e) and all(.    
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2e0: 6973 696e 7374 616e 6365 2863 6f6c 2c20  isinstance(col, 
+0000b2f0: 7374 7229 2066 6f72 2063 6f6c 2069 6e20  str) for col in 
+0000b300: 7573 6563 6f6c 730a 2020 2020 2020 2020  usecols.        
+0000b310: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000b330: 6f6c 756d 6e73 203d 2074 7570 6c65 2863  olumns = tuple(c
+0000b340: 6f6c 2066 6f72 2063 6f6c 2069 6e20 7573  ol for col in us
+0000b350: 6563 6f6c 7329 0a20 2020 2020 2020 2020  ecols).         
+0000b360: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b380: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000b390: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
+0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3b0: 2020 2020 2242 6967 5175 6572 7920 656e      "BigQuery en
+0000b3c0: 6769 6e65 206f 6e6c 7920 7375 7070 6f72  gine only suppor
+0000b3d0: 7473 2061 6e20 6974 6572 6162 6c65 206f  ts an iterable o
+0000b3e0: 6620 7374 7269 6e67 7320 666f 7220 6075  f strings for `u
+0000b3f0: 7365 636f 6c73 602e 2022 0a20 2020 2020  secols`. ".     
+0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b410: 2020 2066 227b 636f 6e73 7461 6e74 732e     f"{constants.
+0000b420: 4645 4544 4241 434b 5f4c 494e 4b7d 220a  FEEDBACK_LINK}".
+0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b440: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+0000b450: 2020 2069 6620 656e 636f 6469 6e67 2069     if encoding i
+0000b460: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2065  s not None and e
+0000b470: 6e63 6f64 696e 6720 6e6f 7420 696e 205f  ncoding not in _
+0000b480: 5641 4c49 445f 454e 434f 4449 4e47 533a  VALID_ENCODINGS:
+0000b490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b4a0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000b4b0: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
+0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4d0: 6622 4269 6751 7565 7279 2065 6e67 696e  f"BigQuery engin
+0000b4e0: 6520 6f6e 6c79 2073 7570 706f 7274 7320  e only supports 
+0000b4f0: 7468 6520 666f 6c6c 6f77 696e 6720 656e  the following en
+0000b500: 636f 6469 6e67 733a 207b 5f56 414c 4944  codings: {_VALID
+0000b510: 5f45 4e43 4f44 494e 4753 7d2e 2022 0a20  _ENCODINGS}. ". 
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2066 227b 636f 6e73 7461 6e74 732e     f"{constants.
+0000b540: 4645 4544 4241 434b 5f4c 494e 4b7d 220a  FEEDBACK_LINK}".
+0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b560: 290a 0a20 2020 2020 2020 2020 2020 206a  )..            j
+0000b570: 6f62 5f63 6f6e 6669 6720 3d20 7365 6c66  ob_config = self
+0000b580: 2e5f 7072 6570 6172 655f 6c6f 6164 5f6a  ._prepare_load_j
+0000b590: 6f62 5f63 6f6e 6669 6728 290a 2020 2020  ob_config().    
+0000b5a0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+0000b5b0: 6967 2e63 7265 6174 655f 6469 7370 6f73  ig.create_dispos
+0000b5c0: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
+0000b5d0: 2e43 7265 6174 6544 6973 706f 7369 7469  .CreateDispositi
+0000b5e0: 6f6e 2e43 5245 4154 455f 4946 5f4e 4545  on.CREATE_IF_NEE
+0000b5f0: 4445 440a 2020 2020 2020 2020 2020 2020  DED.            
+0000b600: 6a6f 625f 636f 6e66 6967 2e73 6f75 7263  job_config.sourc
+0000b610: 655f 666f 726d 6174 203d 2062 6967 7175  e_format = bigqu
+0000b620: 6572 792e 536f 7572 6365 466f 726d 6174  ery.SourceFormat
+0000b630: 2e43 5356 0a20 2020 2020 2020 2020 2020  .CSV.           
+0000b640: 206a 6f62 5f63 6f6e 6669 672e 7772 6974   job_config.writ
+0000b650: 655f 6469 7370 6f73 6974 696f 6e20 3d20  e_disposition = 
+0000b660: 6269 6771 7565 7279 2e57 7269 7465 4469  bigquery.WriteDi
+0000b670: 7370 6f73 6974 696f 6e2e 5752 4954 455f  sposition.WRITE_
+0000b680: 454d 5054 590a 2020 2020 2020 2020 2020  EMPTY.          
+0000b690: 2020 6a6f 625f 636f 6e66 6967 2e61 7574    job_config.aut
+0000b6a0: 6f64 6574 6563 7420 3d20 5472 7565 0a20  odetect = True. 
+0000b6b0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000b6c0: 6f6e 6669 672e 6669 656c 645f 6465 6c69  onfig.field_deli
+0000b6d0: 6d69 7465 7220 3d20 7365 700a 2020 2020  miter = sep.    
+0000b6e0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+0000b6f0: 6967 2e65 6e63 6f64 696e 6720 3d20 656e  ig.encoding = en
+0000b700: 636f 6469 6e67 0a20 2020 2020 2020 2020  coding.         
+0000b710: 2020 206a 6f62 5f63 6f6e 6669 672e 6c61     job_config.la
+0000b720: 6265 6c73 203d 207b 2262 6967 6672 616d  bels = {"bigfram
+0000b730: 6573 2d61 7069 223a 2022 7265 6164 5f63  es-api": "read_c
+0000b740: 7376 227d 0a0a 2020 2020 2020 2020 2020  sv"}..          
+0000b750: 2020 2320 5765 2077 616e 7420 746f 206d    # We want to m
+0000b760: 6174 6368 2070 616e 6461 7320 6265 6861  atch pandas beha
+0000b770: 7669 6f72 2e20 4966 2068 6561 6465 7220  vior. If header 
+0000b780: 6973 2030 2c20 6e6f 2072 6f77 7320 7368  is 0, no rows sh
+0000b790: 6f75 6c64 2062 6520 736b 6970 7065 642c  ould be skipped,
+0000b7a0: 2073 6f20 7765 0a20 2020 2020 2020 2020   so we.         
+0000b7b0: 2020 2023 2064 6f20 6e6f 7420 6e65 6564     # do not need
+0000b7c0: 2074 6f20 7365 7420 6073 6b69 705f 6c65   to set `skip_le
+0000b7d0: 6164 696e 675f 726f 7773 602e 2049 6620  ading_rows`. If 
+0000b7e0: 6865 6164 6572 2069 7320 4e6f 6e65 2c20  header is None, 
+0000b7f0: 7468 656e 2074 6865 7265 2069 7320 6e6f  then there is no
+0000b800: 2068 6561 6465 722e 0a20 2020 2020 2020   header..       
+0000b810: 2020 2020 2023 2053 6574 7469 6e67 2073       # Setting s
+0000b820: 6b69 705f 6c65 6164 696e 675f 726f 7773  kip_leading_rows
+0000b830: 2074 6f20 3020 646f 6573 2074 6861 742e   to 0 does that.
+0000b840: 2049 6620 6865 6164 6572 3d4e 2061 6e64   If header=N and
+0000b850: 204e 3e30 2c20 7765 2077 616e 7420 746f   N>0, we want to
+0000b860: 2073 6b69 7020 4e20 726f 7773 2e0a 2020   skip N rows..  
+0000b870: 2020 2020 2020 2020 2020 6966 2068 6561            if hea
+0000b880: 6465 7220 6973 204e 6f6e 653a 0a20 2020  der is None:.   
+0000b890: 2020 2020 2020 2020 2020 2020 206a 6f62               job
+0000b8a0: 5f63 6f6e 6669 672e 736b 6970 5f6c 6561  _config.skip_lea
+0000b8b0: 6469 6e67 5f72 6f77 7320 3d20 300a 2020  ding_rows = 0.  
+0000b8c0: 2020 2020 2020 2020 2020 656c 6966 2068            elif h
+0000b8d0: 6561 6465 7220 3e20 303a 0a20 2020 2020  eader > 0:.     
+0000b8e0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000b8f0: 6f6e 6669 672e 736b 6970 5f6c 6561 6469  onfig.skip_leadi
+0000b900: 6e67 5f72 6f77 7320 3d20 6865 6164 6572  ng_rows = header
+0000b910: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000b920: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
+0000b930: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
+0000b940: 6228 0a20 2020 2020 2020 2020 2020 2020  b(.             
+0000b950: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
+0000b960: 7566 6665 722c 0a20 2020 2020 2020 2020  uffer,.         
+0000b970: 2020 2020 2020 2074 6162 6c65 2c0a 2020         table,.  
+0000b980: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
+0000b990: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
+0000b9a0: 6669 672c 0a20 2020 2020 2020 2020 2020  fig,.           
+0000b9b0: 2020 2020 2069 6e64 6578 5f63 6f6c 3d69       index_col=i
+0000b9c0: 6e64 6578 5f63 6f6c 2c0a 2020 2020 2020  ndex_col,.      
+0000b9d0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+0000b9e0: 733d 636f 6c75 6d6e 732c 0a20 2020 2020  s=columns,.     
+0000b9f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ba00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ba10: 2020 2069 6620 616e 7928 6172 6720 696e     if any(arg in
+0000ba20: 206b 7761 7267 7320 666f 7220 6172 6720   kwargs for arg 
+0000ba30: 696e 2028 2263 6875 6e6b 7369 7a65 222c  in ("chunksize",
+0000ba40: 2022 6974 6572 6174 6f72 2229 293a 0a20   "iterator")):. 
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000ba60: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+0000ba70: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 2227                "'
+0000ba90: 6368 756e 6b73 697a 6527 2061 6e64 2027  chunksize' and '
+0000baa0: 6974 6572 6174 6f72 2720 6172 6775 6d65  iterator' argume
+0000bab0: 6e74 7320 6172 6520 6e6f 7420 7375 7070  nts are not supp
+0000bac0: 6f72 7465 642e 2022 0a20 2020 2020 2020  orted. ".       
+0000bad0: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+0000bae0: 636f 6e73 7461 6e74 732e 4645 4544 4241  constants.FEEDBA
+0000baf0: 434b 5f4c 494e 4b7d 220a 2020 2020 2020  CK_LINK}".      
+0000bb00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000bb10: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000bb20: 7374 616e 6365 2866 696c 6570 6174 685f  stance(filepath_
+0000bb30: 6f72 5f62 7566 6665 722c 2073 7472 293a  or_buffer, str):
+0000bb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bb50: 2073 656c 662e 5f63 6865 636b 5f66 696c   self._check_fil
+0000bb60: 655f 7369 7a65 2866 696c 6570 6174 685f  e_size(filepath_
+0000bb70: 6f72 5f62 7566 6665 7229 0a20 2020 2020  or_buffer).     
+0000bb80: 2020 2020 2020 2070 616e 6461 735f 6466         pandas_df
+0000bb90: 203d 2070 616e 6461 732e 7265 6164 5f63   = pandas.read_c
+0000bba0: 7376 280a 2020 2020 2020 2020 2020 2020  sv(.            
+0000bbb0: 2020 2020 6669 6c65 7061 7468 5f6f 725f      filepath_or_
+0000bbc0: 6275 6666 6572 2c0a 2020 2020 2020 2020  buffer,.        
+0000bbd0: 2020 2020 2020 2020 7365 703d 7365 702c          sep=sep,
+0000bbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bbf0: 2068 6561 6465 723d 6865 6164 6572 2c0a   header=header,.
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 6e61 6d65 733d 6e61 6d65 732c 0a20 2020  names=names,.   
+0000bc20: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000bc30: 6578 5f63 6f6c 3d69 6e64 6578 5f63 6f6c  ex_col=index_col
+0000bc40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bc50: 2020 7573 6563 6f6c 733d 7573 6563 6f6c    usecols=usecol
+0000bc60: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
+0000bc70: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+0000bc80: 2020 2064 7479 7065 3d64 7479 7065 2c0a     dtype=dtype,.
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 656e 6769 6e65 3d65 6e67 696e 652c 0a20  engine=engine,. 
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000bcc0: 6e63 6f64 696e 673d 656e 636f 6469 6e67  ncoding=encoding
+0000bcd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bce0: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
+0000bcf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000bd00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000bd10: 662e 5f72 6561 645f 7061 6e64 6173 2870  f._read_pandas(p
+0000bd20: 616e 6461 735f 6466 2c20 2272 6561 645f  andas_df, "read_
+0000bd30: 6373 7622 2920 2023 2074 7970 653a 2069  csv")  # type: i
+0000bd40: 676e 6f72 650a 0a20 2020 2064 6566 2072  gnore..    def r
+0000bd50: 6561 645f 7069 636b 6c65 280a 2020 2020  ead_pickle(.    
+0000bd60: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000bd70: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
+0000bd80: 6666 6572 3a20 4669 6c65 5061 7468 207c  ffer: FilePath |
+0000bd90: 2052 6561 6450 6963 6b6c 6542 7566 6665   ReadPickleBuffe
+0000bda0: 722c 0a20 2020 2020 2020 2063 6f6d 7072  r,.        compr
+0000bdb0: 6573 7369 6f6e 3a20 436f 6d70 7265 7373  ession: Compress
+0000bdc0: 696f 6e4f 7074 696f 6e73 203d 2022 696e  ionOptions = "in
+0000bdd0: 6665 7222 2c0a 2020 2020 2020 2020 7374  fer",.        st
+0000bde0: 6f72 6167 655f 6f70 7469 6f6e 733a 2053  orage_options: S
+0000bdf0: 746f 7261 6765 4f70 7469 6f6e 7320 3d20  torageOptions = 
+0000be00: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0000be10: 2020 2020 2070 616e 6461 735f 6f62 6a20       pandas_obj 
+0000be20: 3d20 7061 6e64 6173 2e72 6561 645f 7069  = pandas.read_pi
+0000be30: 636b 6c65 280a 2020 2020 2020 2020 2020  ckle(.          
+0000be40: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
+0000be50: 6666 6572 2c0a 2020 2020 2020 2020 2020  ffer,.          
+0000be60: 2020 636f 6d70 7265 7373 696f 6e3d 636f    compression=co
+0000be70: 6d70 7265 7373 696f 6e2c 0a20 2020 2020  mpression,.     
+0000be80: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
+0000be90: 7074 696f 6e73 3d73 746f 7261 6765 5f6f  ptions=storage_o
+0000bea0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
+0000beb0: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
+0000bec0: 696e 7374 616e 6365 2870 616e 6461 735f  instance(pandas_
+0000bed0: 6f62 6a2c 2070 616e 6461 732e 5365 7269  obj, pandas.Seri
+0000bee0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+0000bef0: 2069 6620 7061 6e64 6173 5f6f 626a 2e6e   if pandas_obj.n
+0000bf00: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
+0000bf10: 2020 2020 2020 2020 2020 2020 2070 616e               pan
+0000bf20: 6461 735f 6f62 6a2e 6e61 6d65 203d 2022  das_obj.name = "
+0000bf30: 3022 0a20 2020 2020 2020 2020 2020 2062  0".            b
+0000bf40: 6967 6672 616d 6573 5f64 6620 3d20 7365  igframes_df = se
+0000bf50: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
+0000bf60: 7061 6e64 6173 5f6f 626a 2e74 6f5f 6672  pandas_obj.to_fr
+0000bf70: 616d 6528 292c 2022 7265 6164 5f70 6963  ame(), "read_pic
+0000bf80: 6b6c 6522 290a 2020 2020 2020 2020 2020  kle").          
+0000bf90: 2020 7265 7475 726e 2062 6967 6672 616d    return bigfram
+0000bfa0: 6573 5f64 665b 6269 6766 7261 6d65 735f  es_df[bigframes_
+0000bfb0: 6466 2e63 6f6c 756d 6e73 5b30 5d5d 0a20  df.columns[0]]. 
+0000bfc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000bfd0: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
+0000bfe0: 7061 6e64 6173 5f6f 626a 2c20 2272 6561  pandas_obj, "rea
+0000bff0: 645f 7069 636b 6c65 2229 0a0a 2020 2020  d_pickle")..    
+0000c000: 6465 6620 7265 6164 5f70 6172 7175 6574  def read_parquet
+0000c010: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000c020: 2020 2020 2020 2020 7061 7468 3a20 7374          path: st
+0000c030: 7220 7c20 494f 5b22 6279 7465 7322 5d2c  r | IO["bytes"],
+0000c040: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000c050: 2020 2020 656e 6769 6e65 3a20 7374 7220      engine: str 
+0000c060: 3d20 2261 7574 6f22 2c0a 2020 2020 2920  = "auto",.    ) 
+0000c070: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
+0000c080: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+0000c090: 7461 626c 6520 3d20 6269 6766 7261 6d65  table = bigframe
+0000c0a0: 735f 696f 2e72 616e 646f 6d5f 7461 626c  s_io.random_tabl
+0000c0b0: 6528 7365 6c66 2e5f 616e 6f6e 796d 6f75  e(self._anonymou
+0000c0c0: 735f 6461 7461 7365 7429 0a0a 2020 2020  s_dataset)..    
+0000c0d0: 2020 2020 6966 2065 6e67 696e 6520 3d3d      if engine ==
+0000c0e0: 2022 6269 6771 7565 7279 223a 0a20 2020   "bigquery":.   
+0000c0f0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000c100: 6669 6720 3d20 7365 6c66 2e5f 7072 6570  fig = self._prep
+0000c110: 6172 655f 6c6f 6164 5f6a 6f62 5f63 6f6e  are_load_job_con
+0000c120: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
+0000c130: 2020 6a6f 625f 636f 6e66 6967 2e63 7265    job_config.cre
+0000c140: 6174 655f 6469 7370 6f73 6974 696f 6e20  ate_disposition 
+0000c150: 3d20 6269 6771 7565 7279 2e43 7265 6174  = bigquery.Creat
+0000c160: 6544 6973 706f 7369 7469 6f6e 2e43 5245  eDisposition.CRE
+0000c170: 4154 455f 4946 5f4e 4545 4445 440a 2020  ATE_IF_NEEDED.  
+0000c180: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
+0000c190: 6e66 6967 2e73 6f75 7263 655f 666f 726d  nfig.source_form
+0000c1a0: 6174 203d 2062 6967 7175 6572 792e 536f  at = bigquery.So
+0000c1b0: 7572 6365 466f 726d 6174 2e50 4152 5155  urceFormat.PARQU
+0000c1c0: 4554 0a20 2020 2020 2020 2020 2020 206a  ET.            j
+0000c1d0: 6f62 5f63 6f6e 6669 672e 7772 6974 655f  ob_config.write_
+0000c1e0: 6469 7370 6f73 6974 696f 6e20 3d20 6269  disposition = bi
+0000c1f0: 6771 7565 7279 2e57 7269 7465 4469 7370  gquery.WriteDisp
+0000c200: 6f73 6974 696f 6e2e 5752 4954 455f 454d  osition.WRITE_EM
+0000c210: 5054 590a 2020 2020 2020 2020 2020 2020  PTY.            
+0000c220: 6a6f 625f 636f 6e66 6967 2e6c 6162 656c  job_config.label
+0000c230: 7320 3d20 7b22 6269 6766 7261 6d65 732d  s = {"bigframes-
+0000c240: 6170 6922 3a20 2272 6561 645f 7061 7271  api": "read_parq
+0000c250: 7565 7422 7d0a 0a20 2020 2020 2020 2020  uet"}..         
+0000c260: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000c270: 7265 6164 5f62 6967 7175 6572 795f 6c6f  read_bigquery_lo
+0000c280: 6164 5f6a 6f62 2870 6174 682c 2074 6162  ad_job(path, tab
+0000c290: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
+0000c2a0: 6f62 5f63 6f6e 6669 6729 0a20 2020 2020  ob_config).     
+0000c2b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c2c0: 2020 2020 2072 6561 645f 7061 7271 7565       read_parque
+0000c2d0: 745f 6b77 6172 6773 3a20 4469 6374 5b73  t_kwargs: Dict[s
+0000c2e0: 7472 2c20 416e 795d 203d 207b 7d0a 2020  tr, Any] = {}.  
+0000c2f0: 2020 2020 2020 2020 2020 6966 2070 616e            if pan
+0000c300: 6461 732e 5f5f 7665 7273 696f 6e5f 5f2e  das.__version__.
+0000c310: 7374 6172 7473 7769 7468 2822 312e 2229  startswith("1.")
+0000c320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c330: 2020 7265 6164 5f70 6172 7175 6574 5f6b    read_parquet_k
+0000c340: 7761 7267 735b 2275 7365 5f6e 756c 6c61  wargs["use_nulla
+0000c350: 626c 655f 6474 7970 6573 225d 203d 2054  ble_dtypes"] = T
+0000c360: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000c370: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000c380: 2020 2020 2020 7265 6164 5f70 6172 7175        read_parqu
+0000c390: 6574 5f6b 7761 7267 735b 2264 7479 7065  et_kwargs["dtype
+0000c3a0: 5f62 6163 6b65 6e64 225d 203d 2022 7079  _backend"] = "py
+0000c3b0: 6172 726f 7722 0a0a 2020 2020 2020 2020  arrow"..        
+0000c3c0: 2020 2020 7061 6e64 6173 5f6f 626a 203d      pandas_obj =
+0000c3d0: 2070 616e 6461 732e 7265 6164 5f70 6172   pandas.read_par
+0000c3e0: 7175 6574 280a 2020 2020 2020 2020 2020  quet(.          
+0000c3f0: 2020 2020 2020 7061 7468 2c0a 2020 2020        path,.    
+0000c400: 2020 2020 2020 2020 2020 2020 656e 6769              engi
+0000c410: 6e65 3d65 6e67 696e 652c 2020 2320 7479  ne=engine,  # ty
+0000c420: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
+0000c430: 2020 2020 2020 2020 2020 202a 2a72 6561             **rea
+0000c440: 645f 7061 7271 7565 745f 6b77 6172 6773  d_parquet_kwargs
+0000c450: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000c460: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c470: 726e 2073 656c 662e 5f72 6561 645f 7061  rn self._read_pa
+0000c480: 6e64 6173 2870 616e 6461 735f 6f62 6a2c  ndas(pandas_obj,
+0000c490: 2022 7265 6164 5f70 6172 7175 6574 2229   "read_parquet")
+0000c4a0: 0a0a 2020 2020 6465 6620 7265 6164 5f6a  ..    def read_j
+0000c4b0: 736f 6e28 0a20 2020 2020 2020 2073 656c  son(.        sel
+0000c4c0: 662c 0a20 2020 2020 2020 2070 6174 685f  f,.        path_
+0000c4d0: 6f72 5f62 7566 3a20 7374 7220 7c20 494f  or_buf: str | IO
+0000c4e0: 5b22 6279 7465 7322 5d2c 0a20 2020 2020  ["bytes"],.     
+0000c4f0: 2020 202a 2c0a 2020 2020 2020 2020 6f72     *,.        or
+0000c500: 6965 6e74 3a20 4c69 7465 7261 6c5b 0a20  ient: Literal[. 
+0000c510: 2020 2020 2020 2020 2020 2022 7370 6c69             "spli
+0000c520: 7422 2c20 2272 6563 6f72 6473 222c 2022  t", "records", "
+0000c530: 696e 6465 7822 2c20 2263 6f6c 756d 6e73  index", "columns
+0000c540: 222c 2022 7661 6c75 6573 222c 2022 7461  ", "values", "ta
+0000c550: 626c 6522 0a20 2020 2020 2020 205d 203d  ble".        ] =
+0000c560: 2022 636f 6c75 6d6e 7322 2c0a 2020 2020   "columns",.    
+0000c570: 2020 2020 6474 7970 653a 204f 7074 696f      dtype: Optio
+0000c580: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
+0000c590: 2c0a 2020 2020 2020 2020 656e 636f 6469  ,.        encodi
+0000c5a0: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
+0000c5b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000c5c0: 2020 6c69 6e65 733a 2062 6f6f 6c20 3d20    lines: bool = 
+0000c5d0: 4661 6c73 652c 0a20 2020 2020 2020 2065  False,.        e
+0000c5e0: 6e67 696e 653a 204c 6974 6572 616c 5b22  ngine: Literal["
+0000c5f0: 756a 736f 6e22 2c20 2270 7961 7272 6f77  ujson", "pyarrow
+0000c600: 222c 2022 6269 6771 7565 7279 225d 203d  ", "bigquery"] =
+0000c610: 2022 756a 736f 6e22 2c0a 2020 2020 2020   "ujson",.      
+0000c620: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
+0000c630: 2920 2d3e 2064 6174 6166 7261 6d65 2e44  ) -> dataframe.D
+0000c640: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
+0000c650: 2020 7461 626c 6520 3d20 6269 6766 7261    table = bigfra
+0000c660: 6d65 735f 696f 2e72 616e 646f 6d5f 7461  mes_io.random_ta
+0000c670: 626c 6528 7365 6c66 2e5f 616e 6f6e 796d  ble(self._anonym
+0000c680: 6f75 735f 6461 7461 7365 7429 0a0a 2020  ous_dataset)..  
+0000c690: 2020 2020 2020 6966 2065 6e67 696e 6520        if engine 
+0000c6a0: 3d3d 2022 6269 6771 7565 7279 223a 0a0a  == "bigquery":..
+0000c6b0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000c6c0: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+0000c6d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c6e0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000c6f0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
+0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c710: 2022 4269 6751 7565 7279 2065 6e67 696e   "BigQuery engin
+0000c720: 6520 646f 6573 206e 6f74 2073 7570 706f  e does not suppo
+0000c730: 7274 2074 6865 2064 7479 7065 2061 7267  rt the dtype arg
+0000c740: 756d 656e 7473 2e22 0a20 2020 2020 2020  uments.".       
+0000c750: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000c760: 2020 2020 2020 2020 6966 206e 6f74 206c          if not l
+0000c770: 696e 6573 3a0a 2020 2020 2020 2020 2020  ines:.          
+0000c780: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+0000c790: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+0000c7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c7b0: 2020 2020 2022 4f6e 6c79 206e 6577 6c69       "Only newli
+0000c7c0: 6e65 2064 656c 696d 6974 6564 204a 534f  ne delimited JSO
+0000c7d0: 4e20 666f 726d 6174 2069 7320 7375 7070  N format is supp
+0000c7e0: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
+0000c7f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000c800: 2020 2020 2020 2069 6620 656e 636f 6469         if encodi
+0000c810: 6e67 2069 7320 6e6f 7420 4e6f 6e65 2061  ng is not None a
+0000c820: 6e64 2065 6e63 6f64 696e 6720 6e6f 7420  nd encoding not 
+0000c830: 696e 205f 5641 4c49 445f 454e 434f 4449  in _VALID_ENCODI
+0000c840: 4e47 533a 0a20 2020 2020 2020 2020 2020  NGS:.           
+0000c850: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+0000c860: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
+0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c880: 2020 2020 6622 4269 6751 7565 7279 2065      f"BigQuery e
+0000c890: 6e67 696e 6520 6f6e 6c79 2073 7570 706f  ngine only suppo
+0000c8a0: 7274 7320 7468 6520 666f 6c6c 6f77 696e  rts the followin
+0000c8b0: 6720 656e 636f 6469 6e67 733a 207b 5f56  g encodings: {_V
+0000c8c0: 414c 4944 5f45 4e43 4f44 494e 4753 7d22  ALID_ENCODINGS}"
+0000c8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c8e0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+0000c8f0: 6966 206c 696e 6573 2061 6e64 206f 7269  if lines and ori
+0000c900: 656e 7420 213d 2022 7265 636f 7264 7322  ent != "records"
+0000c910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c920: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000c930: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000c940: 2020 2020 2020 2020 2227 6c69 6e65 7327          "'lines'
+0000c950: 206b 6579 776f 7264 2069 7320 6f6e 6c79   keyword is only
+0000c960: 2076 616c 6964 2077 6865 6e20 276f 7269   valid when 'ori
+0000c970: 656e 7427 2069 7320 2772 6563 6f72 6473  ent' is 'records
+0000c980: 272e 220a 2020 2020 2020 2020 2020 2020  '.".            
+0000c990: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+0000c9a0: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
+0000c9b0: 7365 6c66 2e5f 7072 6570 6172 655f 6c6f  self._prepare_lo
+0000c9c0: 6164 5f6a 6f62 5f63 6f6e 6669 6728 290a  ad_job_config().
+0000c9d0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+0000c9e0: 636f 6e66 6967 2e63 7265 6174 655f 6469  config.create_di
+0000c9f0: 7370 6f73 6974 696f 6e20 3d20 6269 6771  sposition = bigq
+0000ca00: 7565 7279 2e43 7265 6174 6544 6973 706f  uery.CreateDispo
+0000ca10: 7369 7469 6f6e 2e43 5245 4154 455f 4946  sition.CREATE_IF
+0000ca20: 5f4e 4545 4445 440a 2020 2020 2020 2020  _NEEDED.        
+0000ca30: 2020 2020 6a6f 625f 636f 6e66 6967 2e73      job_config.s
+0000ca40: 6f75 7263 655f 666f 726d 6174 203d 2062  ource_format = b
+0000ca50: 6967 7175 6572 792e 536f 7572 6365 466f  igquery.SourceFo
+0000ca60: 726d 6174 2e4e 4557 4c49 4e45 5f44 454c  rmat.NEWLINE_DEL
+0000ca70: 494d 4954 4544 5f4a 534f 4e0a 2020 2020  IMITED_JSON.    
+0000ca80: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+0000ca90: 6967 2e77 7269 7465 5f64 6973 706f 7369  ig.write_disposi
+0000caa0: 7469 6f6e 203d 2062 6967 7175 6572 792e  tion = bigquery.
+0000cab0: 5772 6974 6544 6973 706f 7369 7469 6f6e  WriteDisposition
+0000cac0: 2e57 5249 5445 5f45 4d50 5459 0a20 2020  .WRITE_EMPTY.   
+0000cad0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000cae0: 6669 672e 6175 746f 6465 7465 6374 203d  fig.autodetect =
+0000caf0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000cb00: 2020 6a6f 625f 636f 6e66 6967 2e65 6e63    job_config.enc
+0000cb10: 6f64 696e 6720 3d20 656e 636f 6469 6e67  oding = encoding
+0000cb20: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
+0000cb30: 5f63 6f6e 6669 672e 6c61 6265 6c73 203d  _config.labels =
+0000cb40: 207b 2262 6967 6672 616d 6573 2d61 7069   {"bigframes-api
+0000cb50: 223a 2022 7265 6164 5f6a 736f 6e22 7d0a  ": "read_json"}.
+0000cb60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000cb70: 7572 6e20 7365 6c66 2e5f 7265 6164 5f62  urn self._read_b
+0000cb80: 6967 7175 6572 795f 6c6f 6164 5f6a 6f62  igquery_load_job
+0000cb90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000cba0: 2020 7061 7468 5f6f 725f 6275 662c 0a20    path_or_buf,. 
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000cbc0: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
+0000cbd0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+0000cbe0: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
+0000cbf0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000cc00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000cc10: 2020 2020 2069 6620 616e 7928 6172 6720       if any(arg 
+0000cc20: 696e 206b 7761 7267 7320 666f 7220 6172  in kwargs for ar
+0000cc30: 6720 696e 2028 2263 6875 6e6b 7369 7a65  g in ("chunksize
+0000cc40: 222c 2022 6974 6572 6174 6f72 2229 293a  ", "iterator")):
+0000cc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc60: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000cc70: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
+0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2227 6368 756e 6b73 697a 6527 2061 6e64  "'chunksize' and
+0000cca0: 2027 6974 6572 6174 6f72 2720 6172 6775   'iterator' argu
+0000ccb0: 6d65 6e74 7320 6172 6520 6e6f 7420 7375  ments are not su
+0000ccc0: 7070 6f72 7465 642e 220a 2020 2020 2020  pported.".      
+0000ccd0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000cce0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000ccf0: 7374 616e 6365 2870 6174 685f 6f72 5f62  stance(path_or_b
+0000cd00: 7566 2c20 7374 7229 3a0a 2020 2020 2020  uf, str):.      
+0000cd10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000cd20: 6368 6563 6b5f 6669 6c65 5f73 697a 6528  check_file_size(
+0000cd30: 7061 7468 5f6f 725f 6275 6629 0a0a 2020  path_or_buf)..  
+0000cd40: 2020 2020 2020 2020 2020 6966 2065 6e67            if eng
+0000cd50: 696e 6520 3d3d 2022 756a 736f 6e22 3a0a  ine == "ujson":.
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 7061 6e64 6173 5f64 6620 3d20 7061 6e64  pandas_df = pand
+0000cd80: 6173 2e72 6561 645f 6a73 6f6e 2820 2023  as.read_json(  #
+0000cd90: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 7061 7468 5f6f 725f 6275 662c 0a20    path_or_buf,. 
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 2020 206f 7269 656e 743d 6f72 6965 6e74     orient=orient
+0000cde0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cdf0: 2020 2020 2020 6474 7970 653d 6474 7970        dtype=dtyp
+0000ce00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000ce10: 2020 2020 2020 2065 6e63 6f64 696e 673d         encoding=
+0000ce20: 656e 636f 6469 6e67 2c0a 2020 2020 2020  encoding,.      
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000ce40: 6e65 733d 6c69 6e65 732c 0a20 2020 2020  nes=lines,.     
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000ce60: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
+0000ce70: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000ce80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ce90: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000cea0: 6e64 6173 5f64 6620 3d20 7061 6e64 6173  ndas_df = pandas
+0000ceb0: 2e72 6561 645f 6a73 6f6e 2820 2023 2074  .read_json(  # t
+0000cec0: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
 0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000cee0: 7061 7468 5f6f 725f 6275 662c 0a20 2020  path_or_buf,.   
-0000cef0: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-0000cf00: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
-0000cf10: 2020 2020 6a6f 625f 636f 6e66 6967 3d6a      job_config=j
-0000cf20: 6f62 5f63 6f6e 6669 672c 0a20 2020 2020  ob_config,.     
-0000cf30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000cf40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000cf50: 2020 2069 6620 616e 7928 6172 6720 696e     if any(arg in
-0000cf60: 206b 7761 7267 7320 666f 7220 6172 6720   kwargs for arg 
-0000cf70: 696e 2028 2263 6875 6e6b 7369 7a65 222c  in ("chunksize",
-0000cf80: 2022 6974 6572 6174 6f72 2229 293a 0a20   "iterator")):. 
-0000cf90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000cfa0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000cfb0: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-0000cfd0: 6368 756e 6b73 697a 6527 2061 6e64 2027  chunksize' and '
-0000cfe0: 6974 6572 6174 6f72 2720 6172 6775 6d65  iterator' argume
-0000cff0: 6e74 7320 6172 6520 6e6f 7420 7375 7070  nts are not supp
-0000d000: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
-0000d010: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000d020: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0000d030: 616e 6365 2870 6174 685f 6f72 5f62 7566  ance(path_or_buf
-0000d040: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0000d050: 2020 2020 2020 2020 7365 6c66 2e5f 6368          self._ch
-0000d060: 6563 6b5f 6669 6c65 5f73 697a 6528 7061  eck_file_size(pa
-0000d070: 7468 5f6f 725f 6275 6629 0a0a 2020 2020  th_or_buf)..    
-0000d080: 2020 2020 2020 2020 6966 2065 6e67 696e          if engin
-0000d090: 6520 3d3d 2022 756a 736f 6e22 3a0a 2020  e == "ujson":.  
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000d0b0: 6e64 6173 5f64 6620 3d20 7061 6e64 6173  ndas_df = pandas
-0000d0c0: 2e72 6561 645f 6a73 6f6e 2820 2023 2074  .read_json(  # t
-0000d0d0: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0f0: 7061 7468 5f6f 725f 6275 662c 0a20 2020  path_or_buf,.   
-0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 206f 7269 656e 743d 6f72 6965 6e74 2c0a   orient=orient,.
-0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d130: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
-0000d140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d150: 2020 2020 2065 6e63 6f64 696e 673d 656e       encoding=en
-0000d160: 636f 6469 6e67 2c0a 2020 2020 2020 2020  coding,.        
-0000d170: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000d180: 733d 6c69 6e65 732c 0a20 2020 2020 2020  s=lines,.       
-0000d190: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
-0000d1a0: 7761 7267 732c 0a20 2020 2020 2020 2020  wargs,.         
-0000d1b0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000d1c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000d1d0: 2020 2020 2020 2020 2020 2020 7061 6e64              pand
-0000d1e0: 6173 5f64 6620 3d20 7061 6e64 6173 2e72  as_df = pandas.r
-0000d1f0: 6561 645f 6a73 6f6e 2820 2023 2074 7970  ead_json(  # typ
-0000d200: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
-0000d210: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000d220: 7468 5f6f 725f 6275 662c 0a20 2020 2020  th_or_buf,.     
-0000d230: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000d240: 7269 656e 743d 6f72 6965 6e74 2c0a 2020  rient=orient,.  
-0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d260: 2020 6474 7970 653d 6474 7970 652c 0a20    dtype=dtype,. 
-0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d280: 2020 2065 6e63 6f64 696e 673d 656e 636f     encoding=enco
-0000d290: 6469 6e67 2c0a 2020 2020 2020 2020 2020  ding,.          
-0000d2a0: 2020 2020 2020 2020 2020 6c69 6e65 733d            lines=
-0000d2b0: 6c69 6e65 732c 0a20 2020 2020 2020 2020  lines,.         
-0000d2c0: 2020 2020 2020 2020 2020 2065 6e67 696e             engin
-0000d2d0: 653d 656e 6769 6e65 2c0a 2020 2020 2020  e=engine,.      
-0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-0000d2f0: 6b77 6172 6773 2c0a 2020 2020 2020 2020  kwargs,.        
-0000d300: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d310: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000d320: 662e 5f72 6561 645f 7061 6e64 6173 2870  f._read_pandas(p
-0000d330: 616e 6461 735f 6466 2c20 2272 6561 645f  andas_df, "read_
-0000d340: 6a73 6f6e 2229 0a0a 2020 2020 6465 6620  json")..    def 
-0000d350: 5f63 6865 636b 5f66 696c 655f 7369 7a65  _check_file_size
-0000d360: 2873 656c 662c 2066 696c 6570 6174 683a  (self, filepath:
-0000d370: 2073 7472 293a 0a20 2020 2020 2020 206d   str):.        m
-0000d380: 6178 5f73 697a 6520 3d20 3130 3234 202a  ax_size = 1024 *
-0000d390: 2031 3032 3420 2a20 3130 3234 2020 2320   1024 * 1024  # 
-0000d3a0: 3120 4742 2069 6e20 6279 7465 730a 2020  1 GB in bytes.  
-0000d3b0: 2020 2020 2020 6966 2066 696c 6570 6174        if filepat
-0000d3c0: 682e 7374 6172 7473 7769 7468 2822 6773  h.startswith("gs
-0000d3d0: 3a2f 2f22 293a 2020 2320 4743 5320 6669  ://"):  # GCS fi
-0000d3e0: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
-0000d3f0: 2020 2020 636c 6965 6e74 203d 2073 746f      client = sto
-0000d400: 7261 6765 2e43 6c69 656e 7428 290a 2020  rage.Client().  
-0000d410: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
-0000d420: 5f6e 616d 652c 2062 6c6f 625f 6e61 6d65  _name, blob_name
-0000d430: 203d 2066 696c 6570 6174 682e 7370 6c69   = filepath.spli
-0000d440: 7428 222f 222c 2033 295b 323a 5d0a 2020  t("/", 3)[2:].  
-0000d450: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
-0000d460: 203d 2063 6c69 656e 742e 6275 636b 6574   = client.bucket
-0000d470: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-0000d480: 2020 2020 2020 2020 2020 626c 6f62 203d            blob =
-0000d490: 2062 7563 6b65 742e 626c 6f62 2862 6c6f   bucket.blob(blo
-0000d4a0: 625f 6e61 6d65 290a 2020 2020 2020 2020  b_name).        
-0000d4b0: 2020 2020 626c 6f62 2e72 656c 6f61 6428      blob.reload(
-0000d4c0: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
-0000d4d0: 6c65 5f73 697a 6520 3d20 626c 6f62 2e73  le_size = blob.s
-0000d4e0: 697a 650a 2020 2020 2020 2020 656c 7365  ize.        else
-0000d4f0: 3a20 2023 206c 6f63 616c 2066 696c 6520  :  # local file 
-0000d500: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-0000d510: 2066 696c 655f 7369 7a65 203d 206f 732e   file_size = os.
-0000d520: 7061 7468 2e67 6574 7369 7a65 2866 696c  path.getsize(fil
-0000d530: 6570 6174 6829 0a0a 2020 2020 2020 2020  epath)..        
-0000d540: 6966 2066 696c 655f 7369 7a65 203e 206d  if file_size > m
-0000d550: 6178 5f73 697a 653a 0a20 2020 2020 2020  ax_size:.       
-0000d560: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
-0000d570: 6f20 4742 0a20 2020 2020 2020 2020 2020  o GB.           
-0000d580: 2066 696c 655f 7369 7a65 203d 2072 6f75   file_size = rou
-0000d590: 6e64 2866 696c 655f 7369 7a65 202f 2028  nd(file_size / (
-0000d5a0: 3130 3234 2a2a 3329 2c20 3129 0a20 2020  1024**3), 1).   
-0000d5b0: 2020 2020 2020 2020 206d 6178 5f73 697a           max_siz
-0000d5c0: 6520 3d20 696e 7428 6d61 785f 7369 7a65  e = int(max_size
-0000d5d0: 202f 2031 3032 342a 2a33 290a 2020 2020   / 1024**3).    
-0000d5e0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-0000d5f0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-0000d600: 2020 2020 2020 2020 6622 4669 6c65 2073          f"File s
-0000d610: 697a 6520 7b66 696c 655f 7369 7a65 7d47  ize {file_size}G
-0000d620: 4220 6578 6365 6564 7320 7b6d 6178 5f73  B exceeds {max_s
-0000d630: 697a 657d 4742 2e20 220a 2020 2020 2020  ize}GB. ".      
-0000d640: 2020 2020 2020 2020 2020 2249 7420 6973            "It is
-0000d650: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-0000d660: 7573 6520 656e 6769 6e65 3d27 6269 6771  use engine='bigq
-0000d670: 7565 7279 2720 220a 2020 2020 2020 2020  uery' ".        
-0000d680: 2020 2020 2020 2020 2266 6f72 206c 6172          "for lar
-0000d690: 6765 2066 696c 6573 2074 6f20 6176 6f69  ge files to avoi
-0000d6a0: 6420 6c6f 6164 696e 6720 7468 6520 6669  d loading the fi
-0000d6b0: 6c65 2069 6e74 6f20 6c6f 6361 6c20 6d65  le into local me
-0000d6c0: 6d6f 7279 2e22 0a20 2020 2020 2020 2020  mory.".         
-0000d6d0: 2020 2029 0a0a 2020 2020 6465 6620 5f63     )..    def _c
-0000d6e0: 7265 6174 655f 656d 7074 795f 7465 6d70  reate_empty_temp
-0000d6f0: 5f74 6162 6c65 280a 2020 2020 2020 2020  _table(.        
-0000d700: 7365 6c66 2c0a 2020 2020 2020 2020 7363  self,.        sc
-0000d710: 6865 6d61 3a20 4974 6572 6162 6c65 5b62  hema: Iterable[b
-0000d720: 6967 7175 6572 792e 5363 6865 6d61 4669  igquery.SchemaFi
-0000d730: 656c 645d 2c0a 2020 2020 2020 2020 636c  eld],.        cl
-0000d740: 7573 7465 725f 636f 6c73 3a20 4c69 7374  uster_cols: List
-0000d750: 5b73 7472 5d2c 0a20 2020 2029 202d 3e20  [str],.    ) -> 
-0000d760: 6269 6771 7565 7279 2e54 6162 6c65 5265  bigquery.TableRe
-0000d770: 6665 7265 6e63 653a 0a20 2020 2020 2020  ference:.       
-0000d780: 2023 2043 616e 2774 2073 6574 2061 2074   # Can't set a t
-0000d790: 6162 6c65 2069 6e20 5f53 4553 5349 4f4e  able in _SESSION
-0000d7a0: 2061 7320 6465 7374 696e 6174 696f 6e20   as destination 
-0000d7b0: 7669 6120 7175 6572 7920 6a6f 6220 4150  via query job AP
-0000d7c0: 492c 2073 6f20 7765 0a20 2020 2020 2020  I, so we.       
-0000d7d0: 2023 2072 756e 2044 444c 2c20 696e 7374   # run DDL, inst
-0000d7e0: 6561 642e 0a20 2020 2020 2020 2064 6174  ead..        dat
-0000d7f0: 6173 6574 203d 2073 656c 662e 5f61 6e6f  aset = self._ano
-0000d800: 6e79 6d6f 7573 5f64 6174 6173 6574 0a20  nymous_dataset. 
-0000d810: 2020 2020 2020 2065 7870 6972 6174 696f         expiratio
-0000d820: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
-0000d830: 2020 6461 7465 7469 6d65 2e64 6174 6574    datetime.datet
-0000d840: 696d 652e 6e6f 7728 6461 7465 7469 6d65  ime.now(datetime
-0000d850: 2e74 696d 657a 6f6e 652e 7574 6329 202b  .timezone.utc) +
-0000d860: 2063 6f6e 7374 616e 7473 2e44 4546 4155   constants.DEFAU
-0000d870: 4c54 5f45 5850 4952 4154 494f 4e0a 2020  LT_EXPIRATION.  
-0000d880: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000d890: 2074 6162 6c65 203d 2062 6967 6672 616d   table = bigfram
-0000d8a0: 6573 5f69 6f2e 6372 6561 7465 5f74 656d  es_io.create_tem
-0000d8b0: 705f 7461 626c 6528 0a20 2020 2020 2020  p_table(.       
-0000d8c0: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
-0000d8d0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-0000d8e0: 6461 7461 7365 742c 0a20 2020 2020 2020  dataset,.       
-0000d8f0: 2020 2020 2065 7870 6972 6174 696f 6e2c       expiration,
-0000d900: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
-0000d910: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
-0000d920: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
-0000d930: 636f 6c75 6d6e 733d 636c 7573 7465 725f  columns=cluster_
-0000d940: 636f 6c73 2c0a 2020 2020 2020 2020 290a  cols,.        ).
-0000d950: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-0000d960: 6967 7175 6572 792e 5461 626c 6552 6566  igquery.TableRef
-0000d970: 6572 656e 6365 2e66 726f 6d5f 7374 7269  erence.from_stri
-0000d980: 6e67 2874 6162 6c65 290a 0a20 2020 2064  ng(table)..    d
-0000d990: 6566 205f 6372 6561 7465 5f74 6f74 616c  ef _create_total
-0000d9a0: 5f6f 7264 6572 696e 6728 0a20 2020 2020  _ordering(.     
-0000d9b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000d9c0: 2074 6162 6c65 3a20 6962 6973 5f74 7970   table: ibis_typ
-0000d9d0: 6573 2e54 6162 6c65 2c0a 2020 2020 2920  es.Table,.    ) 
-0000d9e0: 2d3e 2063 6f72 652e 4172 7261 7956 616c  -> core.ArrayVal
-0000d9f0: 7565 3a0a 2020 2020 2020 2020 2320 5369  ue:.        # Si
-0000da00: 6e63 6520 7468 6973 206d 6967 6874 2061  nce this might a
-0000da10: 6c73 6f20 6265 2075 7365 6420 6173 2074  lso be used as t
-0000da20: 6865 2069 6e64 6578 2c20 646f 6e27 7420  he index, don't 
-0000da30: 7573 6520 7468 6520 6465 6661 756c 740a  use the default.
-0000da40: 2020 2020 2020 2020 2320 226f 7264 6572          # "order
-0000da50: 696e 6720 4944 2220 6e61 6d65 2e0a 2020  ing ID" name..  
-0000da60: 2020 2020 2020 6f72 6465 7269 6e67 5f68        ordering_h
-0000da70: 6173 685f 7061 7274 203d 2067 7569 642e  ash_part = guid.
-0000da80: 6765 6e65 7261 7465 5f67 7569 6428 2262  generate_guid("b
-0000da90: 6967 6672 616d 6573 5f6f 7264 6572 696e  igframes_orderin
-0000daa0: 675f 2229 0a20 2020 2020 2020 206f 7264  g_").        ord
-0000dab0: 6572 696e 675f 7261 6e64 5f70 6172 7420  ering_rand_part 
-0000dac0: 3d20 6775 6964 2e67 656e 6572 6174 655f  = guid.generate_
-0000dad0: 6775 6964 2822 6269 6766 7261 6d65 735f  guid("bigframes_
-0000dae0: 6f72 6465 7269 6e67 5f22 290a 0a20 2020  ordering_")..   
-0000daf0: 2020 2020 2023 2041 6c6c 2069 6e70 7574       # All input
-0000db00: 7320 696e 746f 2068 6173 6820 6d75 7374  s into hash must
-0000db10: 2062 6520 6e6f 6e2d 6e75 6c6c 206f 7220   be non-null or 
-0000db20: 7265 7375 6c74 696e 6720 6861 7368 2077  resulting hash w
-0000db30: 696c 6c20 6265 206e 756c 6c0a 2020 2020  ill be null.    
-0000db40: 2020 2020 7374 725f 7661 6c75 6573 203d      str_values =
-0000db50: 206c 6973 7428 0a20 2020 2020 2020 2020   list(.         
-0000db60: 2020 206d 6170 286c 616d 6264 6120 636f     map(lambda co
-0000db70: 6c3a 205f 636f 6e76 6572 745f 746f 5f6e  l: _convert_to_n
-0000db80: 6f6e 6e75 6c6c 5f73 7472 696e 6728 7461  onnull_string(ta
-0000db90: 626c 655b 636f 6c5d 292c 2074 6162 6c65  ble[col]), table
-0000dba0: 2e63 6f6c 756d 6e73 290a 2020 2020 2020  .columns).      
-0000dbb0: 2020 290a 2020 2020 2020 2020 6675 6c6c    ).        full
-0000dbc0: 5f72 6f77 5f73 7472 203d 2028 0a20 2020  _row_str = (.   
-0000dbd0: 2020 2020 2020 2020 2073 7472 5f76 616c           str_val
-0000dbe0: 7565 735b 305d 2e63 6f6e 6361 7428 2a73  ues[0].concat(*s
-0000dbf0: 7472 5f76 616c 7565 735b 313a 5d29 0a20  tr_values[1:]). 
-0000dc00: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-0000dc10: 6e28 7374 725f 7661 6c75 6573 2920 3e20  n(str_values) > 
-0000dc20: 310a 2020 2020 2020 2020 2020 2020 656c  1.            el
-0000dc30: 7365 2073 7472 5f76 616c 7565 735b 305d  se str_values[0]
-0000dc40: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000dc50: 2020 2066 756c 6c5f 726f 775f 6861 7368     full_row_hash
-0000dc60: 203d 2066 756c 6c5f 726f 775f 7374 722e   = full_row_str.
-0000dc70: 6861 7368 2829 2e6e 616d 6528 6f72 6465  hash().name(orde
-0000dc80: 7269 6e67 5f68 6173 685f 7061 7274 290a  ring_hash_part).
-0000dc90: 2020 2020 2020 2020 2320 5573 6564 2074          # Used t
-0000dca0: 6f20 6469 7361 6d62 6967 7561 7465 2062  o disambiguate b
-0000dcb0: 6574 7765 656e 2069 6465 6e74 6963 616c  etween identical
-0000dcc0: 2072 6f77 7320 2877 6869 6368 2077 696c   rows (which wil
-0000dcd0: 6c20 6861 7665 2069 6465 6e74 6963 616c  l have identical
-0000dce0: 2068 6173 6829 0a20 2020 2020 2020 2072   hash).        r
-0000dcf0: 616e 646f 6d5f 7661 6c75 6520 3d20 6962  andom_value = ib
-0000dd00: 6973 2e72 616e 646f 6d28 292e 6e61 6d65  is.random().name
-0000dd10: 286f 7264 6572 696e 675f 7261 6e64 5f70  (ordering_rand_p
-0000dd20: 6172 7429 0a0a 2020 2020 2020 2020 6f72  art)..        or
-0000dd30: 6967 696e 616c 5f63 6f6c 756d 6e5f 6964  iginal_column_id
-0000dd40: 7320 3d20 7461 626c 652e 636f 6c75 6d6e  s = table.column
-0000dd50: 730a 2020 2020 2020 2020 7461 626c 655f  s.        table_
-0000dd60: 7769 7468 5f6f 7264 6572 696e 6720 3d20  with_ordering = 
-0000dd70: 7461 626c 652e 7365 6c65 6374 280a 2020  table.select(.  
-0000dd80: 2020 2020 2020 2020 2020 6974 6572 746f            iterto
-0000dd90: 6f6c 732e 6368 6169 6e28 6f72 6967 696e  ols.chain(origin
-0000dda0: 616c 5f63 6f6c 756d 6e5f 6964 732c 205b  al_column_ids, [
-0000ddb0: 6675 6c6c 5f72 6f77 5f68 6173 682c 2072  full_row_hash, r
-0000ddc0: 616e 646f 6d5f 7661 6c75 655d 290a 2020  andom_value]).  
-0000ddd0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000dde0: 206f 7264 6572 696e 675f 7265 6631 203d   ordering_ref1 =
-0000ddf0: 206f 7264 6572 2e61 7363 656e 6469 6e67   order.ascending
-0000de00: 5f6f 7665 7228 6f72 6465 7269 6e67 5f68  _over(ordering_h
-0000de10: 6173 685f 7061 7274 290a 2020 2020 2020  ash_part).      
-0000de20: 2020 6f72 6465 7269 6e67 5f72 6566 3220    ordering_ref2 
-0000de30: 3d20 6f72 6465 722e 6173 6365 6e64 696e  = order.ascendin
-0000de40: 675f 6f76 6572 286f 7264 6572 696e 675f  g_over(ordering_
-0000de50: 7261 6e64 5f70 6172 7429 0a20 2020 2020  rand_part).     
-0000de60: 2020 206f 7264 6572 696e 6720 3d20 6f72     ordering = or
-0000de70: 6465 722e 4578 7072 6573 7369 6f6e 4f72  der.ExpressionOr
-0000de80: 6465 7269 6e67 280a 2020 2020 2020 2020  dering(.        
-0000de90: 2020 2020 6f72 6465 7269 6e67 5f76 616c      ordering_val
-0000dea0: 7565 5f63 6f6c 756d 6e73 3d28 6f72 6465  ue_columns=(orde
-0000deb0: 7269 6e67 5f72 6566 312c 206f 7264 6572  ring_ref1, order
-0000dec0: 696e 675f 7265 6632 292c 0a20 2020 2020  ing_ref2),.     
-0000ded0: 2020 2020 2020 2074 6f74 616c 5f6f 7264         total_ord
-0000dee0: 6572 696e 675f 636f 6c75 6d6e 733d 6672  ering_columns=fr
-0000def0: 6f7a 656e 7365 7428 5b6f 7264 6572 696e  ozenset([orderin
-0000df00: 675f 6861 7368 5f70 6172 742c 206f 7264  g_hash_part, ord
-0000df10: 6572 696e 675f 7261 6e64 5f70 6172 745d  ering_rand_part]
-0000df20: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
-0000df30: 2020 2020 2063 6f6c 756d 6e73 203d 205b       columns = [
-0000df40: 7461 626c 655f 7769 7468 5f6f 7264 6572  table_with_order
-0000df50: 696e 675b 636f 6c5d 2066 6f72 2063 6f6c  ing[col] for col
-0000df60: 2069 6e20 6f72 6967 696e 616c 5f63 6f6c   in original_col
-0000df70: 756d 6e5f 6964 735d 0a20 2020 2020 2020  umn_ids].       
-0000df80: 2068 6964 6465 6e5f 636f 6c75 6d6e 7320   hidden_columns 
-0000df90: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-0000dfa0: 7461 626c 655f 7769 7468 5f6f 7264 6572  table_with_order
-0000dfb0: 696e 675b 6f72 6465 7269 6e67 5f68 6173  ing[ordering_has
-0000dfc0: 685f 7061 7274 5d2c 0a20 2020 2020 2020  h_part],.       
-0000dfd0: 2020 2020 2074 6162 6c65 5f77 6974 685f       table_with_
-0000dfe0: 6f72 6465 7269 6e67 5b6f 7264 6572 696e  ordering[orderin
-0000dff0: 675f 7261 6e64 5f70 6172 745d 2c0a 2020  g_rand_part],.  
-0000e000: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-0000e010: 7265 7475 726e 2063 6f72 652e 4172 7261  return core.Arra
-0000e020: 7956 616c 7565 2e66 726f 6d5f 6962 6973  yValue.from_ibis
-0000e030: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0000e040: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000e050: 7461 626c 655f 7769 7468 5f6f 7264 6572  table_with_order
-0000e060: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-0000e070: 2063 6f6c 756d 6e73 2c0a 2020 2020 2020   columns,.      
-0000e080: 2020 2020 2020 6869 6464 656e 5f6f 7264        hidden_ord
-0000e090: 6572 696e 675f 636f 6c75 6d6e 733d 6869  ering_columns=hi
-0000e0a0: 6464 656e 5f63 6f6c 756d 6e73 2c0a 2020  dden_columns,.  
-0000e0b0: 2020 2020 2020 2020 2020 6f72 6465 7269            orderi
-0000e0c0: 6e67 3d6f 7264 6572 696e 672c 0a20 2020  ng=ordering,.   
-0000e0d0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000e0e0: 5f69 6269 735f 746f 5f74 656d 705f 7461  _ibis_to_temp_ta
-0000e0f0: 626c 6528 0a20 2020 2020 2020 2073 656c  ble(.        sel
-0000e100: 662c 0a20 2020 2020 2020 2074 6162 6c65  f,.        table
-0000e110: 3a20 6962 6973 5f74 7970 6573 2e54 6162  : ibis_types.Tab
-0000e120: 6c65 2c0a 2020 2020 2020 2020 636c 7573  le,.        clus
-0000e130: 7465 725f 636f 6c73 3a20 4974 6572 6162  ter_cols: Iterab
-0000e140: 6c65 5b73 7472 5d2c 0a20 2020 2020 2020  le[str],.       
-0000e150: 2061 7069 5f6e 616d 653a 2073 7472 2c0a   api_name: str,.
-0000e160: 2020 2020 2920 2d3e 2062 6967 7175 6572      ) -> bigquer
-0000e170: 792e 5461 626c 6552 6566 6572 656e 6365  y.TableReference
-0000e180: 3a0a 2020 2020 2020 2020 6465 7374 696e  :.        destin
-0000e190: 6174 696f 6e2c 205f 203d 2073 656c 662e  ation, _ = self.
-0000e1a0: 5f71 7565 7279 5f74 6f5f 6465 7374 696e  _query_to_destin
-0000e1b0: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
-0000e1c0: 2020 2073 656c 662e 6962 6973 5f63 6c69     self.ibis_cli
-0000e1d0: 656e 742e 636f 6d70 696c 6528 7461 626c  ent.compile(tabl
-0000e1e0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-0000e1f0: 696e 6465 785f 636f 6c73 3d6c 6973 7428  index_cols=list(
-0000e200: 636c 7573 7465 725f 636f 6c73 292c 0a20  cluster_cols),. 
-0000e210: 2020 2020 2020 2020 2020 2061 7069 5f6e             api_n
-0000e220: 616d 653d 6170 695f 6e61 6d65 2c0a 2020  ame=api_name,.  
-0000e230: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000e240: 2320 5468 6572 6520 7368 6f75 6c64 2061  # There should a
-0000e250: 6c77 6179 7320 6265 2061 2064 6573 7469  lways be a desti
-0000e260: 6e61 7469 6f6e 2074 6162 6c65 2066 6f72  nation table for
-0000e270: 2074 6869 7320 7175 6572 7920 7479 7065   this query type
-0000e280: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000e290: 2074 7970 696e 672e 6361 7374 2862 6967   typing.cast(big
-0000e2a0: 7175 6572 792e 5461 626c 6552 6566 6572  query.TableRefer
-0000e2b0: 656e 6365 2c20 6465 7374 696e 6174 696f  ence, destinatio
-0000e2c0: 6e29 0a0a 2020 2020 6465 6620 7265 6d6f  n)..    def remo
-0000e2d0: 7465 5f66 756e 6374 696f 6e28 0a20 2020  te_function(.   
-0000e2e0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000e2f0: 2020 2069 6e70 7574 5f74 7970 6573 3a20     input_types: 
-0000e300: 4c69 7374 5b74 7970 655d 2c0a 2020 2020  List[type],.    
-0000e310: 2020 2020 6f75 7470 7574 5f74 7970 653a      output_type:
-0000e320: 2074 7970 652c 0a20 2020 2020 2020 2064   type,.        d
-0000e330: 6174 6173 6574 3a20 4f70 7469 6f6e 616c  ataset: Optional
-0000e340: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000e350: 2020 2020 2020 6269 6771 7565 7279 5f63        bigquery_c
-0000e360: 6f6e 6e65 6374 696f 6e3a 204f 7074 696f  onnection: Optio
-0000e370: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000e380: 0a20 2020 2020 2020 2072 6575 7365 3a20  .        reuse: 
-0000e390: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-0000e3a0: 2020 2020 206e 616d 653a 204f 7074 696f       name: Optio
-0000e3b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000e3c0: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
-0000e3d0: 733a 204f 7074 696f 6e61 6c5b 5365 7175  s: Optional[Sequ
-0000e3e0: 656e 6365 5b73 7472 5d5d 203d 204e 6f6e  ence[str]] = Non
-0000e3f0: 652c 0a20 2020 2020 2020 2063 6c6f 7564  e,.        cloud
-0000e400: 5f66 756e 6374 696f 6e5f 7365 7276 6963  _function_servic
-0000e410: 655f 6163 636f 756e 743a 204f 7074 696f  e_account: Optio
-0000e420: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000e430: 0a20 2020 2020 2020 2063 6c6f 7564 5f66  .        cloud_f
-0000e440: 756e 6374 696f 6e5f 6b6d 735f 6b65 795f  unction_kms_key_
-0000e450: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
-0000e460: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0000e470: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
-0000e480: 6f6e 5f64 6f63 6b65 725f 7265 706f 7369  on_docker_reposi
-0000e490: 746f 7279 3a20 4f70 7469 6f6e 616c 5b73  tory: Optional[s
-0000e4a0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0000e4b0: 2020 2020 6d61 785f 6261 7463 6869 6e67      max_batching
-0000e4c0: 5f72 6f77 733a 204f 7074 696f 6e61 6c5b  _rows: Optional[
-0000e4d0: 696e 745d 203d 2031 3030 302c 0a20 2020  int] = 1000,.   
-0000e4e0: 2029 3a0a 2020 2020 2020 2020 2222 2244   ):.        """D
-0000e4f0: 6563 6f72 6174 6f72 2074 6f20 7475 726e  ecorator to turn
-0000e500: 2061 2075 7365 7220 6465 6669 6e65 6420   a user defined 
-0000e510: 6675 6e63 7469 6f6e 2069 6e74 6f20 6120  function into a 
-0000e520: 4269 6751 7565 7279 2072 656d 6f74 6520  BigQuery remote 
-0000e530: 6675 6e63 7469 6f6e 2e20 4368 6563 6b20  function. Check 
-0000e540: 6f75 740a 2020 2020 2020 2020 7468 6520  out.        the 
-0000e550: 636f 6465 2073 616d 706c 6573 2061 743a  code samples at:
-0000e560: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
-0000e570: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
-0000e580: 7279 2f64 6f63 732f 7265 6d6f 7465 2d66  ry/docs/remote-f
-0000e590: 756e 6374 696f 6e73 2362 6967 7175 6572  unctions#bigquer
-0000e5a0: 792d 6461 7461 6672 616d 6573 2e0a 0a20  y-dataframes... 
-0000e5b0: 2020 2020 2020 202e 2e20 6e6f 7465 3a3a         .. note::
-0000e5c0: 0a20 2020 2020 2020 2020 2020 2050 6c65  .            Ple
-0000e5d0: 6173 6520 6d61 6b65 2073 7572 6520 666f  ase make sure fo
-0000e5e0: 6c6c 6f77 696e 6720 6973 2073 6574 7570  llowing is setup
-0000e5f0: 2062 6566 6f72 6520 7573 696e 6720 7468   before using th
-0000e600: 6973 2041 5049 3a0a 0a20 2020 2020 2020  is API:..       
-0000e610: 2031 2e20 4861 7665 2074 6865 2062 656c   1. Have the bel
-0000e620: 6f77 2041 5049 7320 656e 6162 6c65 6420  ow APIs enabled 
-0000e630: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
-0000e640: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
-0000e650: 2042 6967 5175 6572 7920 436f 6e6e 6563   BigQuery Connec
-0000e660: 7469 6f6e 2041 5049 0a20 2020 2020 2020  tion API.       
-0000e670: 2020 2020 202a 2043 6c6f 7564 2046 756e       * Cloud Fun
-0000e680: 6374 696f 6e73 2041 5049 0a20 2020 2020  ctions API.     
-0000e690: 2020 2020 2020 202a 2043 6c6f 7564 2052         * Cloud R
-0000e6a0: 756e 2041 5049 0a20 2020 2020 2020 2020  un API.         
-0000e6b0: 2020 202a 2043 6c6f 7564 2042 7569 6c64     * Cloud Build
-0000e6c0: 2041 5049 0a20 2020 2020 2020 2020 2020   API.           
-0000e6d0: 202a 2041 7274 6966 6163 7420 5265 6769   * Artifact Regi
-0000e6e0: 7374 7279 2041 5049 0a20 2020 2020 2020  stry API.       
-0000e6f0: 2020 2020 202a 2043 6c6f 7564 2052 6573       * Cloud Res
-0000e700: 6f75 7263 6520 4d61 6e61 6765 7220 4150  ource Manager AP
-0000e710: 490a 0a20 2020 2020 2020 2020 2020 5468  I..           Th
-0000e720: 6973 2063 616e 2062 6520 646f 6e65 2066  is can be done f
-0000e730: 726f 6d20 7468 6520 636c 6f75 6420 636f  rom the cloud co
-0000e740: 6e73 6f6c 6520 2863 6861 6e67 6520 6050  nsole (change `P
-0000e750: 524f 4a45 4354 5f49 4460 2074 6f20 796f  ROJECT_ID` to yo
-0000e760: 7572 7329 3a0a 2020 2020 2020 2020 2020  urs):.          
-0000e770: 2068 7474 7073 3a2f 2f63 6f6e 736f 6c65   https://console
-0000e780: 2e63 6c6f 7564 2e67 6f6f 676c 652e 636f  .cloud.google.co
-0000e790: 6d2f 6170 6973 2f65 6e61 626c 6566 6c6f  m/apis/enableflo
-0000e7a0: 773f 6170 6969 643d 6269 6771 7565 7279  w?apiid=bigquery
-0000e7b0: 636f 6e6e 6563 7469 6f6e 2e67 6f6f 676c  connection.googl
-0000e7c0: 6561 7069 732e 636f 6d2c 636c 6f75 6466  eapis.com,cloudf
-0000e7d0: 756e 6374 696f 6e73 2e67 6f6f 676c 6561  unctions.googlea
-0000e7e0: 7069 732e 636f 6d2c 7275 6e2e 676f 6f67  pis.com,run.goog
-0000e7f0: 6c65 6170 6973 2e63 6f6d 2c63 6c6f 7564  leapis.com,cloud
-0000e800: 6275 696c 642e 676f 6f67 6c65 6170 6973  build.googleapis
-0000e810: 2e63 6f6d 2c61 7274 6966 6163 7472 6567  .com,artifactreg
-0000e820: 6973 7472 792e 676f 6f67 6c65 6170 6973  istry.googleapis
-0000e830: 2e63 6f6d 2c63 6c6f 7564 7265 736f 7572  .com,cloudresour
-0000e840: 6365 6d61 6e61 6765 722e 676f 6f67 6c65  cemanager.google
-0000e850: 6170 6973 2e63 6f6d 2670 726f 6a65 6374  apis.com&project
-0000e860: 3d50 524f 4a45 4354 5f49 440a 0a20 2020  =PROJECT_ID..   
-0000e870: 2020 2020 2020 2020 4f72 2066 726f 6d20          Or from 
-0000e880: 7468 6520 6763 6c6f 7564 2043 4c49 3a0a  the gcloud CLI:.
-0000e890: 0a20 2020 2020 2020 2020 2020 6024 2067  .           `$ g
-0000e8a0: 636c 6f75 6420 7365 7276 6963 6573 2065  cloud services e
-0000e8b0: 6e61 626c 6520 6269 6771 7565 7279 636f  nable bigqueryco
-0000e8c0: 6e6e 6563 7469 6f6e 2e67 6f6f 676c 6561  nnection.googlea
-0000e8d0: 7069 732e 636f 6d20 636c 6f75 6466 756e  pis.com cloudfun
-0000e8e0: 6374 696f 6e73 2e67 6f6f 676c 6561 7069  ctions.googleapi
-0000e8f0: 732e 636f 6d20 7275 6e2e 676f 6f67 6c65  s.com run.google
-0000e900: 6170 6973 2e63 6f6d 2063 6c6f 7564 6275  apis.com cloudbu
-0000e910: 696c 642e 676f 6f67 6c65 6170 6973 2e63  ild.googleapis.c
-0000e920: 6f6d 2061 7274 6966 6163 7472 6567 6973  om artifactregis
-0000e930: 7472 792e 676f 6f67 6c65 6170 6973 2e63  try.googleapis.c
-0000e940: 6f6d 2063 6c6f 7564 7265 736f 7572 6365  om cloudresource
-0000e950: 6d61 6e61 6765 722e 676f 6f67 6c65 6170  manager.googleap
-0000e960: 6973 2e63 6f6d 600a 0a20 2020 2020 2020  is.com`..       
-0000e970: 2032 2e20 4861 7665 2066 6f6c 6c6f 7769   2. Have followi
-0000e980: 6e67 2049 414d 2072 6f6c 6573 2065 6e61  ng IAM roles ena
-0000e990: 626c 6564 2066 6f72 2079 6f75 3a0a 0a20  bled for you:.. 
-0000e9a0: 2020 2020 2020 2020 2020 202a 2042 6967             * Big
-0000e9b0: 5175 6572 7920 4461 7461 2045 6469 746f  Query Data Edito
-0000e9c0: 7220 2872 6f6c 6573 2f62 6967 7175 6572  r (roles/bigquer
-0000e9d0: 792e 6461 7461 4564 6974 6f72 290a 2020  y.dataEditor).  
-0000e9e0: 2020 2020 2020 2020 2020 2a20 4269 6751            * BigQ
-0000e9f0: 7565 7279 2043 6f6e 6e65 6374 696f 6e20  uery Connection 
-0000ea00: 4164 6d69 6e20 2872 6f6c 6573 2f62 6967  Admin (roles/big
-0000ea10: 7175 6572 792e 636f 6e6e 6563 7469 6f6e  query.connection
-0000ea20: 4164 6d69 6e29 0a20 2020 2020 2020 2020  Admin).         
-0000ea30: 2020 202a 2043 6c6f 7564 2046 756e 6374     * Cloud Funct
-0000ea40: 696f 6e73 2044 6576 656c 6f70 6572 2028  ions Developer (
-0000ea50: 726f 6c65 732f 636c 6f75 6466 756e 6374  roles/cloudfunct
-0000ea60: 696f 6e73 2e64 6576 656c 6f70 6572 290a  ions.developer).
-0000ea70: 2020 2020 2020 2020 2020 2020 2a20 5365              * Se
-0000ea80: 7276 6963 6520 4163 636f 756e 7420 5573  rvice Account Us
-0000ea90: 6572 2028 726f 6c65 732f 6961 6d2e 7365  er (roles/iam.se
-0000eaa0: 7276 6963 6541 6363 6f75 6e74 5573 6572  rviceAccountUser
-0000eab0: 2920 6f6e 2074 6865 2073 6572 7669 6365  ) on the service
-0000eac0: 2061 6363 6f75 6e74 2060 5052 4f4a 4543   account `PROJEC
-0000ead0: 545f 4e55 4d42 4552 2d63 6f6d 7075 7465  T_NUMBER-compute
-0000eae0: 4064 6576 656c 6f70 6572 2e67 7365 7276  @developer.gserv
-0000eaf0: 6963 6561 6363 6f75 6e74 2e63 6f6d 600a  iceaccount.com`.
-0000eb00: 2020 2020 2020 2020 2020 2020 2a20 5374              * St
-0000eb10: 6f72 6167 6520 4f62 6a65 6374 2056 6965  orage Object Vie
-0000eb20: 7765 7220 2872 6f6c 6573 2f73 746f 7261  wer (roles/stora
-0000eb30: 6765 2e6f 626a 6563 7456 6965 7765 7229  ge.objectViewer)
-0000eb40: 0a20 2020 2020 2020 2020 2020 202a 2050  .            * P
-0000eb50: 726f 6a65 6374 2049 414d 2041 646d 696e  roject IAM Admin
-0000eb60: 2028 726f 6c65 732f 7265 736f 7572 6365   (roles/resource
-0000eb70: 6d61 6e61 6765 722e 7072 6f6a 6563 7449  manager.projectI
-0000eb80: 616d 4164 6d69 6e29 2028 4f6e 6c79 2072  amAdmin) (Only r
-0000eb90: 6571 7569 7265 6420 6966 2074 6865 2062  equired if the b
-0000eba0: 6967 7175 6572 7920 636f 6e6e 6563 7469  igquery connecti
-0000ebb0: 6f6e 2062 6569 6e67 2075 7365 6420 6973  on being used is
-0000ebc0: 206e 6f74 2070 7265 2d63 7265 6174 6564   not pre-created
-0000ebd0: 2061 6e64 2069 7320 6372 6561 7465 6420   and is created 
-0000ebe0: 6479 6e61 6d69 6361 6c6c 7920 7769 7468  dynamically with
-0000ebf0: 2075 7365 7220 6372 6564 656e 7469 616c   user credential
-0000ec00: 732e 290a 0a20 2020 2020 2020 2033 2e20  s.)..        3. 
-0000ec10: 4569 7468 6572 2074 6865 2075 7365 7220  Either the user 
-0000ec20: 6861 7320 7365 7449 616d 506f 6c69 6379  has setIamPolicy
-0000ec30: 2070 7269 7669 6c65 6765 206f 6e20 7468   privilege on th
-0000ec40: 6520 7072 6f6a 6563 742c 206f 7220 6120  e project, or a 
-0000ec50: 4269 6751 7565 7279 2063 6f6e 6e65 6374  BigQuery connect
-0000ec60: 696f 6e20 6973 2070 7265 2d63 7265 6174  ion is pre-creat
-0000ec70: 6564 2077 6974 6820 6e65 6365 7373 6172  ed with necessar
-0000ec80: 7920 4941 4d20 726f 6c65 2073 6574 3a0a  y IAM role set:.
-0000ec90: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
-0000eca0: 546f 2063 7265 6174 6520 6120 636f 6e6e  To create a conn
-0000ecb0: 6563 7469 6f6e 2c20 666f 6c6c 6f77 2068  ection, follow h
-0000ecc0: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
-0000ecd0: 676c 652e 636f 6d2f 6269 6771 7565 7279  gle.com/bigquery
-0000ece0: 2f64 6f63 732f 7265 6665 7265 6e63 652f  /docs/reference/
-0000ecf0: 7374 616e 6461 7264 2d73 716c 2f72 656d  standard-sql/rem
-0000ed00: 6f74 652d 6675 6e63 7469 6f6e 7323 6372  ote-functions#cr
-0000ed10: 6561 7465 5f61 5f63 6f6e 6e65 6374 696f  eate_a_connectio
-0000ed20: 6e0a 2020 2020 2020 2020 2020 2020 322e  n.            2.
-0000ed30: 2054 6f20 7365 7420 7570 2049 414d 2c20   To set up IAM, 
-0000ed40: 666f 6c6c 6f77 2068 7474 7073 3a2f 2f63  follow https://c
-0000ed50: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
-0000ed60: 6269 6771 7565 7279 2f64 6f63 732f 7265  bigquery/docs/re
-0000ed70: 6665 7265 6e63 652f 7374 616e 6461 7264  ference/standard
-0000ed80: 2d73 716c 2f72 656d 6f74 652d 6675 6e63  -sql/remote-func
-0000ed90: 7469 6f6e 7323 6772 616e 745f 7065 726d  tions#grant_perm
-0000eda0: 6973 7369 6f6e 5f6f 6e5f 6675 6e63 7469  ission_on_functi
-0000edb0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0000edc0: 2020 2041 6c74 6572 6e61 7469 7665 6c79     Alternatively
-0000edd0: 2c20 7468 6520 4941 4d20 636f 756c 6420  , the IAM could 
-0000ede0: 616c 736f 2062 6520 7365 7475 7020 7669  also be setup vi
-0000edf0: 6120 7468 6520 6763 6c6f 7564 2043 4c49  a the gcloud CLI
-0000ee00: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ee10: 2020 6024 2067 636c 6f75 6420 7072 6f6a    `$ gcloud proj
-0000ee20: 6563 7473 2061 6464 2d69 616d 2d70 6f6c  ects add-iam-pol
-0000ee30: 6963 792d 6269 6e64 696e 6720 5052 4f4a  icy-binding PROJ
-0000ee40: 4543 545f 4944 202d 2d6d 656d 6265 723d  ECT_ID --member=
-0000ee50: 2273 6572 7669 6365 4163 636f 756e 743a  "serviceAccount:
-0000ee60: 434f 4e4e 4543 5449 4f4e 5f53 4552 5649  CONNECTION_SERVI
-0000ee70: 4345 5f41 4343 4f55 4e54 5f49 4422 202d  CE_ACCOUNT_ID" -
-0000ee80: 2d72 6f6c 653d 2272 6f6c 6573 2f72 756e  -role="roles/run
-0000ee90: 2e69 6e76 6f6b 6572 2260 2e0a 0a20 2020  .invoker"`...   
-0000eea0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000eeb0: 2020 2020 2020 2069 6e70 7574 5f74 7970         input_typ
-0000eec0: 6573 2028 6c69 7374 2874 7970 6529 293a  es (list(type)):
-0000eed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eee0: 204c 6973 7420 6f66 2069 6e70 7574 2064   List of input d
-0000eef0: 6174 6120 7479 7065 7320 696e 2074 6865  ata types in the
-0000ef00: 2075 7365 7220 6465 6669 6e65 6420 6675   user defined fu
-0000ef10: 6e63 7469 6f6e 2e0a 2020 2020 2020 2020  nction..        
-0000ef20: 2020 2020 6f75 7470 7574 5f74 7970 6520      output_type 
-0000ef30: 2874 7970 6529 3a0a 2020 2020 2020 2020  (type):.        
-0000ef40: 2020 2020 2020 2020 4461 7461 2074 7970          Data typ
-0000ef50: 6520 6f66 2074 6865 206f 7574 7075 7420  e of the output 
-0000ef60: 696e 2074 6865 2075 7365 7220 6465 6669  in the user defi
-0000ef70: 6e65 6420 6675 6e63 7469 6f6e 2e0a 2020  ned function..  
-0000ef80: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-0000ef90: 7420 2873 7472 2c20 4f70 7469 6f6e 616c  t (str, Optional
-0000efa0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000efb0: 2020 2044 6174 6173 6574 2069 6e20 7768     Dataset in wh
-0000efc0: 6963 6820 746f 2063 7265 6174 6520 6120  ich to create a 
-0000efd0: 4269 6751 7565 7279 2072 656d 6f74 6520  BigQuery remote 
-0000efe0: 6675 6e63 7469 6f6e 2e20 4974 2073 686f  function. It sho
-0000eff0: 756c 6420 6265 2069 6e0a 2020 2020 2020  uld be in.      
-0000f000: 2020 2020 2020 2020 2020 603c 7072 6f6a            `<proj
-0000f010: 6563 745f 6964 3e2e 3c64 6174 6173 6574  ect_id>.<dataset
-0000f020: 5f6e 616d 653e 6020 6f72 2060 3c64 6174  _name>` or `<dat
-0000f030: 6173 6574 5f6e 616d 653e 6020 666f 726d  aset_name>` form
-0000f040: 6174 2e20 4966 2074 6869 730a 2020 2020  at. If this.    
-0000f050: 2020 2020 2020 2020 2020 2020 7061 7261              para
-0000f060: 6d65 7465 7220 6973 206e 6f74 2070 726f  meter is not pro
-0000f070: 7669 6465 6420 7468 656e 2073 6573 7369  vided then sessi
-0000f080: 6f6e 2064 6174 6173 6574 2069 6420 6973  on dataset id is
-0000f090: 2075 7365 642e 0a20 2020 2020 2020 2020   used..         
-0000f0a0: 2020 2062 6967 7175 6572 795f 636f 6e6e     bigquery_conn
-0000f0b0: 6563 7469 6f6e 2028 7374 722c 204f 7074  ection (str, Opt
-0000f0c0: 696f 6e61 6c29 3a0a 2020 2020 2020 2020  ional):.        
-0000f0d0: 2020 2020 2020 2020 4e61 6d65 206f 6620          Name of 
-0000f0e0: 7468 6520 4269 6751 7565 7279 2063 6f6e  the BigQuery con
-0000f0f0: 6e65 6374 696f 6e2e 2059 6f75 2073 686f  nection. You sho
-0000f100: 756c 6420 6569 7468 6572 2068 6176 6520  uld either have 
-0000f110: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-0000f120: 2020 2020 636f 6e6e 6563 7469 6f6e 2061      connection a
-0000f130: 6c72 6561 6479 2063 7265 6174 6564 2069  lready created i
-0000f140: 6e20 7468 6520 606c 6f63 6174 696f 6e60  n the `location`
-0000f150: 2079 6f75 2068 6176 6520 6368 6f73 656e   you have chosen
-0000f160: 2c20 6f72 0a20 2020 2020 2020 2020 2020  , or.           
-0000f170: 2020 2020 2079 6f75 2073 686f 756c 6420       you should 
-0000f180: 6861 7665 2074 6865 2050 726f 6a65 6374  have the Project
-0000f190: 2049 414d 2041 646d 696e 2072 6f6c 6520   IAM Admin role 
-0000f1a0: 746f 2065 6e61 626c 6520 7468 6520 7365  to enable the se
-0000f1b0: 7276 6963 650a 2020 2020 2020 2020 2020  rvice.          
-0000f1c0: 2020 2020 2020 746f 2063 7265 6174 6520        to create 
-0000f1d0: 7468 6520 636f 6e6e 6563 7469 6f6e 2066  the connection f
-0000f1e0: 6f72 2079 6f75 2069 6620 796f 7520 6e65  or you if you ne
-0000f1f0: 6564 2069 742e 2049 6620 7468 6973 2070  ed it. If this p
-0000f200: 6172 616d 6574 6572 2069 730a 2020 2020  arameter is.    
-0000f210: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
-0000f220: 7072 6f76 6964 6564 2074 6865 6e20 7468  provided then th
-0000f230: 6520 4269 6751 7565 7279 2063 6f6e 6e65  e BigQuery conne
-0000f240: 6374 696f 6e20 6672 6f6d 2074 6865 2073  ction from the s
-0000f250: 6573 7369 6f6e 2069 7320 7573 6564 2e0a  ession is used..
-0000f260: 2020 2020 2020 2020 2020 2020 7265 7573              reus
-0000f270: 6520 2862 6f6f 6c2c 204f 7074 696f 6e61  e (bool, Optiona
-0000f280: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
-0000f290: 2020 2020 5265 7573 6520 7468 6520 7265      Reuse the re
-0000f2a0: 6d6f 7465 2066 756e 6374 696f 6e20 6966  mote function if
-0000f2b0: 2061 6c72 6561 6479 2065 7869 7374 732e   already exists.
-0000f2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f2d0: 2060 5472 7565 6020 6279 2064 6566 6175   `True` by defau
-0000f2e0: 6c74 2c20 7768 6963 6820 7769 6c6c 2072  lt, which will r
-0000f2f0: 6573 756c 7420 696e 2072 6575 7369 6e67  esult in reusing
-0000f300: 2061 6e20 6578 6973 7469 6e67 2072 656d   an existing rem
-0000f310: 6f74 650a 2020 2020 2020 2020 2020 2020  ote.            
-0000f320: 2020 2020 6675 6e63 7469 6f6e 2061 6e64      function and
-0000f330: 2063 6f72 7265 7370 6f6e 6469 6e67 2063   corresponding c
-0000f340: 6c6f 7564 2066 756e 6374 696f 6e20 2869  loud function (i
-0000f350: 6620 616e 7929 2074 6861 7420 7761 730a  f any) that was.
-0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f370: 7072 6576 696f 7573 6c79 2063 7265 6174  previously creat
-0000f380: 6564 2066 6f72 2074 6865 2073 616d 6520  ed for the same 
-0000f390: 7564 662e 0a20 2020 2020 2020 2020 2020  udf..           
-0000f3a0: 2020 2020 2053 6574 7469 6e67 2069 7420       Setting it 
-0000f3b0: 746f 2060 4661 6c73 6560 2077 6f75 6c64  to `False` would
-0000f3c0: 2066 6f72 6365 2063 7265 6174 696e 6720   force creating 
-0000f3d0: 6120 756e 6971 7565 2072 656d 6f74 6520  a unique remote 
-0000f3e0: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
-0000f3f0: 2020 2020 2020 2020 2020 4966 2074 6865            If the
-0000f400: 2072 6571 7569 7265 6420 7265 6d6f 7465   required remote
-0000f410: 2066 756e 6374 696f 6e20 646f 6573 206e   function does n
-0000f420: 6f74 2065 7869 7374 2074 6865 6e20 6974  ot exist then it
-0000f430: 2077 6f75 6c64 2062 650a 2020 2020 2020   would be.      
-0000f440: 2020 2020 2020 2020 2020 6372 6561 7465            create
-0000f450: 6420 6972 7265 7370 6563 7469 7665 206f  d irrespective o
-0000f460: 6620 7468 6973 2070 6172 616d 2e0a 2020  f this param..  
-0000f470: 2020 2020 2020 2020 2020 6e61 6d65 2028            name (
-0000f480: 7374 722c 204f 7074 696f 6e61 6c29 3a0a  str, Optional):.
-0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4a0: 4578 706c 6963 6974 206e 616d 6520 6f66  Explicit name of
-0000f4b0: 2074 6865 2070 6572 7369 7374 6564 2042   the persisted B
-0000f4c0: 6967 5175 6572 7920 7265 6d6f 7465 2066  igQuery remote f
-0000f4d0: 756e 6374 696f 6e2e 2055 7365 2069 7420  unction. Use it 
-0000f4e0: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
-0000f4f0: 2020 2020 2063 6175 7469 6f6e 2c20 6265       caution, be
-0000f500: 6361 7573 6520 7477 6f20 7573 6572 7320  cause two users 
-0000f510: 776f 726b 696e 6720 696e 2074 6865 2073  working in the s
-0000f520: 616d 6520 7072 6f6a 6563 7420 616e 6420  ame project and 
-0000f530: 6461 7461 7365 740a 2020 2020 2020 2020  dataset.        
-0000f540: 2020 2020 2020 2020 636f 756c 6420 6f76          could ov
-0000f550: 6572 7772 6974 6520 6561 6368 206f 7468  erwrite each oth
-0000f560: 6572 2773 2072 656d 6f74 6520 6675 6e63  er's remote func
-0000f570: 7469 6f6e 7320 6966 2074 6865 7920 7573  tions if they us
-0000f580: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
-0000f590: 2020 2020 2020 2020 2020 2070 6572 7369             persi
-0000f5a0: 7374 656e 7420 6e61 6d65 2e0a 2020 2020  stent name..    
-0000f5b0: 2020 2020 2020 2020 7061 636b 6167 6573          packages
-0000f5c0: 2028 7374 725b 5d2c 204f 7074 696f 6e61   (str[], Optiona
-0000f5d0: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
-0000f5e0: 2020 2020 4578 706c 6963 6974 206e 616d      Explicit nam
-0000f5f0: 6520 6f66 2074 6865 2065 7874 6572 6e61  e of the externa
-0000f600: 6c20 7061 636b 6167 6520 6465 7065 6e64  l package depend
-0000f610: 656e 6369 6573 2e20 4561 6368 2064 6570  encies. Each dep
-0000f620: 656e 6465 6e63 790a 2020 2020 2020 2020  endency.        
-0000f630: 2020 2020 2020 2020 6973 2061 6464 6564          is added
-0000f640: 2074 6f20 7468 6520 6072 6571 7569 7265   to the `require
-0000f650: 6d65 6e74 732e 7478 7460 2061 7320 6973  ments.txt` as is
-0000f660: 2c20 616e 6420 6361 6e20 6265 206f 6620  , and can be of 
-0000f670: 7468 6520 666f 726d 0a20 2020 2020 2020  the form.       
-0000f680: 2020 2020 2020 2020 2073 7570 706f 7274           support
-0000f690: 6564 2069 6e20 6874 7470 733a 2f2f 7069  ed in https://pi
-0000f6a0: 702e 7079 7061 2e69 6f2f 656e 2f73 7461  p.pypa.io/en/sta
-0000f6b0: 626c 652f 7265 6665 7265 6e63 652f 7265  ble/reference/re
-0000f6c0: 7175 6972 656d 656e 7473 2d66 696c 652d  quirements-file-
-0000f6d0: 666f 726d 6174 2f2e 0a20 2020 2020 2020  format/..       
-0000f6e0: 2020 2020 2063 6c6f 7564 5f66 756e 6374       cloud_funct
-0000f6f0: 696f 6e5f 7365 7276 6963 655f 6163 636f  ion_service_acco
-0000f700: 756e 7420 2873 7472 2c20 4f70 7469 6f6e  unt (str, Option
-0000f710: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
-0000f720: 2020 2020 2053 6572 7669 6365 2061 6363       Service acc
-0000f730: 6f75 6e74 2074 6f20 7573 6520 666f 7220  ount to use for 
-0000f740: 7468 6520 636c 6f75 6420 6675 6e63 7469  the cloud functi
-0000f750: 6f6e 732e 2049 6620 6e6f 7420 7072 6f76  ons. If not prov
-0000f760: 6964 6564 0a20 2020 2020 2020 2020 2020  ided.           
-0000f770: 2020 2020 2074 6865 6e20 7468 6520 6465       then the de
-0000f780: 6661 756c 7420 7365 7276 6963 6520 6163  fault service ac
-0000f790: 636f 756e 7420 776f 756c 6420 6265 2075  count would be u
-0000f7a0: 7365 642e 2053 6565 0a20 2020 2020 2020  sed. See.       
-0000f7b0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-0000f7c0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-0000f7d0: 6d2f 6675 6e63 7469 6f6e 732f 646f 6373  m/functions/docs
-0000f7e0: 2f73 6563 7572 696e 672f 6675 6e63 7469  /securing/functi
-0000f7f0: 6f6e 2d69 6465 6e74 6974 790a 2020 2020  on-identity.    
-0000f800: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000f810: 6d6f 7265 2064 6574 6169 6c73 2e20 506c  more details. Pl
-0000f820: 6561 7365 206d 616b 6520 7375 7265 2074  ease make sure t
-0000f830: 6865 2073 6572 7669 6365 2061 6363 6f75  he service accou
-0000f840: 6e74 2068 6173 2074 6865 0a20 2020 2020  nt has the.     
-0000f850: 2020 2020 2020 2020 2020 206e 6563 6573             neces
-0000f860: 7361 7279 2049 414d 2070 6572 6d69 7373  sary IAM permiss
-0000f870: 696f 6e73 2063 6f6e 6669 6775 7265 6420  ions configured 
-0000f880: 6173 2064 6573 6372 6962 6564 2069 6e0a  as described in.
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8a0: 6874 7470 733a 2f2f 636c 6f75 642e 676f  https://cloud.go
-0000f8b0: 6f67 6c65 2e63 6f6d 2f66 756e 6374 696f  ogle.com/functio
-0000f8c0: 6e73 2f64 6f63 732f 7265 6665 7265 6e63  ns/docs/referenc
-0000f8d0: 652f 6961 6d2f 726f 6c65 7323 6164 6469  e/iam/roles#addi
-0000f8e0: 7469 6f6e 616c 2d63 6f6e 6669 6775 7261  tional-configura
-0000f8f0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-0000f900: 2020 636c 6f75 645f 6675 6e63 7469 6f6e    cloud_function
-0000f910: 5f6b 6d73 5f6b 6579 5f6e 616d 6520 2873  _kms_key_name (s
-0000f920: 7472 2c20 4f70 7469 6f6e 616c 293a 0a20  tr, Optional):. 
-0000f930: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-0000f940: 7573 746f 6d65 7220 6d61 6e61 6765 6420  ustomer managed 
-0000f950: 656e 6372 7970 7469 6f6e 206b 6579 2074  encryption key t
-0000f960: 6f20 7072 6f74 6563 7420 636c 6f75 6420  o protect cloud 
-0000f970: 6675 6e63 7469 6f6e 7320 616e 640a 2020  functions and.  
-0000f980: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000f990: 6c61 7465 6420 6461 7461 2061 7420 7265  lated data at re
-0000f9a0: 7374 2e20 5468 6973 2069 7320 6f66 2074  st. This is of t
-0000f9b0: 6865 2066 6f72 6d61 740a 2020 2020 2020  he format.      
-0000f9c0: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
-0000f9d0: 7473 2f50 524f 4a45 4354 5f49 442f 6c6f  ts/PROJECT_ID/lo
-0000f9e0: 6361 7469 6f6e 732f 4c4f 4341 5449 4f4e  cations/LOCATION
-0000f9f0: 2f6b 6579 5269 6e67 732f 4b45 5952 494e  /keyRings/KEYRIN
-0000fa00: 472f 6372 7970 746f 4b65 7973 2f4b 4559  G/cryptoKeys/KEY
-0000fa10: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fa20: 2020 5265 6164 2068 7474 7073 3a2f 2f63    Read https://c
-0000fa30: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
-0000fa40: 6675 6e63 7469 6f6e 732f 646f 6373 2f73  functions/docs/s
-0000fa50: 6563 7572 696e 672f 636d 656b 2066 6f72  ecuring/cmek for
-0000fa60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa70: 206d 6f72 6520 6465 7461 696c 7320 696e   more details in
-0000fa80: 636c 7564 696e 6720 6772 616e 7469 6e67  cluding granting
-0000fa90: 206e 6563 6573 7361 7279 2073 6572 7669   necessary servi
-0000faa0: 6365 2061 6363 6f75 6e74 730a 2020 2020  ce accounts.    
-0000fab0: 2020 2020 2020 2020 2020 2020 6163 6365              acce
-0000fac0: 7373 2074 6f20 7468 6520 6b65 792e 0a20  ss to the key.. 
-0000fad0: 2020 2020 2020 2020 2020 2063 6c6f 7564             cloud
-0000fae0: 5f66 756e 6374 696f 6e5f 646f 636b 6572  _function_docker
-0000faf0: 5f72 6570 6f73 6974 6f72 7920 2873 7472  _repository (str
-0000fb00: 2c20 4f70 7469 6f6e 616c 293a 0a20 2020  , Optional):.   
-0000fb10: 2020 2020 2020 2020 2020 2020 2044 6f63               Doc
-0000fb20: 6b65 7220 7265 706f 7369 746f 7279 2063  ker repository c
-0000fb30: 7265 6174 6564 2077 6974 6820 7468 6520  reated with the 
-0000fb40: 7361 6d65 2065 6e63 7279 7074 696f 6e20  same encryption 
-0000fb50: 6b65 7920 6173 0a20 2020 2020 2020 2020  key as.         
-0000fb60: 2020 2020 2020 2060 636c 6f75 645f 6675         `cloud_fu
-0000fb70: 6e63 7469 6f6e 5f6b 6d73 5f6b 6579 5f6e  nction_kms_key_n
-0000fb80: 616d 6560 2074 6f20 7374 6f72 6520 656e  ame` to store en
-0000fb90: 6372 7970 7465 6420 6172 7469 6661 6374  crypted artifact
-0000fba0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000fbb0: 2020 6372 6561 7465 6420 746f 2073 7570    created to sup
-0000fbc0: 706f 7274 2074 6865 2063 6c6f 7564 2066  port the cloud f
-0000fbd0: 756e 6374 696f 6e2e 2054 6869 7320 6973  unction. This is
-0000fbe0: 206f 6620 7468 6520 666f 726d 6174 0a20   of the format. 
-0000fbf0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000fc00: 726f 6a65 6374 732f 5052 4f4a 4543 545f  rojects/PROJECT_
-0000fc10: 4944 2f6c 6f63 6174 696f 6e73 2f4c 4f43  ID/locations/LOC
-0000fc20: 4154 494f 4e2f 7265 706f 7369 746f 7269  ATION/repositori
-0000fc30: 6573 2f52 4550 4f53 4954 4f52 595f 4e41  es/REPOSITORY_NA
-0000fc40: 4d45 2e0a 2020 2020 2020 2020 2020 2020  ME..            
-0000fc50: 2020 2020 466f 7220 6d6f 7265 2064 6574      For more det
-0000fc60: 6169 6c73 2073 6565 0a20 2020 2020 2020  ails see.       
-0000fc70: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-0000fc80: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-0000fc90: 6d2f 6675 6e63 7469 6f6e 732f 646f 6373  m/functions/docs
-0000fca0: 2f73 6563 7572 696e 672f 636d 656b 2362  /securing/cmek#b
-0000fcb0: 6566 6f72 655f 796f 755f 6265 6769 6e2e  efore_you_begin.
-0000fcc0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000fcd0: 5f62 6174 6368 696e 675f 726f 7773 2028  _batching_rows (
-0000fce0: 696e 742c 204f 7074 696f 6e61 6c29 3a0a  int, Optional):.
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd00: 5468 6520 6d61 7869 6d75 6d20 6e75 6d62  The maximum numb
-0000fd10: 6572 206f 6620 726f 7773 2074 6f20 6265  er of rows to be
-0000fd20: 2062 6174 6368 6564 2066 6f72 2070 726f   batched for pro
-0000fd30: 6365 7373 696e 6720 696e 2074 6865 0a20  cessing in the. 
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2042                 B
-0000fd50: 5120 7265 6d6f 7465 2066 756e 6374 696f  Q remote functio
-0000fd60: 6e2e 2044 6566 6175 6c74 2076 616c 7565  n. Default value
-0000fd70: 2069 7320 3130 3030 2e20 4120 6c6f 7765   is 1000. A lowe
-0000fd80: 7220 6e75 6d62 6572 2063 616e 2062 650a  r number can be.
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 7061 7373 6564 2074 6f20 6176 6f69 6420  passed to avoid 
-0000fdb0: 7469 6d65 6f75 7473 2069 6e20 6361 7365  timeouts in case
-0000fdc0: 2074 6865 2075 7365 7220 636f 6465 2069   the user code i
-0000fdd0: 7320 746f 6f20 636f 6d70 6c65 7820 746f  s too complex to
-0000fde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fdf0: 2070 726f 6365 7373 206c 6172 6765 206e   process large n
-0000fe00: 756d 6265 7220 6f66 2072 6f77 7320 6661  umber of rows fa
-0000fe10: 7374 2065 6e6f 7567 682e 2041 2068 6967  st enough. A hig
-0000fe20: 6865 7220 6e75 6d62 6572 2063 616e 2062  her number can b
-0000fe30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000fe40: 2020 7573 6564 2074 6f20 696e 6372 6561    used to increa
-0000fe50: 7365 2074 6872 6f75 6768 7075 7420 696e  se throughput in
-0000fe60: 2063 6173 6520 7468 6520 7573 6572 2063   case the user c
-0000fe70: 6f64 6520 6973 2066 6173 7420 656e 6f75  ode is fast enou
-0000fe80: 6768 2e0a 2020 2020 2020 2020 2020 2020  gh..            
-0000fe90: 2020 2020 604e 6f6e 6560 2063 616e 2062      `None` can b
-0000fea0: 6520 7061 7373 6564 2074 6f20 6c65 7420  e passed to let 
-0000feb0: 4251 2072 656d 6f74 6520 6675 6e63 7469  BQ remote functi
-0000fec0: 6f6e 7320 7365 7276 6963 6520 6170 706c  ons service appl
-0000fed0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0000fee0: 2020 6465 6661 756c 7420 6261 7463 6869    default batchi
-0000fef0: 6e67 2e20 5365 6520 666f 7220 6d6f 7265  ng. See for more
-0000ff00: 2064 6574 6169 6c73 0a20 2020 2020 2020   details.       
-0000ff10: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-0000ff20: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-0000ff30: 6d2f 6269 6771 7565 7279 2f64 6f63 732f  m/bigquery/docs/
-0000ff40: 7265 6d6f 7465 2d66 756e 6374 696f 6e73  remote-functions
-0000ff50: 236c 696d 6974 696e 675f 6e75 6d62 6572  #limiting_number
-0000ff60: 5f6f 665f 726f 7773 5f69 6e5f 615f 6261  _of_rows_in_a_ba
-0000ff70: 7463 685f 7265 7175 6573 742e 0a20 2020  tch_request..   
-0000ff80: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000ff90: 2020 2020 2020 2020 2020 6361 6c6c 6162            callab
-0000ffa0: 6c65 3a20 4120 7265 6d6f 7465 2066 756e  le: A remote fun
-0000ffb0: 6374 696f 6e20 6f62 6a65 6374 2070 6f69  ction object poi
-0000ffc0: 6e74 696e 6720 746f 2074 6865 2063 6c6f  nting to the clo
-0000ffd0: 7564 2061 7373 6574 7320 6372 6561 7465  ud assets create
-0000ffe0: 640a 2020 2020 2020 2020 2020 2020 696e  d.            in
-0000fff0: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-00010000: 746f 2073 7570 706f 7274 2074 6865 2072  to support the r
-00010010: 656d 6f74 6520 6578 6563 7574 696f 6e2e  emote execution.
-00010020: 2054 6865 2063 6c6f 7564 2061 7373 6574   The cloud asset
-00010030: 7320 6361 6e20 6265 0a20 2020 2020 2020  s can be.       
-00010040: 2020 2020 206c 6f63 6174 6564 2074 6872       located thr
-00010050: 6f75 6768 2074 6865 2066 6f6c 6c6f 7769  ough the followi
-00010060: 6e67 2070 726f 7065 7274 6965 7320 7365  ng properties se
-00010070: 7420 696e 2074 6865 206f 626a 6563 743a  t in the object:
-00010080: 0a0a 2020 2020 2020 2020 2020 2020 6062  ..            `b
-00010090: 6967 6672 616d 6573 5f63 6c6f 7564 5f66  igframes_cloud_f
-000100a0: 756e 6374 696f 6e60 202d 2054 6865 2067  unction` - The g
-000100b0: 6f6f 676c 6520 636c 6f75 6420 6675 6e63  oogle cloud func
-000100c0: 7469 6f6e 2064 6570 6c6f 7965 6420 666f  tion deployed fo
-000100d0: 7220 7468 6520 7573 6572 2064 6566 696e  r the user defin
-000100e0: 6564 2063 6f64 652e 0a0a 2020 2020 2020  ed code...      
-000100f0: 2020 2020 2020 6062 6967 6672 616d 6573        `bigframes
-00010100: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
-00010110: 6020 2d20 5468 6520 6269 6771 7565 7279  ` - The bigquery
-00010120: 2072 656d 6f74 6520 6675 6e63 7469 6f6e   remote function
-00010130: 2063 6170 6162 6c65 206f 6620 6361 6c6c   capable of call
-00010140: 696e 6720 696e 746f 2060 6269 6766 7261  ing into `bigfra
-00010150: 6d65 735f 636c 6f75 645f 6675 6e63 7469  mes_cloud_functi
-00010160: 6f6e 602e 0a20 2020 2020 2020 2022 2222  on`..        """
-00010170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010180: 6269 6766 7261 6d65 735f 7266 280a 2020  bigframes_rf(.  
-00010190: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-000101a0: 7479 7065 732c 0a20 2020 2020 2020 2020  types,.         
-000101b0: 2020 206f 7574 7075 745f 7479 7065 2c0a     output_type,.
-000101c0: 2020 2020 2020 2020 2020 2020 7365 7373              sess
-000101d0: 696f 6e3d 7365 6c66 2c0a 2020 2020 2020  ion=self,.      
-000101e0: 2020 2020 2020 6461 7461 7365 743d 6461        dataset=da
-000101f0: 7461 7365 742c 0a20 2020 2020 2020 2020  taset,.         
-00010200: 2020 2062 6967 7175 6572 795f 636f 6e6e     bigquery_conn
-00010210: 6563 7469 6f6e 3d62 6967 7175 6572 795f  ection=bigquery_
-00010220: 636f 6e6e 6563 7469 6f6e 2c0a 2020 2020  connection,.    
-00010230: 2020 2020 2020 2020 7265 7573 653d 7265          reuse=re
-00010240: 7573 652c 0a20 2020 2020 2020 2020 2020  use,.           
-00010250: 206e 616d 653d 6e61 6d65 2c0a 2020 2020   name=name,.    
-00010260: 2020 2020 2020 2020 7061 636b 6167 6573          packages
-00010270: 3d70 6163 6b61 6765 732c 0a20 2020 2020  =packages,.     
-00010280: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
-00010290: 6374 696f 6e5f 7365 7276 6963 655f 6163  ction_service_ac
-000102a0: 636f 756e 743d 636c 6f75 645f 6675 6e63  count=cloud_func
-000102b0: 7469 6f6e 5f73 6572 7669 6365 5f61 6363  tion_service_acc
-000102c0: 6f75 6e74 2c0a 2020 2020 2020 2020 2020  ount,.          
-000102d0: 2020 636c 6f75 645f 6675 6e63 7469 6f6e    cloud_function
-000102e0: 5f6b 6d73 5f6b 6579 5f6e 616d 653d 636c  _kms_key_name=cl
-000102f0: 6f75 645f 6675 6e63 7469 6f6e 5f6b 6d73  oud_function_kms
-00010300: 5f6b 6579 5f6e 616d 652c 0a20 2020 2020  _key_name,.     
-00010310: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
-00010320: 6374 696f 6e5f 646f 636b 6572 5f72 6570  ction_docker_rep
-00010330: 6f73 6974 6f72 793d 636c 6f75 645f 6675  ository=cloud_fu
-00010340: 6e63 7469 6f6e 5f64 6f63 6b65 725f 7265  nction_docker_re
-00010350: 706f 7369 746f 7279 2c0a 2020 2020 2020  pository,.      
-00010360: 2020 2020 2020 6d61 785f 6261 7463 6869        max_batchi
-00010370: 6e67 5f72 6f77 733d 6d61 785f 6261 7463  ng_rows=max_batc
-00010380: 6869 6e67 5f72 6f77 732c 0a20 2020 2020  hing_rows,.     
-00010390: 2020 2029 0a0a 2020 2020 6465 6620 7265     )..    def re
-000103a0: 6164 5f67 6271 5f66 756e 6374 696f 6e28  ad_gbq_function(
-000103b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000103c0: 2020 2020 2020 2066 756e 6374 696f 6e5f         function_
-000103d0: 6e61 6d65 3a20 7374 722c 0a20 2020 2029  name: str,.    )
-000103e0: 3a0a 2020 2020 2020 2020 2222 224c 6f61  :.        """Loa
-000103f0: 6473 2061 2042 6967 5175 6572 7920 6675  ds a BigQuery fu
-00010400: 6e63 7469 6f6e 2066 726f 6d20 4269 6751  nction from BigQ
-00010410: 7565 7279 2e0a 0a20 2020 2020 2020 2054  uery...        T
-00010420: 6865 6e20 6974 2063 616e 2062 6520 6170  hen it can be ap
-00010430: 706c 6965 6420 746f 2061 2044 6174 6146  plied to a DataF
-00010440: 7261 6d65 206f 7220 5365 7269 6573 2e0a  rame or Series..
-00010450: 0a20 2020 2020 2020 202e 2e20 6e6f 7465  .        .. note
-00010460: 3a3a 0a20 2020 2020 2020 2020 2020 2054  ::.            T
-00010470: 6865 2072 6574 7572 6e20 7479 7065 206f  he return type o
-00010480: 6620 7468 6520 6675 6e63 7469 6f6e 206d  f the function m
-00010490: 7573 7420 6265 2065 7870 6c69 6369 746c  ust be explicitl
-000104a0: 7920 7370 6563 6966 6965 6420 696e 2074  y specified in t
-000104b0: 6865 0a20 2020 2020 2020 2020 2020 2066  he.            f
-000104c0: 756e 6374 696f 6e27 7320 6f72 6967 696e  unction's origin
-000104d0: 616c 2064 6566 696e 6974 696f 6e20 6576  al definition ev
-000104e0: 656e 2069 6620 6e6f 7420 6f74 6865 7277  en if not otherw
-000104f0: 6973 6520 7265 7175 6972 6564 2e0a 0a20  ise required... 
-00010500: 2020 2020 2020 2042 6967 5175 6572 7920         BigQuery 
-00010510: 5574 696c 7320 7072 6f76 6964 6573 206d  Utils provides m
-00010520: 616e 7920 7075 626c 6963 2066 756e 6374  any public funct
-00010530: 696f 6e73 2075 6e64 6572 2074 6865 2060  ions under the `
-00010540: 6062 7175 7469 6c60 6020 7072 6f6a 6563  `bqutil`` projec
-00010550: 7420 6f6e 2047 6f6f 676c 6520 436c 6f75  t on Google Clou
-00010560: 6420 506c 6174 666f 726d 2070 726f 6a65  d Platform proje
-00010570: 6374 0a20 2020 2020 2020 2028 5365 653a  ct.        (See:
-00010580: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00010590: 636f 6d2f 476f 6f67 6c65 436c 6f75 6450  com/GoogleCloudP
-000105a0: 6c61 7466 6f72 6d2f 6269 6771 7565 7279  latform/bigquery
-000105b0: 2d75 7469 6c73 2f74 7265 652f 6d61 7374  -utils/tree/mast
-000105c0: 6572 2f75 6466 7323 7573 696e 672d 7468  er/udfs#using-th
-000105d0: 652d 7564 6673 292e 0a20 2020 2020 2020  e-udfs)..       
-000105e0: 2059 6f75 2063 616e 2063 6865 636b 6f75   You can checkou
-000105f0: 7420 436f 6d6d 756e 6974 7920 5544 4673  t Community UDFs
-00010600: 2074 6f20 7573 6520 636f 6d6d 756e 6974   to use communit
-00010610: 792d 636f 6e74 7269 6275 7465 6420 6675  y-contributed fu
-00010620: 6e63 7469 6f6e 732e 0a20 2020 2020 2020  nctions..       
-00010630: 2028 5365 653a 2068 7474 7073 3a2f 2f67   (See: https://g
-00010640: 6974 6875 622e 636f 6d2f 476f 6f67 6c65  ithub.com/Google
-00010650: 436c 6f75 6450 6c61 7466 6f72 6d2f 6269  CloudPlatform/bi
-00010660: 6771 7565 7279 2d75 7469 6c73 2f74 7265  gquery-utils/tre
-00010670: 652f 6d61 7374 6572 2f75 6466 732f 636f  e/master/udfs/co
-00010680: 6d6d 756e 6974 7923 636f 6d6d 756e 6974  mmunity#communit
-00010690: 792d 7564 6673 292e 0a0a 2020 2020 2020  y-udfs)...      
-000106a0: 2020 2a2a 4578 616d 706c 6573 3a2a 2a0a    **Examples:**.
-000106b0: 0a20 2020 2020 2020 2055 7365 2074 6865  .        Use the
-000106c0: 2060 6063 775f 6c6f 7765 725f 6361 7365   ``cw_lower_case
-000106d0: 5f61 7363 6969 5f6f 6e6c 7960 6020 6675  _ascii_only`` fu
-000106e0: 6e63 7469 6f6e 2066 726f 6d20 436f 6d6d  nction from Comm
-000106f0: 756e 6974 7920 5544 4673 2e0a 2020 2020  unity UDFs..    
-00010700: 2020 2020 2868 7474 7073 3a2f 2f67 6974      (https://git
-00010710: 6875 622e 636f 6d2f 476f 6f67 6c65 436c  hub.com/GoogleCl
-00010720: 6f75 6450 6c61 7466 6f72 6d2f 6269 6771  oudPlatform/bigq
-00010730: 7565 7279 2d75 7469 6c73 2f62 6c6f 622f  uery-utils/blob/
-00010740: 6d61 7374 6572 2f75 6466 732f 636f 6d6d  master/udfs/comm
-00010750: 756e 6974 792f 6377 5f6c 6f77 6572 5f63  unity/cw_lower_c
-00010760: 6173 655f 6173 6369 695f 6f6e 6c79 2e73  ase_ascii_only.s
-00010770: 716c 7829 0a0a 2020 2020 2020 2020 2020  qlx)..          
-00010780: 2020 3e3e 3e20 696d 706f 7274 2062 6967    >>> import big
-00010790: 6672 616d 6573 2e70 616e 6461 7320 6173  frames.pandas as
-000107a0: 2062 7064 0a20 2020 2020 2020 2020 2020   bpd.           
-000107b0: 203e 3e3e 2062 7064 2e6f 7074 696f 6e73   >>> bpd.options
-000107c0: 2e64 6973 706c 6179 2e70 726f 6772 6573  .display.progres
-000107d0: 735f 6261 7220 3d20 4e6f 6e65 0a0a 2020  s_bar = None..  
-000107e0: 2020 2020 2020 2020 2020 3e3e 3e20 6466            >>> df
-000107f0: 203d 2062 7064 2e44 6174 6146 7261 6d65   = bpd.DataFrame
-00010800: 287b 2769 6427 3a20 5b31 2c20 322c 2033  ({'id': [1, 2, 3
-00010810: 5d2c 2027 6e61 6d65 273a 205b 2741 5552  ], 'name': ['AUR
-00010820: c389 4c49 4527 2c20 2743 c389 4c45 5354  ..LIE', 'C..LEST
-00010830: 494e 4527 2c20 2744 4150 484e c389 275d  INE', 'DAPHN..']
-00010840: 7d29 0a20 2020 2020 2020 2020 2020 203e  }).            >
-00010850: 3e3e 2064 660a 2020 2020 2020 2020 2020  >> df.          
-00010860: 2020 2020 2069 6420 2020 2020 2020 6e61       id       na
-00010870: 6d65 0a20 2020 2020 2020 2020 2020 2030  me.            0
-00010880: 2020 2031 2020 2020 4155 52c3 894c 4945     1    AUR..LIE
-00010890: 0a20 2020 2020 2020 2020 2020 2031 2020  .            1  
-000108a0: 2032 2020 43c3 894c 4553 5449 4e45 0a20   2  C..LESTINE. 
-000108b0: 2020 2020 2020 2020 2020 2032 2020 2033             2   3
-000108c0: 2020 2020 2044 4150 484e c389 0a20 2020       DAPHN...   
-000108d0: 2020 2020 2020 2020 203c 424c 414e 4b4c           <BLANKL
-000108e0: 494e 453e 0a20 2020 2020 2020 2020 2020  INE>.           
-000108f0: 205b 3320 726f 7773 2078 2032 2063 6f6c   [3 rows x 2 col
-00010900: 756d 6e73 5d0a 0a20 2020 2020 2020 2020  umns]..         
-00010910: 2020 203e 3e3e 2066 756e 6320 3d20 6270     >>> func = bp
-00010920: 642e 7265 6164 5f67 6271 5f66 756e 6374  d.read_gbq_funct
-00010930: 696f 6e28 2262 7175 7469 6c2e 666e 2e63  ion("bqutil.fn.c
-00010940: 775f 6c6f 7765 725f 6361 7365 5f61 7363  w_lower_case_asc
-00010950: 6969 5f6f 6e6c 7922 290a 2020 2020 2020  ii_only").      
-00010960: 2020 2020 2020 3e3e 3e20 6466 3120 3d20        >>> df1 = 
-00010970: 6466 2e61 7373 6967 6e28 6e65 775f 6e61  df.assign(new_na
-00010980: 6d65 3d64 665b 276e 616d 6527 5d2e 6170  me=df['name'].ap
-00010990: 706c 7928 6675 6e63 2929 0a20 2020 2020  ply(func)).     
-000109a0: 2020 2020 2020 203e 3e3e 2064 6631 0a20         >>> df1. 
-000109b0: 2020 2020 2020 2020 2020 2020 2020 6964                id
-000109c0: 2020 2020 2020 206e 616d 6520 2020 6e65         name   ne
-000109d0: 775f 6e61 6d65 0a20 2020 2020 2020 2020  w_name.         
-000109e0: 2020 2030 2020 2031 2020 2020 4155 52c3     0   1    AUR.
-000109f0: 894c 4945 2020 2020 6175 72c3 896c 6965  .LIE    aur..lie
-00010a00: 0a20 2020 2020 2020 2020 2020 2031 2020  .            1  
-00010a10: 2032 2020 43c3 894c 4553 5449 4e45 2020   2  C..LESTINE  
-00010a20: 63c3 896c 6573 7469 6e65 0a20 2020 2020  c..lestine.     
-00010a30: 2020 2020 2020 2032 2020 2033 2020 2020         2   3    
-00010a40: 2044 4150 484e c389 2020 2020 2064 6170   DAPHN..     dap
-00010a50: 686e c389 0a20 2020 2020 2020 2020 2020  hn...           
-00010a60: 203c 424c 414e 4b4c 494e 453e 0a20 2020   <BLANKLINE>.   
-00010a70: 2020 2020 2020 2020 205b 3320 726f 7773           [3 rows
-00010a80: 2078 2033 2063 6f6c 756d 6e73 5d0a 0a20   x 3 columns].. 
-00010a90: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00010aa0: 2020 2020 2020 2020 2066 756e 6374 696f           functio
-00010ab0: 6e5f 6e61 6d65 2028 7374 7229 3a0a 2020  n_name (str):.  
-00010ac0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00010ad0: 6520 6675 6e63 7469 6f6e 2773 206e 616d  e function's nam
-00010ae0: 6520 696e 2042 6967 5175 6572 7920 696e  e in BigQuery in
-00010af0: 2074 6865 2066 6f72 6d61 740a 2020 2020   the format.    
-00010b00: 2020 2020 2020 2020 2020 2020 6070 726f              `pro
-00010b10: 6a65 6374 5f69 642e 6461 7461 7365 745f  ject_id.dataset_
-00010b20: 6964 2e66 756e 6374 696f 6e5f 6e61 6d65  id.function_name
-00010b30: 602c 206f 720a 2020 2020 2020 2020 2020  `, or.          
-00010b40: 2020 2020 2020 6064 6174 6173 6574 5f69        `dataset_i
-00010b50: 642e 6675 6e63 7469 6f6e 5f6e 616d 6560  d.function_name`
-00010b60: 2074 6f20 6c6f 6164 2066 726f 6d20 7468   to load from th
-00010b70: 6520 6465 6661 756c 7420 7072 6f6a 6563  e default projec
-00010b80: 742c 206f 720a 2020 2020 2020 2020 2020  t, or.          
-00010b90: 2020 2020 2020 6066 756e 6374 696f 6e5f        `function_
-00010ba0: 6e61 6d65 6020 746f 206c 6f61 6420 6672  name` to load fr
-00010bb0: 6f6d 2074 6865 2064 6566 6175 6c74 2070  om the default p
-00010bc0: 726f 6a65 6374 2061 6e64 2074 6865 2064  roject and the d
-00010bd0: 6174 6173 6574 0a20 2020 2020 2020 2020  ataset.         
-00010be0: 2020 2020 2020 2061 7373 6f63 6961 7465         associate
-00010bf0: 6420 7769 7468 2074 6865 2063 7572 7265  d with the curre
-00010c00: 6e74 2073 6573 7369 6f6e 2e0a 0a20 2020  nt session...   
-00010c10: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00010c20: 2020 2020 2020 2020 2020 6361 6c6c 6162            callab
-00010c30: 6c65 3a20 4120 6675 6e63 7469 6f6e 206f  le: A function o
-00010c40: 626a 6563 7420 706f 696e 7469 6e67 2074  bject pointing t
-00010c50: 6f20 7468 6520 4269 6751 7565 7279 2066  o the BigQuery f
-00010c60: 756e 6374 696f 6e20 7265 6164 0a20 2020  unction read.   
-00010c70: 2020 2020 2020 2020 2066 726f 6d20 4269           from Bi
-00010c80: 6751 7565 7279 2e0a 0a20 2020 2020 2020  gQuery...       
-00010c90: 2020 2020 2054 6865 206f 626a 6563 7420       The object 
-00010ca0: 6973 2073 696d 696c 6172 2074 6f20 7468  is similar to th
-00010cb0: 6520 6f6e 6520 6372 6561 7465 6420 6279  e one created by
-00010cc0: 2074 6865 2060 7265 6d6f 7465 5f66 756e   the `remote_fun
-00010cd0: 6374 696f 6e60 0a20 2020 2020 2020 2020  ction`.         
-00010ce0: 2020 2064 6563 6f72 6174 6f72 2c20 696e     decorator, in
-00010cf0: 636c 7564 696e 6720 7468 6520 6062 6967  cluding the `big
-00010d00: 6672 616d 6573 5f72 656d 6f74 655f 6675  frames_remote_fu
-00010d10: 6e63 7469 6f6e 6020 7072 6f70 6572 7479  nction` property
-00010d20: 2c20 6275 740a 2020 2020 2020 2020 2020  , but.          
-00010d30: 2020 6e6f 7420 696e 636c 7564 696e 6720    not including 
-00010d40: 7468 6520 6062 6967 6672 616d 6573 5f63  the `bigframes_c
-00010d50: 6c6f 7564 5f66 756e 6374 696f 6e60 2070  loud_function` p
-00010d60: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
-00010d70: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
-00010d80: 7475 726e 2062 6967 6672 616d 6573 5f72  turn bigframes_r
-00010d90: 6766 280a 2020 2020 2020 2020 2020 2020  gf(.            
-00010da0: 6675 6e63 7469 6f6e 5f6e 616d 653d 6675  function_name=fu
-00010db0: 6e63 7469 6f6e 5f6e 616d 652c 0a20 2020  nction_name,.   
-00010dc0: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
-00010dd0: 3d73 656c 662c 0a20 2020 2020 2020 2029  =self,.        )
-00010de0: 0a0a 2020 2020 6465 6620 5f70 7265 7061  ..    def _prepa
-00010df0: 7265 5f71 7565 7279 5f6a 6f62 5f63 6f6e  re_query_job_con
-00010e00: 6669 6728 0a20 2020 2020 2020 2073 656c  fig(.        sel
-00010e10: 662c 0a20 2020 2020 2020 206a 6f62 5f63  f,.        job_c
-00010e20: 6f6e 6669 673a 204f 7074 696f 6e61 6c5b  onfig: Optional[
-00010e30: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-00010e40: 6243 6f6e 6669 675d 203d 204e 6f6e 652c  bConfig] = None,
-00010e50: 0a20 2020 2029 202d 3e20 6269 6771 7565  .    ) -> bigque
-00010e60: 7279 2e51 7565 7279 4a6f 6243 6f6e 6669  ry.QueryJobConfi
-00010e70: 673a 0a20 2020 2020 2020 2069 6620 6a6f  g:.        if jo
-00010e80: 625f 636f 6e66 6967 2069 7320 4e6f 6e65  b_config is None
-00010e90: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
-00010ea0: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
-00010eb0: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
-00010ec0: 6967 2829 0a20 2020 2020 2020 2065 6c73  ig().        els
-00010ed0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-00010ee0: 2043 7265 6174 6520 6120 636f 7079 2073   Create a copy s
-00010ef0: 6f20 7468 6174 2077 6520 646f 6e27 7420  o that we don't 
-00010f00: 6d75 7461 7465 2074 6865 206f 7269 6769  mutate the origi
-00010f10: 6e61 6c20 636f 6e66 6967 2070 6173 7365  nal config passe
-00010f20: 640a 2020 2020 2020 2020 2020 2020 6a6f  d.            jo
-00010f30: 625f 636f 6e66 6967 203d 2074 7970 696e  b_config = typin
-00010f40: 672e 6361 7374 280a 2020 2020 2020 2020  g.cast(.        
-00010f50: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
-00010f60: 2e51 7565 7279 4a6f 6243 6f6e 6669 672c  .QueryJobConfig,
-00010f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f80: 2062 6967 7175 6572 792e 5175 6572 794a   bigquery.QueryJ
-00010f90: 6f62 436f 6e66 6967 2e66 726f 6d5f 6170  obConfig.from_ap
-00010fa0: 695f 7265 7072 286a 6f62 5f63 6f6e 6669  i_repr(job_confi
-00010fb0: 672e 746f 5f61 7069 5f72 6570 7228 2929  g.to_api_repr())
-00010fc0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00010fd0: 0a20 2020 2020 2020 2069 6620 6269 6766  .        if bigf
-00010fe0: 7261 6d65 732e 6f70 7469 6f6e 732e 636f  rames.options.co
-00010ff0: 6d70 7574 652e 6d61 7869 6d75 6d5f 6279  mpute.maximum_by
-00011000: 7465 735f 6269 6c6c 6564 2069 7320 6e6f  tes_billed is no
-00011010: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00011020: 2020 2020 6a6f 625f 636f 6e66 6967 2e6d      job_config.m
-00011030: 6178 696d 756d 5f62 7974 6573 5f62 696c  aximum_bytes_bil
-00011040: 6c65 6420 3d20 280a 2020 2020 2020 2020  led = (.        
-00011050: 2020 2020 2020 2020 6269 6766 7261 6d65          bigframe
-00011060: 732e 6f70 7469 6f6e 732e 636f 6d70 7574  s.options.comput
-00011070: 652e 6d61 7869 6d75 6d5f 6279 7465 735f  e.maximum_bytes_
-00011080: 6269 6c6c 6564 0a20 2020 2020 2020 2020  billed.         
-00011090: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-000110a0: 2073 656c 662e 5f62 715f 6b6d 735f 6b65   self._bq_kms_ke
-000110b0: 795f 6e61 6d65 3a0a 2020 2020 2020 2020  y_name:.        
-000110c0: 2020 2020 6a6f 625f 636f 6e66 6967 2e64      job_config.d
-000110d0: 6573 7469 6e61 7469 6f6e 5f65 6e63 7279  estination_encry
-000110e0: 7074 696f 6e5f 636f 6e66 6967 7572 6174  ption_configurat
-000110f0: 696f 6e20 3d20 280a 2020 2020 2020 2020  ion = (.        
-00011100: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
-00011110: 2e45 6e63 7279 7074 696f 6e43 6f6e 6669  .EncryptionConfi
-00011120: 6775 7261 7469 6f6e 286b 6d73 5f6b 6579  guration(kms_key
-00011130: 5f6e 616d 653d 7365 6c66 2e5f 6271 5f6b  _name=self._bq_k
-00011140: 6d73 5f6b 6579 5f6e 616d 6529 0a20 2020  ms_key_name).   
-00011150: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00011160: 2020 2020 7265 7475 726e 206a 6f62 5f63      return job_c
-00011170: 6f6e 6669 670a 0a20 2020 2064 6566 205f  onfig..    def _
-00011180: 7072 6570 6172 655f 6c6f 6164 5f6a 6f62  prepare_load_job
-00011190: 5f63 6f6e 6669 6728 7365 6c66 2920 2d3e  _config(self) ->
-000111a0: 2062 6967 7175 6572 792e 4c6f 6164 4a6f   bigquery.LoadJo
-000111b0: 6243 6f6e 6669 673a 0a20 2020 2020 2020  bConfig:.       
-000111c0: 2023 2043 7265 6174 6520 6120 636f 7079   # Create a copy
-000111d0: 2073 6f20 7468 6174 2077 6520 646f 6e27   so that we don'
-000111e0: 7420 6d75 7461 7465 2074 6865 206f 7269  t mutate the ori
-000111f0: 6769 6e61 6c20 636f 6e66 6967 2070 6173  ginal config pas
-00011200: 7365 640a 2020 2020 2020 2020 6a6f 625f  sed.        job_
-00011210: 636f 6e66 6967 203d 2062 6967 7175 6572  config = bigquer
-00011220: 792e 4c6f 6164 4a6f 6243 6f6e 6669 6728  y.LoadJobConfig(
-00011230: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00011240: 6c66 2e5f 6271 5f6b 6d73 5f6b 6579 5f6e  lf._bq_kms_key_n
-00011250: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-00011260: 206a 6f62 5f63 6f6e 6669 672e 6465 7374   job_config.dest
-00011270: 696e 6174 696f 6e5f 656e 6372 7970 7469  ination_encrypti
-00011280: 6f6e 5f63 6f6e 6669 6775 7261 7469 6f6e  on_configuration
-00011290: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000112a0: 2020 2020 2062 6967 7175 6572 792e 456e       bigquery.En
-000112b0: 6372 7970 7469 6f6e 436f 6e66 6967 7572  cryptionConfigur
-000112c0: 6174 696f 6e28 6b6d 735f 6b65 795f 6e61  ation(kms_key_na
-000112d0: 6d65 3d73 656c 662e 5f62 715f 6b6d 735f  me=self._bq_kms_
-000112e0: 6b65 795f 6e61 6d65 290a 2020 2020 2020  key_name).      
-000112f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00011300: 2072 6574 7572 6e20 6a6f 625f 636f 6e66   return job_conf
-00011310: 6967 0a0a 2020 2020 6465 6620 5f70 7265  ig..    def _pre
-00011320: 7061 7265 5f63 6f70 795f 6a6f 625f 636f  pare_copy_job_co
-00011330: 6e66 6967 2873 656c 6629 202d 3e20 6269  nfig(self) -> bi
-00011340: 6771 7565 7279 2e43 6f70 794a 6f62 436f  gquery.CopyJobCo
-00011350: 6e66 6967 3a0a 2020 2020 2020 2020 2320  nfig:.        # 
-00011360: 4372 6561 7465 2061 2063 6f70 7920 736f  Create a copy so
-00011370: 2074 6861 7420 7765 2064 6f6e 2774 206d   that we don't m
-00011380: 7574 6174 6520 7468 6520 6f72 6967 696e  utate the origin
-00011390: 616c 2063 6f6e 6669 6720 7061 7373 6564  al config passed
-000113a0: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
-000113b0: 6669 6720 3d20 6269 6771 7565 7279 2e43  fig = bigquery.C
-000113c0: 6f70 794a 6f62 436f 6e66 6967 2829 0a0a  opyJobConfig()..
-000113d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000113e0: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
-000113f0: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
-00011400: 625f 636f 6e66 6967 2e64 6573 7469 6e61  b_config.destina
-00011410: 7469 6f6e 5f65 6e63 7279 7074 696f 6e5f  tion_encryption_
-00011420: 636f 6e66 6967 7572 6174 696f 6e20 3d20  configuration = 
-00011430: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011440: 2020 6269 6771 7565 7279 2e45 6e63 7279    bigquery.Encry
-00011450: 7074 696f 6e43 6f6e 6669 6775 7261 7469  ptionConfigurati
-00011460: 6f6e 286b 6d73 5f6b 6579 5f6e 616d 653d  on(kms_key_name=
-00011470: 7365 6c66 2e5f 6271 5f6b 6d73 5f6b 6579  self._bq_kms_key
-00011480: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
-00011490: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-000114a0: 7475 726e 206a 6f62 5f63 6f6e 6669 670a  turn job_config.
-000114b0: 0a20 2020 2064 6566 205f 7374 6172 745f  .    def _start_
-000114c0: 7175 6572 7928 0a20 2020 2020 2020 2073  query(.        s
-000114d0: 656c 662c 0a20 2020 2020 2020 2073 716c  elf,.        sql
-000114e0: 3a20 7374 722c 0a20 2020 2020 2020 206a  : str,.        j
-000114f0: 6f62 5f63 6f6e 6669 673a 204f 7074 696f  ob_config: Optio
-00011500: 6e61 6c5b 6269 6771 7565 7279 2e6a 6f62  nal[bigquery.job
-00011510: 2e51 7565 7279 4a6f 6243 6f6e 6669 675d  .QueryJobConfig]
-00011520: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00011530: 206d 6178 5f72 6573 756c 7473 3a20 4f70   max_results: Op
-00011540: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00011550: 6e65 2c0a 2020 2020 2020 2020 7469 6d65  ne,.        time
-00011560: 6f75 743a 204f 7074 696f 6e61 6c5b 666c  out: Optional[fl
-00011570: 6f61 745d 203d 204e 6f6e 652c 0a20 2020  oat] = None,.   
-00011580: 2029 202d 3e20 5475 706c 655b 6269 6771   ) -> Tuple[bigq
-00011590: 7565 7279 2e74 6162 6c65 2e52 6f77 4974  uery.table.RowIt
-000115a0: 6572 6174 6f72 2c20 6269 6771 7565 7279  erator, bigquery
-000115b0: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
-000115c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000115d0: 5374 6172 7473 2042 6967 5175 6572 7920  Starts BigQuery 
-000115e0: 7175 6572 7920 6a6f 6220 616e 6420 7761  query job and wa
-000115f0: 6974 7320 666f 7220 7265 7375 6c74 732e  its for results.
-00011600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011610: 2020 2020 206a 6f62 5f63 6f6e 6669 6720       job_config 
-00011620: 3d20 7365 6c66 2e5f 7072 6570 6172 655f  = self._prepare_
-00011630: 7175 6572 795f 6a6f 625f 636f 6e66 6967  query_job_config
-00011640: 286a 6f62 5f63 6f6e 6669 6729 0a20 2020  (job_config).   
-00011650: 2020 2020 2072 6574 7572 6e20 6269 6766       return bigf
-00011660: 7261 6d65 732e 7365 7373 696f 6e2e 5f69  rames.session._i
-00011670: 6f2e 6269 6771 7565 7279 2e73 7461 7274  o.bigquery.start
-00011680: 5f71 7565 7279 5f77 6974 685f 636c 6965  _query_with_clie
-00011690: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-000116a0: 7365 6c66 2e62 7163 6c69 656e 742c 2073  self.bqclient, s
-000116b0: 716c 2c20 6a6f 625f 636f 6e66 6967 2c20  ql, job_config, 
-000116c0: 6d61 785f 7265 7375 6c74 732c 2074 696d  max_results, tim
-000116d0: 656f 7574 0a20 2020 2020 2020 2029 0a0a  eout.        )..
-000116e0: 2020 2020 6465 6620 5f73 7461 7274 5f71      def _start_q
-000116f0: 7565 7279 5f6d 6c5f 6464 6c28 0a20 2020  uery_ml_ddl(.   
-00011700: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00011710: 2020 2073 716c 3a20 7374 722c 0a20 2020     sql: str,.   
-00011720: 2029 202d 3e20 5475 706c 655b 6269 6771   ) -> Tuple[bigq
-00011730: 7565 7279 2e74 6162 6c65 2e52 6f77 4974  uery.table.RowIt
-00011740: 6572 6174 6f72 2c20 6269 6771 7565 7279  erator, bigquery
-00011750: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
-00011760: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011770: 5374 6172 7473 2042 6967 5175 6572 7920  Starts BigQuery 
-00011780: 4d4c 2044 444c 2071 7565 7279 206a 6f62  ML DDL query job
-00011790: 2028 4352 4541 5445 204d 4f44 454c 2f41   (CREATE MODEL/A
-000117a0: 4c54 4552 204d 4f44 454c 2f2e 2e2e 2920  LTER MODEL/...) 
-000117b0: 616e 640a 2020 2020 2020 2020 7761 6974  and.        wait
-000117c0: 7320 666f 7220 7265 7375 6c74 732e 0a20  s for results.. 
-000117d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000117e0: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
-000117f0: 7365 6c66 2e5f 7072 6570 6172 655f 7175  self._prepare_qu
-00011800: 6572 795f 6a6f 625f 636f 6e66 6967 2829  ery_job_config()
-00011810: 0a0a 2020 2020 2020 2020 2320 4251 4d4c  ..        # BQML
-00011820: 2065 7870 6563 7473 206b 6d73 5f6b 6579   expects kms_key
-00011830: 5f6e 616d 6520 7468 726f 7567 6820 4f50  _name through OP
-00011840: 5449 4f4e 5320 616e 6420 6e6f 7420 7468  TIONS and not th
-00011850: 726f 7567 6820 6a6f 6220 636f 6e66 6967  rough job config
-00011860: 2c0a 2020 2020 2020 2020 2320 736f 2077  ,.        # so w
-00011870: 6520 6d75 7374 2072 6573 6574 2061 6e79  e must reset any
-00011880: 2065 6e63 7279 7074 696f 6e20 7365 7420   encryption set 
-00011890: 696e 2074 6865 206a 6f62 2063 6f6e 6669  in the job confi
-000118a0: 670a 2020 2020 2020 2020 2320 6874 7470  g.        # http
-000118b0: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
-000118c0: 2e63 6f6d 2f62 6967 7175 6572 792f 646f  .com/bigquery/do
-000118d0: 6373 2f63 7573 746f 6d65 722d 6d61 6e61  cs/customer-mana
-000118e0: 6765 642d 656e 6372 7970 7469 6f6e 2365  ged-encryption#e
-000118f0: 6e63 7279 7074 2d6d 6f64 656c 0a20 2020  ncrypt-model.   
-00011900: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
-00011910: 6465 7374 696e 6174 696f 6e5f 656e 6372  destination_encr
-00011920: 7970 7469 6f6e 5f63 6f6e 6669 6775 7261  yption_configura
-00011930: 7469 6f6e 203d 204e 6f6e 650a 0a20 2020  tion = None..   
-00011940: 2020 2020 2072 6574 7572 6e20 6269 6766       return bigf
-00011950: 7261 6d65 732e 7365 7373 696f 6e2e 5f69  rames.session._i
-00011960: 6f2e 6269 6771 7565 7279 2e73 7461 7274  o.bigquery.start
-00011970: 5f71 7565 7279 5f77 6974 685f 636c 6965  _query_with_clie
-00011980: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-00011990: 7365 6c66 2e62 7163 6c69 656e 742c 2073  self.bqclient, s
-000119a0: 716c 2c20 6a6f 625f 636f 6e66 6967 0a20  ql, job_config. 
-000119b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-000119c0: 6620 5f63 6163 6865 5f77 6974 685f 636c  f _cache_with_cl
-000119d0: 7573 7465 725f 636f 6c73 280a 2020 2020  uster_cols(.    
-000119e0: 2020 2020 7365 6c66 2c20 6172 7261 795f      self, array_
-000119f0: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
-00011a00: 7956 616c 7565 2c20 636c 7573 7465 725f  yValue, cluster_
-00011a10: 636f 6c73 3a20 7479 7069 6e67 2e53 6571  cols: typing.Seq
-00011a20: 7565 6e63 655b 7374 725d 0a20 2020 2029  uence[str].    )
-00011a30: 202d 3e20 636f 7265 2e41 7272 6179 5661   -> core.ArrayVa
-00011a40: 6c75 653a 0a20 2020 2020 2020 2022 2222  lue:.        """
-00011a50: 4578 6563 7574 6573 2074 6865 2071 7565  Executes the que
-00011a60: 7279 2061 6e64 2075 7365 7320 7468 6520  ry and uses the 
-00011a70: 7265 7375 6c74 696e 6720 7461 626c 6520  resulting table 
-00011a80: 746f 2072 6577 7269 7465 2066 7574 7572  to rewrite futur
-00011a90: 6520 6578 6563 7574 696f 6e73 2e22 2222  e executions."""
-00011aa0: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
-00011ab0: 2055 7365 2074 6869 7320 666f 7220 616c   Use this for al
-00011ac0: 6c20 6578 6563 7574 696f 6e73 3f20 5072  l executions? Pr
-00011ad0: 6f62 6c65 6d20 6973 2074 6861 7420 6361  oblem is that ca
-00011ae0: 6368 696e 6720 6d61 7465 7269 616c 697a  ching materializ
-00011af0: 6573 2065 7874 7261 0a20 2020 2020 2020  es extra.       
-00011b00: 2023 206f 7264 6572 696e 6720 636f 6c75   # ordering colu
-00011b10: 6d6e 730a 2020 2020 2020 2020 636f 6d70  mns.        comp
-00011b20: 696c 6564 5f76 616c 7565 203d 2073 656c  iled_value = sel
-00011b30: 662e 5f63 6f6d 7069 6c65 5f6f 7264 6572  f._compile_order
-00011b40: 6564 2861 7272 6179 5f76 616c 7565 290a  ed(array_value).
-00011b50: 0a20 2020 2020 2020 2069 6269 735f 6578  .        ibis_ex
-00011b60: 7072 203d 2063 6f6d 7069 6c65 645f 7661  pr = compiled_va
-00011b70: 6c75 652e 5f74 6f5f 6962 6973 5f65 7870  lue._to_ibis_exp
-00011b80: 7228 0a20 2020 2020 2020 2020 2020 206f  r(.            o
-00011b90: 7264 6572 696e 675f 6d6f 6465 3d22 756e  rdering_mode="un
-00011ba0: 6f72 6465 7265 6422 2c20 6578 706f 7365  ordered", expose
-00011bb0: 5f68 6964 6465 6e5f 636f 6c73 3d54 7275  _hidden_cols=Tru
-00011bc0: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
-00011bd0: 2020 2020 746d 705f 7461 626c 6520 3d20      tmp_table = 
-00011be0: 7365 6c66 2e5f 6962 6973 5f74 6f5f 7465  self._ibis_to_te
-00011bf0: 6d70 5f74 6162 6c65 280a 2020 2020 2020  mp_table(.      
-00011c00: 2020 2020 2020 6962 6973 5f65 7870 722c        ibis_expr,
-00011c10: 2063 6c75 7374 6572 5f63 6f6c 733d 636c   cluster_cols=cl
-00011c20: 7573 7465 725f 636f 6c73 2c20 6170 695f  uster_cols, api_
-00011c30: 6e61 6d65 3d22 6361 6368 6564 220a 2020  name="cached".  
-00011c40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00011c50: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00011c60: 203d 2073 656c 662e 6962 6973 5f63 6c69   = self.ibis_cli
-00011c70: 656e 742e 7461 626c 6528 0a20 2020 2020  ent.table(.     
-00011c80: 2020 2020 2020 2074 6d70 5f74 6162 6c65         tmp_table
-00011c90: 2e74 6162 6c65 5f69 642c 0a20 2020 2020  .table_id,.     
-00011ca0: 2020 2020 2020 2073 6368 656d 613d 746d         schema=tm
-00011cb0: 705f 7461 626c 652e 6461 7461 7365 745f  p_table.dataset_
-00011cc0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00011cd0: 6461 7461 6261 7365 3d74 6d70 5f74 6162  database=tmp_tab
-00011ce0: 6c65 2e70 726f 6a65 6374 2c0a 2020 2020  le.project,.    
-00011cf0: 2020 2020 290a 2020 2020 2020 2020 6e65      ).        ne
-00011d00: 775f 636f 6c75 6d6e 7320 3d20 5b74 6162  w_columns = [tab
-00011d10: 6c65 5f65 7870 7265 7373 696f 6e5b 636f  le_expression[co
-00011d20: 6c75 6d6e 5d20 666f 7220 636f 6c75 6d6e  lumn] for column
-00011d30: 2069 6e20 636f 6d70 696c 6564 5f76 616c   in compiled_val
-00011d40: 7565 2e63 6f6c 756d 6e5f 6964 735d 0a20  ue.column_ids]. 
-00011d50: 2020 2020 2020 206e 6577 5f68 6964 6465         new_hidde
-00011d60: 6e5f 636f 6c75 6d6e 7320 3d20 5b0a 2020  n_columns = [.  
-00011d70: 2020 2020 2020 2020 2020 7461 626c 655f            table_
-00011d80: 6578 7072 6573 7369 6f6e 5b63 6f6c 756d  expression[colum
-00011d90: 6e5d 0a20 2020 2020 2020 2020 2020 2066  n].            f
-00011da0: 6f72 2063 6f6c 756d 6e20 696e 2063 6f6d  or column in com
-00011db0: 7069 6c65 645f 7661 6c75 652e 5f68 6964  piled_value._hid
-00011dc0: 6465 6e5f 6f72 6465 7269 6e67 5f63 6f6c  den_ordering_col
-00011dd0: 756d 6e5f 6e61 6d65 730a 2020 2020 2020  umn_names.      
-00011de0: 2020 5d0a 2020 2020 2020 2020 2320 544f    ].        # TO
-00011df0: 444f 3a20 496e 7374 6561 642c 206b 6565  DO: Instead, kee
-00011e00: 7020 7365 7373 696f 6e2d 7769 6465 206d  p session-wide m
-00011e10: 6170 206f 6620 6361 6368 6564 2072 6573  ap of cached res
-00011e20: 756c 7473 2061 6e64 2061 7574 6f6d 6174  ults and automat
-00011e30: 6963 616c 6c79 2072 6575 7365 0a20 2020  ically reuse.   
-00011e40: 2020 2020 2072 6574 7572 6e20 636f 7265       return core
-00011e50: 2e41 7272 6179 5661 6c75 652e 6672 6f6d  .ArrayValue.from
-00011e60: 5f69 6269 7328 0a20 2020 2020 2020 2020  _ibis(.         
-00011e70: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00011e80: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
-00011e90: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
-00011ea0: 2020 2063 6f6c 756d 6e73 3d6e 6577 5f63     columns=new_c
-00011eb0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
-00011ec0: 2020 2020 6869 6464 656e 5f6f 7264 6572      hidden_order
-00011ed0: 696e 675f 636f 6c75 6d6e 733d 6e65 775f  ing_columns=new_
-00011ee0: 6869 6464 656e 5f63 6f6c 756d 6e73 2c0a  hidden_columns,.
-00011ef0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-00011f00: 7269 6e67 3d63 6f6d 7069 6c65 645f 7661  ring=compiled_va
-00011f10: 6c75 652e 5f6f 7264 6572 696e 672c 0a20  lue._ordering,. 
-00011f20: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00011f30: 6620 5f63 6163 6865 5f77 6974 685f 6f66  f _cache_with_of
-00011f40: 6673 6574 7328 7365 6c66 2c20 6172 7261  fsets(self, arra
-00011f50: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
-00011f60: 7261 7956 616c 7565 2920 2d3e 2063 6f72  rayValue) -> cor
-00011f70: 652e 4172 7261 7956 616c 7565 3a0a 2020  e.ArrayValue:.  
-00011f80: 2020 2020 2020 2222 2245 7865 6375 7465        """Execute
-00011f90: 7320 7468 6520 7175 6572 7920 616e 6420  s the query and 
-00011fa0: 7573 6573 2074 6865 2072 6573 756c 7469  uses the resulti
-00011fb0: 6e67 2074 6162 6c65 2074 6f20 7265 7772  ng table to rewr
-00011fc0: 6974 6520 6675 7475 7265 2065 7865 6375  ite future execu
-00011fd0: 7469 6f6e 732e 2222 220a 2020 2020 2020  tions.""".      
-00011fe0: 2020 2320 544f 444f 3a20 5573 6520 7468    # TODO: Use th
-00011ff0: 6973 2066 6f72 2061 6c6c 2065 7865 6375  is for all execu
-00012000: 7469 6f6e 733f 2050 726f 626c 656d 2069  tions? Problem i
-00012010: 7320 7468 6174 2063 6163 6869 6e67 206d  s that caching m
-00012020: 6174 6572 6961 6c69 7a65 7320 6578 7472  aterializes extr
-00012030: 610a 2020 2020 2020 2020 2320 6f72 6465  a.        # orde
-00012040: 7269 6e67 2063 6f6c 756d 6e73 0a20 2020  ring columns.   
-00012050: 2020 2020 2063 6f6d 7069 6c65 645f 7661       compiled_va
-00012060: 6c75 6520 3d20 7365 6c66 2e5f 636f 6d70  lue = self._comp
-00012070: 696c 655f 6f72 6465 7265 6428 6172 7261  ile_ordered(arra
-00012080: 795f 7661 6c75 6529 0a0a 2020 2020 2020  y_value)..      
-00012090: 2020 6962 6973 5f65 7870 7220 3d20 636f    ibis_expr = co
-000120a0: 6d70 696c 6564 5f76 616c 7565 2e5f 746f  mpiled_value._to
-000120b0: 5f69 6269 735f 6578 7072 280a 2020 2020  _ibis_expr(.    
-000120c0: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
-000120d0: 5f6d 6f64 653d 226f 6666 7365 745f 636f  _mode="offset_co
-000120e0: 6c22 2c20 6f72 6465 725f 636f 6c5f 6e61  l", order_col_na
-000120f0: 6d65 3d22 6269 6766 7261 6d65 735f 6f66  me="bigframes_of
-00012100: 6673 6574 7322 0a20 2020 2020 2020 2029  fsets".        )
-00012110: 0a20 2020 2020 2020 2074 6d70 5f74 6162  .        tmp_tab
-00012120: 6c65 203d 2073 656c 662e 5f69 6269 735f  le = self._ibis_
-00012130: 746f 5f74 656d 705f 7461 626c 6528 0a20  to_temp_table(. 
-00012140: 2020 2020 2020 2020 2020 2069 6269 735f             ibis_
-00012150: 6578 7072 2c20 636c 7573 7465 725f 636f  expr, cluster_co
-00012160: 6c73 3d5b 2262 6967 6672 616d 6573 5f6f  ls=["bigframes_o
-00012170: 6666 7365 7473 225d 2c20 6170 695f 6e61  ffsets"], api_na
-00012180: 6d65 3d22 6361 6368 6564 220a 2020 2020  me="cached".    
-00012190: 2020 2020 290a 2020 2020 2020 2020 7461      ).        ta
-000121a0: 626c 655f 6578 7072 6573 7369 6f6e 203d  ble_expression =
-000121b0: 2073 656c 662e 6962 6973 5f63 6c69 656e   self.ibis_clien
-000121c0: 742e 7461 626c 6528 0a20 2020 2020 2020  t.table(.       
-000121d0: 2020 2020 2074 6d70 5f74 6162 6c65 2e74       tmp_table.t
-000121e0: 6162 6c65 5f69 642c 0a20 2020 2020 2020  able_id,.       
-000121f0: 2020 2020 2073 6368 656d 613d 746d 705f       schema=tmp_
-00012200: 7461 626c 652e 6461 7461 7365 745f 6964  table.dataset_id
-00012210: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00012220: 7461 6261 7365 3d74 6d70 5f74 6162 6c65  tabase=tmp_table
-00012230: 2e70 726f 6a65 6374 2c0a 2020 2020 2020  .project,.      
-00012240: 2020 290a 2020 2020 2020 2020 6e65 775f    ).        new_
-00012250: 636f 6c75 6d6e 7320 3d20 5b74 6162 6c65  columns = [table
-00012260: 5f65 7870 7265 7373 696f 6e5b 636f 6c75  _expression[colu
-00012270: 6d6e 5d20 666f 7220 636f 6c75 6d6e 2069  mn] for column i
-00012280: 6e20 636f 6d70 696c 6564 5f76 616c 7565  n compiled_value
-00012290: 2e63 6f6c 756d 6e5f 6964 735d 0a20 2020  .column_ids].   
-000122a0: 2020 2020 206e 6577 5f68 6964 6465 6e5f       new_hidden_
-000122b0: 636f 6c75 6d6e 7320 3d20 5b74 6162 6c65  columns = [table
-000122c0: 5f65 7870 7265 7373 696f 6e5b 2262 6967  _expression["big
-000122d0: 6672 616d 6573 5f6f 6666 7365 7473 225d  frames_offsets"]
-000122e0: 5d0a 2020 2020 2020 2020 2320 544f 444f  ].        # TODO
-000122f0: 3a20 496e 7374 6561 642c 206b 6565 7020  : Instead, keep 
-00012300: 7365 7373 696f 6e2d 7769 6465 206d 6170  session-wide map
-00012310: 206f 6620 6361 6368 6564 2072 6573 756c   of cached resul
-00012320: 7473 2061 6e64 2061 7574 6f6d 6174 6963  ts and automatic
-00012330: 616c 6c79 2072 6575 7365 0a20 2020 2020  ally reuse.     
-00012340: 2020 2072 6574 7572 6e20 636f 7265 2e41     return core.A
-00012350: 7272 6179 5661 6c75 652e 6672 6f6d 5f69  rrayValue.from_i
-00012360: 6269 7328 0a20 2020 2020 2020 2020 2020  bis(.           
-00012370: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-00012380: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
-00012390: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-000123a0: 2063 6f6c 756d 6e73 3d6e 6577 5f63 6f6c   columns=new_col
-000123b0: 756d 6e73 2c0a 2020 2020 2020 2020 2020  umns,.          
-000123c0: 2020 6869 6464 656e 5f6f 7264 6572 696e    hidden_orderin
-000123d0: 675f 636f 6c75 6d6e 733d 6e65 775f 6869  g_columns=new_hi
-000123e0: 6464 656e 5f63 6f6c 756d 6e73 2c0a 2020  dden_columns,.  
-000123f0: 2020 2020 2020 2020 2020 6f72 6465 7269            orderi
-00012400: 6e67 3d6f 7264 6572 2e45 7870 7265 7373  ng=order.Express
-00012410: 696f 6e4f 7264 6572 696e 672e 6672 6f6d  ionOrdering.from
-00012420: 5f6f 6666 7365 745f 636f 6c28 2262 6967  _offset_col("big
-00012430: 6672 616d 6573 5f6f 6666 7365 7473 2229  frames_offsets")
-00012440: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00012450: 2064 6566 205f 7369 6d70 6c69 6679 5f77   def _simplify_w
-00012460: 6974 685f 6361 6368 696e 6728 7365 6c66  ith_caching(self
-00012470: 2c20 6172 7261 795f 7661 6c75 653a 2063  , array_value: c
-00012480: 6f72 652e 4172 7261 7956 616c 7565 2920  ore.ArrayValue) 
-00012490: 2d3e 2063 6f72 652e 4172 7261 7956 616c  -> core.ArrayVal
-000124a0: 7565 3a0a 2020 2020 2020 2020 2222 2241  ue:.        """A
-000124b0: 7474 656d 7074 7320 746f 2068 616e 646c  ttempts to handl
-000124c0: 6520 7468 6520 636f 6d70 6c65 7869 7479  e the complexity
-000124d0: 2062 7920 6361 6368 696e 6720 6475 706c   by caching dupl
-000124e0: 6963 6174 6564 2073 7562 7472 6565 7320  icated subtrees 
-000124f0: 616e 6420 6272 6561 6b69 6e67 2074 6865  and breaking the
-00012500: 2071 7565 7279 2069 6e74 6f20 7069 6563   query into piec
-00012510: 6573 2e22 2222 0a20 2020 2020 2020 2069  es.""".        i
-00012520: 6620 6e6f 7420 6269 6766 7261 6d65 732e  f not bigframes.
-00012530: 6f70 7469 6f6e 732e 636f 6d70 7574 652e  options.compute.
-00012540: 656e 6162 6c65 5f6d 756c 7469 5f71 7565  enable_multi_que
-00012550: 7279 5f65 7865 6375 7469 6f6e 3a0a 2020  ry_execution:.  
-00012560: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00012570: 2061 7272 6179 5f76 616c 7565 0a20 2020   array_value.   
-00012580: 2020 2020 206e 6f64 6520 3d20 6172 7261       node = arra
-00012590: 795f 7661 6c75 652e 6e6f 6465 0a20 2020  y_value.node.   
-000125a0: 2020 2020 2069 6620 6e6f 6465 2e70 6c61       if node.pla
-000125b0: 6e6e 696e 675f 636f 6d70 6c65 7869 7479  nning_complexity
-000125c0: 203c 2051 5545 5259 5f43 4f4d 504c 4558   < QUERY_COMPLEX
-000125d0: 4954 595f 4c49 4d49 543a 0a20 2020 2020  ITY_LIMIT:.     
-000125e0: 2020 2020 2020 2072 6574 7572 6e20 6172         return ar
-000125f0: 7261 795f 7661 6c75 650a 0a20 2020 2020  ray_value..     
-00012600: 2020 2066 6f72 205f 2069 6e20 7261 6e67     for _ in rang
-00012610: 6528 4d41 585f 5355 4254 5245 455f 4641  e(MAX_SUBTREE_FA
-00012620: 4354 4f52 494e 4753 293a 0a20 2020 2020  CTORINGS):.     
-00012630: 2020 2020 2020 2075 7064 6174 6564 203d         updated =
-00012640: 2073 656c 662e 5f63 6163 6865 5f6d 6f73   self._cache_mos
-00012650: 745f 636f 6d70 6c65 785f 7375 6274 7265  t_complex_subtre
-00012660: 6528 6e6f 6465 290a 2020 2020 2020 2020  e(node).        
-00012670: 2020 2020 6966 2075 7064 6174 6564 2069      if updated i
-00012680: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00012690: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-000126a0: 6f72 652e 4172 7261 7956 616c 7565 286e  ore.ArrayValue(n
-000126b0: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
-000126c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000126d0: 2020 2020 2020 206e 6f64 6520 3d20 7570         node = up
-000126e0: 6461 7465 640a 0a20 2020 2020 2020 2072  dated..        r
-000126f0: 6574 7572 6e20 636f 7265 2e41 7272 6179  eturn core.Array
-00012700: 5661 6c75 6528 6e6f 6465 290a 0a20 2020  Value(node)..   
-00012710: 2064 6566 205f 6361 6368 655f 6d6f 7374   def _cache_most
-00012720: 5f63 6f6d 706c 6578 5f73 7562 7472 6565  _complex_subtree
-00012730: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00012740: 6e6f 6465 3a20 6e6f 6465 732e 4269 6746  node: nodes.BigF
-00012750: 7261 6d65 4e6f 6465 0a20 2020 2029 202d  rameNode.    ) -
-00012760: 3e20 4f70 7469 6f6e 616c 5b6e 6f64 6573  > Optional[nodes
-00012770: 2e42 6967 4672 616d 654e 6f64 655d 3a0a  .BigFrameNode]:.
-00012780: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00012790: 4966 2071 7565 7279 2066 6169 6c73 2c20  If query fails, 
-000127a0: 7265 7472 7920 7769 7468 206c 6f77 6572  retry with lower
-000127b0: 2063 6f6d 706c 6578 6974 7920 6c69 6d69   complexity limi
-000127c0: 740a 2020 2020 2020 2020 7661 6c69 645f  t.        valid_
-000127d0: 6361 6e64 6964 6174 6573 203d 2074 7261  candidates = tra
-000127e0: 7665 7273 616c 732e 636f 756e 745f 636f  versals.count_co
-000127f0: 6d70 6c65 785f 6e6f 6465 7328 0a20 2020  mplex_nodes(.   
-00012800: 2020 2020 2020 2020 206e 6f64 652c 0a20           node,. 
-00012810: 2020 2020 2020 2020 2020 206d 696e 5f63             min_c
-00012820: 6f6d 706c 6578 6974 793d 2851 5545 5259  omplexity=(QUERY
-00012830: 5f43 4f4d 504c 4558 4954 595f 4c49 4d49  _COMPLEXITY_LIMI
-00012840: 5420 2f20 3530 3029 2c0a 2020 2020 2020  T / 500),.      
-00012850: 2020 2020 2020 6d61 785f 636f 6d70 6c65        max_comple
-00012860: 7869 7479 3d51 5545 5259 5f43 4f4d 504c  xity=QUERY_COMPL
-00012870: 4558 4954 595f 4c49 4d49 542c 0a20 2020  EXITY_LIMIT,.   
-00012880: 2020 2020 2029 2e69 7465 6d73 2829 0a20       ).items(). 
-00012890: 2020 2020 2020 2023 2048 6575 7269 7374         # Heurist
-000128a0: 6963 3a20 7375 6274 7265 655f 636f 6d70  ic: subtree_comp
-000128b0: 6c65 6978 7479 202a 2028 636f 7069 6573  leixty * (copies
-000128c0: 206f 6620 7375 6274 7265 6529 5e32 0a20   of subtree)^2. 
-000128d0: 2020 2020 2020 2062 6573 745f 6361 6e64         best_cand
-000128e0: 6964 6174 6520 3d20 6d61 7828 0a20 2020  idate = max(.   
-000128f0: 2020 2020 2020 2020 2076 616c 6964 5f63           valid_c
-00012900: 616e 6469 6461 7465 732c 0a20 2020 2020  andidates,.     
-00012910: 2020 2020 2020 206b 6579 3d6c 616d 6264         key=lambd
-00012920: 6120 693a 2069 5b30 5d2e 706c 616e 6e69  a i: i[0].planni
-00012930: 6e67 5f63 6f6d 706c 6578 6974 7920 2b20  ng_complexity + 
-00012940: 2869 5b31 5d20 2a2a 2032 292c 0a20 2020  (i[1] ** 2),.   
-00012950: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-00012960: 3d4e 6f6e 652c 0a20 2020 2020 2020 2029  =None,.        )
-00012970: 0a0a 2020 2020 2020 2020 6966 2062 6573  ..        if bes
-00012980: 745f 6361 6e64 6964 6174 6520 6973 204e  t_candidate is N
-00012990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000129a0: 2023 204e 6f20 676f 6f64 2073 7562 7472   # No good subtr
-000129b0: 6565 7320 746f 2063 6163 6865 2c20 6a75  ees to cache, ju
-000129c0: 7374 2072 6574 7572 6e20 6f72 6967 696e  st return origin
-000129d0: 616c 2074 7265 650a 2020 2020 2020 2020  al tree.        
-000129e0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-000129f0: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
-00012a00: 2041 6464 2063 6c75 7374 6572 696e 6720   Add clustering 
-00012a10: 636f 6c75 6d6e 7320 6261 7365 6420 6f6e  columns based on
-00012a20: 2061 6363 6573 7320 7061 7474 6572 6e73   access patterns
-00012a30: 0a20 2020 2020 2020 206d 6174 6572 6961  .        materia
-00012a40: 6c69 7a65 6420 3d20 7365 6c66 2e5f 6361  lized = self._ca
-00012a50: 6368 655f 7769 7468 5f63 6c75 7374 6572  che_with_cluster
-00012a60: 5f63 6f6c 7328 0a20 2020 2020 2020 2020  _cols(.         
-00012a70: 2020 2063 6f72 652e 4172 7261 7956 616c     core.ArrayVal
-00012a80: 7565 2862 6573 745f 6361 6e64 6964 6174  ue(best_candidat
-00012a90: 655b 305d 292c 205b 5d0a 2020 2020 2020  e[0]), [].      
-00012aa0: 2020 292e 6e6f 6465 0a0a 2020 2020 2020    ).node..      
-00012ab0: 2020 7265 7475 726e 2074 7261 7665 7273    return travers
-00012ac0: 616c 732e 7265 706c 6163 655f 6e6f 6465  als.replace_node
-00012ad0: 7328 0a20 2020 2020 2020 2020 2020 206e  s(.            n
-00012ae0: 6f64 652c 2074 6f5f 7265 706c 6163 653d  ode, to_replace=
-00012af0: 6265 7374 5f63 616e 6469 6461 7465 5b30  best_candidate[0
-00012b00: 5d2c 2072 6570 6c61 6365 6d65 6e65 743d  ], replacemenet=
-00012b10: 6d61 7465 7269 616c 697a 6564 0a20 2020  materialized.   
-00012b20: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00012b30: 5f69 735f 7472 6976 6961 6c6c 795f 6578  _is_trivially_ex
-00012b40: 6563 7574 6162 6c65 2873 656c 662c 2061  ecutable(self, a
-00012b50: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
-00012b60: 2e41 7272 6179 5661 6c75 6529 3a0a 2020  .ArrayValue):.  
-00012b70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012b80: 2020 4361 6e20 7468 6520 626c 6f63 6b20    Can the block 
-00012b90: 6265 2065 7661 6c75 6174 6564 2076 6572  be evaluated ver
-00012ba0: 7920 6368 6561 706c 793f 0a20 2020 2020  y cheaply?.     
-00012bb0: 2020 2049 6620 5472 7565 2c20 7468 6520     If True, the 
-00012bc0: 6172 7261 795f 7661 6c75 6520 7072 6f62  array_value prob
-00012bd0: 6162 6c79 2069 7320 6e6f 7420 776f 7274  ably is not wort
-00012be0: 6820 6361 6368 696e 672e 0a20 2020 2020  h caching..     
-00012bf0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00012c00: 204f 6e63 6520 7265 7772 6974 696e 6720   Once rewriting 
-00012c10: 6973 2061 7661 696c 6162 6c65 2c20 7769  is available, wi
-00012c20: 6c6c 2077 616e 7420 746f 2072 6577 7269  ll want to rewri
-00012c30: 7465 2062 6566 6f72 650a 2020 2020 2020  te before.      
-00012c40: 2020 2320 6576 616c 7561 7469 6e67 2065    # evaluating e
-00012c50: 7865 6375 7469 6f6e 2063 6f73 742e 0a20  xecution cost.. 
-00012c60: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-00012c70: 6176 6572 7361 6c73 2e69 735f 7472 6976  aversals.is_triv
-00012c80: 6961 6c6c 795f 6578 6563 7574 6162 6c65  ially_executable
-00012c90: 2861 7272 6179 5f76 616c 7565 2e6e 6f64  (array_value.nod
-00012ca0: 6529 0a0a 2020 2020 6465 6620 5f65 7865  e)..    def _exe
-00012cb0: 6375 7465 280a 2020 2020 2020 2020 7365  cute(.        se
-00012cc0: 6c66 2c0a 2020 2020 2020 2020 6172 7261  lf,.        arra
-00012cd0: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
-00012ce0: 7261 7956 616c 7565 2c0a 2020 2020 2020  rayValue,.      
-00012cf0: 2020 6a6f 625f 636f 6e66 6967 3a20 4f70    job_config: Op
-00012d00: 7469 6f6e 616c 5b62 6967 7175 6572 792e  tional[bigquery.
-00012d10: 6a6f 622e 5175 6572 794a 6f62 436f 6e66  job.QueryJobConf
-00012d20: 6967 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ig] = None,.    
-00012d30: 2020 2020 2a2c 0a20 2020 2020 2020 2073      *,.        s
-00012d40: 6f72 7465 643a 2062 6f6f 6c20 3d20 5472  orted: bool = Tr
-00012d50: 7565 2c0a 2020 2020 2020 2020 6472 795f  ue,.        dry_
-00012d60: 7275 6e3d 4661 6c73 652c 0a20 2020 2020  run=False,.     
-00012d70: 2020 2063 6f6c 5f69 645f 6f76 6572 7269     col_id_overri
-00012d80: 6465 733a 204d 6170 7069 6e67 5b73 7472  des: Mapping[str
-00012d90: 2c20 7374 725d 203d 207b 7d2c 0a20 2020  , str] = {},.   
-00012da0: 2029 202d 3e20 7475 706c 655b 6269 6771   ) -> tuple[bigq
-00012db0: 7565 7279 2e74 6162 6c65 2e52 6f77 4974  uery.table.RowIt
-00012dc0: 6572 6174 6f72 2c20 6269 6771 7565 7279  erator, bigquery
-00012dd0: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
-00012de0: 2020 2020 7371 6c20 3d20 7365 6c66 2e5f      sql = self._
-00012df0: 746f 5f73 716c 280a 2020 2020 2020 2020  to_sql(.        
-00012e00: 2020 2020 6172 7261 795f 7661 6c75 652c      array_value,
-00012e10: 2073 6f72 7465 643d 736f 7274 6564 2c20   sorted=sorted, 
-00012e20: 636f 6c5f 6964 5f6f 7665 7272 6964 6573  col_id_overrides
-00012e30: 3d63 6f6c 5f69 645f 6f76 6572 7269 6465  =col_id_override
-00012e40: 730a 2020 2020 2020 2020 2920 2023 2074  s.        )  # t
-00012e50: 7970 653a 6967 6e6f 7265 0a20 2020 2020  ype:ignore.     
-00012e60: 2020 2069 6620 6a6f 625f 636f 6e66 6967     if job_config
-00012e70: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00012e80: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00012e90: 203d 2062 6967 7175 6572 792e 5175 6572   = bigquery.Quer
-00012ea0: 794a 6f62 436f 6e66 6967 2864 7279 5f72  yJobConfig(dry_r
-00012eb0: 756e 3d64 7279 5f72 756e 290a 2020 2020  un=dry_run).    
-00012ec0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012ed0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00012ee0: 2e64 7279 5f72 756e 203d 2064 7279 5f72  .dry_run = dry_r
-00012ef0: 756e 0a20 2020 2020 2020 2072 6574 7572  un.        retur
-00012f00: 6e20 7365 6c66 2e5f 7374 6172 745f 7175  n self._start_qu
-00012f10: 6572 7928 0a20 2020 2020 2020 2020 2020  ery(.           
-00012f20: 2073 716c 3d73 716c 2c0a 2020 2020 2020   sql=sql,.      
-00012f30: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00012f40: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
-00012f50: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00012f60: 5f70 6565 6b28 0a20 2020 2020 2020 2073  _peek(.        s
-00012f70: 656c 662c 2061 7272 6179 5f76 616c 7565  elf, array_value
-00012f80: 3a20 636f 7265 2e41 7272 6179 5661 6c75  : core.ArrayValu
-00012f90: 652c 206e 5f72 6f77 733a 2069 6e74 0a20  e, n_rows: int. 
-00012fa0: 2020 2029 202d 3e20 7475 706c 655b 6269     ) -> tuple[bi
-00012fb0: 6771 7565 7279 2e74 6162 6c65 2e52 6f77  gquery.table.Row
-00012fc0: 4974 6572 6174 6f72 2c20 6269 6771 7565  Iterator, bigque
-00012fd0: 7279 2e51 7565 7279 4a6f 625d 3a0a 2020  ry.QueryJob]:.  
-00012fe0: 2020 2020 2020 2222 2241 2027 7065 656b        """A 'peek
-00012ff0: 2720 6566 6669 6369 656e 746c 7920 6163  ' efficiently ac
-00013000: 6365 7373 6573 2061 2073 6d61 6c6c 206e  cesses a small n
-00013010: 756d 6265 7220 6f66 2072 6f77 7320 696e  umber of rows in
-00013020: 2074 6865 2064 6174 6166 7261 6d65 2e22   the dataframe."
-00013030: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00013040: 7420 7472 6565 5f70 726f 7065 7274 6965  t tree_propertie
-00013050: 732e 7065 656b 6162 6c65 2861 7272 6179  s.peekable(array
-00013060: 5f76 616c 7565 2e6e 6f64 6529 3a0a 2020  _value.node):.  
-00013070: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00013080: 6773 2e77 6172 6e28 2250 6565 6b69 6e67  gs.warn("Peeking
-00013090: 2074 6869 7320 7661 6c75 6520 6361 6e6e   this value cann
-000130a0: 6f74 2062 6520 646f 6e65 2065 6666 6963  ot be done effic
-000130b0: 6965 6e74 6c79 2e22 290a 2020 2020 2020  iently.").      
-000130c0: 2020 7371 6c20 3d20 7365 6c66 2e5f 636f    sql = self._co
-000130d0: 6d70 696c 655f 756e 6f72 6465 7265 6428  mpile_unordered(
-000130e0: 6172 7261 795f 7661 6c75 6529 2e70 6565  array_value).pee
-000130f0: 6b5f 7371 6c28 6e5f 726f 7773 290a 2020  k_sql(n_rows).  
-00013100: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00013110: 662e 5f73 7461 7274 5f71 7565 7279 280a  f._start_query(.
-00013120: 2020 2020 2020 2020 2020 2020 7371 6c3d              sql=
-00013130: 7371 6c2c 0a20 2020 2020 2020 2029 0a0a  sql,.        )..
-00013140: 2020 2020 6465 6620 5f74 6f5f 7371 6c28      def _to_sql(
-00013150: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00013160: 2020 2020 2020 2061 7272 6179 5f76 616c         array_val
-00013170: 7565 3a20 636f 7265 2e41 7272 6179 5661  ue: core.ArrayVa
-00013180: 6c75 652c 0a20 2020 2020 2020 206f 6666  lue,.        off
-00013190: 7365 745f 636f 6c75 6d6e 3a20 7479 7069  set_column: typi
-000131a0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-000131b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000131c0: 2063 6f6c 5f69 645f 6f76 6572 7269 6465   col_id_override
-000131d0: 733a 2074 7970 696e 672e 4d61 7070 696e  s: typing.Mappin
-000131e0: 675b 7374 722c 2073 7472 5d20 3d20 7b7d  g[str, str] = {}
-000131f0: 2c0a 2020 2020 2020 2020 736f 7274 6564  ,.        sorted
-00013200: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00013210: 2020 2020 2920 2d3e 2073 7472 3a0a 2020      ) -> str:.  
-00013220: 2020 2020 2020 6966 206f 6666 7365 745f        if offset_
-00013230: 636f 6c75 6d6e 3a0a 2020 2020 2020 2020  column:.        
-00013240: 2020 2020 6172 7261 795f 7661 6c75 6520      array_value 
-00013250: 3d20 6172 7261 795f 7661 6c75 652e 7072  = array_value.pr
-00013260: 6f6d 6f74 655f 6f66 6673 6574 7328 6f66  omote_offsets(of
-00013270: 6673 6574 5f63 6f6c 756d 6e29 0a20 2020  fset_column).   
-00013280: 2020 2020 2069 6620 736f 7274 6564 3a0a       if sorted:.
-00013290: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000132a0: 726e 2073 656c 662e 5f63 6f6d 7069 6c65  rn self._compile
-000132b0: 5f6f 7264 6572 6564 2861 7272 6179 5f76  _ordered(array_v
-000132c0: 616c 7565 292e 746f 5f73 716c 280a 2020  alue).to_sql(.  
-000132d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000132e0: 6c5f 6964 5f6f 7665 7272 6964 6573 3d63  l_id_overrides=c
-000132f0: 6f6c 5f69 645f 6f76 6572 7269 6465 732c  ol_id_overrides,
-00013300: 2073 6f72 7465 643d 5472 7565 0a20 2020   sorted=True.   
-00013310: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00013320: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00013330: 636f 6d70 696c 655f 756e 6f72 6465 7265  compile_unordere
-00013340: 6428 6172 7261 795f 7661 6c75 6529 2e74  d(array_value).t
-00013350: 6f5f 7371 6c28 0a20 2020 2020 2020 2020  o_sql(.         
-00013360: 2020 2063 6f6c 5f69 645f 6f76 6572 7269     col_id_overri
-00013370: 6465 733d 636f 6c5f 6964 5f6f 7665 7272  des=col_id_overr
-00013380: 6964 6573 0a20 2020 2020 2020 2029 0a0a  ides.        )..
-00013390: 2020 2020 6465 6620 5f63 6f6d 7069 6c65      def _compile
-000133a0: 5f6f 7264 6572 6564 280a 2020 2020 2020  _ordered(.      
-000133b0: 2020 7365 6c66 2c20 6172 7261 795f 7661    self, array_va
-000133c0: 6c75 653a 2063 6f72 652e 4172 7261 7956  lue: core.ArrayV
-000133d0: 616c 7565 0a20 2020 2029 202d 3e20 6269  alue.    ) -> bi
-000133e0: 6766 7261 6d65 732e 636f 7265 2e63 6f6d  gframes.core.com
-000133f0: 7069 6c65 2e4f 7264 6572 6564 4952 3a0a  pile.OrderedIR:.
-00013400: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00013410: 6967 6672 616d 6573 2e63 6f72 652e 636f  igframes.core.co
-00013420: 6d70 696c 652e 636f 6d70 696c 655f 6f72  mpile.compile_or
-00013430: 6465 7265 645f 6972 2861 7272 6179 5f76  dered_ir(array_v
-00013440: 616c 7565 2e6e 6f64 6529 0a0a 2020 2020  alue.node)..    
-00013450: 6465 6620 5f63 6f6d 7069 6c65 5f75 6e6f  def _compile_uno
-00013460: 7264 6572 6564 280a 2020 2020 2020 2020  rdered(.        
-00013470: 7365 6c66 2c20 6172 7261 795f 7661 6c75  self, array_valu
-00013480: 653a 2063 6f72 652e 4172 7261 7956 616c  e: core.ArrayVal
-00013490: 7565 0a20 2020 2029 202d 3e20 6269 6766  ue.    ) -> bigf
-000134a0: 7261 6d65 732e 636f 7265 2e63 6f6d 7069  rames.core.compi
-000134b0: 6c65 2e55 6e6f 7264 6572 6564 4952 3a0a  le.UnorderedIR:.
-000134c0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-000134d0: 6967 6672 616d 6573 2e63 6f72 652e 636f  igframes.core.co
-000134e0: 6d70 696c 652e 636f 6d70 696c 655f 756e  mpile.compile_un
-000134f0: 6f72 6465 7265 645f 6972 2861 7272 6179  ordered_ir(array
-00013500: 5f76 616c 7565 2e6e 6f64 6529 0a0a 2020  _value.node)..  
-00013510: 2020 6465 6620 5f67 6574 5f74 6162 6c65    def _get_table
-00013520: 5f73 697a 6528 7365 6c66 2c20 6465 7374  _size(self, dest
-00013530: 696e 6174 696f 6e5f 7461 626c 6529 3a0a  ination_table):.
-00013540: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-00013550: 7365 6c66 2e62 7163 6c69 656e 742e 6765  self.bqclient.ge
-00013560: 745f 7461 626c 6528 6465 7374 696e 6174  t_table(destinat
-00013570: 696f 6e5f 7461 626c 6529 0a20 2020 2020  ion_table).     
-00013580: 2020 2072 6574 7572 6e20 7461 626c 652e     return table.
-00013590: 6e75 6d5f 6279 7465 730a 0a20 2020 2064  num_bytes..    d
-000135a0: 6566 205f 726f 7773 5f74 6f5f 6461 7461  ef _rows_to_data
-000135b0: 6672 616d 6528 0a20 2020 2020 2020 2073  frame(.        s
-000135c0: 656c 662c 2072 6f77 5f69 7465 7261 746f  elf, row_iterato
-000135d0: 723a 2062 6967 7175 6572 792e 7461 626c  r: bigquery.tabl
-000135e0: 652e 526f 7749 7465 7261 746f 722c 2064  e.RowIterator, d
-000135f0: 7479 7065 733a 2044 6963 740a 2020 2020  types: Dict.    
-00013600: 2920 2d3e 2070 616e 6461 732e 4461 7461  ) -> pandas.Data
-00013610: 4672 616d 653a 0a20 2020 2020 2020 2023  Frame:.        #
-00013620: 2043 616e 2069 676e 6f72 6520 696e 6665   Can ignore infe
-00013630: 7272 6564 2064 6174 6174 7970 6520 756e  rred datatype un
-00013640: 7469 6c20 6474 7970 6520 656d 756c 6174  til dtype emulat
-00013650: 696f 6e20 6272 6561 6b73 2031 3a31 206d  ion breaks 1:1 m
-00013660: 6170 7069 6e67 2062 6574 7765 656e 2042  apping between B
-00013670: 5120 7479 7065 7320 616e 6420 6269 6766  Q types and bigf
-00013680: 7261 6d65 7320 7479 7065 730a 2020 2020  rames types.    
-00013690: 2020 2020 6474 7970 6573 5f66 726f 6d5f      dtypes_from_
-000136a0: 6271 203d 2062 6967 6672 616d 6573 2e64  bq = bigframes.d
-000136b0: 7479 7065 732e 6266 5f74 7970 655f 6672  types.bf_type_fr
-000136c0: 6f6d 5f74 7970 655f 6b69 6e64 2872 6f77  om_type_kind(row
-000136d0: 5f69 7465 7261 746f 722e 7363 6865 6d61  _iterator.schema
-000136e0: 290a 2020 2020 2020 2020 6172 726f 775f  ).        arrow_
-000136f0: 7461 626c 6520 3d20 726f 775f 6974 6572  table = row_iter
-00013700: 6174 6f72 2e74 6f5f 6172 726f 7728 290a  ator.to_arrow().
-00013710: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00013720: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
-00013730: 2e5f 696f 2e70 616e 6461 732e 6172 726f  ._io.pandas.arro
-00013740: 775f 746f 5f70 616e 6461 7328 6172 726f  w_to_pandas(arro
-00013750: 775f 7461 626c 652c 2064 7479 7065 735f  w_table, dtypes_
-00013760: 6672 6f6d 5f62 7129 0a0a 2020 2020 6465  from_bq)..    de
-00013770: 6620 5f73 7461 7274 5f67 656e 6572 6963  f _start_generic
-00013780: 5f6a 6f62 2873 656c 662c 206a 6f62 3a20  _job(self, job: 
-00013790: 666f 726d 6174 7469 6e67 5f68 656c 7065  formatting_helpe
-000137a0: 7273 2e47 656e 6572 6963 4a6f 6229 3a0a  rs.GenericJob):.
-000137b0: 2020 2020 2020 2020 6966 2062 6967 6672          if bigfr
-000137c0: 616d 6573 2e6f 7074 696f 6e73 2e64 6973  ames.options.dis
-000137d0: 706c 6179 2e70 726f 6772 6573 735f 6261  play.progress_ba
-000137e0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-000137f0: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
-00013800: 7474 696e 675f 6865 6c70 6572 732e 7761  tting_helpers.wa
-00013810: 6974 5f66 6f72 5f6a 6f62 280a 2020 2020  it_for_job(.    
-00013820: 2020 2020 2020 2020 2020 2020 6a6f 622c              job,
-00013830: 2062 6967 6672 616d 6573 2e6f 7074 696f   bigframes.optio
-00013840: 6e73 2e64 6973 706c 6179 2e70 726f 6772  ns.display.progr
-00013850: 6573 735f 6261 720a 2020 2020 2020 2020  ess_bar.        
-00013860: 2020 2020 2920 2023 2057 6169 7420 666f      )  # Wait fo
-00013870: 7220 7468 6520 6a6f 6220 746f 2063 6f6d  r the job to com
-00013880: 706c 6574 650a 2020 2020 2020 2020 656c  plete.        el
-00013890: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000138a0: 6a6f 622e 7265 7375 6c74 2829 0a0a 0a64  job.result()...d
-000138b0: 6566 2063 6f6e 6e65 6374 2863 6f6e 7465  ef connect(conte
-000138c0: 7874 3a20 4f70 7469 6f6e 616c 5b62 6967  xt: Optional[big
-000138d0: 7175 6572 795f 6f70 7469 6f6e 732e 4269  query_options.Bi
-000138e0: 6751 7565 7279 4f70 7469 6f6e 735d 203d  gQueryOptions] =
-000138f0: 204e 6f6e 6529 202d 3e20 5365 7373 696f   None) -> Sessio
-00013900: 6e3a 0a20 2020 2072 6574 7572 6e20 5365  n:.    return Se
-00013910: 7373 696f 6e28 636f 6e74 6578 7429 0a0a  ssion(context)..
-00013920: 0a64 6566 205f 6361 6e5f 636c 7573 7465  .def _can_cluste
-00013930: 725f 6271 2866 6965 6c64 3a20 6269 6771  r_bq(field: bigq
-00013940: 7565 7279 2e53 6368 656d 6146 6965 6c64  uery.SchemaField
-00013950: 293a 0a20 2020 2023 2068 7474 7073 3a2f  ):.    # https:/
-00013960: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-00013970: 6d2f 6269 6771 7565 7279 2f64 6f63 732f  m/bigquery/docs/
-00013980: 636c 7573 7465 7265 642d 7461 626c 6573  clustered-tables
-00013990: 0a20 2020 2023 204e 6f74 6162 6c79 2c20  .    # Notably, 
-000139a0: 666c 6f61 7420 6973 2065 7863 6c75 6465  float is exclude
-000139b0: 640a 2020 2020 7479 7065 5f20 3d20 6669  d.    type_ = fi
-000139c0: 656c 642e 6669 656c 645f 7479 7065 0a20  eld.field_type. 
-000139d0: 2020 2072 6574 7572 6e20 7479 7065 5f20     return type_ 
-000139e0: 696e 2028 0a20 2020 2020 2020 2022 494e  in (.        "IN
-000139f0: 5445 4745 5222 2c0a 2020 2020 2020 2020  TEGER",.        
-00013a00: 2249 4e54 3634 222c 0a20 2020 2020 2020  "INT64",.       
-00013a10: 2022 5354 5249 4e47 222c 0a20 2020 2020   "STRING",.     
-00013a20: 2020 2022 4e55 4d45 5249 4322 2c0a 2020     "NUMERIC",.  
-00013a30: 2020 2020 2020 2244 4543 494d 414c 222c        "DECIMAL",
-00013a40: 0a20 2020 2020 2020 2022 4249 474e 554d  .        "BIGNUM
-00013a50: 4552 4943 222c 0a20 2020 2020 2020 2022  ERIC",.        "
-00013a60: 4249 4744 4543 494d 414c 222c 0a20 2020  BIGDECIMAL",.   
-00013a70: 2020 2020 2022 4441 5445 222c 0a20 2020       "DATE",.   
-00013a80: 2020 2020 2022 4441 5445 5449 4d45 222c       "DATETIME",
-00013a90: 0a20 2020 2020 2020 2022 5449 4d45 5354  .        "TIMEST
-00013aa0: 414d 5022 2c0a 2020 2020 2020 2020 2242  AMP",.        "B
-00013ab0: 4f4f 4c22 2c0a 2020 2020 2020 2020 2242  OOL",.        "B
-00013ac0: 4f4f 4c45 414e 222c 0a20 2020 2029 0a0a  OOLEAN",.    )..
-00013ad0: 0a64 6566 205f 636f 6e76 6572 745f 746f  .def _convert_to
-00013ae0: 5f6e 6f6e 6e75 6c6c 5f73 7472 696e 6728  _nonnull_string(
-00013af0: 636f 6c75 6d6e 3a20 6962 6973 5f74 7970  column: ibis_typ
-00013b00: 6573 2e43 6f6c 756d 6e29 202d 3e20 6962  es.Column) -> ib
-00013b10: 6973 5f74 7970 6573 2e53 7472 696e 6756  is_types.StringV
-00013b20: 616c 7565 3a0a 2020 2020 636f 6c5f 7479  alue:.    col_ty
-00013b30: 7065 203d 2063 6f6c 756d 6e2e 7479 7065  pe = column.type
-00013b40: 2829 0a20 2020 2069 6620 280a 2020 2020  ().    if (.    
-00013b50: 2020 2020 636f 6c5f 7479 7065 2e69 735f      col_type.is_
-00013b60: 6e75 6d65 7269 6328 290a 2020 2020 2020  numeric().      
-00013b70: 2020 6f72 2063 6f6c 5f74 7970 652e 6973    or col_type.is
-00013b80: 5f62 6f6f 6c65 616e 2829 0a20 2020 2020  _boolean().     
-00013b90: 2020 206f 7220 636f 6c5f 7479 7065 2e69     or col_type.i
-00013ba0: 735f 6269 6e61 7279 2829 0a20 2020 2020  s_binary().     
-00013bb0: 2020 206f 7220 636f 6c5f 7479 7065 2e69     or col_type.i
-00013bc0: 735f 7465 6d70 6f72 616c 2829 0a20 2020  s_temporal().   
-00013bd0: 2029 3a0a 2020 2020 2020 2020 7265 7375   ):.        resu
-00013be0: 6c74 203d 2063 6f6c 756d 6e2e 6361 7374  lt = column.cast
-00013bf0: 2869 6269 735f 6474 7970 6573 2e53 7472  (ibis_dtypes.Str
-00013c00: 696e 6728 6e75 6c6c 6162 6c65 3d54 7275  ing(nullable=Tru
-00013c10: 6529 290a 2020 2020 656c 6966 2063 6f6c  e)).    elif col
-00013c20: 5f74 7970 652e 6973 5f67 656f 7370 6174  _type.is_geospat
-00013c30: 6961 6c28 293a 0a20 2020 2020 2020 2072  ial():.        r
-00013c40: 6573 756c 7420 3d20 7479 7069 6e67 2e63  esult = typing.c
-00013c50: 6173 7428 6962 6973 5f74 7970 6573 2e47  ast(ibis_types.G
-00013c60: 656f 5370 6174 6961 6c43 6f6c 756d 6e2c  eoSpatialColumn,
-00013c70: 2063 6f6c 756d 6e29 2e61 735f 7465 7874   column).as_text
-00013c80: 2829 0a20 2020 2065 6c69 6620 636f 6c5f  ().    elif col_
-00013c90: 7479 7065 2e69 735f 7374 7269 6e67 2829  type.is_string()
-00013ca0: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
-00013cb0: 203d 2063 6f6c 756d 6e0a 2020 2020 656c   = column.    el
-00013cc0: 7365 3a0a 2020 2020 2020 2020 2320 544f  se:.        # TO
-00013cd0: 5f4a 534f 4e5f 5354 5249 4e47 2077 6f72  _JSON_STRING wor
-00013ce0: 6b73 2077 6974 6820 616c 6c20 6461 7461  ks with all data
-00013cf0: 2074 7970 6573 2c20 6275 7420 6973 6e27   types, but isn'
-00013d00: 7420 7468 6520 6d6f 7374 2065 6666 6963  t the most effic
-00013d10: 6965 6e74 0a20 2020 2020 2020 2023 204e  ient.        # N
-00013d20: 6565 6465 6420 666f 7220 4a53 4f4e 2c20  eeded for JSON, 
-00013d30: 5354 5255 4354 2061 6e64 2041 5252 4159  STRUCT and ARRAY
-00013d40: 2064 6174 6174 7970 6573 0a20 2020 2020   datatypes.     
-00013d50: 2020 2072 6573 756c 7420 3d20 7665 6e64     result = vend
-00013d60: 6f72 6564 5f69 6269 735f 6f70 732e 546f  ored_ibis_ops.To
-00013d70: 4a73 6f6e 5374 7269 6e67 2863 6f6c 756d  JsonString(colum
-00013d80: 6e29 2e74 6f5f 6578 7072 2829 2020 2320  n).to_expr()  # 
-00013d90: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-00013da0: 2023 2045 7363 6170 6520 6261 636b 736c   # Escape backsl
-00013db0: 6173 6865 7320 616e 6420 7573 6520 6261  ashes and use ba
-00013dc0: 636b 736c 6173 6820 6173 2064 656c 696e  ckslash as delin
-00013dd0: 6561 746f 720a 2020 2020 6573 6361 7065  eator.    escape
-00013de0: 6420 3d20 7479 7069 6e67 2e63 6173 7428  d = typing.cast(
-00013df0: 6962 6973 5f74 7970 6573 2e53 7472 696e  ibis_types.Strin
-00013e00: 6743 6f6c 756d 6e2c 2072 6573 756c 742e  gColumn, result.
-00013e10: 6669 6c6c 6e61 2822 2229 292e 7265 706c  fillna("")).repl
-00013e20: 6163 6528 225c 5c22 2c20 225c 5c5c 5c22  ace("\\", "\\\\"
-00013e30: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
-00013e40: 650a 2020 2020 7265 7475 726e 2074 7970  e.    return typ
-00013e50: 696e 672e 6361 7374 2869 6269 735f 7479  ing.cast(ibis_ty
-00013e60: 7065 732e 5374 7269 6e67 436f 6c75 6d6e  pes.StringColumn
-00013e70: 2c20 6962 6973 2e6c 6974 6572 616c 2822  , ibis.literal("
-00013e80: 5c5c 2229 292e 636f 6e63 6174 2865 7363  \\")).concat(esc
-00013e90: 6170 6564 290a 0a0a 6465 6620 5f74 7261  aped)...def _tra
-00013ea0: 6e73 666f 726d 5f72 6561 645f 6762 715f  nsform_read_gbq_
-00013eb0: 636f 6e66 6967 7572 6174 696f 6e28 636f  configuration(co
-00013ec0: 6e66 6967 7572 6174 696f 6e3a 204f 7074  nfiguration: Opt
-00013ed0: 696f 6e61 6c5b 6469 6374 5d29 202d 3e20  ional[dict]) -> 
-00013ee0: 6469 6374 3a0a 2020 2020 2222 220a 2020  dict:.    """.  
-00013ef0: 2020 466f 7220 6261 636b 7761 7264 732d    For backwards-
-00013f00: 636f 6d70 6174 6962 696c 6974 792c 2063  compatibility, c
-00013f10: 6f6e 7665 7274 2061 6e79 2070 7265 7669  onvert any previ
-00013f20: 6f75 736c 7920 636c 6965 6e74 2d73 6964  ously client-sid
-00013f30: 6520 6f6e 6c79 0a20 2020 2070 6172 616d  e only.    param
-00013f40: 6574 6572 7320 7375 6368 2061 7320 7469  eters such as ti
-00013f50: 6d65 6f75 744d 7320 746f 2074 6865 2070  meoutMs to the p
-00013f60: 726f 7065 7274 7920 6e61 6d65 2065 7870  roperty name exp
-00013f70: 6563 7465 6420 6279 2074 6865 2052 4553  ected by the RES
-00013f80: 5420 4150 492e 0a0a 2020 2020 4d61 6b65  T API...    Make
-00013f90: 7320 6120 636f 7079 206f 6620 636f 6e66  s a copy of conf
-00013fa0: 6967 7572 6174 696f 6e20 6966 2063 6861  iguration if cha
-00013fb0: 6e67 6573 2061 7265 206e 6565 6465 642e  nges are needed.
-00013fc0: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
-00013fd0: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
-00013fe0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00013ff0: 7265 7475 726e 207b 7d0a 0a20 2020 2074  return {}..    t
-00014000: 696d 656f 7574 5f6d 7320 3d20 636f 6e66  imeout_ms = conf
-00014010: 6967 7572 6174 696f 6e2e 6765 7428 2271  iguration.get("q
-00014020: 7565 7279 222c 207b 7d29 2e67 6574 2822  uery", {}).get("
-00014030: 7469 6d65 6f75 744d 7322 290a 2020 2020  timeoutMs").    
-00014040: 6966 2074 696d 656f 7574 5f6d 7320 6973  if timeout_ms is
-00014050: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00014060: 2020 2023 2054 7261 6e73 666f 726d 2074     # Transform t
-00014070: 696d 656f 7574 4d73 2074 6f20 616e 2061  imeoutMs to an a
-00014080: 6374 7561 6c20 7365 7276 6572 2d73 6964  ctual server-sid
-00014090: 6520 636f 6e66 6967 7572 6174 696f 6e2e  e configuration.
-000140a0: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
-000140b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
-000140c0: 6f67 6c65 6170 6973 2f70 7974 686f 6e2d  ogleapis/python-
-000140d0: 6269 6771 7565 7279 2d70 616e 6461 732f  bigquery-pandas/
-000140e0: 6973 7375 6573 2f34 3739 0a20 2020 2020  issues/479.     
-000140f0: 2020 2063 6f6e 6669 6775 7261 7469 6f6e     configuration
-00014100: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-00014110: 2863 6f6e 6669 6775 7261 7469 6f6e 290a  (configuration).
-00014120: 2020 2020 2020 2020 6465 6c20 636f 6e66          del conf
-00014130: 6967 7572 6174 696f 6e5b 2271 7565 7279  iguration["query
-00014140: 225d 5b22 7469 6d65 6f75 744d 7322 5d0a  "]["timeoutMs"].
-00014150: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-00014160: 6174 696f 6e5b 226a 6f62 5469 6d65 6f75  ation["jobTimeou
-00014170: 744d 7322 5d20 3d20 7469 6d65 6f75 745f  tMs"] = timeout_
-00014180: 6d73 0a0a 2020 2020 7265 7475 726e 2063  ms..    return c
-00014190: 6f6e 6669 6775 7261 7469 6f6e 0a         onfiguration.
+0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf00: 206f 7269 656e 743d 6f72 6965 6e74 2c0a   orient=orient,.
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf20: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
+0000cf30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf40: 2020 2020 2065 6e63 6f64 696e 673d 656e       encoding=en
+0000cf50: 636f 6469 6e67 2c0a 2020 2020 2020 2020  coding,.        
+0000cf60: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000cf70: 733d 6c69 6e65 732c 0a20 2020 2020 2020  s=lines,.       
+0000cf80: 2020 2020 2020 2020 2020 2020 2065 6e67               eng
+0000cf90: 696e 653d 656e 6769 6e65 2c0a 2020 2020  ine=engine,.    
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
+0000cfc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000cfd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000cfe0: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
+0000cff0: 2870 616e 6461 735f 6466 2c20 2272 6561  (pandas_df, "rea
+0000d000: 645f 6a73 6f6e 2229 0a0a 2020 2020 6465  d_json")..    de
+0000d010: 6620 5f63 6865 636b 5f66 696c 655f 7369  f _check_file_si
+0000d020: 7a65 2873 656c 662c 2066 696c 6570 6174  ze(self, filepat
+0000d030: 683a 2073 7472 293a 0a20 2020 2020 2020  h: str):.       
+0000d040: 206d 6178 5f73 697a 6520 3d20 3130 3234   max_size = 1024
+0000d050: 202a 2031 3032 3420 2a20 3130 3234 2020   * 1024 * 1024  
+0000d060: 2320 3120 4742 2069 6e20 6279 7465 730a  # 1 GB in bytes.
+0000d070: 2020 2020 2020 2020 6966 2066 696c 6570          if filep
+0000d080: 6174 682e 7374 6172 7473 7769 7468 2822  ath.startswith("
+0000d090: 6773 3a2f 2f22 293a 2020 2320 4743 5320  gs://"):  # GCS 
+0000d0a0: 6669 6c65 2070 6174 680a 2020 2020 2020  file path.      
+0000d0b0: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
+0000d0c0: 746f 7261 6765 2e43 6c69 656e 7428 290a  torage.Client().
+0000d0d0: 2020 2020 2020 2020 2020 2020 6275 636b              buck
+0000d0e0: 6574 5f6e 616d 652c 2062 6c6f 625f 6e61  et_name, blob_na
+0000d0f0: 6d65 203d 2066 696c 6570 6174 682e 7370  me = filepath.sp
+0000d100: 6c69 7428 222f 222c 2033 295b 323a 5d0a  lit("/", 3)[2:].
+0000d110: 2020 2020 2020 2020 2020 2020 6275 636b              buck
+0000d120: 6574 203d 2063 6c69 656e 742e 6275 636b  et = client.buck
+0000d130: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+0000d140: 2020 2020 2020 2020 2020 2020 626c 6f62              blob
+0000d150: 203d 2062 7563 6b65 742e 626c 6f62 2862   = bucket.blob(b
+0000d160: 6c6f 625f 6e61 6d65 290a 2020 2020 2020  lob_name).      
+0000d170: 2020 2020 2020 626c 6f62 2e72 656c 6f61        blob.reloa
+0000d180: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+0000d190: 6669 6c65 5f73 697a 6520 3d20 626c 6f62  file_size = blob
+0000d1a0: 2e73 697a 650a 2020 2020 2020 2020 656c  .size.        el
+0000d1b0: 7365 3a20 2023 206c 6f63 616c 2066 696c  se:  # local fil
+0000d1c0: 6520 7061 7468 0a20 2020 2020 2020 2020  e path.         
+0000d1d0: 2020 2066 696c 655f 7369 7a65 203d 206f     file_size = o
+0000d1e0: 732e 7061 7468 2e67 6574 7369 7a65 2866  s.path.getsize(f
+0000d1f0: 696c 6570 6174 6829 0a0a 2020 2020 2020  ilepath)..      
+0000d200: 2020 6966 2066 696c 655f 7369 7a65 203e    if file_size >
+0000d210: 206d 6178 5f73 697a 653a 0a20 2020 2020   max_size:.     
+0000d220: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+0000d230: 2074 6f20 4742 0a20 2020 2020 2020 2020   to GB.         
+0000d240: 2020 2066 696c 655f 7369 7a65 203d 2072     file_size = r
+0000d250: 6f75 6e64 2866 696c 655f 7369 7a65 202f  ound(file_size /
+0000d260: 2028 3130 3234 2a2a 3329 2c20 3129 0a20   (1024**3), 1). 
+0000d270: 2020 2020 2020 2020 2020 206d 6178 5f73             max_s
+0000d280: 697a 6520 3d20 696e 7428 6d61 785f 7369  ize = int(max_si
+0000d290: 7a65 202f 2031 3032 342a 2a33 290a 2020  ze / 1024**3).  
+0000d2a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000d2b0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+0000d2c0: 2020 2020 2020 2020 2020 6622 4669 6c65            f"File
+0000d2d0: 2073 697a 6520 7b66 696c 655f 7369 7a65   size {file_size
+0000d2e0: 7d47 4220 6578 6365 6564 7320 7b6d 6178  }GB exceeds {max
+0000d2f0: 5f73 697a 657d 4742 2e20 220a 2020 2020  _size}GB. ".    
+0000d300: 2020 2020 2020 2020 2020 2020 2249 7420              "It 
+0000d310: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+0000d320: 6f20 7573 6520 656e 6769 6e65 3d27 6269  o use engine='bi
+0000d330: 6771 7565 7279 2720 220a 2020 2020 2020  gquery' ".      
+0000d340: 2020 2020 2020 2020 2020 2266 6f72 206c            "for l
+0000d350: 6172 6765 2066 696c 6573 2074 6f20 6176  arge files to av
+0000d360: 6f69 6420 6c6f 6164 696e 6720 7468 6520  oid loading the 
+0000d370: 6669 6c65 2069 6e74 6f20 6c6f 6361 6c20  file into local 
+0000d380: 6d65 6d6f 7279 2e22 0a20 2020 2020 2020  memory.".       
+0000d390: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0000d3a0: 5f63 7265 6174 655f 656d 7074 795f 7465  _create_empty_te
+0000d3b0: 6d70 5f74 6162 6c65 280a 2020 2020 2020  mp_table(.      
+0000d3c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000d3d0: 7363 6865 6d61 3a20 4974 6572 6162 6c65  schema: Iterable
+0000d3e0: 5b62 6967 7175 6572 792e 5363 6865 6d61  [bigquery.Schema
+0000d3f0: 4669 656c 645d 2c0a 2020 2020 2020 2020  Field],.        
+0000d400: 636c 7573 7465 725f 636f 6c73 3a20 4c69  cluster_cols: Li
+0000d410: 7374 5b73 7472 5d2c 0a20 2020 2029 202d  st[str],.    ) -
+0000d420: 3e20 6269 6771 7565 7279 2e54 6162 6c65  > bigquery.Table
+0000d430: 5265 6665 7265 6e63 653a 0a20 2020 2020  Reference:.     
+0000d440: 2020 2023 2043 616e 2774 2073 6574 2061     # Can't set a
+0000d450: 2074 6162 6c65 2069 6e20 5f53 4553 5349   table in _SESSI
+0000d460: 4f4e 2061 7320 6465 7374 696e 6174 696f  ON as destinatio
+0000d470: 6e20 7669 6120 7175 6572 7920 6a6f 6220  n via query job 
+0000d480: 4150 492c 2073 6f20 7765 0a20 2020 2020  API, so we.     
+0000d490: 2020 2023 2072 756e 2044 444c 2c20 696e     # run DDL, in
+0000d4a0: 7374 6561 642e 0a20 2020 2020 2020 2064  stead..        d
+0000d4b0: 6174 6173 6574 203d 2073 656c 662e 5f61  ataset = self._a
+0000d4c0: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
+0000d4d0: 0a20 2020 2020 2020 2065 7870 6972 6174  .        expirat
+0000d4e0: 696f 6e20 3d20 280a 2020 2020 2020 2020  ion = (.        
+0000d4f0: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
+0000d500: 6574 696d 652e 6e6f 7728 6461 7465 7469  etime.now(dateti
+0000d510: 6d65 2e74 696d 657a 6f6e 652e 7574 6329  me.timezone.utc)
+0000d520: 202b 2063 6f6e 7374 616e 7473 2e44 4546   + constants.DEF
+0000d530: 4155 4c54 5f45 5850 4952 4154 494f 4e0a  AULT_EXPIRATION.
+0000d540: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000d550: 2020 2074 6162 6c65 203d 2062 6967 6672     table = bigfr
+0000d560: 616d 6573 5f69 6f2e 6372 6561 7465 5f74  ames_io.create_t
+0000d570: 656d 705f 7461 626c 6528 0a20 2020 2020  emp_table(.     
+0000d580: 2020 2020 2020 2073 656c 662e 6271 636c         self.bqcl
+0000d590: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
+0000d5a0: 2020 6461 7461 7365 742c 0a20 2020 2020    dataset,.     
+0000d5b0: 2020 2020 2020 2065 7870 6972 6174 696f         expiratio
+0000d5c0: 6e2c 0a20 2020 2020 2020 2020 2020 2073  n,.            s
+0000d5d0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
+0000d5e0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
+0000d5f0: 725f 636f 6c75 6d6e 733d 636c 7573 7465  r_columns=cluste
+0000d600: 725f 636f 6c73 2c0a 2020 2020 2020 2020  r_cols,.        
+0000d610: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d620: 2062 6967 7175 6572 792e 5461 626c 6552   bigquery.TableR
+0000d630: 6566 6572 656e 6365 2e66 726f 6d5f 7374  eference.from_st
+0000d640: 7269 6e67 2874 6162 6c65 290a 0a20 2020  ring(table)..   
+0000d650: 2064 6566 205f 6372 6561 7465 5f74 6f74   def _create_tot
+0000d660: 616c 5f6f 7264 6572 696e 6728 0a20 2020  al_ordering(.   
+0000d670: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000d680: 2020 2074 6162 6c65 3a20 6962 6973 5f74     table: ibis_t
+0000d690: 7970 6573 2e54 6162 6c65 2c0a 2020 2020  ypes.Table,.    
+0000d6a0: 2020 2020 7461 626c 655f 726f 7773 3a20      table_rows: 
+0000d6b0: 4f70 7469 6f6e 616c 5b69 6e74 5d2c 0a20  Optional[int],. 
+0000d6c0: 2020 2029 202d 3e20 636f 7265 2e41 7272     ) -> core.Arr
+0000d6d0: 6179 5661 6c75 653a 0a20 2020 2020 2020  ayValue:.       
+0000d6e0: 2023 2053 696e 6365 2074 6869 7320 6d69   # Since this mi
+0000d6f0: 6768 7420 616c 736f 2062 6520 7573 6564  ght also be used
+0000d700: 2061 7320 7468 6520 696e 6465 782c 2064   as the index, d
+0000d710: 6f6e 2774 2075 7365 2074 6865 2064 6566  on't use the def
+0000d720: 6175 6c74 0a20 2020 2020 2020 2023 2022  ault.        # "
+0000d730: 6f72 6465 7269 6e67 2049 4422 206e 616d  ordering ID" nam
+0000d740: 652e 0a0a 2020 2020 2020 2020 2320 466f  e...        # Fo
+0000d750: 7220 736d 616c 6c20 7461 626c 6573 2c20  r small tables, 
+0000d760: 3634 2062 6974 7320 6973 2065 6e6f 7567  64 bits is enoug
+0000d770: 6820 746f 2061 766f 6964 2063 6f6c 6c69  h to avoid colli
+0000d780: 7369 6f6e 732c 2031 3238 2062 6974 7320  sions, 128 bits 
+0000d790: 7769 6c6c 206e 6576 6572 2065 7665 7220  will never ever 
+0000d7a0: 636f 6c6c 6964 6520 6e6f 206d 6174 7465  collide no matte
+0000d7b0: 7220 7768 6174 0a20 2020 2020 2020 2023  r what.        #
+0000d7c0: 2041 7373 756d 6520 7461 626c 6520 6973   Assume table is
+0000d7d0: 206c 6172 6765 2069 6620 7461 626c 6520   large if table 
+0000d7e0: 726f 7720 636f 756e 7420 6973 2075 6e6b  row count is unk
+0000d7f0: 6e6f 776e 0a20 2020 2020 2020 2075 7365  nown.        use
+0000d800: 5f64 6f75 626c 655f 6861 7368 203d 2028  _double_hash = (
+0000d810: 0a20 2020 2020 2020 2020 2020 2028 7461  .            (ta
+0000d820: 626c 655f 726f 7773 2069 7320 4e6f 6e65  ble_rows is None
+0000d830: 2920 6f72 2028 7461 626c 655f 726f 7773  ) or (table_rows
+0000d840: 203d 3d20 3029 206f 7220 2874 6162 6c65   == 0) or (table
+0000d850: 5f72 6f77 7320 3e20 3130 3030 3030 290a  _rows > 100000).
+0000d860: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000d870: 2020 206f 7264 6572 696e 675f 6861 7368     ordering_hash
+0000d880: 5f70 6172 7420 3d20 6775 6964 2e67 656e  _part = guid.gen
+0000d890: 6572 6174 655f 6775 6964 2822 6269 6766  erate_guid("bigf
+0000d8a0: 7261 6d65 735f 6f72 6465 7269 6e67 5f22  rames_ordering_"
+0000d8b0: 290a 2020 2020 2020 2020 6f72 6465 7269  ).        orderi
+0000d8c0: 6e67 5f68 6173 685f 7061 7274 3220 3d20  ng_hash_part2 = 
+0000d8d0: 6775 6964 2e67 656e 6572 6174 655f 6775  guid.generate_gu
+0000d8e0: 6964 2822 6269 6766 7261 6d65 735f 6f72  id("bigframes_or
+0000d8f0: 6465 7269 6e67 5f22 290a 2020 2020 2020  dering_").      
+0000d900: 2020 6f72 6465 7269 6e67 5f72 616e 645f    ordering_rand_
+0000d910: 7061 7274 203d 2067 7569 642e 6765 6e65  part = guid.gene
+0000d920: 7261 7465 5f67 7569 6428 2262 6967 6672  rate_guid("bigfr
+0000d930: 616d 6573 5f6f 7264 6572 696e 675f 2229  ames_ordering_")
+0000d940: 0a0a 2020 2020 2020 2020 2320 416c 6c20  ..        # All 
+0000d950: 696e 7075 7473 2069 6e74 6f20 6861 7368  inputs into hash
+0000d960: 206d 7573 7420 6265 206e 6f6e 2d6e 756c   must be non-nul
+0000d970: 6c20 6f72 2072 6573 756c 7469 6e67 2068  l or resulting h
+0000d980: 6173 6820 7769 6c6c 2062 6520 6e75 6c6c  ash will be null
+0000d990: 0a20 2020 2020 2020 2073 7472 5f76 616c  .        str_val
+0000d9a0: 7565 7320 3d20 6c69 7374 280a 2020 2020  ues = list(.    
+0000d9b0: 2020 2020 2020 2020 6d61 7028 6c61 6d62          map(lamb
+0000d9c0: 6461 2063 6f6c 3a20 5f63 6f6e 7665 7274  da col: _convert
+0000d9d0: 5f74 6f5f 6e6f 6e6e 756c 6c5f 7374 7269  _to_nonnull_stri
+0000d9e0: 6e67 2874 6162 6c65 5b63 6f6c 5d29 2c20  ng(table[col]), 
+0000d9f0: 7461 626c 652e 636f 6c75 6d6e 7329 0a20  table.columns). 
+0000da00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000da10: 2066 756c 6c5f 726f 775f 7374 7220 3d20   full_row_str = 
+0000da20: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
+0000da30: 725f 7661 6c75 6573 5b30 5d2e 636f 6e63  r_values[0].conc
+0000da40: 6174 282a 7374 725f 7661 6c75 6573 5b31  at(*str_values[1
+0000da50: 3a5d 290a 2020 2020 2020 2020 2020 2020  :]).            
+0000da60: 6966 206c 656e 2873 7472 5f76 616c 7565  if len(str_value
+0000da70: 7329 203e 2031 0a20 2020 2020 2020 2020  s) > 1.         
+0000da80: 2020 2065 6c73 6520 7374 725f 7661 6c75     else str_valu
+0000da90: 6573 5b30 5d0a 2020 2020 2020 2020 290a  es[0].        ).
+0000daa0: 2020 2020 2020 2020 6675 6c6c 5f72 6f77          full_row
+0000dab0: 5f68 6173 6820 3d20 6675 6c6c 5f72 6f77  _hash = full_row
+0000dac0: 5f73 7472 2e68 6173 6828 292e 6e61 6d65  _str.hash().name
+0000dad0: 286f 7264 6572 696e 675f 6861 7368 5f70  (ordering_hash_p
+0000dae0: 6172 7429 0a20 2020 2020 2020 2023 2042  art).        # B
+0000daf0: 7920 6d6f 6469 6679 696e 6720 7661 6c75  y modifying valu
+0000db00: 6520 736c 6967 6874 6c79 2c20 7765 2067  e slightly, we g
+0000db10: 6574 2061 6e6f 7468 6572 2068 6173 6820  et another hash 
+0000db20: 756e 636f 7272 656c 6174 6564 2077 6974  uncorrelated wit
+0000db30: 6820 7468 6520 6669 7273 740a 2020 2020  h the first.    
+0000db40: 2020 2020 6675 6c6c 5f72 6f77 5f68 6173      full_row_has
+0000db50: 685f 7032 203d 2028 6675 6c6c 5f72 6f77  h_p2 = (full_row
+0000db60: 5f73 7472 202b 2022 5f22 292e 6861 7368  _str + "_").hash
+0000db70: 2829 2e6e 616d 6528 6f72 6465 7269 6e67  ().name(ordering
+0000db80: 5f68 6173 685f 7061 7274 3229 0a20 2020  _hash_part2).   
+0000db90: 2020 2020 2023 2055 7365 6420 746f 2064       # Used to d
+0000dba0: 6973 616d 6269 6775 6174 6520 6265 7477  isambiguate betw
+0000dbb0: 6565 6e20 6964 656e 7469 6361 6c20 726f  een identical ro
+0000dbc0: 7773 2028 7768 6963 6820 7769 6c6c 2068  ws (which will h
+0000dbd0: 6176 6520 6964 656e 7469 6361 6c20 6861  ave identical ha
+0000dbe0: 7368 290a 2020 2020 2020 2020 7261 6e64  sh).        rand
+0000dbf0: 6f6d 5f76 616c 7565 203d 2069 6269 732e  om_value = ibis.
+0000dc00: 7261 6e64 6f6d 2829 2e6e 616d 6528 6f72  random().name(or
+0000dc10: 6465 7269 6e67 5f72 616e 645f 7061 7274  dering_rand_part
+0000dc20: 290a 0a20 2020 2020 2020 206f 7264 6572  )..        order
+0000dc30: 5f76 616c 7565 7320 3d20 280a 2020 2020  _values = (.    
+0000dc40: 2020 2020 2020 2020 5b66 756c 6c5f 726f          [full_ro
+0000dc50: 775f 6861 7368 2c20 6675 6c6c 5f72 6f77  w_hash, full_row
+0000dc60: 5f68 6173 685f 7032 2c20 7261 6e64 6f6d  _hash_p2, random
+0000dc70: 5f76 616c 7565 5d0a 2020 2020 2020 2020  _value].        
+0000dc80: 2020 2020 6966 2075 7365 5f64 6f75 626c      if use_doubl
+0000dc90: 655f 6861 7368 0a20 2020 2020 2020 2020  e_hash.         
+0000dca0: 2020 2065 6c73 6520 5b66 756c 6c5f 726f     else [full_ro
+0000dcb0: 775f 6861 7368 2c20 7261 6e64 6f6d 5f76  w_hash, random_v
+0000dcc0: 616c 7565 5d0a 2020 2020 2020 2020 290a  alue].        ).
+0000dcd0: 0a20 2020 2020 2020 206f 7269 6769 6e61  .        origina
+0000dce0: 6c5f 636f 6c75 6d6e 5f69 6473 203d 2074  l_column_ids = t
+0000dcf0: 6162 6c65 2e63 6f6c 756d 6e73 0a20 2020  able.columns.   
+0000dd00: 2020 2020 2074 6162 6c65 5f77 6974 685f       table_with_
+0000dd10: 6f72 6465 7269 6e67 203d 2074 6162 6c65  ordering = table
+0000dd20: 2e73 656c 6563 7428 0a20 2020 2020 2020  .select(.       
+0000dd30: 2020 2020 2069 7465 7274 6f6f 6c73 2e63       itertools.c
+0000dd40: 6861 696e 286f 7269 6769 6e61 6c5f 636f  hain(original_co
+0000dd50: 6c75 6d6e 5f69 6473 2c20 6f72 6465 725f  lumn_ids, order_
+0000dd60: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
+0000dd70: 290a 0a20 2020 2020 2020 206f 7264 6572  )..        order
+0000dd80: 696e 6720 3d20 6f72 6465 722e 4578 7072  ing = order.Expr
+0000dd90: 6573 7369 6f6e 4f72 6465 7269 6e67 280a  essionOrdering(.
+0000dda0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+0000ddb0: 7269 6e67 5f76 616c 7565 5f63 6f6c 756d  ring_value_colum
+0000ddc0: 6e73 3d74 7570 6c65 280a 2020 2020 2020  ns=tuple(.      
+0000ddd0: 2020 2020 2020 2020 2020 6f72 6465 722e            order.
+0000dde0: 6173 6365 6e64 696e 675f 6f76 6572 2863  ascending_over(c
+0000ddf0: 6f6c 2e67 6574 5f6e 616d 6528 2929 2066  ol.get_name()) f
+0000de00: 6f72 2063 6f6c 2069 6e20 6f72 6465 725f  or col in order_
+0000de10: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+0000de20: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+0000de30: 2020 746f 7461 6c5f 6f72 6465 7269 6e67    total_ordering
+0000de40: 5f63 6f6c 756d 6e73 3d66 726f 7a65 6e73  _columns=frozens
+0000de50: 6574 2863 6f6c 2e67 6574 5f6e 616d 6528  et(col.get_name(
+0000de60: 2920 666f 7220 636f 6c20 696e 206f 7264  ) for col in ord
+0000de70: 6572 5f76 616c 7565 7329 2c0a 2020 2020  er_values),.    
+0000de80: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+0000de90: 6c75 6d6e 7320 3d20 5b74 6162 6c65 5f77  lumns = [table_w
+0000dea0: 6974 685f 6f72 6465 7269 6e67 5b63 6f6c  ith_ordering[col
+0000deb0: 5d20 666f 7220 636f 6c20 696e 206f 7269  ] for col in ori
+0000dec0: 6769 6e61 6c5f 636f 6c75 6d6e 5f69 6473  ginal_column_ids
+0000ded0: 5d0a 2020 2020 2020 2020 6869 6464 656e  ].        hidden
+0000dee0: 5f63 6f6c 756d 6e73 203d 205b 7461 626c  _columns = [tabl
+0000def0: 655f 7769 7468 5f6f 7264 6572 696e 675b  e_with_ordering[
+0000df00: 636f 6c2e 6765 745f 6e61 6d65 2829 5d20  col.get_name()] 
+0000df10: 666f 7220 636f 6c20 696e 206f 7264 6572  for col in order
+0000df20: 5f76 616c 7565 735d 0a20 2020 2020 2020  _values].       
+0000df30: 2072 6574 7572 6e20 636f 7265 2e41 7272   return core.Arr
+0000df40: 6179 5661 6c75 652e 6672 6f6d 5f69 6269  ayValue.from_ibi
+0000df50: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
+0000df60: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000df70: 2074 6162 6c65 5f77 6974 685f 6f72 6465   table_with_orde
+0000df80: 7269 6e67 2c0a 2020 2020 2020 2020 2020  ring,.          
+0000df90: 2020 636f 6c75 6d6e 732c 0a20 2020 2020    columns,.     
+0000dfa0: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
+0000dfb0: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d68  dering_columns=h
+0000dfc0: 6964 6465 6e5f 636f 6c75 6d6e 732c 0a20  idden_columns,. 
+0000dfd0: 2020 2020 2020 2020 2020 206f 7264 6572             order
+0000dfe0: 696e 673d 6f72 6465 7269 6e67 2c0a 2020  ing=ordering,.  
+0000dff0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000e000: 205f 6962 6973 5f74 6f5f 7465 6d70 5f74   _ibis_to_temp_t
+0000e010: 6162 6c65 280a 2020 2020 2020 2020 7365  able(.        se
+0000e020: 6c66 2c0a 2020 2020 2020 2020 7461 626c  lf,.        tabl
+0000e030: 653a 2069 6269 735f 7479 7065 732e 5461  e: ibis_types.Ta
+0000e040: 626c 652c 0a20 2020 2020 2020 2063 6c75  ble,.        clu
+0000e050: 7374 6572 5f63 6f6c 733a 2049 7465 7261  ster_cols: Itera
+0000e060: 626c 655b 7374 725d 2c0a 2020 2020 2020  ble[str],.      
+0000e070: 2020 6170 695f 6e61 6d65 3a20 7374 722c    api_name: str,
+0000e080: 0a20 2020 2029 202d 3e20 6269 6771 7565  .    ) -> bigque
+0000e090: 7279 2e54 6162 6c65 5265 6665 7265 6e63  ry.TableReferenc
+0000e0a0: 653a 0a20 2020 2020 2020 2064 6573 7469  e:.        desti
+0000e0b0: 6e61 7469 6f6e 2c20 5f20 3d20 7365 6c66  nation, _ = self
+0000e0c0: 2e5f 7175 6572 795f 746f 5f64 6573 7469  ._query_to_desti
+0000e0d0: 6e61 7469 6f6e 280a 2020 2020 2020 2020  nation(.        
+0000e0e0: 2020 2020 7365 6c66 2e69 6269 735f 636c      self.ibis_cl
+0000e0f0: 6965 6e74 2e63 6f6d 7069 6c65 2874 6162  ient.compile(tab
+0000e100: 6c65 292c 0a20 2020 2020 2020 2020 2020  le),.           
+0000e110: 2069 6e64 6578 5f63 6f6c 733d 6c69 7374   index_cols=list
+0000e120: 2863 6c75 7374 6572 5f63 6f6c 7329 2c0a  (cluster_cols),.
+0000e130: 2020 2020 2020 2020 2020 2020 6170 695f              api_
+0000e140: 6e61 6d65 3d61 7069 5f6e 616d 652c 0a20  name=api_name,. 
+0000e150: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000e160: 2023 2054 6865 7265 2073 686f 756c 6420   # There should 
+0000e170: 616c 7761 7973 2062 6520 6120 6465 7374  always be a dest
+0000e180: 696e 6174 696f 6e20 7461 626c 6520 666f  ination table fo
+0000e190: 7220 7468 6973 2071 7565 7279 2074 7970  r this query typ
+0000e1a0: 652e 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+0000e1b0: 6e20 7479 7069 6e67 2e63 6173 7428 6269  n typing.cast(bi
+0000e1c0: 6771 7565 7279 2e54 6162 6c65 5265 6665  gquery.TableRefe
+0000e1d0: 7265 6e63 652c 2064 6573 7469 6e61 7469  rence, destinati
+0000e1e0: 6f6e 290a 0a20 2020 2064 6566 2072 656d  on)..    def rem
+0000e1f0: 6f74 655f 6675 6e63 7469 6f6e 280a 2020  ote_function(.  
+0000e200: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000e210: 2020 2020 696e 7075 745f 7479 7065 733a      input_types:
+0000e220: 2055 6e69 6f6e 5b74 7970 652c 2053 6571   Union[type, Seq
+0000e230: 7565 6e63 655b 7479 7065 5d5d 2c0a 2020  uence[type]],.  
+0000e240: 2020 2020 2020 6f75 7470 7574 5f74 7970        output_typ
+0000e250: 653a 2074 7970 652c 0a20 2020 2020 2020  e: type,.       
+0000e260: 2064 6174 6173 6574 3a20 4f70 7469 6f6e   dataset: Option
+0000e270: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000e280: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
+0000e290: 5f63 6f6e 6e65 6374 696f 6e3a 204f 7074  _connection: Opt
+0000e2a0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000e2b0: 652c 0a20 2020 2020 2020 2072 6575 7365  e,.        reuse
+0000e2c0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+0000e2d0: 2020 2020 2020 206e 616d 653a 204f 7074         name: Opt
+0000e2e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000e2f0: 652c 0a20 2020 2020 2020 2070 6163 6b61  e,.        packa
+0000e300: 6765 733a 204f 7074 696f 6e61 6c5b 5365  ges: Optional[Se
+0000e310: 7175 656e 6365 5b73 7472 5d5d 203d 204e  quence[str]] = N
+0000e320: 6f6e 652c 0a20 2020 2020 2020 2063 6c6f  one,.        clo
+0000e330: 7564 5f66 756e 6374 696f 6e5f 7365 7276  ud_function_serv
+0000e340: 6963 655f 6163 636f 756e 743a 204f 7074  ice_account: Opt
+0000e350: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000e360: 652c 0a20 2020 2020 2020 2063 6c6f 7564  e,.        cloud
+0000e370: 5f66 756e 6374 696f 6e5f 6b6d 735f 6b65  _function_kms_ke
+0000e380: 795f 6e61 6d65 3a20 4f70 7469 6f6e 616c  y_name: Optional
+0000e390: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000e3a0: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
+0000e3b0: 7469 6f6e 5f64 6f63 6b65 725f 7265 706f  tion_docker_repo
+0000e3c0: 7369 746f 7279 3a20 4f70 7469 6f6e 616c  sitory: Optional
+0000e3d0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000e3e0: 2020 2020 2020 6d61 785f 6261 7463 6869        max_batchi
+0000e3f0: 6e67 5f72 6f77 733a 204f 7074 696f 6e61  ng_rows: Optiona
+0000e400: 6c5b 696e 745d 203d 2031 3030 302c 0a20  l[int] = 1000,. 
+0000e410: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
+0000e420: 6374 696f 6e5f 7469 6d65 6f75 743a 204f  ction_timeout: O
+0000e430: 7074 696f 6e61 6c5b 696e 745d 203d 2036  ptional[int] = 6
+0000e440: 3030 2c0a 2020 2020 293a 0a20 2020 2020  00,.    ):.     
+0000e450: 2020 2022 2222 4465 636f 7261 746f 7220     """Decorator 
+0000e460: 746f 2074 7572 6e20 6120 7573 6572 2064  to turn a user d
+0000e470: 6566 696e 6564 2066 756e 6374 696f 6e20  efined function 
+0000e480: 696e 746f 2061 2042 6967 5175 6572 7920  into a BigQuery 
+0000e490: 7265 6d6f 7465 2066 756e 6374 696f 6e2e  remote function.
+0000e4a0: 2043 6865 636b 206f 7574 0a20 2020 2020   Check out.     
+0000e4b0: 2020 2074 6865 2063 6f64 6520 7361 6d70     the code samp
+0000e4c0: 6c65 7320 6174 3a20 6874 7470 733a 2f2f  les at: https://
+0000e4d0: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
+0000e4e0: 2f62 6967 7175 6572 792f 646f 6373 2f72  /bigquery/docs/r
+0000e4f0: 656d 6f74 652d 6675 6e63 7469 6f6e 7323  emote-functions#
+0000e500: 6269 6771 7565 7279 2d64 6174 6166 7261  bigquery-datafra
+0000e510: 6d65 732e 0a0a 2020 2020 2020 2020 2e2e  mes...        ..
+0000e520: 206e 6f74 653a 3a0a 2020 2020 2020 2020   note::.        
+0000e530: 2020 2020 506c 6561 7365 206d 616b 6520      Please make 
+0000e540: 7375 7265 2066 6f6c 6c6f 7769 6e67 2069  sure following i
+0000e550: 7320 7365 7475 7020 6265 666f 7265 2075  s setup before u
+0000e560: 7369 6e67 2074 6869 7320 4150 493a 0a0a  sing this API:..
+0000e570: 2020 2020 2020 2020 312e 2048 6176 6520          1. Have 
+0000e580: 7468 6520 6265 6c6f 7720 4150 4973 2065  the below APIs e
+0000e590: 6e61 626c 6564 2066 6f72 2079 6f75 7220  nabled for your 
+0000e5a0: 7072 6f6a 6563 743a 0a0a 2020 2020 2020  project:..      
+0000e5b0: 2020 2020 2020 2a20 4269 6751 7565 7279        * BigQuery
+0000e5c0: 2043 6f6e 6e65 6374 696f 6e20 4150 490a   Connection API.
+0000e5d0: 2020 2020 2020 2020 2020 2020 2a20 436c              * Cl
+0000e5e0: 6f75 6420 4675 6e63 7469 6f6e 7320 4150  oud Functions AP
+0000e5f0: 490a 2020 2020 2020 2020 2020 2020 2a20  I.            * 
+0000e600: 436c 6f75 6420 5275 6e20 4150 490a 2020  Cloud Run API.  
+0000e610: 2020 2020 2020 2020 2020 2a20 436c 6f75            * Clou
+0000e620: 6420 4275 696c 6420 4150 490a 2020 2020  d Build API.    
+0000e630: 2020 2020 2020 2020 2a20 4172 7469 6661          * Artifa
+0000e640: 6374 2052 6567 6973 7472 7920 4150 490a  ct Registry API.
+0000e650: 2020 2020 2020 2020 2020 2020 2a20 436c              * Cl
+0000e660: 6f75 6420 5265 736f 7572 6365 204d 616e  oud Resource Man
+0000e670: 6167 6572 2041 5049 0a0a 2020 2020 2020  ager API..      
+0000e680: 2020 2020 2054 6869 7320 6361 6e20 6265       This can be
+0000e690: 2064 6f6e 6520 6672 6f6d 2074 6865 2063   done from the c
+0000e6a0: 6c6f 7564 2063 6f6e 736f 6c65 2028 6368  loud console (ch
+0000e6b0: 616e 6765 2060 5052 4f4a 4543 545f 4944  ange `PROJECT_ID
+0000e6c0: 6020 746f 2079 6f75 7273 293a 0a20 2020  ` to yours):.   
+0000e6d0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+0000e6e0: 636f 6e73 6f6c 652e 636c 6f75 642e 676f  console.cloud.go
+0000e6f0: 6f67 6c65 2e63 6f6d 2f61 7069 732f 656e  ogle.com/apis/en
+0000e700: 6162 6c65 666c 6f77 3f61 7069 6964 3d62  ableflow?apiid=b
+0000e710: 6967 7175 6572 7963 6f6e 6e65 6374 696f  igqueryconnectio
+0000e720: 6e2e 676f 6f67 6c65 6170 6973 2e63 6f6d  n.googleapis.com
+0000e730: 2c63 6c6f 7564 6675 6e63 7469 6f6e 732e  ,cloudfunctions.
+0000e740: 676f 6f67 6c65 6170 6973 2e63 6f6d 2c72  googleapis.com,r
+0000e750: 756e 2e67 6f6f 676c 6561 7069 732e 636f  un.googleapis.co
+0000e760: 6d2c 636c 6f75 6462 7569 6c64 2e67 6f6f  m,cloudbuild.goo
+0000e770: 676c 6561 7069 732e 636f 6d2c 6172 7469  gleapis.com,arti
+0000e780: 6661 6374 7265 6769 7374 7279 2e67 6f6f  factregistry.goo
+0000e790: 676c 6561 7069 732e 636f 6d2c 636c 6f75  gleapis.com,clou
+0000e7a0: 6472 6573 6f75 7263 656d 616e 6167 6572  dresourcemanager
+0000e7b0: 2e67 6f6f 676c 6561 7069 732e 636f 6d26  .googleapis.com&
+0000e7c0: 7072 6f6a 6563 743d 5052 4f4a 4543 545f  project=PROJECT_
+0000e7d0: 4944 0a0a 2020 2020 2020 2020 2020 204f  ID..           O
+0000e7e0: 7220 6672 6f6d 2074 6865 2067 636c 6f75  r from the gclou
+0000e7f0: 6420 434c 493a 0a0a 2020 2020 2020 2020  d CLI:..        
+0000e800: 2020 2060 2420 6763 6c6f 7564 2073 6572     `$ gcloud ser
+0000e810: 7669 6365 7320 656e 6162 6c65 2062 6967  vices enable big
+0000e820: 7175 6572 7963 6f6e 6e65 6374 696f 6e2e  queryconnection.
+0000e830: 676f 6f67 6c65 6170 6973 2e63 6f6d 2063  googleapis.com c
+0000e840: 6c6f 7564 6675 6e63 7469 6f6e 732e 676f  loudfunctions.go
+0000e850: 6f67 6c65 6170 6973 2e63 6f6d 2072 756e  ogleapis.com run
+0000e860: 2e67 6f6f 676c 6561 7069 732e 636f 6d20  .googleapis.com 
+0000e870: 636c 6f75 6462 7569 6c64 2e67 6f6f 676c  cloudbuild.googl
+0000e880: 6561 7069 732e 636f 6d20 6172 7469 6661  eapis.com artifa
+0000e890: 6374 7265 6769 7374 7279 2e67 6f6f 676c  ctregistry.googl
+0000e8a0: 6561 7069 732e 636f 6d20 636c 6f75 6472  eapis.com cloudr
+0000e8b0: 6573 6f75 7263 656d 616e 6167 6572 2e67  esourcemanager.g
+0000e8c0: 6f6f 676c 6561 7069 732e 636f 6d60 0a0a  oogleapis.com`..
+0000e8d0: 2020 2020 2020 2020 322e 2048 6176 6520          2. Have 
+0000e8e0: 666f 6c6c 6f77 696e 6720 4941 4d20 726f  following IAM ro
+0000e8f0: 6c65 7320 656e 6162 6c65 6420 666f 7220  les enabled for 
+0000e900: 796f 753a 0a0a 2020 2020 2020 2020 2020  you:..          
+0000e910: 2020 2a20 4269 6751 7565 7279 2044 6174    * BigQuery Dat
+0000e920: 6120 4564 6974 6f72 2028 726f 6c65 732f  a Editor (roles/
+0000e930: 6269 6771 7565 7279 2e64 6174 6145 6469  bigquery.dataEdi
+0000e940: 746f 7229 0a20 2020 2020 2020 2020 2020  tor).           
+0000e950: 202a 2042 6967 5175 6572 7920 436f 6e6e   * BigQuery Conn
+0000e960: 6563 7469 6f6e 2041 646d 696e 2028 726f  ection Admin (ro
+0000e970: 6c65 732f 6269 6771 7565 7279 2e63 6f6e  les/bigquery.con
+0000e980: 6e65 6374 696f 6e41 646d 696e 290a 2020  nectionAdmin).  
+0000e990: 2020 2020 2020 2020 2020 2a20 436c 6f75            * Clou
+0000e9a0: 6420 4675 6e63 7469 6f6e 7320 4465 7665  d Functions Deve
+0000e9b0: 6c6f 7065 7220 2872 6f6c 6573 2f63 6c6f  loper (roles/clo
+0000e9c0: 7564 6675 6e63 7469 6f6e 732e 6465 7665  udfunctions.deve
+0000e9d0: 6c6f 7065 7229 0a20 2020 2020 2020 2020  loper).         
+0000e9e0: 2020 202a 2053 6572 7669 6365 2041 6363     * Service Acc
+0000e9f0: 6f75 6e74 2055 7365 7220 2872 6f6c 6573  ount User (roles
+0000ea00: 2f69 616d 2e73 6572 7669 6365 4163 636f  /iam.serviceAcco
+0000ea10: 756e 7455 7365 7229 206f 6e20 7468 6520  untUser) on the 
+0000ea20: 7365 7276 6963 6520 6163 636f 756e 7420  service account 
+0000ea30: 6050 524f 4a45 4354 5f4e 554d 4245 522d  `PROJECT_NUMBER-
+0000ea40: 636f 6d70 7574 6540 6465 7665 6c6f 7065  compute@develope
+0000ea50: 722e 6773 6572 7669 6365 6163 636f 756e  r.gserviceaccoun
+0000ea60: 742e 636f 6d60 0a20 2020 2020 2020 2020  t.com`.         
+0000ea70: 2020 202a 2053 746f 7261 6765 204f 626a     * Storage Obj
+0000ea80: 6563 7420 5669 6577 6572 2028 726f 6c65  ect Viewer (role
+0000ea90: 732f 7374 6f72 6167 652e 6f62 6a65 6374  s/storage.object
+0000eaa0: 5669 6577 6572 290a 2020 2020 2020 2020  Viewer).        
+0000eab0: 2020 2020 2a20 5072 6f6a 6563 7420 4941      * Project IA
+0000eac0: 4d20 4164 6d69 6e20 2872 6f6c 6573 2f72  M Admin (roles/r
+0000ead0: 6573 6f75 7263 656d 616e 6167 6572 2e70  esourcemanager.p
+0000eae0: 726f 6a65 6374 4961 6d41 646d 696e 2920  rojectIamAdmin) 
+0000eaf0: 284f 6e6c 7920 7265 7175 6972 6564 2069  (Only required i
+0000eb00: 6620 7468 6520 6269 6771 7565 7279 2063  f the bigquery c
+0000eb10: 6f6e 6e65 6374 696f 6e20 6265 696e 6720  onnection being 
+0000eb20: 7573 6564 2069 7320 6e6f 7420 7072 652d  used is not pre-
+0000eb30: 6372 6561 7465 6420 616e 6420 6973 2063  created and is c
+0000eb40: 7265 6174 6564 2064 796e 616d 6963 616c  reated dynamical
+0000eb50: 6c79 2077 6974 6820 7573 6572 2063 7265  ly with user cre
+0000eb60: 6465 6e74 6961 6c73 2e29 0a0a 2020 2020  dentials.)..    
+0000eb70: 2020 2020 332e 2045 6974 6865 7220 7468      3. Either th
+0000eb80: 6520 7573 6572 2068 6173 2073 6574 4961  e user has setIa
+0000eb90: 6d50 6f6c 6963 7920 7072 6976 696c 6567  mPolicy privileg
+0000eba0: 6520 6f6e 2074 6865 2070 726f 6a65 6374  e on the project
+0000ebb0: 2c20 6f72 2061 2042 6967 5175 6572 7920  , or a BigQuery 
+0000ebc0: 636f 6e6e 6563 7469 6f6e 2069 7320 7072  connection is pr
+0000ebd0: 652d 6372 6561 7465 6420 7769 7468 206e  e-created with n
+0000ebe0: 6563 6573 7361 7279 2049 414d 2072 6f6c  ecessary IAM rol
+0000ebf0: 6520 7365 743a 0a0a 2020 2020 2020 2020  e set:..        
+0000ec00: 2020 2020 312e 2054 6f20 6372 6561 7465      1. To create
+0000ec10: 2061 2063 6f6e 6e65 6374 696f 6e2c 2066   a connection, f
+0000ec20: 6f6c 6c6f 7720 6874 7470 733a 2f2f 636c  ollow https://cl
+0000ec30: 6f75 642e 676f 6f67 6c65 2e63 6f6d 2f62  oud.google.com/b
+0000ec40: 6967 7175 6572 792f 646f 6373 2f72 6566  igquery/docs/ref
+0000ec50: 6572 656e 6365 2f73 7461 6e64 6172 642d  erence/standard-
+0000ec60: 7371 6c2f 7265 6d6f 7465 2d66 756e 6374  sql/remote-funct
+0000ec70: 696f 6e73 2363 7265 6174 655f 615f 636f  ions#create_a_co
+0000ec80: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
+0000ec90: 2020 2020 2032 2e20 546f 2073 6574 2075       2. To set u
+0000eca0: 7020 4941 4d2c 2066 6f6c 6c6f 7720 6874  p IAM, follow ht
+0000ecb0: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
+0000ecc0: 6c65 2e63 6f6d 2f62 6967 7175 6572 792f  le.com/bigquery/
+0000ecd0: 646f 6373 2f72 6566 6572 656e 6365 2f73  docs/reference/s
+0000ece0: 7461 6e64 6172 642d 7371 6c2f 7265 6d6f  tandard-sql/remo
+0000ecf0: 7465 2d66 756e 6374 696f 6e73 2367 7261  te-functions#gra
+0000ed00: 6e74 5f70 6572 6d69 7373 696f 6e5f 6f6e  nt_permission_on
+0000ed10: 5f66 756e 6374 696f 6e0a 0a20 2020 2020  _function..     
+0000ed20: 2020 2020 2020 2020 2020 416c 7465 726e            Altern
+0000ed30: 6174 6976 656c 792c 2074 6865 2049 414d  atively, the IAM
+0000ed40: 2063 6f75 6c64 2061 6c73 6f20 6265 2073   could also be s
+0000ed50: 6574 7570 2076 6961 2074 6865 2067 636c  etup via the gcl
+0000ed60: 6f75 6420 434c 493a 0a0a 2020 2020 2020  oud CLI:..      
+0000ed70: 2020 2020 2020 2020 2060 2420 6763 6c6f           `$ gclo
+0000ed80: 7564 2070 726f 6a65 6374 7320 6164 642d  ud projects add-
+0000ed90: 6961 6d2d 706f 6c69 6379 2d62 696e 6469  iam-policy-bindi
+0000eda0: 6e67 2050 524f 4a45 4354 5f49 4420 2d2d  ng PROJECT_ID --
+0000edb0: 6d65 6d62 6572 3d22 7365 7276 6963 6541  member="serviceA
+0000edc0: 6363 6f75 6e74 3a43 4f4e 4e45 4354 494f  ccount:CONNECTIO
+0000edd0: 4e5f 5345 5256 4943 455f 4143 434f 554e  N_SERVICE_ACCOUN
+0000ede0: 545f 4944 2220 2d2d 726f 6c65 3d22 726f  T_ID" --role="ro
+0000edf0: 6c65 732f 7275 6e2e 696e 766f 6b65 7222  les/run.invoker"
+0000ee00: 602e 0a0a 2020 2020 2020 2020 4172 6773  `...        Args
+0000ee10: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
+0000ee20: 7075 745f 7479 7065 7320 2874 7970 6520  put_types (type 
+0000ee30: 6f72 2073 6571 7565 6e63 6528 7479 7065  or sequence(type
+0000ee40: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000ee50: 2020 2020 496e 7075 7420 6461 7461 2074      Input data t
+0000ee60: 7970 652c 206f 7220 7365 7175 656e 6365  ype, or sequence
+0000ee70: 206f 6620 696e 7075 7420 6461 7461 2074   of input data t
+0000ee80: 7970 6573 2069 6e20 7468 6520 7573 6572  ypes in the user
+0000ee90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eea0: 2064 6566 696e 6564 2066 756e 6374 696f   defined functio
+0000eeb0: 6e2e 0a20 2020 2020 2020 2020 2020 206f  n..            o
+0000eec0: 7574 7075 745f 7479 7065 2028 7479 7065  utput_type (type
+0000eed0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000eee0: 2020 2044 6174 6120 7479 7065 206f 6620     Data type of 
+0000eef0: 7468 6520 6f75 7470 7574 2069 6e20 7468  the output in th
+0000ef00: 6520 7573 6572 2064 6566 696e 6564 2066  e user defined f
+0000ef10: 756e 6374 696f 6e2e 0a20 2020 2020 2020  unction..       
+0000ef20: 2020 2020 2064 6174 6173 6574 2028 7374       dataset (st
+0000ef30: 722c 204f 7074 696f 6e61 6c29 3a0a 2020  r, Optional):.  
+0000ef40: 2020 2020 2020 2020 2020 2020 2020 4461                Da
+0000ef50: 7461 7365 7420 696e 2077 6869 6368 2074  taset in which t
+0000ef60: 6f20 6372 6561 7465 2061 2042 6967 5175  o create a BigQu
+0000ef70: 6572 7920 7265 6d6f 7465 2066 756e 6374  ery remote funct
+0000ef80: 696f 6e2e 2049 7420 7368 6f75 6c64 2062  ion. It should b
+0000ef90: 6520 696e 0a20 2020 2020 2020 2020 2020  e in.           
+0000efa0: 2020 2020 2060 3c70 726f 6a65 6374 5f69       `<project_i
+0000efb0: 643e 2e3c 6461 7461 7365 745f 6e61 6d65  d>.<dataset_name
+0000efc0: 3e60 206f 7220 603c 6461 7461 7365 745f  >` or `<dataset_
+0000efd0: 6e61 6d65 3e60 2066 6f72 6d61 742e 2049  name>` format. I
+0000efe0: 6620 7468 6973 0a20 2020 2020 2020 2020  f this.         
+0000eff0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+0000f000: 2069 7320 6e6f 7420 7072 6f76 6964 6564   is not provided
+0000f010: 2074 6865 6e20 7365 7373 696f 6e20 6461   then session da
+0000f020: 7461 7365 7420 6964 2069 7320 7573 6564  taset id is used
+0000f030: 2e0a 2020 2020 2020 2020 2020 2020 6269  ..            bi
+0000f040: 6771 7565 7279 5f63 6f6e 6e65 6374 696f  gquery_connectio
+0000f050: 6e20 2873 7472 2c20 4f70 7469 6f6e 616c  n (str, Optional
+0000f060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000f070: 2020 204e 616d 6520 6f66 2074 6865 2042     Name of the B
+0000f080: 6967 5175 6572 7920 636f 6e6e 6563 7469  igQuery connecti
+0000f090: 6f6e 2e20 596f 7520 7368 6f75 6c64 2065  on. You should e
+0000f0a0: 6974 6865 7220 6861 7665 2074 6865 0a20  ither have the. 
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f0c0: 6f6e 6e65 6374 696f 6e20 616c 7265 6164  onnection alread
+0000f0d0: 7920 6372 6561 7465 6420 696e 2074 6865  y created in the
+0000f0e0: 2060 6c6f 6361 7469 6f6e 6020 796f 7520   `location` you 
+0000f0f0: 6861 7665 2063 686f 7365 6e2c 206f 720a  have chosen, or.
+0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f110: 796f 7520 7368 6f75 6c64 2068 6176 6520  you should have 
+0000f120: 7468 6520 5072 6f6a 6563 7420 4941 4d20  the Project IAM 
+0000f130: 4164 6d69 6e20 726f 6c65 2074 6f20 656e  Admin role to en
+0000f140: 6162 6c65 2074 6865 2073 6572 7669 6365  able the service
+0000f150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f160: 2074 6f20 6372 6561 7465 2074 6865 2063   to create the c
+0000f170: 6f6e 6e65 6374 696f 6e20 666f 7220 796f  onnection for yo
+0000f180: 7520 6966 2079 6f75 206e 6565 6420 6974  u if you need it
+0000f190: 2e20 4966 2074 6869 7320 7061 7261 6d65  . If this parame
+0000f1a0: 7465 7220 6973 0a20 2020 2020 2020 2020  ter is.         
+0000f1b0: 2020 2020 2020 206e 6f74 2070 726f 7669         not provi
+0000f1c0: 6465 6420 7468 656e 2074 6865 2042 6967  ded then the Big
+0000f1d0: 5175 6572 7920 636f 6e6e 6563 7469 6f6e  Query connection
+0000f1e0: 2066 726f 6d20 7468 6520 7365 7373 696f   from the sessio
+0000f1f0: 6e20 6973 2075 7365 642e 0a20 2020 2020  n is used..     
+0000f200: 2020 2020 2020 2072 6575 7365 2028 626f         reuse (bo
+0000f210: 6f6c 2c20 4f70 7469 6f6e 616c 293a 0a20  ol, Optional):. 
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+0000f230: 6575 7365 2074 6865 2072 656d 6f74 6520  euse the remote 
+0000f240: 6675 6e63 7469 6f6e 2069 6620 616c 7265  function if alre
+0000f250: 6164 7920 6578 6973 7473 2e0a 2020 2020  ady exists..    
+0000f260: 2020 2020 2020 2020 2020 2020 6054 7275              `Tru
+0000f270: 6560 2062 7920 6465 6661 756c 742c 2077  e` by default, w
+0000f280: 6869 6368 2077 696c 6c20 7265 7375 6c74  hich will result
+0000f290: 2069 6e20 7265 7573 696e 6720 616e 2065   in reusing an e
+0000f2a0: 7869 7374 696e 6720 7265 6d6f 7465 0a20  xisting remote. 
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f2c0: 756e 6374 696f 6e20 616e 6420 636f 7272  unction and corr
+0000f2d0: 6573 706f 6e64 696e 6720 636c 6f75 6420  esponding cloud 
+0000f2e0: 6675 6e63 7469 6f6e 2028 6966 2061 6e79  function (if any
+0000f2f0: 2920 7468 6174 2077 6173 0a20 2020 2020  ) that was.     
+0000f300: 2020 2020 2020 2020 2020 2070 7265 7669             previ
+0000f310: 6f75 736c 7920 6372 6561 7465 6420 666f  ously created fo
+0000f320: 7220 7468 6520 7361 6d65 2075 6466 2e0a  r the same udf..
+0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f340: 5365 7474 696e 6720 6974 2074 6f20 6046  Setting it to `F
+0000f350: 616c 7365 6020 776f 756c 6420 666f 7263  alse` would forc
+0000f360: 6520 6372 6561 7469 6e67 2061 2075 6e69  e creating a uni
+0000f370: 7175 6520 7265 6d6f 7465 2066 756e 6374  que remote funct
+0000f380: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+0000f390: 2020 2020 2049 6620 7468 6520 7265 7175       If the requ
+0000f3a0: 6972 6564 2072 656d 6f74 6520 6675 6e63  ired remote func
+0000f3b0: 7469 6f6e 2064 6f65 7320 6e6f 7420 6578  tion does not ex
+0000f3c0: 6973 7420 7468 656e 2069 7420 776f 756c  ist then it woul
+0000f3d0: 6420 6265 0a20 2020 2020 2020 2020 2020  d be.           
+0000f3e0: 2020 2020 2063 7265 6174 6564 2069 7272       created irr
+0000f3f0: 6573 7065 6374 6976 6520 6f66 2074 6869  espective of thi
+0000f400: 7320 7061 7261 6d2e 0a20 2020 2020 2020  s param..       
+0000f410: 2020 2020 206e 616d 6520 2873 7472 2c20       name (str, 
+0000f420: 4f70 7469 6f6e 616c 293a 0a20 2020 2020  Optional):.     
+0000f430: 2020 2020 2020 2020 2020 2045 7870 6c69             Expli
+0000f440: 6369 7420 6e61 6d65 206f 6620 7468 6520  cit name of the 
+0000f450: 7065 7273 6973 7465 6420 4269 6751 7565  persisted BigQue
+0000f460: 7279 2072 656d 6f74 6520 6675 6e63 7469  ry remote functi
+0000f470: 6f6e 2e20 5573 6520 6974 2077 6974 680a  on. Use it with.
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 6361 7574 696f 6e2c 2062 6563 6175 7365  caution, because
+0000f4a0: 2074 776f 2075 7365 7273 2077 6f72 6b69   two users worki
+0000f4b0: 6e67 2069 6e20 7468 6520 7361 6d65 2070  ng in the same p
+0000f4c0: 726f 6a65 6374 2061 6e64 2064 6174 6173  roject and datas
+0000f4d0: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
+0000f4e0: 2020 2063 6f75 6c64 206f 7665 7277 7269     could overwri
+0000f4f0: 7465 2065 6163 6820 6f74 6865 7227 7320  te each other's 
+0000f500: 7265 6d6f 7465 2066 756e 6374 696f 6e73  remote functions
+0000f510: 2069 6620 7468 6579 2075 7365 2074 6865   if they use the
+0000f520: 2073 616d 650a 2020 2020 2020 2020 2020   same.          
+0000f530: 2020 2020 2020 7065 7273 6973 7465 6e74        persistent
+0000f540: 206e 616d 652e 0a20 2020 2020 2020 2020   name..         
+0000f550: 2020 2070 6163 6b61 6765 7320 2873 7472     packages (str
+0000f560: 5b5d 2c20 4f70 7469 6f6e 616c 293a 0a20  [], Optional):. 
+0000f570: 2020 2020 2020 2020 2020 2020 2020 2045                 E
+0000f580: 7870 6c69 6369 7420 6e61 6d65 206f 6620  xplicit name of 
+0000f590: 7468 6520 6578 7465 726e 616c 2070 6163  the external pac
+0000f5a0: 6b61 6765 2064 6570 656e 6465 6e63 6965  kage dependencie
+0000f5b0: 732e 2045 6163 6820 6465 7065 6e64 656e  s. Each dependen
+0000f5c0: 6379 0a20 2020 2020 2020 2020 2020 2020  cy.             
+0000f5d0: 2020 2069 7320 6164 6465 6420 746f 2074     is added to t
+0000f5e0: 6865 2060 7265 7175 6972 656d 656e 7473  he `requirements
+0000f5f0: 2e74 7874 6020 6173 2069 732c 2061 6e64  .txt` as is, and
+0000f600: 2063 616e 2062 6520 6f66 2074 6865 2066   can be of the f
+0000f610: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
+0000f620: 2020 2020 7375 7070 6f72 7465 6420 696e      supported in
+0000f630: 2068 7474 7073 3a2f 2f70 6970 2e70 7970   https://pip.pyp
+0000f640: 612e 696f 2f65 6e2f 7374 6162 6c65 2f72  a.io/en/stable/r
+0000f650: 6566 6572 656e 6365 2f72 6571 7569 7265  eference/require
+0000f660: 6d65 6e74 732d 6669 6c65 2d66 6f72 6d61  ments-file-forma
+0000f670: 742f 2e0a 2020 2020 2020 2020 2020 2020  t/..            
+0000f680: 636c 6f75 645f 6675 6e63 7469 6f6e 5f73  cloud_function_s
+0000f690: 6572 7669 6365 5f61 6363 6f75 6e74 2028  ervice_account (
+0000f6a0: 7374 722c 204f 7074 696f 6e61 6c29 3a0a  str, Optional):.
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 5365 7276 6963 6520 6163 636f 756e 7420  Service account 
+0000f6d0: 746f 2075 7365 2066 6f72 2074 6865 2063  to use for the c
+0000f6e0: 6c6f 7564 2066 756e 6374 696f 6e73 2e20  loud functions. 
+0000f6f0: 4966 206e 6f74 2070 726f 7669 6465 640a  If not provided.
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f710: 7468 656e 2074 6865 2064 6566 6175 6c74  then the default
+0000f720: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
+0000f730: 2077 6f75 6c64 2062 6520 7573 6564 2e20   would be used. 
+0000f740: 5365 650a 2020 2020 2020 2020 2020 2020  See.            
+0000f750: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
+0000f760: 642e 676f 6f67 6c65 2e63 6f6d 2f66 756e  d.google.com/fun
+0000f770: 6374 696f 6e73 2f64 6f63 732f 7365 6375  ctions/docs/secu
+0000f780: 7269 6e67 2f66 756e 6374 696f 6e2d 6964  ring/function-id
+0000f790: 656e 7469 7479 0a20 2020 2020 2020 2020  entity.         
+0000f7a0: 2020 2020 2020 2066 6f72 206d 6f72 6520         for more 
+0000f7b0: 6465 7461 696c 732e 2050 6c65 6173 6520  details. Please 
+0000f7c0: 6d61 6b65 2073 7572 6520 7468 6520 7365  make sure the se
+0000f7d0: 7276 6963 6520 6163 636f 756e 7420 6861  rvice account ha
+0000f7e0: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
+0000f7f0: 2020 2020 2020 6e65 6365 7373 6172 7920        necessary 
+0000f800: 4941 4d20 7065 726d 6973 7369 6f6e 7320  IAM permissions 
+0000f810: 636f 6e66 6967 7572 6564 2061 7320 6465  configured as de
+0000f820: 7363 7269 6265 6420 696e 0a20 2020 2020  scribed in.     
+0000f830: 2020 2020 2020 2020 2020 2068 7474 7073             https
+0000f840: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+0000f850: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
+0000f860: 6373 2f72 6566 6572 656e 6365 2f69 616d  cs/reference/iam
+0000f870: 2f72 6f6c 6573 2361 6464 6974 696f 6e61  /roles#additiona
+0000f880: 6c2d 636f 6e66 6967 7572 6174 696f 6e2e  l-configuration.
+0000f890: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+0000f8a0: 7564 5f66 756e 6374 696f 6e5f 6b6d 735f  ud_function_kms_
+0000f8b0: 6b65 795f 6e61 6d65 2028 7374 722c 204f  key_name (str, O
+0000f8c0: 7074 696f 6e61 6c29 3a0a 2020 2020 2020  ptional):.      
+0000f8d0: 2020 2020 2020 2020 2020 4375 7374 6f6d            Custom
+0000f8e0: 6572 206d 616e 6167 6564 2065 6e63 7279  er managed encry
+0000f8f0: 7074 696f 6e20 6b65 7920 746f 2070 726f  ption key to pro
+0000f900: 7465 6374 2063 6c6f 7564 2066 756e 6374  tect cloud funct
+0000f910: 696f 6e73 2061 6e64 0a20 2020 2020 2020  ions and.       
+0000f920: 2020 2020 2020 2020 2072 656c 6174 6564           related
+0000f930: 2064 6174 6120 6174 2072 6573 742e 2054   data at rest. T
+0000f940: 6869 7320 6973 206f 6620 7468 6520 666f  his is of the fo
+0000f950: 726d 6174 0a20 2020 2020 2020 2020 2020  rmat.           
+0000f960: 2020 2020 2070 726f 6a65 6374 732f 5052       projects/PR
+0000f970: 4f4a 4543 545f 4944 2f6c 6f63 6174 696f  OJECT_ID/locatio
+0000f980: 6e73 2f4c 4f43 4154 494f 4e2f 6b65 7952  ns/LOCATION/keyR
+0000f990: 696e 6773 2f4b 4559 5249 4e47 2f63 7279  ings/KEYRING/cry
+0000f9a0: 7074 6f4b 6579 732f 4b45 592e 0a20 2020  ptoKeys/KEY..   
+0000f9b0: 2020 2020 2020 2020 2020 2020 2052 6561               Rea
+0000f9c0: 6420 6874 7470 733a 2f2f 636c 6f75 642e  d https://cloud.
+0000f9d0: 676f 6f67 6c65 2e63 6f6d 2f66 756e 6374  google.com/funct
+0000f9e0: 696f 6e73 2f64 6f63 732f 7365 6375 7269  ions/docs/securi
+0000f9f0: 6e67 2f63 6d65 6b20 666f 720a 2020 2020  ng/cmek for.    
+0000fa00: 2020 2020 2020 2020 2020 2020 6d6f 7265              more
+0000fa10: 2064 6574 6169 6c73 2069 6e63 6c75 6469   details includi
+0000fa20: 6e67 2067 7261 6e74 696e 6720 6e65 6365  ng granting nece
+0000fa30: 7373 6172 7920 7365 7276 6963 6520 6163  ssary service ac
+0000fa40: 636f 756e 7473 0a20 2020 2020 2020 2020  counts.         
+0000fa50: 2020 2020 2020 2061 6363 6573 7320 746f         access to
+0000fa60: 2074 6865 206b 6579 2e0a 2020 2020 2020   the key..      
+0000fa70: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
+0000fa80: 7469 6f6e 5f64 6f63 6b65 725f 7265 706f  tion_docker_repo
+0000fa90: 7369 746f 7279 2028 7374 722c 204f 7074  sitory (str, Opt
+0000faa0: 696f 6e61 6c29 3a0a 2020 2020 2020 2020  ional):.        
+0000fab0: 2020 2020 2020 2020 446f 636b 6572 2072          Docker r
+0000fac0: 6570 6f73 6974 6f72 7920 6372 6561 7465  epository create
+0000fad0: 6420 7769 7468 2074 6865 2073 616d 6520  d with the same 
+0000fae0: 656e 6372 7970 7469 6f6e 206b 6579 2061  encryption key a
+0000faf0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000fb00: 2020 6063 6c6f 7564 5f66 756e 6374 696f    `cloud_functio
+0000fb10: 6e5f 6b6d 735f 6b65 795f 6e61 6d65 6020  n_kms_key_name` 
+0000fb20: 746f 2073 746f 7265 2065 6e63 7279 7074  to store encrypt
+0000fb30: 6564 2061 7274 6966 6163 7473 0a20 2020  ed artifacts.   
+0000fb40: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+0000fb50: 6174 6564 2074 6f20 7375 7070 6f72 7420  ated to support 
+0000fb60: 7468 6520 636c 6f75 6420 6675 6e63 7469  the cloud functi
+0000fb70: 6f6e 2e20 5468 6973 2069 7320 6f66 2074  on. This is of t
+0000fb80: 6865 2066 6f72 6d61 740a 2020 2020 2020  he format.      
+0000fb90: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
+0000fba0: 7473 2f50 524f 4a45 4354 5f49 442f 6c6f  ts/PROJECT_ID/lo
+0000fbb0: 6361 7469 6f6e 732f 4c4f 4341 5449 4f4e  cations/LOCATION
+0000fbc0: 2f72 6570 6f73 6974 6f72 6965 732f 5245  /repositories/RE
+0000fbd0: 504f 5349 544f 5259 5f4e 414d 452e 0a20  POSITORY_NAME.. 
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0000fbf0: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
+0000fc00: 7365 650a 2020 2020 2020 2020 2020 2020  see.            
+0000fc10: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
+0000fc20: 642e 676f 6f67 6c65 2e63 6f6d 2f66 756e  d.google.com/fun
+0000fc30: 6374 696f 6e73 2f64 6f63 732f 7365 6375  ctions/docs/secu
+0000fc40: 7269 6e67 2f63 6d65 6b23 6265 666f 7265  ring/cmek#before
+0000fc50: 5f79 6f75 5f62 6567 696e 2e0a 2020 2020  _you_begin..    
+0000fc60: 2020 2020 2020 2020 6d61 785f 6261 7463          max_batc
+0000fc70: 6869 6e67 5f72 6f77 7320 2869 6e74 2c20  hing_rows (int, 
+0000fc80: 4f70 7469 6f6e 616c 293a 0a20 2020 2020  Optional):.     
+0000fc90: 2020 2020 2020 2020 2020 2054 6865 206d             The m
+0000fca0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+0000fcb0: 2072 6f77 7320 746f 2062 6520 6261 7463   rows to be batc
+0000fcc0: 6865 6420 666f 7220 7072 6f63 6573 7369  hed for processi
+0000fcd0: 6e67 2069 6e20 7468 650a 2020 2020 2020  ng in the.      
+0000fce0: 2020 2020 2020 2020 2020 4251 2072 656d            BQ rem
+0000fcf0: 6f74 6520 6675 6e63 7469 6f6e 2e20 4465  ote function. De
+0000fd00: 6661 756c 7420 7661 6c75 6520 6973 2031  fault value is 1
+0000fd10: 3030 302e 2041 206c 6f77 6572 206e 756d  000. A lower num
+0000fd20: 6265 7220 6361 6e20 6265 0a20 2020 2020  ber can be.     
+0000fd30: 2020 2020 2020 2020 2020 2070 6173 7365             passe
+0000fd40: 6420 746f 2061 766f 6964 2074 696d 656f  d to avoid timeo
+0000fd50: 7574 7320 696e 2063 6173 6520 7468 6520  uts in case the 
+0000fd60: 7573 6572 2063 6f64 6520 6973 2074 6f6f  user code is too
+0000fd70: 2063 6f6d 706c 6578 2074 6f0a 2020 2020   complex to.    
+0000fd80: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+0000fd90: 6573 7320 6c61 7267 6520 6e75 6d62 6572  ess large number
+0000fda0: 206f 6620 726f 7773 2066 6173 7420 656e   of rows fast en
+0000fdb0: 6f75 6768 2e20 4120 6869 6768 6572 206e  ough. A higher n
+0000fdc0: 756d 6265 7220 6361 6e20 6265 0a20 2020  umber can be.   
+0000fdd0: 2020 2020 2020 2020 2020 2020 2075 7365               use
+0000fde0: 6420 746f 2069 6e63 7265 6173 6520 7468  d to increase th
+0000fdf0: 726f 7567 6870 7574 2069 6e20 6361 7365  roughput in case
+0000fe00: 2074 6865 2075 7365 7220 636f 6465 2069   the user code i
+0000fe10: 7320 6661 7374 2065 6e6f 7567 682e 0a20  s fast enough.. 
+0000fe20: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+0000fe30: 4e6f 6e65 6020 6361 6e20 6265 2070 6173  None` can be pas
+0000fe40: 7365 6420 746f 206c 6574 2042 5120 7265  sed to let BQ re
+0000fe50: 6d6f 7465 2066 756e 6374 696f 6e73 2073  mote functions s
+0000fe60: 6572 7669 6365 2061 7070 6c79 0a20 2020  ervice apply.   
+0000fe70: 2020 2020 2020 2020 2020 2020 2064 6566               def
+0000fe80: 6175 6c74 2062 6174 6368 696e 672e 2053  ault batching. S
+0000fe90: 6565 2066 6f72 206d 6f72 6520 6465 7461  ee for more deta
+0000fea0: 696c 730a 2020 2020 2020 2020 2020 2020  ils.            
+0000feb0: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
+0000fec0: 642e 676f 6f67 6c65 2e63 6f6d 2f62 6967  d.google.com/big
+0000fed0: 7175 6572 792f 646f 6373 2f72 656d 6f74  query/docs/remot
+0000fee0: 652d 6675 6e63 7469 6f6e 7323 6c69 6d69  e-functions#limi
+0000fef0: 7469 6e67 5f6e 756d 6265 725f 6f66 5f72  ting_number_of_r
+0000ff00: 6f77 735f 696e 5f61 5f62 6174 6368 5f72  ows_in_a_batch_r
+0000ff10: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
+0000ff20: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+0000ff30: 6f6e 5f74 696d 656f 7574 2028 696e 742c  on_timeout (int,
+0000ff40: 204f 7074 696f 6e61 6c29 3a0a 2020 2020   Optional):.    
+0000ff50: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000ff60: 6d61 7869 6d75 6d20 616d 6f75 6e74 206f  maximum amount o
+0000ff70: 6620 7469 6d65 2028 696e 2073 6563 6f6e  f time (in secon
+0000ff80: 6473 2920 4269 6751 7565 7279 2073 686f  ds) BigQuery sho
+0000ff90: 756c 6420 7761 6974 2066 6f72 0a20 2020  uld wait for.   
+0000ffa0: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000ffb0: 2063 6c6f 7564 2066 756e 6374 696f 6e20   cloud function 
+0000ffc0: 746f 2072 6574 7572 6e20 6120 7265 7370  to return a resp
+0000ffd0: 6f6e 7365 2e20 5365 6520 666f 7220 6d6f  onse. See for mo
+0000ffe0: 7265 2064 6574 6169 6c73 0a20 2020 2020  re details.     
+0000fff0: 2020 2020 2020 2020 2020 2068 7474 7073             https
+00010000: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+00010010: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
+00010020: 6373 2f63 6f6e 6669 6775 7269 6e67 2f74  cs/configuring/t
+00010030: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
+00010040: 2020 2020 2020 2020 506c 6561 7365 206e          Please n
+00010050: 6f74 6520 7468 6174 2065 7665 6e20 7468  ote that even th
+00010060: 6f75 6768 2074 6865 2063 6c6f 7564 2066  ough the cloud f
+00010070: 756e 6374 696f 6e20 2832 6e64 2067 656e  unction (2nd gen
+00010080: 2920 6974 7365 6c66 0a20 2020 2020 2020  ) itself.       
+00010090: 2020 2020 2020 2020 2061 6c6c 6f77 7320           allows 
+000100a0: 7365 6574 696e 6720 7570 2074 6f20 3630  seeting up to 60
+000100b0: 206d 696e 7574 6573 206f 6620 7469 6d65   minutes of time
+000100c0: 6f75 742c 2042 6967 5175 6572 7920 7265  out, BigQuery re
+000100d0: 6d6f 7465 0a20 2020 2020 2020 2020 2020  mote.           
+000100e0: 2020 2020 2066 756e 6374 696f 6e20 6361       function ca
+000100f0: 6e20 7761 6974 206f 6e6c 7920 7570 2074  n wait only up t
+00010100: 6f20 3230 206d 696e 7574 6573 2c20 7365  o 20 minutes, se
+00010110: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
+00010120: 6c73 0a20 2020 2020 2020 2020 2020 2020  ls.             
+00010130: 2020 2068 7474 7073 3a2f 2f63 6c6f 7564     https://cloud
+00010140: 2e67 6f6f 676c 652e 636f 6d2f 6269 6771  .google.com/bigq
+00010150: 7565 7279 2f71 756f 7461 7323 7265 6d6f  uery/quotas#remo
+00010160: 7465 5f66 756e 6374 696f 6e5f 6c69 6d69  te_function_limi
+00010170: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00010180: 2020 2020 4279 2064 6566 6175 6c74 2042      By default B
+00010190: 6967 5175 6572 7920 4461 7461 4672 616d  igQuery DataFram
+000101a0: 6573 2075 7365 7320 6120 3130 206d 696e  es uses a 10 min
+000101b0: 7574 6520 7469 6d65 6f75 742e 2060 4e6f  ute timeout. `No
+000101c0: 6e65 600a 2020 2020 2020 2020 2020 2020  ne`.            
+000101d0: 2020 2020 6361 6e20 6265 2070 6173 7365      can be passe
+000101e0: 6420 746f 206c 6574 2074 6865 2063 6c6f  d to let the clo
+000101f0: 7564 2066 756e 6374 696f 6e73 2064 6566  ud functions def
+00010200: 6175 6c74 2074 696d 656f 7574 2074 616b  ault timeout tak
+00010210: 6520 6566 6665 6374 2e0a 2020 2020 2020  e effect..      
+00010220: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00010230: 2020 2020 2020 2063 616c 6c61 626c 653a         callable:
+00010240: 2041 2072 656d 6f74 6520 6675 6e63 7469   A remote functi
+00010250: 6f6e 206f 626a 6563 7420 706f 696e 7469  on object pointi
+00010260: 6e67 2074 6f20 7468 6520 636c 6f75 6420  ng to the cloud 
+00010270: 6173 7365 7473 2063 7265 6174 6564 0a20  assets created. 
+00010280: 2020 2020 2020 2020 2020 2069 6e20 7468             in th
+00010290: 6520 6261 636b 6772 6f75 6e64 2074 6f20  e background to 
+000102a0: 7375 7070 6f72 7420 7468 6520 7265 6d6f  support the remo
+000102b0: 7465 2065 7865 6375 7469 6f6e 2e20 5468  te execution. Th
+000102c0: 6520 636c 6f75 6420 6173 7365 7473 2063  e cloud assets c
+000102d0: 616e 2062 650a 2020 2020 2020 2020 2020  an be.          
+000102e0: 2020 6c6f 6361 7465 6420 7468 726f 7567    located throug
+000102f0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
+00010300: 7072 6f70 6572 7469 6573 2073 6574 2069  properties set i
+00010310: 6e20 7468 6520 6f62 6a65 6374 3a0a 0a20  n the object:.. 
+00010320: 2020 2020 2020 2020 2020 2060 6269 6766             `bigf
+00010330: 7261 6d65 735f 636c 6f75 645f 6675 6e63  rames_cloud_func
+00010340: 7469 6f6e 6020 2d20 5468 6520 676f 6f67  tion` - The goog
+00010350: 6c65 2063 6c6f 7564 2066 756e 6374 696f  le cloud functio
+00010360: 6e20 6465 706c 6f79 6564 2066 6f72 2074  n deployed for t
+00010370: 6865 2075 7365 7220 6465 6669 6e65 6420  he user defined 
+00010380: 636f 6465 2e0a 0a20 2020 2020 2020 2020  code...         
+00010390: 2020 2060 6269 6766 7261 6d65 735f 7265     `bigframes_re
+000103a0: 6d6f 7465 5f66 756e 6374 696f 6e60 202d  mote_function` -
+000103b0: 2054 6865 2062 6967 7175 6572 7920 7265   The bigquery re
+000103c0: 6d6f 7465 2066 756e 6374 696f 6e20 6361  mote function ca
+000103d0: 7061 626c 6520 6f66 2063 616c 6c69 6e67  pable of calling
+000103e0: 2069 6e74 6f20 6062 6967 6672 616d 6573   into `bigframes
+000103f0: 5f63 6c6f 7564 5f66 756e 6374 696f 6e60  _cloud_function`
+00010400: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00010410: 2020 2020 2020 7265 7475 726e 2062 6967        return big
+00010420: 6672 616d 6573 5f72 6628 0a20 2020 2020  frames_rf(.     
+00010430: 2020 2020 2020 2069 6e70 7574 5f74 7970         input_typ
+00010440: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00010450: 6f75 7470 7574 5f74 7970 652c 0a20 2020  output_type,.   
+00010460: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+00010470: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
+00010480: 2020 2064 6174 6173 6574 3d64 6174 6173     dataset=datas
+00010490: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+000104a0: 6269 6771 7565 7279 5f63 6f6e 6e65 6374  bigquery_connect
+000104b0: 696f 6e3d 6269 6771 7565 7279 5f63 6f6e  ion=bigquery_con
+000104c0: 6e65 6374 696f 6e2c 0a20 2020 2020 2020  nection,.       
+000104d0: 2020 2020 2072 6575 7365 3d72 6575 7365       reuse=reuse
+000104e0: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
+000104f0: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
+00010500: 2020 2020 2070 6163 6b61 6765 733d 7061       packages=pa
+00010510: 636b 6167 6573 2c0a 2020 2020 2020 2020  ckages,.        
+00010520: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+00010530: 6f6e 5f73 6572 7669 6365 5f61 6363 6f75  on_service_accou
+00010540: 6e74 3d63 6c6f 7564 5f66 756e 6374 696f  nt=cloud_functio
+00010550: 6e5f 7365 7276 6963 655f 6163 636f 756e  n_service_accoun
+00010560: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
+00010570: 6c6f 7564 5f66 756e 6374 696f 6e5f 6b6d  loud_function_km
+00010580: 735f 6b65 795f 6e61 6d65 3d63 6c6f 7564  s_key_name=cloud
+00010590: 5f66 756e 6374 696f 6e5f 6b6d 735f 6b65  _function_kms_ke
+000105a0: 795f 6e61 6d65 2c0a 2020 2020 2020 2020  y_name,.        
+000105b0: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+000105c0: 6f6e 5f64 6f63 6b65 725f 7265 706f 7369  on_docker_reposi
+000105d0: 746f 7279 3d63 6c6f 7564 5f66 756e 6374  tory=cloud_funct
+000105e0: 696f 6e5f 646f 636b 6572 5f72 6570 6f73  ion_docker_repos
+000105f0: 6974 6f72 792c 0a20 2020 2020 2020 2020  itory,.         
+00010600: 2020 206d 6178 5f62 6174 6368 696e 675f     max_batching_
+00010610: 726f 7773 3d6d 6178 5f62 6174 6368 696e  rows=max_batchin
+00010620: 675f 726f 7773 2c0a 2020 2020 2020 2020  g_rows,.        
+00010630: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+00010640: 6f6e 5f74 696d 656f 7574 3d63 6c6f 7564  on_timeout=cloud
+00010650: 5f66 756e 6374 696f 6e5f 7469 6d65 6f75  _function_timeou
+00010660: 742c 0a20 2020 2020 2020 2029 0a0a 2020  t,.        )..  
+00010670: 2020 6465 6620 7265 6164 5f67 6271 5f66    def read_gbq_f
+00010680: 756e 6374 696f 6e28 0a20 2020 2020 2020  unction(.       
+00010690: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+000106a0: 756e 6374 696f 6e5f 6e61 6d65 3a20 7374  unction_name: st
+000106b0: 722c 0a20 2020 2029 3a0a 2020 2020 2020  r,.    ):.      
+000106c0: 2020 2222 224c 6f61 6473 2061 2042 6967    """Loads a Big
+000106d0: 5175 6572 7920 6675 6e63 7469 6f6e 2066  Query function f
+000106e0: 726f 6d20 4269 6751 7565 7279 2e0a 0a20  rom BigQuery... 
+000106f0: 2020 2020 2020 2054 6865 6e20 6974 2063         Then it c
+00010700: 616e 2062 6520 6170 706c 6965 6420 746f  an be applied to
+00010710: 2061 2044 6174 6146 7261 6d65 206f 7220   a DataFrame or 
+00010720: 5365 7269 6573 2e0a 0a20 2020 2020 2020  Series...       
+00010730: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
+00010740: 2020 2020 2020 2054 6865 2072 6574 7572         The retur
+00010750: 6e20 7479 7065 206f 6620 7468 6520 6675  n type of the fu
+00010760: 6e63 7469 6f6e 206d 7573 7420 6265 2065  nction must be e
+00010770: 7870 6c69 6369 746c 7920 7370 6563 6966  xplicitly specif
+00010780: 6965 6420 696e 2074 6865 0a20 2020 2020  ied in the.     
+00010790: 2020 2020 2020 2066 756e 6374 696f 6e27         function'
+000107a0: 7320 6f72 6967 696e 616c 2064 6566 696e  s original defin
+000107b0: 6974 696f 6e20 6576 656e 2069 6620 6e6f  ition even if no
+000107c0: 7420 6f74 6865 7277 6973 6520 7265 7175  t otherwise requ
+000107d0: 6972 6564 2e0a 0a20 2020 2020 2020 2042  ired...        B
+000107e0: 6967 5175 6572 7920 5574 696c 7320 7072  igQuery Utils pr
+000107f0: 6f76 6964 6573 206d 616e 7920 7075 626c  ovides many publ
+00010800: 6963 2066 756e 6374 696f 6e73 2075 6e64  ic functions und
+00010810: 6572 2074 6865 2060 6062 7175 7469 6c60  er the ``bqutil`
+00010820: 6020 7072 6f6a 6563 7420 6f6e 2047 6f6f  ` project on Goo
+00010830: 676c 6520 436c 6f75 6420 506c 6174 666f  gle Cloud Platfo
+00010840: 726d 2070 726f 6a65 6374 0a20 2020 2020  rm project.     
+00010850: 2020 2028 5365 653a 2068 7474 7073 3a2f     (See: https:/
+00010860: 2f67 6974 6875 622e 636f 6d2f 476f 6f67  /github.com/Goog
+00010870: 6c65 436c 6f75 6450 6c61 7466 6f72 6d2f  leCloudPlatform/
+00010880: 6269 6771 7565 7279 2d75 7469 6c73 2f74  bigquery-utils/t
+00010890: 7265 652f 6d61 7374 6572 2f75 6466 7323  ree/master/udfs#
+000108a0: 7573 696e 672d 7468 652d 7564 6673 292e  using-the-udfs).
+000108b0: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
+000108c0: 2063 6865 636b 6f75 7420 436f 6d6d 756e   checkout Commun
+000108d0: 6974 7920 5544 4673 2074 6f20 7573 6520  ity UDFs to use 
+000108e0: 636f 6d6d 756e 6974 792d 636f 6e74 7269  community-contri
+000108f0: 6275 7465 6420 6675 6e63 7469 6f6e 732e  buted functions.
+00010900: 0a20 2020 2020 2020 2028 5365 653a 2068  .        (See: h
+00010910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00010920: 6d2f 476f 6f67 6c65 436c 6f75 6450 6c61  m/GoogleCloudPla
+00010930: 7466 6f72 6d2f 6269 6771 7565 7279 2d75  tform/bigquery-u
+00010940: 7469 6c73 2f74 7265 652f 6d61 7374 6572  tils/tree/master
+00010950: 2f75 6466 732f 636f 6d6d 756e 6974 7923  /udfs/community#
+00010960: 636f 6d6d 756e 6974 792d 7564 6673 292e  community-udfs).
+00010970: 0a0a 2020 2020 2020 2020 2a2a 4578 616d  ..        **Exam
+00010980: 706c 6573 3a2a 2a0a 0a20 2020 2020 2020  ples:**..       
+00010990: 2055 7365 2074 6865 2060 6063 775f 6c6f   Use the ``cw_lo
+000109a0: 7765 725f 6361 7365 5f61 7363 6969 5f6f  wer_case_ascii_o
+000109b0: 6e6c 7960 6020 6675 6e63 7469 6f6e 2066  nly`` function f
+000109c0: 726f 6d20 436f 6d6d 756e 6974 7920 5544  rom Community UD
+000109d0: 4673 2e0a 2020 2020 2020 2020 2868 7474  Fs..        (htt
+000109e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000109f0: 476f 6f67 6c65 436c 6f75 6450 6c61 7466  GoogleCloudPlatf
+00010a00: 6f72 6d2f 6269 6771 7565 7279 2d75 7469  orm/bigquery-uti
+00010a10: 6c73 2f62 6c6f 622f 6d61 7374 6572 2f75  ls/blob/master/u
+00010a20: 6466 732f 636f 6d6d 756e 6974 792f 6377  dfs/community/cw
+00010a30: 5f6c 6f77 6572 5f63 6173 655f 6173 6369  _lower_case_asci
+00010a40: 695f 6f6e 6c79 2e73 716c 7829 0a0a 2020  i_only.sqlx)..  
+00010a50: 2020 2020 2020 2020 2020 3e3e 3e20 696d            >>> im
+00010a60: 706f 7274 2062 6967 6672 616d 6573 2e70  port bigframes.p
+00010a70: 616e 6461 7320 6173 2062 7064 0a20 2020  andas as bpd.   
+00010a80: 2020 2020 2020 2020 203e 3e3e 2062 7064           >>> bpd
+00010a90: 2e6f 7074 696f 6e73 2e64 6973 706c 6179  .options.display
+00010aa0: 2e70 726f 6772 6573 735f 6261 7220 3d20  .progress_bar = 
+00010ab0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+00010ac0: 2020 3e3e 3e20 6466 203d 2062 7064 2e44    >>> df = bpd.D
+00010ad0: 6174 6146 7261 6d65 287b 2769 6427 3a20  ataFrame({'id': 
+00010ae0: 5b31 2c20 322c 2033 5d2c 2027 6e61 6d65  [1, 2, 3], 'name
+00010af0: 273a 205b 2741 5552 c389 4c49 4527 2c20  ': ['AUR..LIE', 
+00010b00: 2743 c389 4c45 5354 494e 4527 2c20 2744  'C..LESTINE', 'D
+00010b10: 4150 484e c389 275d 7d29 0a20 2020 2020  APHN..']}).     
+00010b20: 2020 2020 2020 203e 3e3e 2064 660a 2020         >>> df.  
+00010b30: 2020 2020 2020 2020 2020 2020 2069 6420               id 
+00010b40: 2020 2020 2020 6e61 6d65 0a20 2020 2020        name.     
+00010b50: 2020 2020 2020 2030 2020 2031 2020 2020         0   1    
+00010b60: 4155 52c3 894c 4945 0a20 2020 2020 2020  AUR..LIE.       
+00010b70: 2020 2020 2031 2020 2032 2020 43c3 894c       1   2  C..L
+00010b80: 4553 5449 4e45 0a20 2020 2020 2020 2020  ESTINE.         
+00010b90: 2020 2032 2020 2033 2020 2020 2044 4150     2   3     DAP
+00010ba0: 484e c389 0a20 2020 2020 2020 2020 2020  HN...           
+00010bb0: 203c 424c 414e 4b4c 494e 453e 0a20 2020   <BLANKLINE>.   
+00010bc0: 2020 2020 2020 2020 205b 3320 726f 7773           [3 rows
+00010bd0: 2078 2032 2063 6f6c 756d 6e73 5d0a 0a20   x 2 columns].. 
+00010be0: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
+00010bf0: 756e 6320 3d20 6270 642e 7265 6164 5f67  unc = bpd.read_g
+00010c00: 6271 5f66 756e 6374 696f 6e28 2262 7175  bq_function("bqu
+00010c10: 7469 6c2e 666e 2e63 775f 6c6f 7765 725f  til.fn.cw_lower_
+00010c20: 6361 7365 5f61 7363 6969 5f6f 6e6c 7922  case_ascii_only"
+00010c30: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00010c40: 3e20 6466 3120 3d20 6466 2e61 7373 6967  > df1 = df.assig
+00010c50: 6e28 6e65 775f 6e61 6d65 3d64 665b 276e  n(new_name=df['n
+00010c60: 616d 6527 5d2e 6170 706c 7928 6675 6e63  ame'].apply(func
+00010c70: 2929 0a20 2020 2020 2020 2020 2020 203e  )).            >
+00010c80: 3e3e 2064 6631 0a20 2020 2020 2020 2020  >> df1.         
+00010c90: 2020 2020 2020 6964 2020 2020 2020 206e        id       n
+00010ca0: 616d 6520 2020 6e65 775f 6e61 6d65 0a20  ame   new_name. 
+00010cb0: 2020 2020 2020 2020 2020 2030 2020 2031             0   1
+00010cc0: 2020 2020 4155 52c3 894c 4945 2020 2020      AUR..LIE    
+00010cd0: 6175 72c3 896c 6965 0a20 2020 2020 2020  aur..lie.       
+00010ce0: 2020 2020 2031 2020 2032 2020 43c3 894c       1   2  C..L
+00010cf0: 4553 5449 4e45 2020 63c3 896c 6573 7469  ESTINE  c..lesti
+00010d00: 6e65 0a20 2020 2020 2020 2020 2020 2032  ne.            2
+00010d10: 2020 2033 2020 2020 2044 4150 484e c389     3     DAPHN..
+00010d20: 2020 2020 2064 6170 686e c389 0a20 2020       daphn...   
+00010d30: 2020 2020 2020 2020 203c 424c 414e 4b4c           <BLANKL
+00010d40: 494e 453e 0a20 2020 2020 2020 2020 2020  INE>.           
+00010d50: 205b 3320 726f 7773 2078 2033 2063 6f6c   [3 rows x 3 col
+00010d60: 756d 6e73 5d0a 0a20 2020 2020 2020 2041  umns]..        A
+00010d70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00010d80: 2066 756e 6374 696f 6e5f 6e61 6d65 2028   function_name (
+00010d90: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00010da0: 2020 2020 2020 7468 6520 6675 6e63 7469        the functi
+00010db0: 6f6e 2773 206e 616d 6520 696e 2042 6967  on's name in Big
+00010dc0: 5175 6572 7920 696e 2074 6865 2066 6f72  Query in the for
+00010dd0: 6d61 740a 2020 2020 2020 2020 2020 2020  mat.            
+00010de0: 2020 2020 6070 726f 6a65 6374 5f69 642e      `project_id.
+00010df0: 6461 7461 7365 745f 6964 2e66 756e 6374  dataset_id.funct
+00010e00: 696f 6e5f 6e61 6d65 602c 206f 720a 2020  ion_name`, or.  
+00010e10: 2020 2020 2020 2020 2020 2020 2020 6064                `d
+00010e20: 6174 6173 6574 5f69 642e 6675 6e63 7469  ataset_id.functi
+00010e30: 6f6e 5f6e 616d 6560 2074 6f20 6c6f 6164  on_name` to load
+00010e40: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
+00010e50: 7420 7072 6f6a 6563 742c 206f 720a 2020  t project, or.  
+00010e60: 2020 2020 2020 2020 2020 2020 2020 6066                `f
+00010e70: 756e 6374 696f 6e5f 6e61 6d65 6020 746f  unction_name` to
+00010e80: 206c 6f61 6420 6672 6f6d 2074 6865 2064   load from the d
+00010e90: 6566 6175 6c74 2070 726f 6a65 6374 2061  efault project a
+00010ea0: 6e64 2074 6865 2064 6174 6173 6574 0a20  nd the dataset. 
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00010ec0: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+00010ed0: 6865 2063 7572 7265 6e74 2073 6573 7369  he current sessi
+00010ee0: 6f6e 2e0a 0a20 2020 2020 2020 2052 6574  on...        Ret
+00010ef0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00010f00: 2020 6361 6c6c 6162 6c65 3a20 4120 6675    callable: A fu
+00010f10: 6e63 7469 6f6e 206f 626a 6563 7420 706f  nction object po
+00010f20: 696e 7469 6e67 2074 6f20 7468 6520 4269  inting to the Bi
+00010f30: 6751 7565 7279 2066 756e 6374 696f 6e20  gQuery function 
+00010f40: 7265 6164 0a20 2020 2020 2020 2020 2020  read.           
+00010f50: 2066 726f 6d20 4269 6751 7565 7279 2e0a   from BigQuery..
+00010f60: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00010f70: 206f 626a 6563 7420 6973 2073 696d 696c   object is simil
+00010f80: 6172 2074 6f20 7468 6520 6f6e 6520 6372  ar to the one cr
+00010f90: 6561 7465 6420 6279 2074 6865 2060 7265  eated by the `re
+00010fa0: 6d6f 7465 5f66 756e 6374 696f 6e60 0a20  mote_function`. 
+00010fb0: 2020 2020 2020 2020 2020 2064 6563 6f72             decor
+00010fc0: 6174 6f72 2c20 696e 636c 7564 696e 6720  ator, including 
+00010fd0: 7468 6520 6062 6967 6672 616d 6573 5f72  the `bigframes_r
+00010fe0: 656d 6f74 655f 6675 6e63 7469 6f6e 6020  emote_function` 
+00010ff0: 7072 6f70 6572 7479 2c20 6275 740a 2020  property, but.  
+00011000: 2020 2020 2020 2020 2020 6e6f 7420 696e            not in
+00011010: 636c 7564 696e 6720 7468 6520 6062 6967  cluding the `big
+00011020: 6672 616d 6573 5f63 6c6f 7564 5f66 756e  frames_cloud_fun
+00011030: 6374 696f 6e60 2070 726f 7065 7274 792e  ction` property.
+00011040: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00011050: 2020 2020 2020 7265 7475 726e 2062 6967        return big
+00011060: 6672 616d 6573 5f72 6766 280a 2020 2020  frames_rgf(.    
+00011070: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+00011080: 5f6e 616d 653d 6675 6e63 7469 6f6e 5f6e  _name=function_n
+00011090: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+000110a0: 2073 6573 7369 6f6e 3d73 656c 662c 0a20   session=self,. 
+000110b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+000110c0: 6620 5f70 7265 7061 7265 5f71 7565 7279  f _prepare_query
+000110d0: 5f6a 6f62 5f63 6f6e 6669 6728 0a20 2020  _job_config(.   
+000110e0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000110f0: 2020 206a 6f62 5f63 6f6e 6669 673a 204f     job_config: O
+00011100: 7074 696f 6e61 6c5b 6269 6771 7565 7279  ptional[bigquery
+00011110: 2e51 7565 7279 4a6f 6243 6f6e 6669 675d  .QueryJobConfig]
+00011120: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
+00011130: 3e20 6269 6771 7565 7279 2e51 7565 7279  > bigquery.Query
+00011140: 4a6f 6243 6f6e 6669 673a 0a20 2020 2020  JobConfig:.     
+00011150: 2020 2069 6620 6a6f 625f 636f 6e66 6967     if job_config
+00011160: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00011170: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00011180: 203d 2062 6967 7175 6572 792e 5175 6572   = bigquery.Quer
+00011190: 794a 6f62 436f 6e66 6967 2829 0a20 2020  yJobConfig().   
+000111a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000111b0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+000111c0: 6120 636f 7079 2073 6f20 7468 6174 2077  a copy so that w
+000111d0: 6520 646f 6e27 7420 6d75 7461 7465 2074  e don't mutate t
+000111e0: 6865 206f 7269 6769 6e61 6c20 636f 6e66  he original conf
+000111f0: 6967 2070 6173 7365 640a 2020 2020 2020  ig passed.      
+00011200: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00011210: 203d 2074 7970 696e 672e 6361 7374 280a   = typing.cast(.
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
+00011240: 6243 6f6e 6669 672c 0a20 2020 2020 2020  bConfig,.       
+00011250: 2020 2020 2020 2020 2062 6967 7175 6572           bigquer
+00011260: 792e 5175 6572 794a 6f62 436f 6e66 6967  y.QueryJobConfig
+00011270: 2e66 726f 6d5f 6170 695f 7265 7072 286a  .from_api_repr(j
+00011280: 6f62 5f63 6f6e 6669 672e 746f 5f61 7069  ob_config.to_api
+00011290: 5f72 6570 7228 2929 2c0a 2020 2020 2020  _repr()),.      
+000112a0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000112b0: 2069 6620 6269 6766 7261 6d65 732e 6f70   if bigframes.op
+000112c0: 7469 6f6e 732e 636f 6d70 7574 652e 6d61  tions.compute.ma
+000112d0: 7869 6d75 6d5f 6279 7465 735f 6269 6c6c  ximum_bytes_bill
+000112e0: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ed is not None:.
+000112f0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+00011300: 636f 6e66 6967 2e6d 6178 696d 756d 5f62  config.maximum_b
+00011310: 7974 6573 5f62 696c 6c65 6420 3d20 280a  ytes_billed = (.
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 6269 6766 7261 6d65 732e 6f70 7469 6f6e  bigframes.option
+00011340: 732e 636f 6d70 7574 652e 6d61 7869 6d75  s.compute.maximu
+00011350: 6d5f 6279 7465 735f 6269 6c6c 6564 0a20  m_bytes_billed. 
+00011360: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00011370: 2020 2020 2020 6966 2073 656c 662e 5f62        if self._b
+00011380: 715f 6b6d 735f 6b65 795f 6e61 6d65 3a0a  q_kms_key_name:.
+00011390: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+000113a0: 636f 6e66 6967 2e64 6573 7469 6e61 7469  config.destinati
+000113b0: 6f6e 5f65 6e63 7279 7074 696f 6e5f 636f  on_encryption_co
+000113c0: 6e66 6967 7572 6174 696f 6e20 3d20 280a  nfiguration = (.
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113e0: 6269 6771 7565 7279 2e45 6e63 7279 7074  bigquery.Encrypt
+000113f0: 696f 6e43 6f6e 6669 6775 7261 7469 6f6e  ionConfiguration
+00011400: 286b 6d73 5f6b 6579 5f6e 616d 653d 7365  (kms_key_name=se
+00011410: 6c66 2e5f 6271 5f6b 6d73 5f6b 6579 5f6e  lf._bq_kms_key_n
+00011420: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00011430: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00011440: 726e 206a 6f62 5f63 6f6e 6669 670a 0a20  rn job_config.. 
+00011450: 2020 2064 6566 205f 7072 6570 6172 655f     def _prepare_
+00011460: 6c6f 6164 5f6a 6f62 5f63 6f6e 6669 6728  load_job_config(
+00011470: 7365 6c66 2920 2d3e 2062 6967 7175 6572  self) -> bigquer
+00011480: 792e 4c6f 6164 4a6f 6243 6f6e 6669 673a  y.LoadJobConfig:
+00011490: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+000114a0: 6520 6120 636f 7079 2073 6f20 7468 6174  e a copy so that
+000114b0: 2077 6520 646f 6e27 7420 6d75 7461 7465   we don't mutate
+000114c0: 2074 6865 206f 7269 6769 6e61 6c20 636f   the original co
+000114d0: 6e66 6967 2070 6173 7365 640a 2020 2020  nfig passed.    
+000114e0: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
+000114f0: 2062 6967 7175 6572 792e 4c6f 6164 4a6f   bigquery.LoadJo
+00011500: 6243 6f6e 6669 6728 290a 0a20 2020 2020  bConfig()..     
+00011510: 2020 2069 6620 7365 6c66 2e5f 6271 5f6b     if self._bq_k
+00011520: 6d73 5f6b 6579 5f6e 616d 653a 0a20 2020  ms_key_name:.   
+00011530: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+00011540: 6669 672e 6465 7374 696e 6174 696f 6e5f  fig.destination_
+00011550: 656e 6372 7970 7469 6f6e 5f63 6f6e 6669  encryption_confi
+00011560: 6775 7261 7469 6f6e 203d 2028 0a20 2020  guration = (.   
+00011570: 2020 2020 2020 2020 2020 2020 2062 6967               big
+00011580: 7175 6572 792e 456e 6372 7970 7469 6f6e  query.Encryption
+00011590: 436f 6e66 6967 7572 6174 696f 6e28 6b6d  Configuration(km
+000115a0: 735f 6b65 795f 6e61 6d65 3d73 656c 662e  s_key_name=self.
+000115b0: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
+000115c0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+000115d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000115e0: 6a6f 625f 636f 6e66 6967 0a0a 2020 2020  job_config..    
+000115f0: 6465 6620 5f70 7265 7061 7265 5f63 6f70  def _prepare_cop
+00011600: 795f 6a6f 625f 636f 6e66 6967 2873 656c  y_job_config(sel
+00011610: 6629 202d 3e20 6269 6771 7565 7279 2e43  f) -> bigquery.C
+00011620: 6f70 794a 6f62 436f 6e66 6967 3a0a 2020  opyJobConfig:.  
+00011630: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
+00011640: 2063 6f70 7920 736f 2074 6861 7420 7765   copy so that we
+00011650: 2064 6f6e 2774 206d 7574 6174 6520 7468   don't mutate th
+00011660: 6520 6f72 6967 696e 616c 2063 6f6e 6669  e original confi
+00011670: 6720 7061 7373 6564 0a20 2020 2020 2020  g passed.       
+00011680: 206a 6f62 5f63 6f6e 6669 6720 3d20 6269   job_config = bi
+00011690: 6771 7565 7279 2e43 6f70 794a 6f62 436f  gquery.CopyJobCo
+000116a0: 6e66 6967 2829 0a0a 2020 2020 2020 2020  nfig()..        
+000116b0: 6966 2073 656c 662e 5f62 715f 6b6d 735f  if self._bq_kms_
+000116c0: 6b65 795f 6e61 6d65 3a0a 2020 2020 2020  key_name:.      
+000116d0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+000116e0: 2e64 6573 7469 6e61 7469 6f6e 5f65 6e63  .destination_enc
+000116f0: 7279 7074 696f 6e5f 636f 6e66 6967 7572  ryption_configur
+00011700: 6174 696f 6e20 3d20 280a 2020 2020 2020  ation = (.      
+00011710: 2020 2020 2020 2020 2020 6269 6771 7565            bigque
+00011720: 7279 2e45 6e63 7279 7074 696f 6e43 6f6e  ry.EncryptionCon
+00011730: 6669 6775 7261 7469 6f6e 286b 6d73 5f6b  figuration(kms_k
+00011740: 6579 5f6e 616d 653d 7365 6c66 2e5f 6271  ey_name=self._bq
+00011750: 5f6b 6d73 5f6b 6579 5f6e 616d 6529 0a20  _kms_key_name). 
+00011760: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00011770: 2020 2020 2020 7265 7475 726e 206a 6f62        return job
+00011780: 5f63 6f6e 6669 670a 0a20 2020 2064 6566  _config..    def
+00011790: 205f 7374 6172 745f 7175 6572 7928 0a20   _start_query(. 
+000117a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000117b0: 2020 2020 2073 716c 3a20 7374 722c 0a20       sql: str,. 
+000117c0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+000117d0: 673a 204f 7074 696f 6e61 6c5b 6269 6771  g: Optional[bigq
+000117e0: 7565 7279 2e6a 6f62 2e51 7565 7279 4a6f  uery.job.QueryJo
+000117f0: 6243 6f6e 6669 675d 203d 204e 6f6e 652c  bConfig] = None,
+00011800: 0a20 2020 2020 2020 206d 6178 5f72 6573  .        max_res
+00011810: 756c 7473 3a20 4f70 7469 6f6e 616c 5b69  ults: Optional[i
+00011820: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00011830: 2020 2020 7469 6d65 6f75 743a 204f 7074      timeout: Opt
+00011840: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
+00011850: 6f6e 652c 0a20 2020 2029 202d 3e20 5475  one,.    ) -> Tu
+00011860: 706c 655b 6269 6771 7565 7279 2e74 6162  ple[bigquery.tab
+00011870: 6c65 2e52 6f77 4974 6572 6174 6f72 2c20  le.RowIterator, 
+00011880: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
+00011890: 625d 3a0a 2020 2020 2020 2020 2222 220a  b]:.        """.
+000118a0: 2020 2020 2020 2020 5374 6172 7473 2042          Starts B
+000118b0: 6967 5175 6572 7920 7175 6572 7920 6a6f  igQuery query jo
+000118c0: 6220 616e 6420 7761 6974 7320 666f 7220  b and waits for 
+000118d0: 7265 7375 6c74 732e 0a20 2020 2020 2020  results..       
+000118e0: 2022 2222 0a20 2020 2020 2020 206a 6f62   """.        job
+000118f0: 5f63 6f6e 6669 6720 3d20 7365 6c66 2e5f  _config = self._
+00011900: 7072 6570 6172 655f 7175 6572 795f 6a6f  prepare_query_jo
+00011910: 625f 636f 6e66 6967 286a 6f62 5f63 6f6e  b_config(job_con
+00011920: 6669 6729 0a20 2020 2020 2020 2072 6574  fig).        ret
+00011930: 7572 6e20 6269 6766 7261 6d65 732e 7365  urn bigframes.se
+00011940: 7373 696f 6e2e 5f69 6f2e 6269 6771 7565  ssion._io.bigque
+00011950: 7279 2e73 7461 7274 5f71 7565 7279 5f77  ry.start_query_w
+00011960: 6974 685f 636c 6965 6e74 280a 2020 2020  ith_client(.    
+00011970: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
+00011980: 6c69 656e 742c 2073 716c 2c20 6a6f 625f  lient, sql, job_
+00011990: 636f 6e66 6967 2c20 6d61 785f 7265 7375  config, max_resu
+000119a0: 6c74 732c 2074 696d 656f 7574 0a20 2020  lts, timeout.   
+000119b0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+000119c0: 5f73 7461 7274 5f71 7565 7279 5f6d 6c5f  _start_query_ml_
+000119d0: 6464 6c28 0a20 2020 2020 2020 2073 656c  ddl(.        sel
+000119e0: 662c 0a20 2020 2020 2020 2073 716c 3a20  f,.        sql: 
+000119f0: 7374 722c 0a20 2020 2029 202d 3e20 5475  str,.    ) -> Tu
+00011a00: 706c 655b 6269 6771 7565 7279 2e74 6162  ple[bigquery.tab
+00011a10: 6c65 2e52 6f77 4974 6572 6174 6f72 2c20  le.RowIterator, 
+00011a20: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
+00011a30: 625d 3a0a 2020 2020 2020 2020 2222 220a  b]:.        """.
+00011a40: 2020 2020 2020 2020 5374 6172 7473 2042          Starts B
+00011a50: 6967 5175 6572 7920 4d4c 2044 444c 2071  igQuery ML DDL q
+00011a60: 7565 7279 206a 6f62 2028 4352 4541 5445  uery job (CREATE
+00011a70: 204d 4f44 454c 2f41 4c54 4552 204d 4f44   MODEL/ALTER MOD
+00011a80: 454c 2f2e 2e2e 2920 616e 640a 2020 2020  EL/...) and.    
+00011a90: 2020 2020 7761 6974 7320 666f 7220 7265      waits for re
+00011aa0: 7375 6c74 732e 0a20 2020 2020 2020 2022  sults..        "
+00011ab0: 2222 0a20 2020 2020 2020 206a 6f62 5f63  "".        job_c
+00011ac0: 6f6e 6669 6720 3d20 7365 6c66 2e5f 7072  onfig = self._pr
+00011ad0: 6570 6172 655f 7175 6572 795f 6a6f 625f  epare_query_job_
+00011ae0: 636f 6e66 6967 2829 0a0a 2020 2020 2020  config()..      
+00011af0: 2020 2320 4251 4d4c 2065 7870 6563 7473    # BQML expects
+00011b00: 206b 6d73 5f6b 6579 5f6e 616d 6520 7468   kms_key_name th
+00011b10: 726f 7567 6820 4f50 5449 4f4e 5320 616e  rough OPTIONS an
+00011b20: 6420 6e6f 7420 7468 726f 7567 6820 6a6f  d not through jo
+00011b30: 6220 636f 6e66 6967 2c0a 2020 2020 2020  b config,.      
+00011b40: 2020 2320 736f 2077 6520 6d75 7374 2072    # so we must r
+00011b50: 6573 6574 2061 6e79 2065 6e63 7279 7074  eset any encrypt
+00011b60: 696f 6e20 7365 7420 696e 2074 6865 206a  ion set in the j
+00011b70: 6f62 2063 6f6e 6669 670a 2020 2020 2020  ob config.      
+00011b80: 2020 2320 6874 7470 733a 2f2f 636c 6f75    # https://clou
+00011b90: 642e 676f 6f67 6c65 2e63 6f6d 2f62 6967  d.google.com/big
+00011ba0: 7175 6572 792f 646f 6373 2f63 7573 746f  query/docs/custo
+00011bb0: 6d65 722d 6d61 6e61 6765 642d 656e 6372  mer-managed-encr
+00011bc0: 7970 7469 6f6e 2365 6e63 7279 7074 2d6d  yption#encrypt-m
+00011bd0: 6f64 656c 0a20 2020 2020 2020 206a 6f62  odel.        job
+00011be0: 5f63 6f6e 6669 672e 6465 7374 696e 6174  _config.destinat
+00011bf0: 696f 6e5f 656e 6372 7970 7469 6f6e 5f63  ion_encryption_c
+00011c00: 6f6e 6669 6775 7261 7469 6f6e 203d 204e  onfiguration = N
+00011c10: 6f6e 650a 0a20 2020 2020 2020 2072 6574  one..        ret
+00011c20: 7572 6e20 6269 6766 7261 6d65 732e 7365  urn bigframes.se
+00011c30: 7373 696f 6e2e 5f69 6f2e 6269 6771 7565  ssion._io.bigque
+00011c40: 7279 2e73 7461 7274 5f71 7565 7279 5f77  ry.start_query_w
+00011c50: 6974 685f 636c 6965 6e74 280a 2020 2020  ith_client(.    
+00011c60: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
+00011c70: 6c69 656e 742c 2073 716c 2c20 6a6f 625f  lient, sql, job_
+00011c80: 636f 6e66 6967 0a20 2020 2020 2020 2029  config.        )
+00011c90: 0a0a 2020 2020 6465 6620 5f63 6163 6865  ..    def _cache
+00011ca0: 5f77 6974 685f 636c 7573 7465 725f 636f  _with_cluster_co
+00011cb0: 6c73 280a 2020 2020 2020 2020 7365 6c66  ls(.        self
+00011cc0: 2c20 6172 7261 795f 7661 6c75 653a 2063  , array_value: c
+00011cd0: 6f72 652e 4172 7261 7956 616c 7565 2c20  ore.ArrayValue, 
+00011ce0: 636c 7573 7465 725f 636f 6c73 3a20 7479  cluster_cols: ty
+00011cf0: 7069 6e67 2e53 6571 7565 6e63 655b 7374  ping.Sequence[st
+00011d00: 725d 0a20 2020 2029 202d 3e20 636f 7265  r].    ) -> core
+00011d10: 2e41 7272 6179 5661 6c75 653a 0a20 2020  .ArrayValue:.   
+00011d20: 2020 2020 2022 2222 4578 6563 7574 6573       """Executes
+00011d30: 2074 6865 2071 7565 7279 2061 6e64 2075   the query and u
+00011d40: 7365 7320 7468 6520 7265 7375 6c74 696e  ses the resultin
+00011d50: 6720 7461 626c 6520 746f 2072 6577 7269  g table to rewri
+00011d60: 7465 2066 7574 7572 6520 6578 6563 7574  te future execut
+00011d70: 696f 6e73 2e22 2222 0a20 2020 2020 2020  ions.""".       
+00011d80: 2023 2054 4f44 4f3a 2055 7365 2074 6869   # TODO: Use thi
+00011d90: 7320 666f 7220 616c 6c20 6578 6563 7574  s for all execut
+00011da0: 696f 6e73 3f20 5072 6f62 6c65 6d20 6973  ions? Problem is
+00011db0: 2074 6861 7420 6361 6368 696e 6720 6d61   that caching ma
+00011dc0: 7465 7269 616c 697a 6573 2065 7874 7261  terializes extra
+00011dd0: 0a20 2020 2020 2020 2023 206f 7264 6572  .        # order
+00011de0: 696e 6720 636f 6c75 6d6e 730a 2020 2020  ing columns.    
+00011df0: 2020 2020 636f 6d70 696c 6564 5f76 616c      compiled_val
+00011e00: 7565 203d 2073 656c 662e 5f63 6f6d 7069  ue = self._compi
+00011e10: 6c65 5f6f 7264 6572 6564 2861 7272 6179  le_ordered(array
+00011e20: 5f76 616c 7565 290a 0a20 2020 2020 2020  _value)..       
+00011e30: 2069 6269 735f 6578 7072 203d 2063 6f6d   ibis_expr = com
+00011e40: 7069 6c65 645f 7661 6c75 652e 5f74 6f5f  piled_value._to_
+00011e50: 6962 6973 5f65 7870 7228 0a20 2020 2020  ibis_expr(.     
+00011e60: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
+00011e70: 6d6f 6465 3d22 756e 6f72 6465 7265 6422  mode="unordered"
+00011e80: 2c20 6578 706f 7365 5f68 6964 6465 6e5f  , expose_hidden_
+00011e90: 636f 6c73 3d54 7275 650a 2020 2020 2020  cols=True.      
+00011ea0: 2020 290a 2020 2020 2020 2020 746d 705f    ).        tmp_
+00011eb0: 7461 626c 6520 3d20 7365 6c66 2e5f 6962  table = self._ib
+00011ec0: 6973 5f74 6f5f 7465 6d70 5f74 6162 6c65  is_to_temp_table
+00011ed0: 280a 2020 2020 2020 2020 2020 2020 6962  (.            ib
+00011ee0: 6973 5f65 7870 722c 2063 6c75 7374 6572  is_expr, cluster
+00011ef0: 5f63 6f6c 733d 636c 7573 7465 725f 636f  _cols=cluster_co
+00011f00: 6c73 2c20 6170 695f 6e61 6d65 3d22 6361  ls, api_name="ca
+00011f10: 6368 6564 220a 2020 2020 2020 2020 290a  ched".        ).
+00011f20: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
+00011f30: 7072 6573 7369 6f6e 203d 2073 656c 662e  pression = self.
+00011f40: 6962 6973 5f63 6c69 656e 742e 7461 626c  ibis_client.tabl
+00011f50: 6528 0a20 2020 2020 2020 2020 2020 2074  e(.            t
+00011f60: 6d70 5f74 6162 6c65 2e74 6162 6c65 5f69  mp_table.table_i
+00011f70: 642c 0a20 2020 2020 2020 2020 2020 2073  d,.            s
+00011f80: 6368 656d 613d 746d 705f 7461 626c 652e  chema=tmp_table.
+00011f90: 6461 7461 7365 745f 6964 2c0a 2020 2020  dataset_id,.    
+00011fa0: 2020 2020 2020 2020 6461 7461 6261 7365          database
+00011fb0: 3d74 6d70 5f74 6162 6c65 2e70 726f 6a65  =tmp_table.proje
+00011fc0: 6374 2c0a 2020 2020 2020 2020 290a 2020  ct,.        ).  
+00011fd0: 2020 2020 2020 6e65 775f 636f 6c75 6d6e        new_column
+00011fe0: 7320 3d20 5b74 6162 6c65 5f65 7870 7265  s = [table_expre
+00011ff0: 7373 696f 6e5b 636f 6c75 6d6e 5d20 666f  ssion[column] fo
+00012000: 7220 636f 6c75 6d6e 2069 6e20 636f 6d70  r column in comp
+00012010: 696c 6564 5f76 616c 7565 2e63 6f6c 756d  iled_value.colum
+00012020: 6e5f 6964 735d 0a20 2020 2020 2020 206e  n_ids].        n
+00012030: 6577 5f68 6964 6465 6e5f 636f 6c75 6d6e  ew_hidden_column
+00012040: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+00012050: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
+00012060: 6f6e 5b63 6f6c 756d 6e5d 0a20 2020 2020  on[column].     
+00012070: 2020 2020 2020 2066 6f72 2063 6f6c 756d         for colum
+00012080: 6e20 696e 2063 6f6d 7069 6c65 645f 7661  n in compiled_va
+00012090: 6c75 652e 5f68 6964 6465 6e5f 6f72 6465  lue._hidden_orde
+000120a0: 7269 6e67 5f63 6f6c 756d 6e5f 6e61 6d65  ring_column_name
+000120b0: 730a 2020 2020 2020 2020 5d0a 2020 2020  s.        ].    
+000120c0: 2020 2020 2320 544f 444f 3a20 496e 7374      # TODO: Inst
+000120d0: 6561 642c 206b 6565 7020 7365 7373 696f  ead, keep sessio
+000120e0: 6e2d 7769 6465 206d 6170 206f 6620 6361  n-wide map of ca
+000120f0: 6368 6564 2072 6573 756c 7473 2061 6e64  ched results and
+00012100: 2061 7574 6f6d 6174 6963 616c 6c79 2072   automatically r
+00012110: 6575 7365 0a20 2020 2020 2020 2072 6574  euse.        ret
+00012120: 7572 6e20 636f 7265 2e41 7272 6179 5661  urn core.ArrayVa
+00012130: 6c75 652e 6672 6f6d 5f69 6269 7328 0a20  lue.from_ibis(. 
+00012140: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00012150: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+00012160: 6c65 5f65 7870 7265 7373 696f 6e2c 0a20  le_expression,. 
+00012170: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+00012180: 6e73 3d6e 6577 5f63 6f6c 756d 6e73 2c0a  ns=new_columns,.
+00012190: 2020 2020 2020 2020 2020 2020 6869 6464              hidd
+000121a0: 656e 5f6f 7264 6572 696e 675f 636f 6c75  en_ordering_colu
+000121b0: 6d6e 733d 6e65 775f 6869 6464 656e 5f63  mns=new_hidden_c
+000121c0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+000121d0: 2020 2020 6f72 6465 7269 6e67 3d63 6f6d      ordering=com
+000121e0: 7069 6c65 645f 7661 6c75 652e 5f6f 7264  piled_value._ord
+000121f0: 6572 696e 672c 0a20 2020 2020 2020 2029  ering,.        )
+00012200: 0a0a 2020 2020 6465 6620 5f63 6163 6865  ..    def _cache
+00012210: 5f77 6974 685f 6f66 6673 6574 7328 7365  _with_offsets(se
+00012220: 6c66 2c20 6172 7261 795f 7661 6c75 653a  lf, array_value:
+00012230: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
+00012240: 2920 2d3e 2063 6f72 652e 4172 7261 7956  ) -> core.ArrayV
+00012250: 616c 7565 3a0a 2020 2020 2020 2020 2222  alue:.        ""
+00012260: 2245 7865 6375 7465 7320 7468 6520 7175  "Executes the qu
+00012270: 6572 7920 616e 6420 7573 6573 2074 6865  ery and uses the
+00012280: 2072 6573 756c 7469 6e67 2074 6162 6c65   resulting table
+00012290: 2074 6f20 7265 7772 6974 6520 6675 7475   to rewrite futu
+000122a0: 7265 2065 7865 6375 7469 6f6e 732e 2222  re executions.""
+000122b0: 220a 2020 2020 2020 2020 2320 544f 444f  ".        # TODO
+000122c0: 3a20 5573 6520 7468 6973 2066 6f72 2061  : Use this for a
+000122d0: 6c6c 2065 7865 6375 7469 6f6e 733f 2050  ll executions? P
+000122e0: 726f 626c 656d 2069 7320 7468 6174 2063  roblem is that c
+000122f0: 6163 6869 6e67 206d 6174 6572 6961 6c69  aching materiali
+00012300: 7a65 7320 6578 7472 610a 2020 2020 2020  zes extra.      
+00012310: 2020 2320 6f72 6465 7269 6e67 2063 6f6c    # ordering col
+00012320: 756d 6e73 0a20 2020 2020 2020 2063 6f6d  umns.        com
+00012330: 7069 6c65 645f 7661 6c75 6520 3d20 7365  piled_value = se
+00012340: 6c66 2e5f 636f 6d70 696c 655f 6f72 6465  lf._compile_orde
+00012350: 7265 6428 6172 7261 795f 7661 6c75 6529  red(array_value)
+00012360: 0a0a 2020 2020 2020 2020 6962 6973 5f65  ..        ibis_e
+00012370: 7870 7220 3d20 636f 6d70 696c 6564 5f76  xpr = compiled_v
+00012380: 616c 7565 2e5f 746f 5f69 6269 735f 6578  alue._to_ibis_ex
+00012390: 7072 280a 2020 2020 2020 2020 2020 2020  pr(.            
+000123a0: 6f72 6465 7269 6e67 5f6d 6f64 653d 226f  ordering_mode="o
+000123b0: 6666 7365 745f 636f 6c22 2c20 6f72 6465  ffset_col", orde
+000123c0: 725f 636f 6c5f 6e61 6d65 3d22 6269 6766  r_col_name="bigf
+000123d0: 7261 6d65 735f 6f66 6673 6574 7322 0a20  rames_offsets". 
+000123e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000123f0: 2074 6d70 5f74 6162 6c65 203d 2073 656c   tmp_table = sel
+00012400: 662e 5f69 6269 735f 746f 5f74 656d 705f  f._ibis_to_temp_
+00012410: 7461 626c 6528 0a20 2020 2020 2020 2020  table(.         
+00012420: 2020 2069 6269 735f 6578 7072 2c20 636c     ibis_expr, cl
+00012430: 7573 7465 725f 636f 6c73 3d5b 2262 6967  uster_cols=["big
+00012440: 6672 616d 6573 5f6f 6666 7365 7473 225d  frames_offsets"]
+00012450: 2c20 6170 695f 6e61 6d65 3d22 6361 6368  , api_name="cach
+00012460: 6564 220a 2020 2020 2020 2020 290a 2020  ed".        ).  
+00012470: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
+00012480: 6573 7369 6f6e 203d 2073 656c 662e 6962  ession = self.ib
+00012490: 6973 5f63 6c69 656e 742e 7461 626c 6528  is_client.table(
+000124a0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
+000124b0: 5f74 6162 6c65 2e74 6162 6c65 5f69 642c  _table.table_id,
+000124c0: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
+000124d0: 656d 613d 746d 705f 7461 626c 652e 6461  ema=tmp_table.da
+000124e0: 7461 7365 745f 6964 2c0a 2020 2020 2020  taset_id,.      
+000124f0: 2020 2020 2020 6461 7461 6261 7365 3d74        database=t
+00012500: 6d70 5f74 6162 6c65 2e70 726f 6a65 6374  mp_table.project
+00012510: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00012520: 2020 2020 6e65 775f 636f 6c75 6d6e 7320      new_columns 
+00012530: 3d20 5b74 6162 6c65 5f65 7870 7265 7373  = [table_express
+00012540: 696f 6e5b 636f 6c75 6d6e 5d20 666f 7220  ion[column] for 
+00012550: 636f 6c75 6d6e 2069 6e20 636f 6d70 696c  column in compil
+00012560: 6564 5f76 616c 7565 2e63 6f6c 756d 6e5f  ed_value.column_
+00012570: 6964 735d 0a20 2020 2020 2020 206e 6577  ids].        new
+00012580: 5f68 6964 6465 6e5f 636f 6c75 6d6e 7320  _hidden_columns 
+00012590: 3d20 5b74 6162 6c65 5f65 7870 7265 7373  = [table_express
+000125a0: 696f 6e5b 2262 6967 6672 616d 6573 5f6f  ion["bigframes_o
+000125b0: 6666 7365 7473 225d 5d0a 2020 2020 2020  ffsets"]].      
+000125c0: 2020 2320 544f 444f 3a20 496e 7374 6561    # TODO: Instea
+000125d0: 642c 206b 6565 7020 7365 7373 696f 6e2d  d, keep session-
+000125e0: 7769 6465 206d 6170 206f 6620 6361 6368  wide map of cach
+000125f0: 6564 2072 6573 756c 7473 2061 6e64 2061  ed results and a
+00012600: 7574 6f6d 6174 6963 616c 6c79 2072 6575  utomatically reu
+00012610: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
+00012620: 6e20 636f 7265 2e41 7272 6179 5661 6c75  n core.ArrayValu
+00012630: 652e 6672 6f6d 5f69 6269 7328 0a20 2020  e.from_ibis(.   
+00012640: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00012650: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00012660: 5f65 7870 7265 7373 696f 6e2c 0a20 2020  _expression,.   
+00012670: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00012680: 3d6e 6577 5f63 6f6c 756d 6e73 2c0a 2020  =new_columns,.  
+00012690: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
+000126a0: 5f6f 7264 6572 696e 675f 636f 6c75 6d6e  _ordering_column
+000126b0: 733d 6e65 775f 6869 6464 656e 5f63 6f6c  s=new_hidden_col
+000126c0: 756d 6e73 2c0a 2020 2020 2020 2020 2020  umns,.          
+000126d0: 2020 6f72 6465 7269 6e67 3d6f 7264 6572    ordering=order
+000126e0: 2e45 7870 7265 7373 696f 6e4f 7264 6572  .ExpressionOrder
+000126f0: 696e 672e 6672 6f6d 5f6f 6666 7365 745f  ing.from_offset_
+00012700: 636f 6c28 2262 6967 6672 616d 6573 5f6f  col("bigframes_o
+00012710: 6666 7365 7473 2229 2c0a 2020 2020 2020  ffsets"),.      
+00012720: 2020 290a 0a20 2020 2064 6566 205f 7369    )..    def _si
+00012730: 6d70 6c69 6679 5f77 6974 685f 6361 6368  mplify_with_cach
+00012740: 696e 6728 7365 6c66 2c20 6172 7261 795f  ing(self, array_
+00012750: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
+00012760: 7956 616c 7565 2920 2d3e 2063 6f72 652e  yValue) -> core.
+00012770: 4172 7261 7956 616c 7565 3a0a 2020 2020  ArrayValue:.    
+00012780: 2020 2020 2222 2241 7474 656d 7074 7320      """Attempts 
+00012790: 746f 2068 616e 646c 6520 7468 6520 636f  to handle the co
+000127a0: 6d70 6c65 7869 7479 2062 7920 6361 6368  mplexity by cach
+000127b0: 696e 6720 6475 706c 6963 6174 6564 2073  ing duplicated s
+000127c0: 7562 7472 6565 7320 616e 6420 6272 6561  ubtrees and brea
+000127d0: 6b69 6e67 2074 6865 2071 7565 7279 2069  king the query i
+000127e0: 6e74 6f20 7069 6563 6573 2e22 2222 0a20  nto pieces.""". 
+000127f0: 2020 2020 2020 2069 6620 6e6f 7420 6269         if not bi
+00012800: 6766 7261 6d65 732e 6f70 7469 6f6e 732e  gframes.options.
+00012810: 636f 6d70 7574 652e 656e 6162 6c65 5f6d  compute.enable_m
+00012820: 756c 7469 5f71 7565 7279 5f65 7865 6375  ulti_query_execu
+00012830: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00012840: 2020 7265 7475 726e 2061 7272 6179 5f76    return array_v
+00012850: 616c 7565 0a20 2020 2020 2020 206e 6f64  alue.        nod
+00012860: 6520 3d20 6172 7261 795f 7661 6c75 652e  e = array_value.
+00012870: 6e6f 6465 0a20 2020 2020 2020 2069 6620  node.        if 
+00012880: 6e6f 6465 2e70 6c61 6e6e 696e 675f 636f  node.planning_co
+00012890: 6d70 6c65 7869 7479 203c 2051 5545 5259  mplexity < QUERY
+000128a0: 5f43 4f4d 504c 4558 4954 595f 4c49 4d49  _COMPLEXITY_LIMI
+000128b0: 543a 0a20 2020 2020 2020 2020 2020 2072  T:.            r
+000128c0: 6574 7572 6e20 6172 7261 795f 7661 6c75  eturn array_valu
+000128d0: 650a 0a20 2020 2020 2020 2066 6f72 205f  e..        for _
+000128e0: 2069 6e20 7261 6e67 6528 4d41 585f 5355   in range(MAX_SU
+000128f0: 4254 5245 455f 4641 4354 4f52 494e 4753  BTREE_FACTORINGS
+00012900: 293a 0a20 2020 2020 2020 2020 2020 2075  ):.            u
+00012910: 7064 6174 6564 203d 2073 656c 662e 5f63  pdated = self._c
+00012920: 6163 6865 5f6d 6f73 745f 636f 6d70 6c65  ache_most_comple
+00012930: 785f 7375 6274 7265 6528 6e6f 6465 290a  x_subtree(node).
+00012940: 2020 2020 2020 2020 2020 2020 6966 2075              if u
+00012950: 7064 6174 6564 2069 7320 4e6f 6e65 3a0a  pdated is None:.
+00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012970: 7265 7475 726e 2063 6f72 652e 4172 7261  return core.Arra
+00012980: 7956 616c 7565 286e 6f64 6529 0a20 2020  yValue(node).   
+00012990: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000129a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000129b0: 6f64 6520 3d20 7570 6461 7465 640a 0a20  ode = updated.. 
+000129c0: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
+000129d0: 7265 2e41 7272 6179 5661 6c75 6528 6e6f  re.ArrayValue(no
+000129e0: 6465 290a 0a20 2020 2064 6566 205f 6361  de)..    def _ca
+000129f0: 6368 655f 6d6f 7374 5f63 6f6d 706c 6578  che_most_complex
+00012a00: 5f73 7562 7472 6565 280a 2020 2020 2020  _subtree(.      
+00012a10: 2020 7365 6c66 2c20 6e6f 6465 3a20 6e6f    self, node: no
+00012a20: 6465 732e 4269 6746 7261 6d65 4e6f 6465  des.BigFrameNode
+00012a30: 0a20 2020 2029 202d 3e20 4f70 7469 6f6e  .    ) -> Option
+00012a40: 616c 5b6e 6f64 6573 2e42 6967 4672 616d  al[nodes.BigFram
+00012a50: 654e 6f64 655d 3a0a 2020 2020 2020 2020  eNode]:.        
+00012a60: 2320 544f 444f 3a20 4966 2071 7565 7279  # TODO: If query
+00012a70: 2066 6169 6c73 2c20 7265 7472 7920 7769   fails, retry wi
+00012a80: 7468 206c 6f77 6572 2063 6f6d 706c 6578  th lower complex
+00012a90: 6974 7920 6c69 6d69 740a 2020 2020 2020  ity limit.      
+00012aa0: 2020 7661 6c69 645f 6361 6e64 6964 6174    valid_candidat
+00012ab0: 6573 203d 2074 7261 7665 7273 616c 732e  es = traversals.
+00012ac0: 636f 756e 745f 636f 6d70 6c65 785f 6e6f  count_complex_no
+00012ad0: 6465 7328 0a20 2020 2020 2020 2020 2020  des(.           
+00012ae0: 206e 6f64 652c 0a20 2020 2020 2020 2020   node,.         
+00012af0: 2020 206d 696e 5f63 6f6d 706c 6578 6974     min_complexit
+00012b00: 793d 2851 5545 5259 5f43 4f4d 504c 4558  y=(QUERY_COMPLEX
+00012b10: 4954 595f 4c49 4d49 5420 2f20 3530 3029  ITY_LIMIT / 500)
+00012b20: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+00012b30: 785f 636f 6d70 6c65 7869 7479 3d51 5545  x_complexity=QUE
+00012b40: 5259 5f43 4f4d 504c 4558 4954 595f 4c49  RY_COMPLEXITY_LI
+00012b50: 4d49 542c 0a20 2020 2020 2020 2029 2e69  MIT,.        ).i
+00012b60: 7465 6d73 2829 0a20 2020 2020 2020 2023  tems().        #
+00012b70: 2048 6575 7269 7374 6963 3a20 7375 6274   Heuristic: subt
+00012b80: 7265 655f 636f 6d70 6c65 6978 7479 202a  ree_compleixty *
+00012b90: 2028 636f 7069 6573 206f 6620 7375 6274   (copies of subt
+00012ba0: 7265 6529 5e32 0a20 2020 2020 2020 2062  ree)^2.        b
+00012bb0: 6573 745f 6361 6e64 6964 6174 6520 3d20  est_candidate = 
+00012bc0: 6d61 7828 0a20 2020 2020 2020 2020 2020  max(.           
+00012bd0: 2076 616c 6964 5f63 616e 6469 6461 7465   valid_candidate
+00012be0: 732c 0a20 2020 2020 2020 2020 2020 206b  s,.            k
+00012bf0: 6579 3d6c 616d 6264 6120 693a 2069 5b30  ey=lambda i: i[0
+00012c00: 5d2e 706c 616e 6e69 6e67 5f63 6f6d 706c  ].planning_compl
+00012c10: 6578 6974 7920 2b20 2869 5b31 5d20 2a2a  exity + (i[1] **
+00012c20: 2032 292c 0a20 2020 2020 2020 2020 2020   2),.           
+00012c30: 2064 6566 6175 6c74 3d4e 6f6e 652c 0a20   default=None,. 
+00012c40: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00012c50: 2020 6966 2062 6573 745f 6361 6e64 6964    if best_candid
+00012c60: 6174 6520 6973 204e 6f6e 653a 0a20 2020  ate is None:.   
+00012c70: 2020 2020 2020 2020 2023 204e 6f20 676f           # No go
+00012c80: 6f64 2073 7562 7472 6565 7320 746f 2063  od subtrees to c
+00012c90: 6163 6865 2c20 6a75 7374 2072 6574 7572  ache, just retur
+00012ca0: 6e20 6f72 6967 696e 616c 2074 7265 650a  n original tree.
+00012cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012cc0: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
+00012cd0: 2023 2054 4f44 4f3a 2041 6464 2063 6c75   # TODO: Add clu
+00012ce0: 7374 6572 696e 6720 636f 6c75 6d6e 7320  stering columns 
+00012cf0: 6261 7365 6420 6f6e 2061 6363 6573 7320  based on access 
+00012d00: 7061 7474 6572 6e73 0a20 2020 2020 2020  patterns.       
+00012d10: 206d 6174 6572 6961 6c69 7a65 6420 3d20   materialized = 
+00012d20: 7365 6c66 2e5f 6361 6368 655f 7769 7468  self._cache_with
+00012d30: 5f63 6c75 7374 6572 5f63 6f6c 7328 0a20  _cluster_cols(. 
+00012d40: 2020 2020 2020 2020 2020 2063 6f72 652e             core.
+00012d50: 4172 7261 7956 616c 7565 2862 6573 745f  ArrayValue(best_
+00012d60: 6361 6e64 6964 6174 655b 305d 292c 205b  candidate[0]), [
+00012d70: 5d0a 2020 2020 2020 2020 292e 6e6f 6465  ].        ).node
+00012d80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00012d90: 2074 7261 7665 7273 616c 732e 7265 706c   traversals.repl
+00012da0: 6163 655f 6e6f 6465 7328 0a20 2020 2020  ace_nodes(.     
+00012db0: 2020 2020 2020 206e 6f64 652c 2074 6f5f         node, to_
+00012dc0: 7265 706c 6163 653d 6265 7374 5f63 616e  replace=best_can
+00012dd0: 6469 6461 7465 5b30 5d2c 2072 6570 6c61  didate[0], repla
+00012de0: 6365 6d65 6e65 743d 6d61 7465 7269 616c  cemenet=material
+00012df0: 697a 6564 0a20 2020 2020 2020 2029 0a0a  ized.        )..
+00012e00: 2020 2020 6465 6620 5f69 735f 7472 6976      def _is_triv
+00012e10: 6961 6c6c 795f 6578 6563 7574 6162 6c65  ially_executable
+00012e20: 2873 656c 662c 2061 7272 6179 5f76 616c  (self, array_val
+00012e30: 7565 3a20 636f 7265 2e41 7272 6179 5661  ue: core.ArrayVa
+00012e40: 6c75 6529 3a0a 2020 2020 2020 2020 2222  lue):.        ""
+00012e50: 220a 2020 2020 2020 2020 4361 6e20 7468  ".        Can th
+00012e60: 6520 626c 6f63 6b20 6265 2065 7661 6c75  e block be evalu
+00012e70: 6174 6564 2076 6572 7920 6368 6561 706c  ated very cheapl
+00012e80: 793f 0a20 2020 2020 2020 2049 6620 5472  y?.        If Tr
+00012e90: 7565 2c20 7468 6520 6172 7261 795f 7661  ue, the array_va
+00012ea0: 6c75 6520 7072 6f62 6162 6c79 2069 7320  lue probably is 
+00012eb0: 6e6f 7420 776f 7274 6820 6361 6368 696e  not worth cachin
+00012ec0: 672e 0a20 2020 2020 2020 2022 2222 0a20  g..        """. 
+00012ed0: 2020 2020 2020 2023 204f 6e63 6520 7265         # Once re
+00012ee0: 7772 6974 696e 6720 6973 2061 7661 696c  writing is avail
+00012ef0: 6162 6c65 2c20 7769 6c6c 2077 616e 7420  able, will want 
+00012f00: 746f 2072 6577 7269 7465 2062 6566 6f72  to rewrite befor
+00012f10: 650a 2020 2020 2020 2020 2320 6576 616c  e.        # eval
+00012f20: 7561 7469 6e67 2065 7865 6375 7469 6f6e  uating execution
+00012f30: 2063 6f73 742e 0a20 2020 2020 2020 2072   cost..        r
+00012f40: 6574 7572 6e20 7472 6176 6572 7361 6c73  eturn traversals
+00012f50: 2e69 735f 7472 6976 6961 6c6c 795f 6578  .is_trivially_ex
+00012f60: 6563 7574 6162 6c65 2861 7272 6179 5f76  ecutable(array_v
+00012f70: 616c 7565 2e6e 6f64 6529 0a0a 2020 2020  alue.node)..    
+00012f80: 6465 6620 5f65 7865 6375 7465 280a 2020  def _execute(.  
+00012f90: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00012fa0: 2020 2020 6172 7261 795f 7661 6c75 653a      array_value:
+00012fb0: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
+00012fc0: 2c0a 2020 2020 2020 2020 6a6f 625f 636f  ,.        job_co
+00012fd0: 6e66 6967 3a20 4f70 7469 6f6e 616c 5b62  nfig: Optional[b
+00012fe0: 6967 7175 6572 792e 6a6f 622e 5175 6572  igquery.job.Quer
+00012ff0: 794a 6f62 436f 6e66 6967 5d20 3d20 4e6f  yJobConfig] = No
+00013000: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
+00013010: 2020 2020 2020 2073 6f72 7465 643a 2062         sorted: b
+00013020: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+00013030: 2020 2020 6472 795f 7275 6e3d 4661 6c73      dry_run=Fals
+00013040: 652c 0a20 2020 2020 2020 2063 6f6c 5f69  e,.        col_i
+00013050: 645f 6f76 6572 7269 6465 733a 204d 6170  d_overrides: Map
+00013060: 7069 6e67 5b73 7472 2c20 7374 725d 203d  ping[str, str] =
+00013070: 207b 7d2c 0a20 2020 2029 202d 3e20 7475   {},.    ) -> tu
+00013080: 706c 655b 6269 6771 7565 7279 2e74 6162  ple[bigquery.tab
+00013090: 6c65 2e52 6f77 4974 6572 6174 6f72 2c20  le.RowIterator, 
+000130a0: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
+000130b0: 625d 3a0a 2020 2020 2020 2020 7371 6c20  b]:.        sql 
+000130c0: 3d20 7365 6c66 2e5f 746f 5f73 716c 280a  = self._to_sql(.
+000130d0: 2020 2020 2020 2020 2020 2020 6172 7261              arra
+000130e0: 795f 7661 6c75 652c 2073 6f72 7465 643d  y_value, sorted=
+000130f0: 736f 7274 6564 2c20 636f 6c5f 6964 5f6f  sorted, col_id_o
+00013100: 7665 7272 6964 6573 3d63 6f6c 5f69 645f  verrides=col_id_
+00013110: 6f76 6572 7269 6465 730a 2020 2020 2020  overrides.      
+00013120: 2020 2920 2023 2074 7970 653a 6967 6e6f    )  # type:igno
+00013130: 7265 0a20 2020 2020 2020 2069 6620 6a6f  re.        if jo
+00013140: 625f 636f 6e66 6967 2069 7320 4e6f 6e65  b_config is None
+00013150: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
+00013160: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
+00013170: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
+00013180: 6967 2864 7279 5f72 756e 3d64 7279 5f72  ig(dry_run=dry_r
+00013190: 756e 290a 2020 2020 2020 2020 656c 7365  un).        else
+000131a0: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
+000131b0: 625f 636f 6e66 6967 2e64 7279 5f72 756e  b_config.dry_run
+000131c0: 203d 2064 7279 5f72 756e 0a20 2020 2020   = dry_run.     
+000131d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000131e0: 7374 6172 745f 7175 6572 7928 0a20 2020  start_query(.   
+000131f0: 2020 2020 2020 2020 2073 716c 3d73 716c           sql=sql
+00013200: 2c0a 2020 2020 2020 2020 2020 2020 6a6f  ,.            jo
+00013210: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
+00013220: 6669 672c 0a20 2020 2020 2020 2029 0a0a  fig,.        )..
+00013230: 2020 2020 6465 6620 5f70 6565 6b28 0a20      def _peek(. 
+00013240: 2020 2020 2020 2073 656c 662c 2061 7272         self, arr
+00013250: 6179 5f76 616c 7565 3a20 636f 7265 2e41  ay_value: core.A
+00013260: 7272 6179 5661 6c75 652c 206e 5f72 6f77  rrayValue, n_row
+00013270: 733a 2069 6e74 0a20 2020 2029 202d 3e20  s: int.    ) -> 
+00013280: 7475 706c 655b 6269 6771 7565 7279 2e74  tuple[bigquery.t
+00013290: 6162 6c65 2e52 6f77 4974 6572 6174 6f72  able.RowIterator
+000132a0: 2c20 6269 6771 7565 7279 2e51 7565 7279  , bigquery.Query
+000132b0: 4a6f 625d 3a0a 2020 2020 2020 2020 2222  Job]:.        ""
+000132c0: 2241 2027 7065 656b 2720 6566 6669 6369  "A 'peek' effici
+000132d0: 656e 746c 7920 6163 6365 7373 6573 2061  ently accesses a
+000132e0: 2073 6d61 6c6c 206e 756d 6265 7220 6f66   small number of
+000132f0: 2072 6f77 7320 696e 2074 6865 2064 6174   rows in the dat
+00013300: 6166 7261 6d65 2e22 2222 0a20 2020 2020  aframe.""".     
+00013310: 2020 2069 6620 6e6f 7420 7472 6565 5f70     if not tree_p
+00013320: 726f 7065 7274 6965 732e 7065 656b 6162  roperties.peekab
+00013330: 6c65 2861 7272 6179 5f76 616c 7565 2e6e  le(array_value.n
+00013340: 6f64 6529 3a0a 2020 2020 2020 2020 2020  ode):.          
+00013350: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00013360: 2250 6565 6b69 6e67 2074 6869 7320 7661  "Peeking this va
+00013370: 6c75 6520 6361 6e6e 6f74 2062 6520 646f  lue cannot be do
+00013380: 6e65 2065 6666 6963 6965 6e74 6c79 2e22  ne efficiently."
+00013390: 290a 2020 2020 2020 2020 7371 6c20 3d20  ).        sql = 
+000133a0: 7365 6c66 2e5f 636f 6d70 696c 655f 756e  self._compile_un
+000133b0: 6f72 6465 7265 6428 6172 7261 795f 7661  ordered(array_va
+000133c0: 6c75 6529 2e70 6565 6b5f 7371 6c28 6e5f  lue).peek_sql(n_
+000133d0: 726f 7773 290a 2020 2020 2020 2020 7265  rows).        re
+000133e0: 7475 726e 2073 656c 662e 5f73 7461 7274  turn self._start
+000133f0: 5f71 7565 7279 280a 2020 2020 2020 2020  _query(.        
+00013400: 2020 2020 7371 6c3d 7371 6c2c 0a20 2020      sql=sql,.   
+00013410: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00013420: 5f74 6f5f 7371 6c28 0a20 2020 2020 2020  _to_sql(.       
+00013430: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
+00013440: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
+00013450: 2e41 7272 6179 5661 6c75 652c 0a20 2020  .ArrayValue,.   
+00013460: 2020 2020 206f 6666 7365 745f 636f 6c75       offset_colu
+00013470: 6d6e 3a20 7479 7069 6e67 2e4f 7074 696f  mn: typing.Optio
+00013480: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00013490: 0a20 2020 2020 2020 2063 6f6c 5f69 645f  .        col_id_
+000134a0: 6f76 6572 7269 6465 733a 2074 7970 696e  overrides: typin
+000134b0: 672e 4d61 7070 696e 675b 7374 722c 2073  g.Mapping[str, s
+000134c0: 7472 5d20 3d20 7b7d 2c0a 2020 2020 2020  tr] = {},.      
+000134d0: 2020 736f 7274 6564 3a20 626f 6f6c 203d    sorted: bool =
+000134e0: 2046 616c 7365 2c0a 2020 2020 2920 2d3e   False,.    ) ->
+000134f0: 2073 7472 3a0a 2020 2020 2020 2020 6966   str:.        if
+00013500: 206f 6666 7365 745f 636f 6c75 6d6e 3a0a   offset_column:.
+00013510: 2020 2020 2020 2020 2020 2020 6172 7261              arra
+00013520: 795f 7661 6c75 6520 3d20 6172 7261 795f  y_value = array_
+00013530: 7661 6c75 652e 7072 6f6d 6f74 655f 6f66  value.promote_of
+00013540: 6673 6574 7328 6f66 6673 6574 5f63 6f6c  fsets(offset_col
+00013550: 756d 6e29 0a20 2020 2020 2020 2069 6620  umn).        if 
+00013560: 736f 7274 6564 3a0a 2020 2020 2020 2020  sorted:.        
+00013570: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00013580: 5f63 6f6d 7069 6c65 5f6f 7264 6572 6564  _compile_ordered
+00013590: 2861 7272 6179 5f76 616c 7565 292e 746f  (array_value).to
+000135a0: 5f73 716c 280a 2020 2020 2020 2020 2020  _sql(.          
+000135b0: 2020 2020 2020 636f 6c5f 6964 5f6f 7665        col_id_ove
+000135c0: 7272 6964 6573 3d63 6f6c 5f69 645f 6f76  rrides=col_id_ov
+000135d0: 6572 7269 6465 732c 2073 6f72 7465 643d  errides, sorted=
+000135e0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+000135f0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+00013600: 6e20 7365 6c66 2e5f 636f 6d70 696c 655f  n self._compile_
+00013610: 756e 6f72 6465 7265 6428 6172 7261 795f  unordered(array_
+00013620: 7661 6c75 6529 2e74 6f5f 7371 6c28 0a20  value).to_sql(. 
+00013630: 2020 2020 2020 2020 2020 2063 6f6c 5f69             col_i
+00013640: 645f 6f76 6572 7269 6465 733d 636f 6c5f  d_overrides=col_
+00013650: 6964 5f6f 7665 7272 6964 6573 0a20 2020  id_overrides.   
+00013660: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00013670: 5f63 6f6d 7069 6c65 5f6f 7264 6572 6564  _compile_ordered
+00013680: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00013690: 6172 7261 795f 7661 6c75 653a 2063 6f72  array_value: cor
+000136a0: 652e 4172 7261 7956 616c 7565 0a20 2020  e.ArrayValue.   
+000136b0: 2029 202d 3e20 6269 6766 7261 6d65 732e   ) -> bigframes.
+000136c0: 636f 7265 2e63 6f6d 7069 6c65 2e4f 7264  core.compile.Ord
+000136d0: 6572 6564 4952 3a0a 2020 2020 2020 2020  eredIR:.        
+000136e0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
+000136f0: 2e63 6f72 652e 636f 6d70 696c 652e 636f  .core.compile.co
+00013700: 6d70 696c 655f 6f72 6465 7265 645f 6972  mpile_ordered_ir
+00013710: 2861 7272 6179 5f76 616c 7565 2e6e 6f64  (array_value.nod
+00013720: 6529 0a0a 2020 2020 6465 6620 5f63 6f6d  e)..    def _com
+00013730: 7069 6c65 5f75 6e6f 7264 6572 6564 280a  pile_unordered(.
+00013740: 2020 2020 2020 2020 7365 6c66 2c20 6172          self, ar
+00013750: 7261 795f 7661 6c75 653a 2063 6f72 652e  ray_value: core.
+00013760: 4172 7261 7956 616c 7565 0a20 2020 2029  ArrayValue.    )
+00013770: 202d 3e20 6269 6766 7261 6d65 732e 636f   -> bigframes.co
+00013780: 7265 2e63 6f6d 7069 6c65 2e55 6e6f 7264  re.compile.Unord
+00013790: 6572 6564 4952 3a0a 2020 2020 2020 2020  eredIR:.        
+000137a0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
+000137b0: 2e63 6f72 652e 636f 6d70 696c 652e 636f  .core.compile.co
+000137c0: 6d70 696c 655f 756e 6f72 6465 7265 645f  mpile_unordered_
+000137d0: 6972 2861 7272 6179 5f76 616c 7565 2e6e  ir(array_value.n
+000137e0: 6f64 6529 0a0a 2020 2020 6465 6620 5f67  ode)..    def _g
+000137f0: 6574 5f74 6162 6c65 5f73 697a 6528 7365  et_table_size(se
+00013800: 6c66 2c20 6465 7374 696e 6174 696f 6e5f  lf, destination_
+00013810: 7461 626c 6529 3a0a 2020 2020 2020 2020  table):.        
+00013820: 7461 626c 6520 3d20 7365 6c66 2e62 7163  table = self.bqc
+00013830: 6c69 656e 742e 6765 745f 7461 626c 6528  lient.get_table(
+00013840: 6465 7374 696e 6174 696f 6e5f 7461 626c  destination_tabl
+00013850: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00013860: 6e20 7461 626c 652e 6e75 6d5f 6279 7465  n table.num_byte
+00013870: 730a 0a20 2020 2064 6566 205f 726f 7773  s..    def _rows
+00013880: 5f74 6f5f 6461 7461 6672 616d 6528 0a20  _to_dataframe(. 
+00013890: 2020 2020 2020 2073 656c 662c 2072 6f77         self, row
+000138a0: 5f69 7465 7261 746f 723a 2062 6967 7175  _iterator: bigqu
+000138b0: 6572 792e 7461 626c 652e 526f 7749 7465  ery.table.RowIte
+000138c0: 7261 746f 722c 2064 7479 7065 733a 2044  rator, dtypes: D
+000138d0: 6963 740a 2020 2020 2920 2d3e 2070 616e  ict.    ) -> pan
+000138e0: 6461 732e 4461 7461 4672 616d 653a 0a20  das.DataFrame:. 
+000138f0: 2020 2020 2020 2023 2043 616e 2069 676e         # Can ign
+00013900: 6f72 6520 696e 6665 7272 6564 2064 6174  ore inferred dat
+00013910: 6174 7970 6520 756e 7469 6c20 6474 7970  atype until dtyp
+00013920: 6520 656d 756c 6174 696f 6e20 6272 6561  e emulation brea
+00013930: 6b73 2031 3a31 206d 6170 7069 6e67 2062  ks 1:1 mapping b
+00013940: 6574 7765 656e 2042 5120 7479 7065 7320  etween BQ types 
+00013950: 616e 6420 6269 6766 7261 6d65 7320 7479  and bigframes ty
+00013960: 7065 730a 2020 2020 2020 2020 6474 7970  pes.        dtyp
+00013970: 6573 5f66 726f 6d5f 6271 203d 2062 6967  es_from_bq = big
+00013980: 6672 616d 6573 2e64 7479 7065 732e 6266  frames.dtypes.bf
+00013990: 5f74 7970 655f 6672 6f6d 5f74 7970 655f  _type_from_type_
+000139a0: 6b69 6e64 2872 6f77 5f69 7465 7261 746f  kind(row_iterato
+000139b0: 722e 7363 6865 6d61 290a 2020 2020 2020  r.schema).      
+000139c0: 2020 6172 726f 775f 7461 626c 6520 3d20    arrow_table = 
+000139d0: 726f 775f 6974 6572 6174 6f72 2e74 6f5f  row_iterator.to_
+000139e0: 6172 726f 7728 290a 2020 2020 2020 2020  arrow().        
+000139f0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
+00013a00: 2e73 6573 7369 6f6e 2e5f 696f 2e70 616e  .session._io.pan
+00013a10: 6461 732e 6172 726f 775f 746f 5f70 616e  das.arrow_to_pan
+00013a20: 6461 7328 6172 726f 775f 7461 626c 652c  das(arrow_table,
+00013a30: 2064 7479 7065 735f 6672 6f6d 5f62 7129   dtypes_from_bq)
+00013a40: 0a0a 2020 2020 6465 6620 5f73 7461 7274  ..    def _start
+00013a50: 5f67 656e 6572 6963 5f6a 6f62 2873 656c  _generic_job(sel
+00013a60: 662c 206a 6f62 3a20 666f 726d 6174 7469  f, job: formatti
+00013a70: 6e67 5f68 656c 7065 7273 2e47 656e 6572  ng_helpers.Gener
+00013a80: 6963 4a6f 6229 3a0a 2020 2020 2020 2020  icJob):.        
+00013a90: 6966 2062 6967 6672 616d 6573 2e6f 7074  if bigframes.opt
+00013aa0: 696f 6e73 2e64 6973 706c 6179 2e70 726f  ions.display.pro
+00013ab0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+00013ac0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00013ad0: 2020 2066 6f72 6d61 7474 696e 675f 6865     formatting_he
+00013ae0: 6c70 6572 732e 7761 6974 5f66 6f72 5f6a  lpers.wait_for_j
+00013af0: 6f62 280a 2020 2020 2020 2020 2020 2020  ob(.            
+00013b00: 2020 2020 6a6f 622c 2062 6967 6672 616d      job, bigfram
+00013b10: 6573 2e6f 7074 696f 6e73 2e64 6973 706c  es.options.displ
+00013b20: 6179 2e70 726f 6772 6573 735f 6261 720a  ay.progress_bar.
+00013b30: 2020 2020 2020 2020 2020 2020 2920 2023              )  #
+00013b40: 2057 6169 7420 666f 7220 7468 6520 6a6f   Wait for the jo
+00013b50: 6220 746f 2063 6f6d 706c 6574 650a 2020  b to complete.  
+00013b60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00013b70: 2020 2020 2020 2020 6a6f 622e 7265 7375          job.resu
+00013b80: 6c74 2829 0a0a 0a64 6566 2063 6f6e 6e65  lt()...def conne
+00013b90: 6374 2863 6f6e 7465 7874 3a20 4f70 7469  ct(context: Opti
+00013ba0: 6f6e 616c 5b62 6967 7175 6572 795f 6f70  onal[bigquery_op
+00013bb0: 7469 6f6e 732e 4269 6751 7565 7279 4f70  tions.BigQueryOp
+00013bc0: 7469 6f6e 735d 203d 204e 6f6e 6529 202d  tions] = None) -
+00013bd0: 3e20 5365 7373 696f 6e3a 0a20 2020 2072  > Session:.    r
+00013be0: 6574 7572 6e20 5365 7373 696f 6e28 636f  eturn Session(co
+00013bf0: 6e74 6578 7429 0a0a 0a64 6566 205f 6361  ntext)...def _ca
+00013c00: 6e5f 636c 7573 7465 725f 6271 2866 6965  n_cluster_bq(fie
+00013c10: 6c64 3a20 6269 6771 7565 7279 2e53 6368  ld: bigquery.Sch
+00013c20: 656d 6146 6965 6c64 293a 0a20 2020 2023  emaField):.    #
+00013c30: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
+00013c40: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
+00013c50: 7279 2f64 6f63 732f 636c 7573 7465 7265  ry/docs/clustere
+00013c60: 642d 7461 626c 6573 0a20 2020 2023 204e  d-tables.    # N
+00013c70: 6f74 6162 6c79 2c20 666c 6f61 7420 6973  otably, float is
+00013c80: 2065 7863 6c75 6465 640a 2020 2020 7479   excluded.    ty
+00013c90: 7065 5f20 3d20 6669 656c 642e 6669 656c  pe_ = field.fiel
+00013ca0: 645f 7479 7065 0a20 2020 2072 6574 7572  d_type.    retur
+00013cb0: 6e20 7479 7065 5f20 696e 2028 0a20 2020  n type_ in (.   
+00013cc0: 2020 2020 2022 494e 5445 4745 5222 2c0a       "INTEGER",.
+00013cd0: 2020 2020 2020 2020 2249 4e54 3634 222c          "INT64",
+00013ce0: 0a20 2020 2020 2020 2022 5354 5249 4e47  .        "STRING
+00013cf0: 222c 0a20 2020 2020 2020 2022 4e55 4d45  ",.        "NUME
+00013d00: 5249 4322 2c0a 2020 2020 2020 2020 2244  RIC",.        "D
+00013d10: 4543 494d 414c 222c 0a20 2020 2020 2020  ECIMAL",.       
+00013d20: 2022 4249 474e 554d 4552 4943 222c 0a20   "BIGNUMERIC",. 
+00013d30: 2020 2020 2020 2022 4249 4744 4543 494d         "BIGDECIM
+00013d40: 414c 222c 0a20 2020 2020 2020 2022 4441  AL",.        "DA
+00013d50: 5445 222c 0a20 2020 2020 2020 2022 4441  TE",.        "DA
+00013d60: 5445 5449 4d45 222c 0a20 2020 2020 2020  TETIME",.       
+00013d70: 2022 5449 4d45 5354 414d 5022 2c0a 2020   "TIMESTAMP",.  
+00013d80: 2020 2020 2020 2242 4f4f 4c22 2c0a 2020        "BOOL",.  
+00013d90: 2020 2020 2020 2242 4f4f 4c45 414e 222c        "BOOLEAN",
+00013da0: 0a20 2020 2029 0a0a 0a64 6566 205f 636f  .    )...def _co
+00013db0: 6e76 6572 745f 746f 5f6e 6f6e 6e75 6c6c  nvert_to_nonnull
+00013dc0: 5f73 7472 696e 6728 636f 6c75 6d6e 3a20  _string(column: 
+00013dd0: 6962 6973 5f74 7970 6573 2e43 6f6c 756d  ibis_types.Colum
+00013de0: 6e29 202d 3e20 6962 6973 5f74 7970 6573  n) -> ibis_types
+00013df0: 2e53 7472 696e 6756 616c 7565 3a0a 2020  .StringValue:.  
+00013e00: 2020 636f 6c5f 7479 7065 203d 2063 6f6c    col_type = col
+00013e10: 756d 6e2e 7479 7065 2829 0a20 2020 2069  umn.type().    i
+00013e20: 6620 280a 2020 2020 2020 2020 636f 6c5f  f (.        col_
+00013e30: 7479 7065 2e69 735f 6e75 6d65 7269 6328  type.is_numeric(
+00013e40: 290a 2020 2020 2020 2020 6f72 2063 6f6c  ).        or col
+00013e50: 5f74 7970 652e 6973 5f62 6f6f 6c65 616e  _type.is_boolean
+00013e60: 2829 0a20 2020 2020 2020 206f 7220 636f  ().        or co
+00013e70: 6c5f 7479 7065 2e69 735f 6269 6e61 7279  l_type.is_binary
+00013e80: 2829 0a20 2020 2020 2020 206f 7220 636f  ().        or co
+00013e90: 6c5f 7479 7065 2e69 735f 7465 6d70 6f72  l_type.is_tempor
+00013ea0: 616c 2829 0a20 2020 2029 3a0a 2020 2020  al().    ):.    
+00013eb0: 2020 2020 7265 7375 6c74 203d 2063 6f6c      result = col
+00013ec0: 756d 6e2e 6361 7374 2869 6269 735f 6474  umn.cast(ibis_dt
+00013ed0: 7970 6573 2e53 7472 696e 6728 6e75 6c6c  ypes.String(null
+00013ee0: 6162 6c65 3d54 7275 6529 290a 2020 2020  able=True)).    
+00013ef0: 656c 6966 2063 6f6c 5f74 7970 652e 6973  elif col_type.is
+00013f00: 5f67 656f 7370 6174 6961 6c28 293a 0a20  _geospatial():. 
+00013f10: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00013f20: 7479 7069 6e67 2e63 6173 7428 6962 6973  typing.cast(ibis
+00013f30: 5f74 7970 6573 2e47 656f 5370 6174 6961  _types.GeoSpatia
+00013f40: 6c43 6f6c 756d 6e2c 2063 6f6c 756d 6e29  lColumn, column)
+00013f50: 2e61 735f 7465 7874 2829 0a20 2020 2065  .as_text().    e
+00013f60: 6c69 6620 636f 6c5f 7479 7065 2e69 735f  lif col_type.is_
+00013f70: 7374 7269 6e67 2829 3a0a 2020 2020 2020  string():.      
+00013f80: 2020 7265 7375 6c74 203d 2063 6f6c 756d    result = colum
+00013f90: 6e0a 2020 2020 656c 7365 3a0a 2020 2020  n.    else:.    
+00013fa0: 2020 2020 2320 544f 5f4a 534f 4e5f 5354      # TO_JSON_ST
+00013fb0: 5249 4e47 2077 6f72 6b73 2077 6974 6820  RING works with 
+00013fc0: 616c 6c20 6461 7461 2074 7970 6573 2c20  all data types, 
+00013fd0: 6275 7420 6973 6e27 7420 7468 6520 6d6f  but isn't the mo
+00013fe0: 7374 2065 6666 6963 6965 6e74 0a20 2020  st efficient.   
+00013ff0: 2020 2020 2023 204e 6565 6465 6420 666f       # Needed fo
+00014000: 7220 4a53 4f4e 2c20 5354 5255 4354 2061  r JSON, STRUCT a
+00014010: 6e64 2041 5252 4159 2064 6174 6174 7970  nd ARRAY datatyp
+00014020: 6573 0a20 2020 2020 2020 2072 6573 756c  es.        resul
+00014030: 7420 3d20 7665 6e64 6f72 6564 5f69 6269  t = vendored_ibi
+00014040: 735f 6f70 732e 546f 4a73 6f6e 5374 7269  s_ops.ToJsonStri
+00014050: 6e67 2863 6f6c 756d 6e29 2e74 6f5f 6578  ng(column).to_ex
+00014060: 7072 2829 2020 2320 7479 7065 3a20 6967  pr()  # type: ig
+00014070: 6e6f 7265 0a20 2020 2023 2045 7363 6170  nore.    # Escap
+00014080: 6520 6261 636b 736c 6173 6865 7320 616e  e backslashes an
+00014090: 6420 7573 6520 6261 636b 736c 6173 6820  d use backslash 
+000140a0: 6173 2064 656c 696e 6561 746f 720a 2020  as delineator.  
+000140b0: 2020 6573 6361 7065 6420 3d20 7479 7069    escaped = typi
+000140c0: 6e67 2e63 6173 7428 6962 6973 5f74 7970  ng.cast(ibis_typ
+000140d0: 6573 2e53 7472 696e 6743 6f6c 756d 6e2c  es.StringColumn,
+000140e0: 2072 6573 756c 742e 6669 6c6c 6e61 2822   result.fillna("
+000140f0: 2229 292e 7265 706c 6163 6528 225c 5c22  ")).replace("\\"
+00014100: 2c20 225c 5c5c 5c22 2920 2023 2074 7970  , "\\\\")  # typ
+00014110: 653a 2069 676e 6f72 650a 2020 2020 7265  e: ignore.    re
+00014120: 7475 726e 2074 7970 696e 672e 6361 7374  turn typing.cast
+00014130: 2869 6269 735f 7479 7065 732e 5374 7269  (ibis_types.Stri
+00014140: 6e67 436f 6c75 6d6e 2c20 6962 6973 2e6c  ngColumn, ibis.l
+00014150: 6974 6572 616c 2822 5c5c 2229 292e 636f  iteral("\\")).co
+00014160: 6e63 6174 2865 7363 6170 6564 290a 0a0a  ncat(escaped)...
+00014170: 6465 6620 5f74 7261 6e73 666f 726d 5f72  def _transform_r
+00014180: 6561 645f 6762 715f 636f 6e66 6967 7572  ead_gbq_configur
+00014190: 6174 696f 6e28 636f 6e66 6967 7572 6174  ation(configurat
+000141a0: 696f 6e3a 204f 7074 696f 6e61 6c5b 6469  ion: Optional[di
+000141b0: 6374 5d29 202d 3e20 6469 6374 3a0a 2020  ct]) -> dict:.  
+000141c0: 2020 2222 220a 2020 2020 466f 7220 6261    """.    For ba
+000141d0: 636b 7761 7264 732d 636f 6d70 6174 6962  ckwards-compatib
+000141e0: 696c 6974 792c 2063 6f6e 7665 7274 2061  ility, convert a
+000141f0: 6e79 2070 7265 7669 6f75 736c 7920 636c  ny previously cl
+00014200: 6965 6e74 2d73 6964 6520 6f6e 6c79 0a20  ient-side only. 
+00014210: 2020 2070 6172 616d 6574 6572 7320 7375     parameters su
+00014220: 6368 2061 7320 7469 6d65 6f75 744d 7320  ch as timeoutMs 
+00014230: 746f 2074 6865 2070 726f 7065 7274 7920  to the property 
+00014240: 6e61 6d65 2065 7870 6563 7465 6420 6279  name expected by
+00014250: 2074 6865 2052 4553 5420 4150 492e 0a0a   the REST API...
+00014260: 2020 2020 4d61 6b65 7320 6120 636f 7079      Makes a copy
+00014270: 206f 6620 636f 6e66 6967 7572 6174 696f   of configuratio
+00014280: 6e20 6966 2063 6861 6e67 6573 2061 7265  n if changes are
+00014290: 206e 6565 6465 642e 0a20 2020 2022 2222   needed..    """
+000142a0: 0a0a 2020 2020 6966 2063 6f6e 6669 6775  ..    if configu
+000142b0: 7261 7469 6f6e 2069 7320 4e6f 6e65 3a0a  ration is None:.
+000142c0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+000142d0: 7d0a 0a20 2020 2074 696d 656f 7574 5f6d  }..    timeout_m
+000142e0: 7320 3d20 636f 6e66 6967 7572 6174 696f  s = configuratio
+000142f0: 6e2e 6765 7428 2271 7565 7279 222c 207b  n.get("query", {
+00014300: 7d29 2e67 6574 2822 7469 6d65 6f75 744d  }).get("timeoutM
+00014310: 7322 290a 2020 2020 6966 2074 696d 656f  s").    if timeo
+00014320: 7574 5f6d 7320 6973 206e 6f74 204e 6f6e  ut_ms is not Non
+00014330: 653a 0a20 2020 2020 2020 2023 2054 7261  e:.        # Tra
+00014340: 6e73 666f 726d 2074 696d 656f 7574 4d73  nsform timeoutMs
+00014350: 2074 6f20 616e 2061 6374 7561 6c20 7365   to an actual se
+00014360: 7276 6572 2d73 6964 6520 636f 6e66 6967  rver-side config
+00014370: 7572 6174 696f 6e2e 0a20 2020 2020 2020  uration..       
+00014380: 2023 2068 7474 7073 3a2f 2f67 6974 6875   # https://githu
+00014390: 622e 636f 6d2f 676f 6f67 6c65 6170 6973  b.com/googleapis
+000143a0: 2f70 7974 686f 6e2d 6269 6771 7565 7279  /python-bigquery
+000143b0: 2d70 616e 6461 732f 6973 7375 6573 2f34  -pandas/issues/4
+000143c0: 3739 0a20 2020 2020 2020 2063 6f6e 6669  79.        confi
+000143d0: 6775 7261 7469 6f6e 203d 2063 6f70 792e  guration = copy.
+000143e0: 6465 6570 636f 7079 2863 6f6e 6669 6775  deepcopy(configu
+000143f0: 7261 7469 6f6e 290a 2020 2020 2020 2020  ration).        
+00014400: 6465 6c20 636f 6e66 6967 7572 6174 696f  del configuratio
+00014410: 6e5b 2271 7565 7279 225d 5b22 7469 6d65  n["query"]["time
+00014420: 6f75 744d 7322 5d0a 2020 2020 2020 2020  outMs"].        
+00014430: 636f 6e66 6967 7572 6174 696f 6e5b 226a  configuration["j
+00014440: 6f62 5469 6d65 6f75 744d 7322 5d20 3d20  obTimeoutMs"] = 
+00014450: 7469 6d65 6f75 745f 6d73 0a0a 2020 2020  timeout_ms..    
+00014460: 7265 7475 726e 2063 6f6e 6669 6775 7261  return configura
+00014470: 7469 6f6e 0a                             tion.
```

### Comparing `bigframes-1.3.0/bigframes/session/_io/__init__.py` & `bigframes-1.4.0/bigframes/session/_io/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/session/_io/bigquery.py` & `bigframes-1.4.0/bigframes/session/_io/bigquery.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import datetime
 import itertools
 import os
 import textwrap
 import types
 from typing import Dict, Iterable, Optional, Sequence, Tuple, Union
 import uuid
+import warnings
 
 import google.api_core.exceptions
 import google.cloud.bigquery as bigquery
 
 import bigframes
 from bigframes.core import log_adapter
 import bigframes.formatting_helpers as formatting_helpers
@@ -117,14 +118,67 @@
 
 
 def table_ref_to_sql(table: bigquery.TableReference) -> str:
     """Format a table reference as escaped SQL."""
     return f"`{table.project}`.`{table.dataset_id}`.`{table.table_id}`"
 
 
+def get_snapshot_datetime_and_table_metadata(
+    bqclient: bigquery.Client,
+    table_ref: bigquery.TableReference,
+    *,
+    api_name: str,
+    cache: Dict[bigquery.TableReference, Tuple[datetime.datetime, bigquery.Table]],
+    use_cache: bool = True,
+) -> Tuple[datetime.datetime, bigquery.Table]:
+    cached_table = cache.get(table_ref)
+    if use_cache and cached_table is not None:
+        snapshot_timestamp, _ = cached_table
+
+        # Cache hit could be unexpected. See internal issue 329545805.
+        # Raise a warning with more information about how to avoid the
+        # problems with the cache.
+        warnings.warn(
+            f"Reading cached table from {snapshot_timestamp} to avoid "
+            "incompatibilies with previous reads of this table. To read "
+            "the latest version, set `use_cache=False` or close the "
+            "current session with Session.close() or "
+            "bigframes.pandas.close_session().",
+            # There are many layers before we get to (possibly) the user's code:
+            # pandas.read_gbq_table
+            # -> with_default_session
+            # -> Session.read_gbq_table
+            # -> _read_gbq_table
+            # -> _get_snapshot_sql_and_primary_key
+            # -> get_snapshot_datetime_and_table_metadata
+            stacklevel=7,
+        )
+        return cached_table
+
+    # TODO(swast): It's possible that the table metadata is changed between now
+    # and when we run the CURRENT_TIMESTAMP() query to see when we can time
+    # travel to. Find a way to fetch the table metadata and BQ's current time
+    # atomically.
+    table = bqclient.get_table(table_ref)
+
+    # TODO(b/336521938): Refactor to make sure we set the "bigframes-api"
+    # whereever we execute a query.
+    job_config = bigquery.QueryJobConfig()
+    job_config.labels["bigframes-api"] = api_name
+    snapshot_timestamp = list(
+        bqclient.query(
+            "SELECT CURRENT_TIMESTAMP() AS `current_timestamp`",
+            job_config=job_config,
+        ).result()
+    )[0][0]
+    cached_table = (snapshot_timestamp, table)
+    cache[table_ref] = cached_table
+    return cached_table
+
+
 def create_snapshot_sql(
     table_ref: bigquery.TableReference, current_timestamp: datetime.datetime
 ) -> str:
     """Query a table via 'time travel' for consistent reads."""
     # If we have an anonymous query results table, it can't be modified and
     # there isn't any BigQuery time travel.
     if table_ref.dataset_id.startswith("_"):
```

### Comparing `bigframes-1.3.0/bigframes/session/_io/pandas.py` & `bigframes-1.4.0/bigframes/session/_io/pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/session/clients.py` & `bigframes-1.4.0/bigframes/session/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes/version.py` & `bigframes-1.4.0/bigframes/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
```

### Comparing `bigframes-1.3.0/bigframes.egg-info/PKG-INFO` & `bigframes-1.4.0/bigframes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.3.0
+Version: 1.4.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -82,14 +82,15 @@
 
 Documentation
 -------------
 
 * `BigQuery DataFrames source code (GitHub) <https://github.com/googleapis/python-bigquery-dataframes>`_
 * `BigQuery DataFrames sample notebooks <https://github.com/googleapis/python-bigquery-dataframes/tree/main/notebooks>`_
 * `BigQuery DataFrames API reference <https://cloud.google.com/python/docs/reference/bigframes/latest/summary_overview>`_
+* `BigQuery DataFrames supported pandas APIs <https://cloud.google.com/python/docs/reference/bigframes/latest/supported_pandas_apis>`_
 
 
 Getting started with BigQuery DataFrames
 ----------------------------------------
 Try the `BigQuery DataFrames quickstart <https://cloud.google.com/bigquery/docs/dataframes-quickstart>`_
 to get up and running in just a few minutes.
```

### Comparing `bigframes-1.3.0/bigframes.egg-info/SOURCES.txt` & `bigframes-1.4.0/bigframes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/bigframes.egg-info/requires.txt` & `bigframes-1.4.0/bigframes.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/setup.py` & `bigframes-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/__init__.py` & `bigframes-1.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/hockey_players.json` & `bigframes-1.4.0/tests/data/hockey_players.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/hockey_players.jsonl` & `bigframes-1.4.0/tests/data/hockey_players.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/nested.jsonl` & `bigframes-1.4.0/tests/data/nested.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/nested_schema.json` & `bigframes-1.4.0/tests/data/nested_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/penguins.jsonl` & `bigframes-1.4.0/tests/data/penguins.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/penguins_schema.json` & `bigframes-1.4.0/tests/data/penguins_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/scalars.jsonl` & `bigframes-1.4.0/tests/data/scalars.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/scalars_schema.json` & `bigframes-1.4.0/tests/data/scalars_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/data/time_series.jsonl` & `bigframes-1.4.0/tests/data/time_series.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/__init__.py` & `bigframes-1.4.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/conftest.py` & `bigframes-1.4.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/__init__.py` & `bigframes-1.4.0/tests/system/large/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_cluster.py` & `bigframes-1.4.0/tests/system/large/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_compose.py` & `bigframes-1.4.0/tests/system/large/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_core.py` & `bigframes-1.4.0/tests/system/large/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_decomposition.py` & `bigframes-1.4.0/tests/system/large/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_ensemble.py` & `bigframes-1.4.0/tests/system/large/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_forecasting.py` & `bigframes-1.4.0/tests/system/large/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_linear_model.py` & `bigframes-1.4.0/tests/system/large/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/ml/test_pipeline.py` & `bigframes-1.4.0/tests/system/large/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/test_location.py` & `bigframes-1.4.0/tests/system/large/test_location.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/large/test_remote_function.py` & `bigframes-1.4.0/tests/system/large/test_remote_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,14 +306,43 @@
     finally:
         # clean up the gcp assets created for the remote function
         cleanup_remote_function_assets(
             session.bqclient, session.cloudfunctionsclient, remote_add_one
         )
 
 
+@pytest.mark.parametrize(
+    ("input_types"),
+    [
+        pytest.param([int], id="list-of-int"),
+        pytest.param(int, id="int"),
+    ],
+)
+@pytest.mark.flaky(retries=2, delay=120)
+def test_remote_function_input_types(session, scalars_dfs, input_types):
+    try:
+
+        def add_one(x):
+            return x + 1
+
+        remote_add_one = session.remote_function(input_types, int)(add_one)
+
+        scalars_df, scalars_pandas_df = scalars_dfs
+
+        bf_result = scalars_df.int64_too.map(remote_add_one).to_pandas()
+        pd_result = scalars_pandas_df.int64_too.map(add_one)
+
+        pandas.testing.assert_series_equal(bf_result, pd_result, check_dtype=False)
+    finally:
+        # clean up the gcp assets created for the remote function
+        cleanup_remote_function_assets(
+            session.bqclient, session.cloudfunctionsclient, remote_add_one
+        )
+
+
 @pytest.mark.flaky(retries=2, delay=120)
 def test_remote_function_explicit_dataset_not_created(
     session,
     scalars_dfs,
     dataset_id_not_created,
     bq_cf_connection,
 ):
@@ -1332,7 +1361,56 @@
 
         pandas.testing.assert_series_equal(bf_result, pd_result, check_dtype=False)
     finally:
         # clean up the gcp assets created for the remote function
         cleanup_remote_function_assets(
             session.bqclient, session.cloudfunctionsclient, square_remote
         )
+
+
+@pytest.mark.parametrize(
+    ("timeout_args", "effective_gcf_timeout"),
+    [
+        pytest.param({}, 600, id="no-set"),
+        pytest.param({"cloud_function_timeout": None}, 60, id="set-None"),
+        pytest.param({"cloud_function_timeout": 1200}, 1200, id="set-max-allowed"),
+    ],
+)
+@pytest.mark.flaky(retries=2, delay=120)
+def test_remote_function_gcf_timeout(
+    session, scalars_dfs, timeout_args, effective_gcf_timeout
+):
+    try:
+
+        def square(x):
+            return x * x
+
+        square_remote = session.remote_function(
+            [int], int, reuse=False, **timeout_args
+        )(square)
+
+        # Assert that the GCF is created with the intended maximum timeout
+        gcf = session.cloudfunctionsclient.get_function(
+            name=square_remote.bigframes_cloud_function
+        )
+        assert gcf.service_config.timeout_seconds == effective_gcf_timeout
+
+        scalars_df, scalars_pandas_df = scalars_dfs
+
+        bf_result = scalars_df["int64_too"].apply(square_remote).to_pandas()
+        pd_result = scalars_pandas_df["int64_too"].apply(square)
+
+        pandas.testing.assert_series_equal(bf_result, pd_result, check_dtype=False)
+    finally:
+        # clean up the gcp assets created for the remote function
+        cleanup_remote_function_assets(
+            session.bqclient, session.cloudfunctionsclient, square_remote
+        )
+
+
+@pytest.mark.flaky(retries=2, delay=120)
+def test_remote_function_gcf_timeout_max_supported_exceeded(session):
+    with pytest.raises(ValueError):
+
+        @session.remote_function([int], int, reuse=False, cloud_function_timeout=1201)
+        def square(x):
+            return x * x
```

### Comparing `bigframes-1.3.0/tests/system/large/test_session.py` & `bigframes-1.4.0/tests/system/large/test_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/load/test_large_tables.py` & `bigframes-1.4.0/tests/system/load/test_large_tables.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,7 +86,18 @@
         row_count += batch_row_count
 
         # Attempt to save on memory by manually removing the batch df
         # from local memory after finishing with processing.
         del df
 
     assert row_count == expected_row_count
+
+
+def test_to_pandas_large_table():
+    df = bpd.read_gbq("load_testing.scalars_10gb")
+    # df will be downloaded locally
+    expected_row_count, expected_column_count = df.shape
+
+    df = df.to_pandas()
+    row_count, column_count = df.shape
+    assert column_count == expected_column_count
+    assert row_count == expected_row_count
```

### Comparing `bigframes-1.3.0/tests/system/small/__init__.py` & `bigframes-1.4.0/tests/system/small/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/__init__.py` & `bigframes-1.4.0/tests/system/small/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/conftest.py` & `bigframes-1.4.0/tests/system/small/ml/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_cluster.py` & `bigframes-1.4.0/tests/system/small/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_core.py` & `bigframes-1.4.0/tests/system/small/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_decomposition.py` & `bigframes-1.4.0/tests/system/small/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_ensemble.py` & `bigframes-1.4.0/tests/system/small/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_forecasting.py` & `bigframes-1.4.0/tests/system/small/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_imported.py` & `bigframes-1.4.0/tests/system/small/ml/test_imported.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_linear_model.py` & `bigframes-1.4.0/tests/system/small/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_llm.py` & `bigframes-1.4.0/tests/system/small/ml/test_llm.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_metrics.py` & `bigframes-1.4.0/tests/system/small/ml/test_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_metrics_pairwise.py` & `bigframes-1.4.0/tests/system/small/ml/test_metrics_pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_model_selection.py` & `bigframes-1.4.0/tests/system/small/ml/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_preprocessing.py` & `bigframes-1.4.0/tests/system/small/ml/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_register.py` & `bigframes-1.4.0/tests/system/small/ml/test_register.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/ml/test_remote.py` & `bigframes-1.4.0/tests/system/small/ml/test_remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/operations/__init__.py` & `bigframes-1.4.0/tests/system/small/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/operations/test_datetimes.py` & `bigframes-1.4.0/tests/system/small/operations/test_datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/operations/test_plotting.py` & `bigframes-1.4.0/tests/system/small/operations/test_plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/operations/test_strings.py` & `bigframes-1.4.0/tests/system/small/operations/test_strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/regression/test_issue355_merge_after_filter.py` & `bigframes-1.4.0/tests/system/small/regression/test_issue355_merge_after_filter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_dataframe.py` & `bigframes-1.4.0/tests/system/small/test_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2386,20 +2386,35 @@
         bf_result,
     )
 
 
 def test_dataframe_agg_single_string(scalars_dfs):
     numeric_cols = ["int64_col", "int64_too", "float64_col"]
     scalars_df, scalars_pandas_df = scalars_dfs
+
     bf_result = scalars_df[numeric_cols].agg("sum").to_pandas()
     pd_result = scalars_pandas_df[numeric_cols].agg("sum")
 
-    # Pandas may produce narrower numeric types, but bigframes always produces Float64
-    pd_result = pd_result.astype("Float64")
-    pd.testing.assert_series_equal(pd_result, bf_result, check_index_type=False)
+    assert bf_result.dtype == "Float64"
+    pd.testing.assert_series_equal(
+        pd_result, bf_result, check_dtype=False, check_index_type=False
+    )
+
+
+def test_dataframe_agg_int_single_string(scalars_dfs):
+    numeric_cols = ["int64_col", "int64_too", "bool_col"]
+    scalars_df, scalars_pandas_df = scalars_dfs
+
+    bf_result = scalars_df[numeric_cols].agg("sum").to_pandas()
+    pd_result = scalars_pandas_df[numeric_cols].agg("sum")
+
+    assert bf_result.dtype == "Int64"
+    pd.testing.assert_series_equal(
+        pd_result, bf_result, check_dtype=False, check_index_type=False
+    )
 
 
 def test_dataframe_agg_multi_string(scalars_dfs):
     numeric_cols = ["int64_col", "int64_too", "float64_col"]
     aggregations = [
         "sum",
         "mean",
@@ -2427,14 +2442,35 @@
 
     # Double-check that median is at least plausible.
     assert (
         (bf_result.loc["min", :] <= bf_median) & (bf_median <= bf_result.loc["max", :])
     ).all()
 
 
+def test_dataframe_agg_int_multi_string(scalars_dfs):
+    numeric_cols = ["int64_col", "int64_too", "bool_col"]
+    aggregations = [
+        "sum",
+        "nunique",
+        "count",
+    ]
+    scalars_df, scalars_pandas_df = scalars_dfs
+    bf_result = scalars_df[numeric_cols].agg(aggregations).to_pandas()
+    pd_result = scalars_pandas_df[numeric_cols].agg(aggregations)
+
+    for dtype in bf_result.dtypes:
+        assert dtype == "Int64"
+
+    # Pandas may produce narrower numeric types
+    # Pandas has object index type
+    pd.testing.assert_frame_equal(
+        pd_result, bf_result, check_dtype=False, check_index_type=False
+    )
+
+
 @skip_legacy_pandas
 def test_df_describe(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     # pyarrows time columns fail in pandas
     unsupported_columns = ["datetime_col", "timestamp_col", "time_col", "date_col"]
     bf_result = scalars_df.describe().to_pandas()
 
@@ -2461,14 +2497,51 @@
         (bf_min <= bf_p25)
         & (bf_p25 <= bf_p50)
         & (bf_p50 <= bf_p50)
         & (bf_p75 <= bf_max)
     ).all()
 
 
+def test_df_transpose():
+    # Include some floats to ensure type coercion
+    values = [[0, 3.5, True], [1, 4.5, False], [2, 6.5, None]]
+    # Test complex case of both axes being multi-indices with non-unique elements
+    columns = pd.Index(["A", "B", "A"], dtype=pd.StringDtype(storage="pyarrow"))
+    columns_multi = pd.MultiIndex.from_arrays([columns, columns], names=["c1", "c2"])
+    index = pd.Index(["b", "a", "a"], dtype=pd.StringDtype(storage="pyarrow"))
+    rows_multi = pd.MultiIndex.from_arrays([index, index], names=["r1", "r2"])
+
+    pd_df = pandas.DataFrame(values, index=rows_multi, columns=columns_multi)
+    bf_df = dataframe.DataFrame(values, index=rows_multi, columns=columns_multi)
+
+    pd_result = pd_df.T
+    bf_result = bf_df.T.to_pandas()
+
+    pd.testing.assert_frame_equal(pd_result, bf_result, check_dtype=False)
+
+
+def test_df_transpose_error():
+    with pytest.raises(TypeError, match="Cannot coerce.*to a common type."):
+        dataframe.DataFrame([[1, "hello"], [2, "world"]]).transpose()
+
+
+def test_df_transpose_repeated_uses_cache():
+    bf_df = dataframe.DataFrame([[1, 2.5], [2, 3.5]])
+    pd_df = pandas.DataFrame([[1, 2.5], [2, 3.5]])
+    # Transposing many times so that operation will fail from complexity if not using cache
+    for i in range(10):
+        # Cache still works even with simple scalar binop
+        bf_df = bf_df.transpose() + i
+        pd_df = pd_df.transpose() + i
+
+    pd.testing.assert_frame_equal(
+        pd_df, bf_df.to_pandas(), check_dtype=False, check_index_type=False
+    )
+
+
 @pytest.mark.parametrize(
     ("ordered"),
     [
         (True),
         (False),
     ],
 )
@@ -2956,49 +3029,105 @@
     with pytest.raises(Exception):
         bf_df.loc[bf_df["int64_too"] == 1, "string_col"] = 99
     with pytest.raises(Exception):
         pd_df.loc[pd_df["int64_too"] == 1, "string_col"] = 99
 
 
 @pytest.mark.parametrize(
+    ("col", "op"),
+    [
+        # Int aggregates
+        pytest.param("int64_col", lambda x: x.sum(), id="int-sum"),
+        pytest.param("int64_col", lambda x: x.min(), id="int-min"),
+        pytest.param("int64_col", lambda x: x.max(), id="int-max"),
+        pytest.param("int64_col", lambda x: x.count(), id="int-count"),
+        pytest.param("int64_col", lambda x: x.nunique(), id="int-nunique"),
+        # Float aggregates
+        pytest.param("float64_col", lambda x: x.count(), id="float-count"),
+        pytest.param("float64_col", lambda x: x.nunique(), id="float-nunique"),
+        # Bool aggregates
+        pytest.param("bool_col", lambda x: x.sum(), id="bool-sum"),
+        pytest.param("bool_col", lambda x: x.count(), id="bool-count"),
+        pytest.param("bool_col", lambda x: x.nunique(), id="bool-nunique"),
+        # String aggregates
+        pytest.param("string_col", lambda x: x.count(), id="string-count"),
+        pytest.param("string_col", lambda x: x.nunique(), id="string-nunique"),
+    ],
+)
+def test_dataframe_aggregate_int(scalars_df_index, scalars_pandas_df_index, col, op):
+    bf_result = op(scalars_df_index[[col]]).to_pandas()
+    pd_result = op(scalars_pandas_df_index[[col]])
+
+    # Check dtype separately
+    assert bf_result.dtype == "Int64"
+
+    # Pandas may produce narrower numeric types
+    # Pandas has object index type
+    assert_series_equal(pd_result, bf_result, check_dtype=False, check_index_type=False)
+
+
+@pytest.mark.parametrize(
+    ("col", "op"),
+    [
+        pytest.param("bool_col", lambda x: x.min(), id="bool-min"),
+        pytest.param("bool_col", lambda x: x.max(), id="bool-max"),
+    ],
+)
+def test_dataframe_aggregate_bool(scalars_df_index, scalars_pandas_df_index, col, op):
+    bf_result = op(scalars_df_index[[col]]).to_pandas()
+    pd_result = op(scalars_pandas_df_index[[col]])
+
+    # Check dtype separately
+    assert bf_result.dtype == "boolean"
+
+    # Pandas may produce narrower numeric types
+    # Pandas has object index type
+    assert_series_equal(pd_result, bf_result, check_dtype=False, check_index_type=False)
+
+
+@pytest.mark.parametrize(
     ("ordered"),
     [
         (True),
         (False),
     ],
 )
 @pytest.mark.parametrize(
-    ("op"),
+    ("op", "bf_dtype"),
     [
-        (lambda x: x.sum(numeric_only=True)),
-        (lambda x: x.mean(numeric_only=True)),
-        (lambda x: x.min(numeric_only=True)),
-        (lambda x: x.max(numeric_only=True)),
-        (lambda x: x.std(numeric_only=True)),
-        (lambda x: x.var(numeric_only=True)),
-        (lambda x: x.count(numeric_only=False)),
-        (lambda x: x.nunique()),
+        (lambda x: x.sum(numeric_only=True), "Float64"),
+        (lambda x: x.mean(numeric_only=True), "Float64"),
+        (lambda x: x.min(numeric_only=True), "Float64"),
+        (lambda x: x.max(numeric_only=True), "Float64"),
+        (lambda x: x.std(numeric_only=True), "Float64"),
+        (lambda x: x.var(numeric_only=True), "Float64"),
+        (lambda x: x.count(numeric_only=False), "Int64"),
+        (lambda x: x.nunique(), "Int64"),
     ],
     ids=["sum", "mean", "min", "max", "std", "var", "count", "nunique"],
 )
-def test_dataframe_aggregates(scalars_df_index, scalars_pandas_df_index, op, ordered):
+def test_dataframe_aggregates(
+    scalars_df_index, scalars_pandas_df_index, op, bf_dtype, ordered
+):
     col_names = ["int64_too", "float64_col", "string_col", "int64_col", "bool_col"]
     bf_series = op(scalars_df_index[col_names])
-    pd_series = op(scalars_pandas_df_index[col_names])
     bf_result = bf_series.to_pandas(ordered=ordered)
+    pd_result = op(scalars_pandas_df_index[col_names])
+
+    # Check dtype separately
+    assert bf_result.dtype == bf_dtype
 
     # Pandas may produce narrower numeric types, but bigframes always produces Float64
     # Pandas has object index type
-    pd_series.index = pd_series.index.astype(pd.StringDtype(storage="pyarrow"))
     assert_series_equal(
-        pd_series,
+        pd_result,
         bf_result,
+        check_dtype=False,
         check_index_type=False,
         ignore_order=not ordered,
-        check_dtype=False,
     )
 
 
 @pytest.mark.parametrize(
     ("op"),
     [
         (lambda x: x.sum(axis=1, numeric_only=True)),
@@ -4071,15 +4200,15 @@
 
 def test_df_cached(scalars_df_index):
     df = scalars_df_index.set_index(["int64_too", "int64_col"]).sort_values(
         "string_col"
     )
     df = df[df["rowindex_2"] % 2 == 0]
 
-    df_cached_copy = df._cached()
+    df_cached_copy = df.cache()
     pandas.testing.assert_frame_equal(df.to_pandas(), df_cached_copy.to_pandas())
 
 
 def test_df_dot_inline(session):
     df1 = pd.DataFrame([[1, 2, 3], [2, 5, 7]])
     df2 = pd.DataFrame([[2, 4, 8], [1, 5, 10], [3, 6, 9]])
```

### Comparing `bigframes-1.3.0/tests/system/small/test_dataframe_io.py` & `bigframes-1.4.0/tests/system/small/test_dataframe_io.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_encryption.py` & `bigframes-1.4.0/tests/system/small/test_encryption.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_groupby.py` & `bigframes-1.4.0/tests/system/small/test_groupby.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_ibis.py` & `bigframes-1.4.0/tests/system/small/test_ibis.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_index.py` & `bigframes-1.4.0/tests/system/small/test_index.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_ipython.py` & `bigframes-1.4.0/tests/system/small/test_ipython.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_multiindex.py` & `bigframes-1.4.0/tests/system/small/test_multiindex.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_numpy.py` & `bigframes-1.4.0/tests/system/small/test_numpy.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_pandas.py` & `bigframes-1.4.0/tests/system/small/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_pandas_options.py` & `bigframes-1.4.0/tests/system/small/test_pandas_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_progress_bar.py` & `bigframes-1.4.0/tests/system/small/test_progress_bar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_remote_function.py` & `bigframes-1.4.0/tests/system/small/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_scalar.py` & `bigframes-1.4.0/tests/system/small/test_scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_series.py` & `bigframes-1.4.0/tests/system/small/test_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,83 @@
 
     # BigQuery DataFrame default indices use nullable Int64 always
     pd_result.index = pd_result.index.astype("Int64")
 
     pd.testing.assert_series_equal(bf_result, pd_result)
 
 
+def test_series_construct_reindex():
+    bf_result = series.Series(
+        series.Series({1: 10, 2: 30, 3: 30}), index=[3, 2], dtype="Int64"
+    ).to_pandas()
+    pd_result = pd.Series(pd.Series({1: 10, 2: 30, 3: 30}), index=[3, 2], dtype="Int64")
+
+    # BigQuery DataFrame default indices use nullable Int64 always
+    pd_result.index = pd_result.index.astype("Int64")
+
+    pd.testing.assert_series_equal(bf_result, pd_result)
+
+
+def test_series_construct_from_list_w_index():
+    bf_result = series.Series(
+        [1, 1, 2, 3, 5, 8, 13], index=[10, 20, 30, 40, 50, 60, 70], dtype="Int64"
+    ).to_pandas()
+    pd_result = pd.Series(
+        [1, 1, 2, 3, 5, 8, 13], index=[10, 20, 30, 40, 50, 60, 70], dtype="Int64"
+    )
+
+    # BigQuery DataFrame default indices use nullable Int64 always
+    pd_result.index = pd_result.index.astype("Int64")
+
+    pd.testing.assert_series_equal(bf_result, pd_result)
+
+
+def test_series_construct_empty(session: bigframes.Session):
+    bf_series: series.Series = series.Series(session=session)
+    pd_series: pd.Series = pd.Series()
+
+    bf_result = bf_series.empty
+    pd_result = pd_series.empty
+
+    assert pd_result
+    assert bf_result == pd_result
+
+
+def test_series_construct_scalar_no_index():
+    bf_result = series.Series("hello world", dtype="string[pyarrow]").to_pandas()
+    pd_result = pd.Series("hello world", dtype="string[pyarrow]")
+
+    # BigQuery DataFrame default indices use nullable Int64 always
+    pd_result.index = pd_result.index.astype("Int64")
+
+    pd.testing.assert_series_equal(bf_result, pd_result)
+
+
+def test_series_construct_scalar_w_index():
+    bf_result = series.Series(
+        "hello world", dtype="string[pyarrow]", index=[0, 2, 1]
+    ).to_pandas()
+    pd_result = pd.Series("hello world", dtype="string[pyarrow]", index=[0, 2, 1])
+
+    # BigQuery DataFrame default indices use nullable Int64 always
+    pd_result.index = pd_result.index.astype("Int64")
+
+    pd.testing.assert_series_equal(bf_result, pd_result)
+
+
+def test_series_construct_nan():
+    bf_result = series.Series(numpy.nan).to_pandas()
+    pd_result = pd.Series(numpy.nan)
+
+    pd_result.index = pd_result.index.astype("Int64")
+    pd_result = pd_result.astype("Float64")
+
+    pd.testing.assert_series_equal(bf_result, pd_result)
+
+
 def test_series_construct_from_list_escaped_strings():
     """Check that special characters are supported."""
     strings = [
         "string\nwith\nnewline",
         "string\twith\ttabs",
         "string\\with\\backslashes",
     ]
@@ -945,25 +1014,14 @@
 
     # BigQuery DataFrames default indices use nullable Int64 always
     pd_result.index = pd_result.index.astype("Int64")
 
     pd.testing.assert_frame_equal(bf_result.to_pandas(), pd_result)
 
 
-def test_series_add_pandas_series_not_implemented(scalars_dfs):
-    scalars_df, _ = scalars_dfs
-    with pytest.raises(NotImplementedError):
-        (
-            scalars_df["float64_col"]
-            + pd.Series(
-                [1, 1, 1, 1],
-            )
-        ).to_pandas()
-
-
 def test_copy(scalars_df_index, scalars_pandas_df_index):
     col_name = "float64_col"
     # Expect mutation on original not to effect_copy
     bf_series = scalars_df_index[col_name].copy()
     bf_copy = bf_series.copy()
     bf_copy.loc[0] = 5.6
     bf_series.loc[0] = 3.4
@@ -1265,14 +1323,35 @@
 
     assert_series_equal(
         bf_result,
         pd_result,
     )
 
 
+@pytest.mark.parametrize(
+    ("other",),
+    [
+        ([-1.4, 2.3, None],),
+        (pd.Index([-1.4, 2.3, None]),),
+        (pd.Series([-1.4, 2.3, None], index=[44, 2, 1]),),
+    ],
+)
+@skip_legacy_pandas
+def test_series_binop_w_other_types(scalars_dfs, other):
+    scalars_df, scalars_pandas_df = scalars_dfs
+
+    bf_result = (scalars_df["int64_col"].head(3) + other).to_pandas()
+    pd_result = scalars_pandas_df["int64_col"].head(3) + other
+
+    assert_series_equal(
+        bf_result,
+        pd_result,
+    )
+
+
 @skip_legacy_pandas
 def test_series_combine_first(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     int64_col = scalars_df["int64_col"].head(7)
     float64_col = scalars_df["float64_col"].tail(7)
     bf_result = int64_col.combine_first(float64_col).to_pandas()
 
@@ -1767,25 +1846,14 @@
         scalars_pandas_df["string_col"] == "won't find this"
     ].empty
 
     assert pd_result
     assert pd_result == bf_result
 
 
-def test_empty_true_memtable(session: bigframes.Session):
-    bf_series: series.Series = series.Series(session=session)
-    pd_series: pd.Series = pd.Series()
-
-    bf_result = bf_series.empty
-    pd_result = pd_series.empty
-
-    assert pd_result
-    assert bf_result == pd_result
-
-
 def test_series_names(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
     bf_result = scalars_df["string_col"].copy()
     bf_result.index.name = "new index name"
     bf_result.name = "new series name"
```

### Comparing `bigframes-1.3.0/tests/system/small/test_session.py` & `bigframes-1.4.0/tests/system/small/test_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/small/test_window.py` & `bigframes-1.4.0/tests/system/small/test_window.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/system/utils.py` & `bigframes-1.4.0/tests/system/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/__init__.py` & `bigframes-1.4.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/_config/__init__.py` & `bigframes-1.4.0/tests/unit/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/_config/test_bigquery_options.py` & `bigframes-1.4.0/tests/unit/_config/test_bigquery_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/core/__init__.py` & `bigframes-1.4.0/tests/unit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/core/test_bf_utils.py` & `bigframes-1.4.0/tests/unit/core/test_bf_utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/core/test_blocks.py` & `bigframes-1.4.0/tests/unit/core/test_blocks.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/core/test_expression.py` & `bigframes-1.4.0/tests/unit/core/test_expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/core/test_log_adapter.py` & `bigframes-1.4.0/tests/unit/core/test_log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/ml/__init__.py` & `bigframes-1.4.0/tests/unit/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/ml/test_api_primitives.py` & `bigframes-1.4.0/tests/unit/ml/test_api_primitives.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/ml/test_compose.py` & `bigframes-1.4.0/tests/unit/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/ml/test_golden_sql.py` & `bigframes-1.4.0/tests/unit/ml/test_golden_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     return bqml_model_factory
 
 
 @pytest.fixture
 def mock_y():
     mock_y = mock.create_autospec(spec=bpd.DataFrame)
     mock_y.columns = pd.Index(["input_column_label"])
-    mock_y._cached.return_value = mock_y
+    mock_y.cache.return_value = mock_y
 
     return mock_y
 
 
 @pytest.fixture
 def mock_X(mock_y, mock_session):
     mock_X = mock.create_autospec(spec=bpd.DataFrame)
@@ -79,15 +79,15 @@
     )
     mock_X.join(mock_y).sql = "input_X_y_sql"
     mock_X.join(mock_y)._to_sql_query.return_value = (
         "input_X_y_sql",
         ["index_column_id"],
         ["index_column_label"],
     )
-    mock_X._cached.return_value = mock_X
+    mock_X.cache.return_value = mock_X
 
     return mock_X
 
 
 @pytest.fixture
 def bqml_model(mock_session):
     bqml_model = core.BqmlModel(
```

### Comparing `bigframes-1.3.0/tests/unit/ml/test_pipeline.py` & `bigframes-1.4.0/tests/unit/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/ml/test_sql.py` & `bigframes-1.4.0/tests/unit/ml/test_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,14 +315,28 @@
     assert (
         sql
         == """SELECT * FROM ML.PREDICT(MODEL `my_project_id.my_dataset_id.my_model_id`,
   (input_X_sql))"""
     )
 
 
+def test_ml_llm_evaluate_correct(
+    model_manipulation_sql_generator: ml_sql.ModelManipulationSqlGenerator,
+    mock_df: bpd.DataFrame,
+):
+    sql = model_manipulation_sql_generator.ml_llm_evaluate(
+        source_df=mock_df, task_type="CLASSIFICATION"
+    )
+    assert (
+        sql
+        == """SELECT * FROM ML.EVALUATE(MODEL `my_project_id.my_dataset_id.my_model_id`,
+            (input_X_sql), STRUCT("CLASSIFICATION" AS task_type))"""
+    )
+
+
 def test_ml_evaluate_correct(
     model_manipulation_sql_generator: ml_sql.ModelManipulationSqlGenerator,
     mock_df: bpd.DataFrame,
 ):
     sql = model_manipulation_sql_generator.ml_evaluate(source_df=mock_df)
     assert (
         sql
```

### Comparing `bigframes-1.3.0/tests/unit/resources.py` & `bigframes-1.4.0/tests/unit/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,23 +40,33 @@
     table_schema: Sequence[google.cloud.bigquery.SchemaField] = TEST_SCHEMA,
     anonymous_dataset: Optional[google.cloud.bigquery.DatasetReference] = None,
 ) -> bigframes.Session:
     credentials = mock.create_autospec(
         google.auth.credentials.Credentials, instance=True
     )
 
+    if anonymous_dataset is None:
+        anonymous_dataset = google.cloud.bigquery.DatasetReference(
+            "test-project",
+            "test_dataset",
+        )
+
     if bqclient is None:
         bqclient = mock.create_autospec(google.cloud.bigquery.Client, instance=True)
         bqclient.project = "test-project"
 
         # Mock the location.
         table = mock.create_autospec(google.cloud.bigquery.Table, instance=True)
         table._properties = {}
         type(table).location = mock.PropertyMock(return_value="test-region")
         type(table).schema = mock.PropertyMock(return_value=table_schema)
+        type(table).reference = mock.PropertyMock(
+            return_value=anonymous_dataset.table("test_table")
+        )
+        type(table).num_rows = mock.PropertyMock(return_value=1000000000)
         bqclient.get_table.return_value = table
 
     if anonymous_dataset is None:
         anonymous_dataset = google.cloud.bigquery.DatasetReference(
             "test-project",
             "test_dataset",
         )
```

### Comparing `bigframes-1.3.0/tests/unit/session/__init__.py` & `bigframes-1.4.0/tests/unit/session/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/session/test_clients.py` & `bigframes-1.4.0/tests/unit/session/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/session/test_io_bigquery.py` & `bigframes-1.4.0/tests/unit/session/test_io_bigquery.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/session/test_io_pandas.py` & `bigframes-1.4.0/tests/unit/session/test_io_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/session/test_session.py` & `bigframes-1.4.0/tests/unit/session/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,18 +38,31 @@
 
 def test_read_gbq_cached_table():
     session = resources.create_bigquery_session()
     table_ref = google.cloud.bigquery.TableReference(
         google.cloud.bigquery.DatasetReference("my-project", "my_dataset"),
         "my_table",
     )
-    session._df_snapshot[table_ref] = datetime.datetime(
-        1999, 1, 2, 3, 4, 5, 678901, tzinfo=datetime.timezone.utc
+    table = google.cloud.bigquery.Table(table_ref)
+    table._properties["location"] = session._location
+    session._df_snapshot[table_ref] = (
+        datetime.datetime(1999, 1, 2, 3, 4, 5, 678901, tzinfo=datetime.timezone.utc),
+        table,
     )
 
+    def get_table_mock(table_ref):
+        table = google.cloud.bigquery.Table(
+            table_ref, (google.cloud.bigquery.SchemaField("col", "INTEGER"),)
+        )
+        table._properties["numRows"] = "1000000000"
+        table._properties["location"] = session._location
+        return table
+
+    session.bqclient.get_table = get_table_mock
+
     with pytest.warns(UserWarning, match=re.escape("use_cache=False")):
         df = session.read_gbq("my-project.my_dataset.my_table")
 
     assert "1999-01-02T03:04:05.678901" in df.sql
 
 
 def test_read_gbq_clustered_table_ok_default_index_with_primary_key():
@@ -130,18 +143,21 @@
                 "Access Denied: BigQuery BigQuery: Permission denied while getting Drive credentials."
             )
 
         return session_query_mock(query, *args, **kwargs)
 
     session.bqclient.query = query_mock
 
-    def get_table_mock(dataset_ref):
-        dataset = google.cloud.bigquery.Dataset(dataset_ref)
-        dataset.location = session._location
-        return dataset
+    def get_table_mock(table_ref):
+        table = google.cloud.bigquery.Table(
+            table_ref, (google.cloud.bigquery.SchemaField("col", "INTEGER"),)
+        )
+        table._properties["numRows"] = 1000000000
+        table._properties["location"] = session._location
+        return table
 
     session.bqclient.get_table = get_table_mock
 
     api = getattr(session, api_name)
     with pytest.raises(
         google.api_core.exceptions.Forbidden,
         match="Check https://cloud.google.com/bigquery/docs/query-drive-data#Google_Drive_permissions.",
```

### Comparing `bigframes-1.3.0/tests/unit/test_clients.py` & `bigframes-1.4.0/tests/unit/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_compute_options.py` & `bigframes-1.4.0/tests/unit/test_compute_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_core.py` & `bigframes-1.4.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_dataframe.py` & `bigframes-1.4.0/tests/unit/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_dtypes.py` & `bigframes-1.4.0/tests/unit/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_features.py` & `bigframes-1.4.0/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_formatting_helper.py` & `bigframes-1.4.0/tests/unit/test_formatting_helper.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_formatting_helpers.py` & `bigframes-1.4.0/tests/unit/test_formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_pandas.py` & `bigframes-1.4.0/tests/unit/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/tests/unit/test_remote_function.py` & `bigframes-1.4.0/tests/unit/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/cpython/LICENSE` & `bigframes-1.4.0/third_party/bigframes_vendored/cpython/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/cpython/_pprint.py` & `bigframes-1.4.0/third_party/bigframes_vendored/cpython/_pprint.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE` & `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py` & `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py` & `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py` & `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py` & `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py` & `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/LICENSE.txt` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/README.md` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py` & `bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/AUTHORS.md` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/LICENSE` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/README.md` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/_config/config.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/_config/config.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/common.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/align.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/align.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/common.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/engines.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/engines.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/eval.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/expr.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/expr.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/ops.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/ops.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/scope.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/scope.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/config_init.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/config_init.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/frame.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,96 @@
                 Whether to ensure that the returned value is not a view
                 on another array.
             na_value (default None):
                 The value to use for missing values.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    @property
+    def T(self) -> DataFrame:
+        """
+        The transpose of the DataFrame.
+
+        All columns must be the same dtype (numerics can be coerced to a common supertype).
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+            >>> df = bpd.DataFrame({'col1': [1, 2], 'col2': [3, 4]})
+            >>> df
+               col1  col2
+            0     1     3
+            1     2     4
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+            >>> df.T
+                  0  1
+            col1  1  2
+            col2  3  4
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+        Returns:
+            DataFrame: The transposed DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def transpose(self) -> DataFrame:
+        """
+        Transpose index and columns.
+
+        Reflect the DataFrame over its main diagonal by writing rows as columns
+        and vice-versa. The property :attr:`.T` is an accessor to the method
+        :meth:`transpose`.
+
+        All columns must be the same dtype (numerics can be coerced to a common supertype).
+
+        **Examples:**
+
+            **Square DataFrame with homogeneous dtype**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+
+            >>> d1 = {'col1': [1, 2], 'col2': [3, 4]}
+            >>> df1 = bpd.DataFrame(data=d1)
+            >>> df1
+               col1  col2
+            0     1     3
+            1     2     4
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+            >>> df1_transposed = df1.T  # or df1.transpose()
+            >>> df1_transposed
+                  0  1
+            col1  1  2
+            col2  3  4
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+            When the dtype is homogeneous in the original DataFrame, we get a
+            transposed DataFrame with the same dtype:
+
+            >>> df1.dtypes
+            col1    Int64
+            col2    Int64
+            dtype: object
+            >>> df1_transposed.dtypes
+            0    Int64
+            1    Int64
+            dtype: object
+
+        Returns:
+            DataFrame: The transposed DataFrame.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def info(
         self,
         verbose: bool | None = None,
         buf=None,
         max_cols: int | None = None,
         memory_usage: bool | None = None,
         show_counts: bool | None = None,
@@ -3806,15 +3888,15 @@
             >>> bpd.options.display.progress_bar = None
 
         Let's use ``reuse=False`` flag to make sure a new ``remote_function``
         is created every time we run the following code, but you can skip it
         to potentially reuse a previously deployed ``remote_function`` from
         the same user defined function.
 
-            >>> @bpd.remote_function([int], float, reuse=False)
+            >>> @bpd.remote_function(int, float, reuse=False)
             ... def minutes_to_hours(x):
             ...     return x/60
 
             >>> df_minutes = bpd.DataFrame(
             ...     {"system_minutes" : [0, 30, 60, 90, 120],
             ...      "user_minutes" : [0, 15, 75, 90, 6]})
             >>> df_minutes
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/generic.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/generic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/base.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexing.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/series.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,15 +1177,15 @@
 
         For applying arbitrary python function a `remote_funciton` is recommended.
         Let's use ``reuse=False`` flag to make sure a new `remote_function`
         is created every time we run the following code, but you can skip it
         to potentially reuse a previously deployed `remote_function` from
         the same user defined function.
 
-            >>> @bpd.remote_function([int], float, reuse=False)
+            >>> @bpd.remote_function(int, float, reuse=False)
             ... def minutes_to_hours(x):
             ...     return x/60
 
             >>> minutes = bpd.Series([0, 30, 60, 90, 120])
             >>> minutes
             0      0
             1     30
@@ -1204,15 +1204,15 @@
             dtype: Float64
 
         To turn a user defined function with external package dependencies into
         a `remote_function`, you would provide the names of the packages via
         `packages` param.
 
             >>> @bpd.remote_function(
-            ...     [str],
+            ...     str,
             ...     str,
             ...     reuse=False,
             ...     packages=["cryptography"],
             ... )
             ... def get_hash(input):
             ...     from cryptography.fernet import Fernet
             ...
@@ -3337,15 +3337,15 @@
             dtype: Int64
 
         You can also use a remote function to evaluate the mask condition. This
         is useful in situation such as the following, where the mask
         condition is evaluated based on a complicated business logic which cannot
         be expressed in form of a Series.
 
-            >>> @bpd.remote_function([str], bool, reuse=False)
+            >>> @bpd.remote_function(str, bool, reuse=False)
             ... def should_mask(name):
             ...     hash = 0
             ...     for char_ in name:
             ...         hash += ord(char_)
             ...     return hash % 2 == 0
 
             >>> s = bpd.Series(["Alice", "Bob", "Caroline"])
@@ -3856,15 +3856,15 @@
             1     puppy
             2      <NA>
             3      <NA>
             dtype: string
 
         It also accepts a remote function:
 
-            >>> @bpd.remote_function([str], str)
+            >>> @bpd.remote_function(str, str)
             ... def my_mapper(val):
             ...     vowels = ["a", "e", "i", "o", "u"]
             ...     if val:
             ...         return "".join([
             ...             ch.upper() if ch in vowels else ch for ch in val
             ...         ])
             ...     return "N/A"
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/rolling.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/rolling.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/common.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/gbq.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/gbq.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parquet.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parquet.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/pickle.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/pickle.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/pandas/_typing.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/pandas/_typing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/plotting/_core.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_exceptions.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_exceptions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_validators.py` & `bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_validators.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/COPYING` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/COPYING`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/base.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 DataFrame of shape (n_samples, n_features). Training data.
             y (default None):
                 Not used, present here for API consistency by convention.
 
         Returns:
-            KMeans: Fitted Estimator.
+            KMeans: Fitted estimator.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def predict(
         self,
         X,
     ):
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
             y (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 Series or DataFrame of shape (n_samples,) or (n_samples, n_targets).
                 Target values. Will be cast to X's dtype if necessary.
 
 
         Returns:
-            ForestModel: Fitted Estimator.
+            ForestModel: Fitted estimator.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
 
 class ForestRegressor(RegressorMixin, BaseForest, metaclass=ABCMeta):
     """
     Base class for forest of trees-based regressors.
@@ -91,15 +91,15 @@
     to improve the predictive accuracy and control over-fitting.
 
     Args:
         n_estimators (Optional[int]):
             Number of parallel trees constructed during each iteration. Default to 100. Minimum value is 2.
         tree_method (Optional[str]):
             Specify which tree method to use. Default to "auto". If this parameter is set to
-            default, XGBoost will choose the most conservative option available. Possible values: ""exact", "approx",
+            default, XGBoost will choose the most conservative option available. Possible values: "exact", "approx",
             "hist".
         min_child_weight (Optional[float]):
             Minimum sum of instance weight(hessian) needed in a child. Default to 1.
         colsample_bytree (Optional[float]):
             Subsample ratio of columns when constructing each tree. Default to 1.0. The value should be between 0 and 1.
         colsample_bylevel (Optional[float]):
             Subsample ratio of columns for each level. Default to 1.0. The value should be between 0 and 1.
@@ -156,15 +156,15 @@
     improve the predictive accuracy and control over-fitting.
 
     Args:
         n_estimators (Optional[int]):
             Number of parallel trees constructed during each iteration. Default to 100. Minimum value is 2.
         tree_method (Optional[str]):
             Specify which tree method to use. Default to "auto". If this parameter is set to
-            default, XGBoost will choose the most conservative option available. Possible values: ""exact", "approx",
+            default, XGBoost will choose the most conservative option available. Possible values: "exact", "approx",
             "hist".
         min_child_weight (Optional[float]):
             Minimum sum of instance weight(hessian) needed in a child. Default to 1.
         colsample_bytree (Optional[float]):
             Subsample ratio of columns when constructing each tree. Default to 1.0. The value should be between 0 and 1.
         colsample_bylevel (Optional[float]):
             Subsample ratio of columns for each level. Default to 1.0. The value should be between 0 and 1.
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,10 +105,10 @@
                 Series or DataFrame of shape (n_samples, n_features). Training data.
 
             y (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 Series or DataFrame of shape (n_samples,) or (n_samples, n_targets).
                 Target values. Will be cast to X's dtype if necessary.
 
         Returns:
-            LinearRegression: Fitted Estimator.
+            LinearRegression: Fitted estimator.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,10 +75,10 @@
                 the number of features.
 
             y (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 DataFrame of shape (n_samples,). Target vector relative to X.
 
 
         Returns:
-            LogisticRegression: Fitted Estimator.
+            LogisticRegression: Fitted estimator.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,40 +17,40 @@
     Args:
         X (Series or single column DataFrame of array of numeric type):
             Input data.
         Y (Series or single column DataFrame of array of numeric type):
             Input data. X and Y are mapped by indexes, must have the same index.
 
     Returns:
-        bigframes.dataframe.DataFrame: DataFrame with columns of X, Y and cosine_distance
+        bigframes.dataframe.DataFrame: DataFrame with columns of X, Y and cosine_distance.
     """
     raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
 
 def paired_manhattan_distance(X, Y) -> bpd.DataFrame:
     """Compute the L1 distances between the vectors in X and Y.
 
     Args:
         X (Series or single column DataFrame of array of numeric type):
             Input data.
         Y (Series or single column DataFrame of array of numeric type):
             Input data. X and Y are mapped by indexes, must have the same index.
 
     Returns:
-        bigframes.dataframe.DataFrame: DataFrame with columns of X, Y and manhattan_distance
+        bigframes.dataframe.DataFrame: DataFrame with columns of X, Y and manhattan_distance.
     """
     raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
 
 def paired_euclidean_distances(X, Y) -> bpd.DataFrame:
     """Compute the paired euclidean distances between X and Y.
 
     Args:
         X (Series or single column DataFrame of array of numeric type):
             Input data.
         Y (Series or single column DataFrame of array of numeric type):
             Input data. X and Y are mapped by indexes, must have the same index.
 
     Returns:
-        bigframes.dataframe.DataFrame: DataFrame with columns of X, Y and euclidean_distance
+        bigframes.dataframe.DataFrame: DataFrame with columns of X, Y and euclidean_distance.
     """
     raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/pipeline.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,16 @@
 
     Sequentially apply a list of transforms and a final estimator.
     Intermediate steps of the pipeline must be `transforms`. That is, they
     must implement `fit` and `transform` methods.
     The final estimator only needs to implement `fit`.
 
     The purpose of the pipeline is to assemble several steps that can be
-    cross-validated together while setting different parameters. This
-    simplifies code and allows for deploying an estimator and peprocessing
-    together, e.g. with `Pipeline.to_gbq(...).`
+    cross-validated together while setting different parameters. This simplifies code and allows for
+    deploying an estimator and preprocessing together, e.g. with `Pipeline.to_gbq(...).`
     """
 
     def fit(
         self,
         X,
         y,
     ):
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,10 +80,10 @@
         """Transform X using one-hot encoding.
 
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 The DataFrame or Series to be transformed.
 
         Returns:
-            bigframes.dataframe.DataFrame: The result is categorized as index: number, value: number.
-                Where index is the position of the dict that seeing the category, and value is 0 or 1."""
+            bigframes.dataframe.DataFrame: The result is categorized as index: number, value: number,
+                where index is the position of the dict seeing the category, and value is 0 or 1."""
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py` & `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/xgboost/LICENSE` & `bigframes-1.4.0/third_party/bigframes_vendored/xgboost/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.3.0/third_party/bigframes_vendored/xgboost/sklearn.py` & `bigframes-1.4.0/third_party/bigframes_vendored/xgboost/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 Series or DataFrame of shape (n_samples, n_features). Training data.
 
             y (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 DataFrame of shape (n_samples,) or (n_samples, n_targets).
                 Target values. Will be cast to X's dtype if necessary.
 
         Returns:
-            XGBModel: Fitted Estimator.
+            XGBModel: Fitted estimator.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
 
 class XGBClassifierMixIn:
     """MixIn for classification."""
 
@@ -59,15 +59,15 @@
             Number of parallel trees constructed during each iteration. Default to 1.
         booster (Optional[str]):
             Specify which booster to use: gbtree or dart. Default to "gbtree".
         dart_normalized_type (Optional[str]):
             Type of normalization algorithm for DART booster. Possible values: "TREE", "FOREST". Default to "TREE".
         tree_method (Optional[str]):
             Specify which tree method to use.  Default to "auto". If this parameter is set to
-            default, XGBoost will choose the most conservative option available. Possible values: ""exact", "approx",
+            default, XGBoost will choose the most conservative option available. Possible values: "exact", "approx",
             "hist".
         min_child_weight (Optional[float]):
             Minimum sum of instance weight(hessian) needed in a child. Default to 1.
         colsample_bytree (Optional[float]):
             Subsample ratio of columns when constructing each tree. Default to 1.0.
         colsample_bylevel (Optional[float]):
             Subsample ratio of columns for each level. Default to 1.0.
@@ -106,15 +106,15 @@
             Number of parallel trees constructed during each iteration. Default to 1.
         booster (Optional[str]):
             Specify which booster to use: gbtree or dart. Default to "gbtree".
         dart_normalized_type (Optional[str]):
             Type of normalization algorithm for DART booster. Possible values: "TREE", "FOREST". Default to "TREE".
         tree_method (Optional[str]):
             Specify which tree method to use.  Default to "auto". If this parameter is set to
-            default, XGBoost will choose the most conservative option available. Possible values: ""exact", "approx",
+            default, XGBoost will choose the most conservative option available. Possible values: "exact", "approx",
             "hist".
         min_child_weight (Optional[float]):
             Minimum sum of instance weight(hessian) needed in a child. Default to 1.
         colsample_bytree (Optional[float]):
             Subsample ratio of columns when constructing each tree. Default to 1.0.
         colsample_bylevel (Optional[float]):
             Subsample ratio of columns for each level. Default to 1.0.
```

