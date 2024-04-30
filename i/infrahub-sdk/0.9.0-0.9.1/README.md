# Comparing `tmp/infrahub_sdk-0.9.0.tar.gz` & `tmp/infrahub_sdk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahub_sdk-0.9.0.tar", max compression
+gzip compressed data, was "infrahub_sdk-0.9.1.tar", max compression
```

## Comparing `infrahub_sdk-0.9.0.tar` & `infrahub_sdk-0.9.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0       34 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/README.md
--rw-r--r--   0        0        0     1941 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/__init__.py
--rw-r--r--   0        0        0     4207 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/analyzer.py
--rw-r--r--   0        0        0      892 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/async_typer.py
--rw-r--r--   0        0        0     2148 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/batch.py
--rw-r--r--   0        0        0    10121 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/branch.py
--rw-r--r--   0        0        0     6132 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/checks.py
--rw-r--r--   0        0        0    49831 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/client.py
--rw-r--r--   0        0        0     4765 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/config.py
--rw-r--r--   0        0        0      138 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/constants.py
--rw-r--r--   0        0        0        0 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/__init__.py
--rw-r--r--   0        0        0     7193 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/branch.py
--rw-r--r--   0        0        0     7974 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/check.py
--rw-r--r--   0        0        0      328 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/cli.py
--rw-r--r--   0        0        0    11482 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/cli_commands.py
--rw-r--r--   0        0        0     1456 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/client.py
--rw-r--r--   0        0        0     2892 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/config.py
--rw-r--r--   0        0        0      472 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/exceptions.py
--rw-r--r--   0        0        0     2076 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/exporter.py
--rw-r--r--   0        0        0     2021 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/importer.py
--rw-r--r--   0        0        0     1577 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/repository.py
--rw-r--r--   0        0        0     5751 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/schema.py
--rw-r--r--   0        0        0      403 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/transform.py
--rw-r--r--   0        0        0     3468 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/utils.py
--rw-r--r--   0        0        0     4260 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/ctl/validate.py
--rw-r--r--   0        0        0      585 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/data.py
--rw-r--r--   0        0        0     3999 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/exceptions.py
--rw-r--r--   0        0        0     5746 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/graphql.py
--rw-r--r--   0        0        0     1181 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/jinja2.py
--rw-r--r--   0        0        0    68862 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/node.py
--rw-r--r--   0        0        0     4351 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/object_store.py
--rw-r--r--   0        0        0     2006 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/playback.py
--rw-r--r--   0        0        0        0 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     2217 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/exceptions.py
--rw-r--r--   0        0        0     1026 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/__init__.py
--rw-r--r--   0        0        0     2750 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/base.py
--rw-r--r--   0        0        0     3286 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/check.py
--rw-r--r--   0        0        0     2367 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/graphql_query.py
--rw-r--r--   0        0        0     5384 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/jinja2_transform.py
--rw-r--r--   0        0        0     3805 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/python_transform.py
--rw-r--r--   0        0        0     4206 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/loader.py
--rw-r--r--   0        0        0     7390 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/models.py
--rw-r--r--   0        0        0     4483 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/plugin.py
--rw-r--r--   0        0        0      558 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/utils.py
--rw-r--r--   0        0        0     1034 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/queries.py
--rw-r--r--   0        0        0    11549 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/query_groups.py
--rw-r--r--   0        0        0     2282 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/recorder.py
--rw-r--r--   0        0        0    33812 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/schema.py
--rw-r--r--   0        0        0     2638 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/store.py
--rw-r--r--   0        0        0     6535 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/task_report.py
--rw-r--r--   0        0        0     2637 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/timestamp.py
--rw-r--r--   0        0        0     1092 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/topological_sort.py
--rw-r--r--   0        0        0        0 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/__init__.py
--rw-r--r--   0        0        0       56 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/constants.py
--rw-r--r--   0        0        0      257 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-15 10:22:25.555012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/exporter/__init__.py
--rw-r--r--   0        0        0      306 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/exporter/interface.py
--rw-r--r--   0        0        0     6960 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/exporter/json.py
--rw-r--r--   0        0        0        0 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/importer/__init__.py
--rw-r--r--   0        0        0      203 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/importer/interface.py
--rw-r--r--   0        0        0     9699 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/importer/json.py
--rw-r--r--   0        0        0     1239 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transfer/schema_sorter.py
--rw-r--r--   0        0        0     3641 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/transforms.py
--rw-r--r--   0        0        0      777 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/types.py
--rw-r--r--   0        0        0     9865 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/utils.py
--rw-r--r--   0        0        0     2135 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/uuidt.py
--rw-r--r--   0        0        0      751 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/infrahub_sdk/yaml.py
--rw-r--r--   0        0        0     7637 2024-03-15 10:22:25.559012 infrahub_sdk-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 infrahub_sdk-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-03-19 08:44:15.084405 infrahub_sdk-0.9.1/README.md
+-rw-r--r--   0        0        0     1941 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/__init__.py
+-rw-r--r--   0        0        0     4207 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/analyzer.py
+-rw-r--r--   0        0        0      892 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/async_typer.py
+-rw-r--r--   0        0        0     2148 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/batch.py
+-rw-r--r--   0        0        0    10121 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/branch.py
+-rw-r--r--   0        0        0     6132 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/checks.py
+-rw-r--r--   0        0        0    49831 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/client.py
+-rw-r--r--   0        0        0     4765 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/config.py
+-rw-r--r--   0        0        0      138 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/constants.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/__init__.py
+-rw-r--r--   0        0        0     7193 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/branch.py
+-rw-r--r--   0        0        0     7974 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/check.py
+-rw-r--r--   0        0        0      328 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/cli.py
+-rw-r--r--   0        0        0    11482 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/cli_commands.py
+-rw-r--r--   0        0        0     1456 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/client.py
+-rw-r--r--   0        0        0     2893 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/config.py
+-rw-r--r--   0        0        0      472 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/exceptions.py
+-rw-r--r--   0        0        0     2076 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/exporter.py
+-rw-r--r--   0        0        0     2021 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/importer.py
+-rw-r--r--   0        0        0     1577 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/repository.py
+-rw-r--r--   0        0        0     5751 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/schema.py
+-rw-r--r--   0        0        0      403 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/transform.py
+-rw-r--r--   0        0        0     3468 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/utils.py
+-rw-r--r--   0        0        0     4260 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/ctl/validate.py
+-rw-r--r--   0        0        0      585 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/data.py
+-rw-r--r--   0        0        0     3999 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/exceptions.py
+-rw-r--r--   0        0        0     5746 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/graphql.py
+-rw-r--r--   0        0        0     1181 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/jinja2.py
+-rw-r--r--   0        0        0    68862 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/node.py
+-rw-r--r--   0        0        0     4351 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/object_store.py
+-rw-r--r--   0        0        0     2006 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/playback.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     2217 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/exceptions.py
+-rw-r--r--   0        0        0     1026 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/__init__.py
+-rw-r--r--   0        0        0     2750 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/base.py
+-rw-r--r--   0        0        0     3286 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/check.py
+-rw-r--r--   0        0        0     2367 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/graphql_query.py
+-rw-r--r--   0        0        0     5384 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/jinja2_transform.py
+-rw-r--r--   0        0        0     3805 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/python_transform.py
+-rw-r--r--   0        0        0     4206 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/loader.py
+-rw-r--r--   0        0        0     7390 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/models.py
+-rw-r--r--   0        0        0     4483 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0      558 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/utils.py
+-rw-r--r--   0        0        0     1034 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/queries.py
+-rw-r--r--   0        0        0    11549 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/query_groups.py
+-rw-r--r--   0        0        0     2282 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/recorder.py
+-rw-r--r--   0        0        0    33812 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/schema.py
+-rw-r--r--   0        0        0     2638 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/store.py
+-rw-r--r--   0        0        0     6535 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/task_report.py
+-rw-r--r--   0        0        0     2633 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/timestamp.py
+-rw-r--r--   0        0        0     1088 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/topological_sort.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/__init__.py
+-rw-r--r--   0        0        0       56 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/constants.py
+-rw-r--r--   0        0        0      237 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/exporter/__init__.py
+-rw-r--r--   0        0        0      298 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/exporter/interface.py
+-rw-r--r--   0        0        0     6960 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/exporter/json.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/importer/__init__.py
+-rw-r--r--   0        0        0      195 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/importer/interface.py
+-rw-r--r--   0        0        0     9701 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/importer/json.py
+-rw-r--r--   0        0        0     1239 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transfer/schema_sorter.py
+-rw-r--r--   0        0        0     3641 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/transforms.py
+-rw-r--r--   0        0        0      761 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/types.py
+-rw-r--r--   0        0        0     9865 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/utils.py
+-rw-r--r--   0        0        0     2135 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/uuidt.py
+-rw-r--r--   0        0        0      751 2024-03-19 08:44:15.088405 infrahub_sdk-0.9.1/infrahub_sdk/yaml.py
+-rw-r--r--   0        0        0     7802 2024-03-19 08:44:15.092405 infrahub_sdk-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 infrahub_sdk-0.9.1/PKG-INFO
```

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/__init__.py` & `infrahub_sdk-0.9.1/infrahub_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/analyzer.py` & `infrahub_sdk-0.9.1/infrahub_sdk/analyzer.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/async_typer.py` & `infrahub_sdk-0.9.1/infrahub_sdk/async_typer.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/batch.py` & `infrahub_sdk-0.9.1/infrahub_sdk/batch.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/branch.py` & `infrahub_sdk-0.9.1/infrahub_sdk/branch.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/checks.py` & `infrahub_sdk-0.9.1/infrahub_sdk/checks.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/client.py` & `infrahub_sdk-0.9.1/infrahub_sdk/client.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/config.py` & `infrahub_sdk-0.9.1/infrahub_sdk/config.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/branch.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/branch.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/check.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/check.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/cli_commands.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/cli_commands.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/client.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/client.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/config.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Config Clas."""
+
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import toml
 import typer
 
 try:
```

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/exporter.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/exporter.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/importer.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/importer.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/repository.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/repository.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/schema.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/schema.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/utils.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/utils.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/ctl/validate.py` & `infrahub_sdk-0.9.1/infrahub_sdk/ctl/validate.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/data.py` & `infrahub_sdk-0.9.1/infrahub_sdk/data.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/exceptions.py` & `infrahub_sdk-0.9.1/infrahub_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/graphql.py` & `infrahub_sdk-0.9.1/infrahub_sdk/graphql.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/jinja2.py` & `infrahub_sdk-0.9.1/infrahub_sdk/jinja2.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/node.py` & `infrahub_sdk-0.9.1/infrahub_sdk/node.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/object_store.py` & `infrahub_sdk-0.9.1/infrahub_sdk/object_store.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/playback.py` & `infrahub_sdk-0.9.1/infrahub_sdk/playback.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/exceptions.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/__init__.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/base.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/base.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/check.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/check.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/graphql_query.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/graphql_query.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/jinja2_transform.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/jinja2_transform.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/items/python_transform.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/items/python_transform.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/loader.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/loader.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/models.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/models.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/plugin.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/pytest_plugin/utils.py` & `infrahub_sdk-0.9.1/infrahub_sdk/pytest_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/queries.py` & `infrahub_sdk-0.9.1/infrahub_sdk/queries.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/query_groups.py` & `infrahub_sdk-0.9.1/infrahub_sdk/query_groups.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/recorder.py` & `infrahub_sdk-0.9.1/infrahub_sdk/recorder.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/schema.py` & `infrahub_sdk-0.9.1/infrahub_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/store.py` & `infrahub_sdk-0.9.1/infrahub_sdk/store.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/task_report.py` & `infrahub_sdk-0.9.1/infrahub_sdk/task_report.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/timestamp.py` & `infrahub_sdk-0.9.1/infrahub_sdk/timestamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 REGEX_MAPPING = {
     "seconds": r"(\d+)(s|sec|second|seconds)",
     "minutes": r"(\d+)(m|min|minute|minutes)",
     "hours": r"(\d+)(h|hour|hours)",
 }
 
 
-class TimestampFormatError(ValueError):
-    ...
+class TimestampFormatError(ValueError): ...
 
 
 class Timestamp:
     def __init__(self, value: Optional[Union[str, DateTime, Timestamp]] = None):
         if value and isinstance(value, DateTime):
             self.obj = value
         elif value and isinstance(value, self.__class__):
```

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/topological_sort.py` & `infrahub_sdk-0.9.1/infrahub_sdk/topological_sort.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from itertools import chain
 from typing import Iterable, List, Mapping, Set
 
 
-class DependencyCycleExistsError(Exception):
-    ...
+class DependencyCycleExistsError(Exception): ...
 
 
 def topological_sort(dependency_dict: Mapping[str, Iterable[str]]) -> List[Set[str]]:
     if not dependency_dict:
         return []
 
     missing_dependent_keys = set(chain(*dependency_dict.values())) - set(dependency_dict.keys())
```

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/transfer/exporter/json.py` & `infrahub_sdk-0.9.1/infrahub_sdk/transfer/exporter/json.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/transfer/importer/json.py` & `infrahub_sdk-0.9.1/infrahub_sdk/transfer/importer/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,17 @@
     async def remove_and_store_optional_relationships(self) -> None:
         for node in self.all_nodes.values():
             node_kind = node.get_kind()
 
             # Build a relationship name to relationship schema map, so we can retrieve the schema based on the name of a relationship later
             for relationship_schema in self.schemas_by_kind[node_kind].relationships:
                 if relationship_schema.optional:
-                    self.optional_relationships_schemas_by_node_kind[node_kind][
-                        relationship_schema.name
-                    ] = relationship_schema
+                    self.optional_relationships_schemas_by_node_kind[node_kind][relationship_schema.name] = (
+                        relationship_schema
+                    )
 
             for relationship_name in self.optional_relationships_schemas_by_node_kind[node_kind].keys():
                 relationship_value = getattr(node, relationship_name)
                 if isinstance(relationship_value, RelationshipManager):
                     if relationship_value.peer_ids:
                         self.optional_relationships_by_node[node.id][relationship_name] = relationship_value
                         setattr(node, relationship_name, None)
```

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/transfer/schema_sorter.py` & `infrahub_sdk-0.9.1/infrahub_sdk/transfer/schema_sorter.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/transforms.py` & `infrahub_sdk-0.9.1/infrahub_sdk/transforms.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/types.py` & `infrahub_sdk-0.9.1/infrahub_sdk/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,22 +19,20 @@
     def __call__(
         self,
         url: str,
         method: HTTPMethod,
         headers: Dict[str, Any],
         timeout: int,
         payload: Optional[Dict] = None,
-    ) -> httpx.Response:
-        ...
+    ) -> httpx.Response: ...
 
 
 @runtime_checkable
 class AsyncRequester(Protocol):
     async def __call__(
         self,
         url: str,
         method: HTTPMethod,
         headers: Dict[str, Any],
         timeout: int,
         payload: Optional[Dict] = None,
-    ) -> httpx.Response:
-        ...
+    ) -> httpx.Response: ...
```

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/utils.py` & `infrahub_sdk-0.9.1/infrahub_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/uuidt.py` & `infrahub_sdk-0.9.1/infrahub_sdk/uuidt.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/infrahub_sdk/yaml.py` & `infrahub_sdk-0.9.1/infrahub_sdk/yaml.py`

 * *Files identical despite different names*

### Comparing `infrahub_sdk-0.9.0/pyproject.toml` & `infrahub_sdk-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "infrahub-sdk"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python Client to interact with Infrahub"
 authors = ["OpsMill <contact@opsmill.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://opsmill.io"
 repository = "https://opsmill.io"
 documentation = "https://opsmill.io"
@@ -32,16 +32,16 @@
 pendulum = [
     { version = ">=2", python = ">=3.8,<3.12" },
     { version = ">=3", python = ">=3.12" }
 ]
 gitpython = "^3"
 Jinja2 = { version = "^3", optional = true }
 numpy = [
-    { version = "^1.24.2", optional = true , python = ">=3.8,<3.12" },
-    { version = "^1.26.2", optional = true , python = ">=3.12" }
+    { version = "^1.24.2", optional = true,  python = ">=3.8,<3.12" },
+    { version = "^1.26.2", optional = true,  python = ">=3.12" }
 ]
 pyarrow = { version = "^14", optional = true }
 rich = { version = "^13", optional = true }
 toml = { version = "^0.10", optional = true }
 typer = { version = "^0", optional = true }
 ujson = { version = "^5", optional = true }
 pytest = { version = "*", optional = true }
@@ -60,15 +60,15 @@
 requests = "*"
 pre-commit = "^2.20.0"
 autoflake = "*"
 types-toml = "*"
 types-ujson = "*"
 types-pyyaml = "*"
 typer-cli = "*"
-ruff = "^0.1.5"
+ruff = "0.3.3"
 pytest-xdist = "^3.3.1"
 types-python-slugify = "^8.0.0.3"
 
 [tool.poetry.extras]
 ctl = [
     "Jinja2",
     "numpy",
@@ -81,14 +81,25 @@
 ]
 tests = [
     "Jinja2",
     "pytest",
     "pyyaml",
     "rich"
 ]
+all = [
+    "Jinja2",
+    "numpy",
+    "pyarrow",
+    "pytest",
+    "pyyaml",
+    "rich",
+    "toml",
+    "typer",
+    "ujson"
+]
 
 [tool.poetry.scripts]
 infrahubctl = "infrahub_sdk.ctl.cli:app"
 
 [tool.poetry.plugins."pytest11"]
 "pytest-infrahub"="infrahub_sdk.pytest_plugin.plugin"
 
@@ -133,14 +144,15 @@
     too-many-instance-attributes,
     too-many-statements,
     fixme,
     consider-using-f-string,
     protected-access,
     import-self,
     wrong-import-order,
+    multiple-statements,
     """
 
 [tool.pylint.miscellaneous]
 notes = """,
     FIXME,
     XXX,
     """
@@ -186,22 +198,24 @@
         "env",
         "_build",
         "build",
         "dist",
         "examples",
 ]
 
+
+[tool.ruff.lint]
+preview = true
+
 task-tags = [
     "FIXME",
     "TODO",
     "XXX",
 ]
 
-[tool.ruff.lint]
-preview = true
 
 select = [
     "ASYNC", # flake8-async
     "B",     # flake8-bugbear
     "C4",    # flake8-comprehensions
     "C90",   # mccabe complexity
     "DJ",    # flake8-django
@@ -262,19 +276,19 @@
 
 [tool.ruff.lint.isort]
 known-first-party = ["infrahub_sdk", "infrahub_ctl"]
 
 [tool.ruff.lint.pycodestyle]
 max-line-length = 150
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 # Target max-complexity=10
 max-complexity = 17
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 
 "tests/**/*.py" = [
     "PLR2004", # Magic value used in comparison
 ]
 
 "tests/unit/sdk/test_client.py" = [
     "W293", # Blank line contains whitespace (used within output check)
```

### Comparing `infrahub_sdk-0.9.0/PKG-INFO` & `infrahub_sdk-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: infrahub-sdk
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python Client to interact with Infrahub
 Home-page: https://opsmill.io
 License: Apache-2.0
 Author: OpsMill
 Author-email: contact@opsmill.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: all
 Provides-Extra: ctl
 Provides-Extra: tests
-Requires-Dist: Jinja2 (>=3,<4) ; extra == "ctl" or extra == "tests"
+Requires-Dist: Jinja2 (>=3,<4) ; extra == "ctl" or extra == "tests" or extra == "all"
 Requires-Dist: gitpython (>=3,<4)
 Requires-Dist: graphql-core (>=3.1,<3.3)
 Requires-Dist: httpx (>=0.20) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: httpx (>=0.23) ; python_version >= "3.11"
-Requires-Dist: numpy (>=1.24.2,<2.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "ctl")
-Requires-Dist: numpy (>=1.26.2,<2.0.0) ; (python_version >= "3.12") and (extra == "ctl")
+Requires-Dist: numpy (>=1.24.2,<2.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "ctl" or extra == "all")
+Requires-Dist: numpy (>=1.26.2,<2.0.0) ; (python_version >= "3.12") and (extra == "ctl" or extra == "all")
 Requires-Dist: pendulum (>=2) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: pendulum (>=3) ; python_version >= "3.12"
-Requires-Dist: pyarrow (>=14,<15) ; extra == "ctl"
+Requires-Dist: pyarrow (>=14,<15) ; extra == "ctl" or extra == "all"
 Requires-Dist: pydantic (>=1.7.4,!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0)
-Requires-Dist: pytest ; extra == "tests"
-Requires-Dist: pyyaml (>=6,<7) ; extra == "ctl" or extra == "tests"
-Requires-Dist: rich (>=13,<14) ; extra == "ctl" or extra == "tests"
-Requires-Dist: toml (>=0.10,<0.11) ; extra == "ctl"
-Requires-Dist: typer (>=0,<1) ; extra == "ctl"
-Requires-Dist: ujson (>=5,<6) ; extra == "ctl"
+Requires-Dist: pytest ; extra == "tests" or extra == "all"
+Requires-Dist: pyyaml (>=6,<7) ; extra == "ctl" or extra == "tests" or extra == "all"
+Requires-Dist: rich (>=13,<14) ; extra == "ctl" or extra == "tests" or extra == "all"
+Requires-Dist: toml (>=0.10,<0.11) ; extra == "ctl" or extra == "all"
+Requires-Dist: typer (>=0,<1) ; extra == "ctl" or extra == "all"
+Requires-Dist: ujson (>=5,<6) ; extra == "ctl" or extra == "all"
 Project-URL: Documentation, https://opsmill.io
 Project-URL: Repository, https://opsmill.io
 Description-Content-Type: text/markdown
 
 # Infrahub SDK
 
 .. Coming Soon ...
```

