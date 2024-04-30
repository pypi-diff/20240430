# Comparing `tmp/hamcontestanalysis-1.0.0.tar.gz` & `tmp/hamcontestanalysis-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamcontestanalysis-1.0.0.tar", max compression
+gzip compressed data, was "hamcontestanalysis-1.1.0.tar", max compression
```

## Comparing `hamcontestanalysis-1.0.0.tar` & `hamcontestanalysis-1.1.0.tar`

### file list

```diff
@@ -1,124 +1,123 @@
--rw-r--r--   0        0        0     1078 2024-04-24 11:02:43.281711 hamcontestanalysis-1.0.0/LICENSE
--rw-r--r--   0        0        0     2620 2024-04-24 11:02:43.281711 hamcontestanalysis-1.0.0/README.md
--rw-r--r--   0        0        0     2119 2024-04-24 11:02:59.473737 hamcontestanalysis-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       11 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/__init__.py
--rw-r--r--   0        0        0      127 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/__main__.py
--rw-r--r--   0        0        0      133 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/__init__.py
--rw-r--r--   0        0        0     1495 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/dashboard.py
--rw-r--r--   0        0        0     1540 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/download.py
--rw-r--r--   0        0        0      567 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/main.py
--rw-r--r--   0        0        0    13680 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/plot.py
--rw-r--r--   0        0        0      344 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/__init__.py
--rw-r--r--   0        0        0      259 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/logging.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/__init__.py
--rw-r--r--   0        0        0     2762 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/arrldx.py
--rw-r--r--   0        0        0     2456 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/cqwpx.py
--rw-r--r--   0        0        0     3089 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/cqww.py
--rw-r--r--   0        0        0     6915 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/general.py
--rw-r--r--   0        0        0     2791 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/iaru.py
--rw-r--r--   0        0        0      932 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/base.py
--rw-r--r--   0        0        0     2537 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/contest.py
--rw-r--r--   0        0        0      211 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/info.py
--rw-r--r--   0        0        0      366 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/logging.py
--rw-r--r--   0        0        0      965 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/settings.py
--rw-r--r--   0        0        0     1379 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/storage.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/arrldx/__init__.py
--rw-r--r--   0        0        0     3718 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/arrldx/storage_source.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/cqwpx/__init__.py
--rw-r--r--   0        0        0     2917 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/cqwpx/storage_source.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/cqww/__init__.py
--rw-r--r--   0        0        0     2935 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/cqww/storage_source.py
--rw-r--r--   0        0        0      818 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/data_sink.py
--rw-r--r--   0        0        0      779 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/data_source.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/iaru/__init__.py
--rw-r--r--   0        0        0     3409 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/iaru/storage_source.py
--rw-r--r--   0        0        0     2239 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/processed_contest_source.py
--rw-r--r--   0        0        0     1805 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/processed_rbn_source.py
--rw-r--r--   0        0        0     9875 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/raw_contest_cabrillo.py
--rw-r--r--   0        0        0      835 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/raw_contest_sink.py
--rw-r--r--   0        0        0      416 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/raw_rbn_sink.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/rbn/__init__.py
--rw-r--r--   0        0        0     3983 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/rbn/storage_source.py
--rw-r--r--   0        0        0     4603 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/storage_sink.py
--rw-r--r--   0        0        0     4497 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/storage_source.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/__init__.py
--rw-r--r--   0        0        0      885 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/assets/css/test.css
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/search.py
--rw-r--r--   0        0        0     2095 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_direction.py
--rw-r--r--   0        0        0     4935 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_evolution.py
--rw-r--r--   0        0        0     5010 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_log.py
--rw-r--r--   0        0        0     2621 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_propagation.py
--rw-r--r--   0        0        0     4945 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rates.py
--rw-r--r--   0        0        0     5927 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rbn.py
--rw-r--r--   0        0        0     2974 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_summary.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/__init__.py
--rw-r--r--   0        0        0      601 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/navbar.py
--rw-r--r--   0        0        0     2083 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/search.py
--rw-r--r--   0        0        0      520 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_direction.py
--rw-r--r--   0        0        0      904 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_evolution.py
--rw-r--r--   0        0        0      989 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_log.py
--rw-r--r--   0        0        0      538 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_propagation.py
--rw-r--r--   0        0        0      781 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_rates.py
--rw-r--r--   0        0        0      829 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_rbn.py
--rw-r--r--   0        0        0      839 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_summary.py
--rw-r--r--   0        0        0     3921 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/contest_analysis.py
--rw-r--r--   0        0        0     5357 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/snr_analysis.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/download/__init__.py
--rw-r--r--   0        0        0     1384 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/download/data_manipulation.py
--rw-r--r--   0        0        0     5604 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/download/main.py
--rw-r--r--   0        0        0      126 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/arrldx/__init__.py
--rw-r--r--   0        0        0     4620 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/arrldx/plot_contest_evolution.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/__init__.py
--rw-r--r--   0        0        0     1749 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_frequency.py
--rw-r--r--   0        0        0     5619 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_log_heatmap.py
--rw-r--r--   0        0        0     3256 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_minutes_from_previous_call.py
--rw-r--r--   0        0        0     2550 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_qso_direction.py
--rw-r--r--   0        0        0     3907 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_qsos_hour.py
--rw-r--r--   0        0        0     2869 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_rate.py
--rw-r--r--   0        0        0     2947 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_rolling_rate.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/cqwpx/__init__.py
--rw-r--r--   0        0        0     4633 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/cqwpx/plot_contest_evolution.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/cqww/__init__.py
--rw-r--r--   0        0        0     4571 2024-04-24 11:02:43.285711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/cqww/plot_contest_evolution.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/iaru/__init__.py
--rw-r--r--   0        0        0     4635 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/iaru/plot_contest_evolution.py
--rw-r--r--   0        0        0     2221 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/plot_base.py
--rw-r--r--   0        0        0     2143 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/plot_rbn_base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/__init__.py
--rw-r--r--   0        0        0     3451 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_band_conditions.py
--rw-r--r--   0        0        0     3824 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_cw_speed.py
--rw-r--r--   0        0        0     4061 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_number_rbn_spots.py
--rw-r--r--   0        0        0     3448 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_snr.py
--rw-r--r--   0        0        0     8088 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_snr_band_continent.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/py.typed
--rw-r--r--   0        0        0      638 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/settings/contest.yaml
--rw-r--r--   0        0        0      133 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/settings/info.yaml
--rw-r--r--   0        0        0      578 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/settings/logging.yaml
--rw-r--r--   0        0        0      317 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/settings/storage.yaml
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/arrldx/__init__.py
--rw-r--r--   0        0        0     1479 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/arrldx/table_contest_log.py
--rw-r--r--   0        0        0     2206 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/arrldx/table_contest_summary.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqwpx/__init__.py
--rw-r--r--   0        0        0     1614 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqwpx/table_contest_log.py
--rw-r--r--   0        0        0     2205 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqwpx/table_contest_summary.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqww/__init__.py
--rw-r--r--   0        0        0     2941 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqww/table_contest_log.py
--rw-r--r--   0        0        0     2365 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqww/table_contest_summary.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/iaru/__init__.py
--rw-r--r--   0        0        0     1479 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/iaru/table_contest_log.py
--rw-r--r--   0        0        0     2206 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/iaru/table_contest_summary.py
--rw-r--r--   0        0        0     4151 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/table_base.py
--rw-r--r--   0        0        0      210 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/__init__.py
--rw-r--r--   0        0        0      460 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/calculations/__init__.py
--rw-r--r--   0        0        0     1642 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/calculations/contests.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/dashboards/__init__.py
--rw-r--r--   0        0        0     1643 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/dashboards/callbacks_manager.py
--rw-r--r--   0        0        0        0 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/types/__init__.py
--rw-r--r--   0        0        0     1026 2024-04-24 11:02:43.289711 hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/types/dataframe_types.py
--rw-r--r--   0        0        0     3893 1970-01-01 00:00:00.000000 hamcontestanalysis-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-30 18:11:37.645761 hamcontestanalysis-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3043 2024-04-30 18:11:51.413756 hamcontestanalysis-1.1.0/README.md
+-rw-r--r--   0        0        0     2178 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/__main__.py
+-rw-r--r--   0        0        0      133 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/__init__.py
+-rw-r--r--   0        0        0      853 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/dashboard.py
+-rw-r--r--   0        0        0     1540 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/download.py
+-rw-r--r--   0        0        0      567 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/main.py
+-rw-r--r--   0        0        0    13680 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/plot.py
+-rw-r--r--   0        0        0      344 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/logging.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/__init__.py
+-rw-r--r--   0        0        0     2762 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/arrldx.py
+-rw-r--r--   0        0        0     2456 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/cqwpx.py
+-rw-r--r--   0        0        0     3089 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/cqww.py
+-rw-r--r--   0        0        0     6904 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/general.py
+-rw-r--r--   0        0        0     2791 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/iaru.py
+-rw-r--r--   0        0        0      932 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/base.py
+-rw-r--r--   0        0        0     2537 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/contest.py
+-rw-r--r--   0        0        0      211 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/info.py
+-rw-r--r--   0        0        0      366 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/logging.py
+-rw-r--r--   0        0        0      965 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/settings.py
+-rw-r--r--   0        0        0     1509 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/storage.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/arrldx/__init__.py
+-rw-r--r--   0        0        0     3718 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/arrldx/storage_source.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/cqwpx/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/cqwpx/storage_source.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/cqww/__init__.py
+-rw-r--r--   0        0        0     2935 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/cqww/storage_source.py
+-rw-r--r--   0        0        0      818 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/data_sink.py
+-rw-r--r--   0        0        0      779 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/data_source.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/iaru/__init__.py
+-rw-r--r--   0        0        0     3409 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/iaru/storage_source.py
+-rw-r--r--   0        0        0     2239 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/processed_contest_source.py
+-rw-r--r--   0        0        0     1805 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/processed_rbn_source.py
+-rw-r--r--   0        0        0     9875 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/raw_contest_cabrillo.py
+-rw-r--r--   0        0        0      835 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/raw_contest_sink.py
+-rw-r--r--   0        0        0      416 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/raw_rbn_sink.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/rbn/__init__.py
+-rw-r--r--   0        0        0     3983 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/rbn/storage_source.py
+-rw-r--r--   0        0        0     4603 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/storage_sink.py
+-rw-r--r--   0        0        0     4497 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/storage_source.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/assets/css/test.css
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/search.py
+-rw-r--r--   0        0        0     2095 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_direction.py
+-rw-r--r--   0        0        0     4935 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_evolution.py
+-rw-r--r--   0        0        0     5010 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_log.py
+-rw-r--r--   0        0        0     2621 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_propagation.py
+-rw-r--r--   0        0        0     4945 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rates.py
+-rw-r--r--   0        0        0     5927 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rbn.py
+-rw-r--r--   0        0        0     2974 2024-04-30 18:11:37.649761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_summary.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/navbar.py
+-rw-r--r--   0        0        0     2083 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/search.py
+-rw-r--r--   0        0        0      520 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_direction.py
+-rw-r--r--   0        0        0      904 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_evolution.py
+-rw-r--r--   0        0        0      989 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_log.py
+-rw-r--r--   0        0        0      538 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_propagation.py
+-rw-r--r--   0        0        0      781 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_rates.py
+-rw-r--r--   0        0        0      829 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_rbn.py
+-rw-r--r--   0        0        0      839 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_summary.py
+-rw-r--r--   0        0        0     3921 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/contest_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/download/__init__.py
+-rw-r--r--   0        0        0     1384 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/download/data_manipulation.py
+-rw-r--r--   0        0        0     5604 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/download/main.py
+-rw-r--r--   0        0        0      126 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/arrldx/__init__.py
+-rw-r--r--   0        0        0     4812 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/arrldx/plot_contest_evolution.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/__init__.py
+-rw-r--r--   0        0        0     1940 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_frequency.py
+-rw-r--r--   0        0        0     5810 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_log_heatmap.py
+-rw-r--r--   0        0        0     3442 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_minutes_from_previous_call.py
+-rw-r--r--   0        0        0     2750 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_qso_direction.py
+-rw-r--r--   0        0        0     4098 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_qsos_hour.py
+-rw-r--r--   0        0        0     3060 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_rate.py
+-rw-r--r--   0        0        0     3138 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_rolling_rate.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/cqwpx/__init__.py
+-rw-r--r--   0        0        0     4823 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/cqwpx/plot_contest_evolution.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/cqww/__init__.py
+-rw-r--r--   0        0        0     4761 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/cqww/plot_contest_evolution.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/iaru/__init__.py
+-rw-r--r--   0        0        0     4825 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/iaru/plot_contest_evolution.py
+-rw-r--r--   0        0        0     2538 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/plot_base.py
+-rw-r--r--   0        0        0     2425 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/plot_rbn_base.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/__init__.py
+-rw-r--r--   0        0        0     3642 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_band_conditions.py
+-rw-r--r--   0        0        0     4364 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_cw_speed.py
+-rw-r--r--   0        0        0     4554 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_number_rbn_spots.py
+-rw-r--r--   0        0        0     3941 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_snr.py
+-rw-r--r--   0        0        0     8573 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_snr_band_continent.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/py.typed
+-rw-r--r--   0        0        0      638 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/settings/contest.yaml
+-rw-r--r--   0        0        0      133 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/settings/info.yaml
+-rw-r--r--   0        0        0      578 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/settings/logging.yaml
+-rw-r--r--   0        0        0      497 2024-04-30 18:11:51.417756 hamcontestanalysis-1.1.0/src/hamcontestanalysis/settings/storage.yaml
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/arrldx/__init__.py
+-rw-r--r--   0        0        0     1479 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/arrldx/table_contest_log.py
+-rw-r--r--   0        0        0     2206 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/arrldx/table_contest_summary.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqwpx/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqwpx/table_contest_log.py
+-rw-r--r--   0        0        0     2205 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqwpx/table_contest_summary.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqww/__init__.py
+-rw-r--r--   0        0        0     2941 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqww/table_contest_log.py
+-rw-r--r--   0        0        0     2365 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqww/table_contest_summary.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/iaru/__init__.py
+-rw-r--r--   0        0        0     1479 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/iaru/table_contest_log.py
+-rw-r--r--   0        0        0     2206 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/iaru/table_contest_summary.py
+-rw-r--r--   0        0        0     4151 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/table_base.py
+-rw-r--r--   0        0        0      210 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/calculations/__init__.py
+-rw-r--r--   0        0        0     1642 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/calculations/contests.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/dashboards/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/dashboards/callbacks_manager.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/types/__init__.py
+-rw-r--r--   0        0        0     1026 2024-04-30 18:11:37.653761 hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/types/dataframe_types.py
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 hamcontestanalysis-1.1.0/PKG-INFO
```

### Comparing `hamcontestanalysis-1.0.0/LICENSE` & `hamcontestanalysis-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/README.md` & `hamcontestanalysis-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # HamContestAnalysis
 
 [![PyPI](https://img.shields.io/pypi/v/hamcontestanalysis.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/hamcontestanalysis.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/hamcontestanalysis)][python version]
 [![License](https://img.shields.io/pypi/l/hamcontestanalysis)][license]
 
 [![Read the documentation at https://hamcontestanalysis.readthedocs.io/](https://img.shields.io/readthedocs/hamcontestanalysis/latest.svg?label=Read%20the%20Docs)][read the docs]
 [![Tests](https://github.com/rogercaminal/hamcontestanalysis/workflows/Tests/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/rogercaminal/hamcontestanalysis/branch/main/graph/badge.svg)][codecov]
 
@@ -17,33 +16,39 @@
 [python version]: https://pypi.org/project/hamcontestanalysis
 [read the docs]: https://hamcontestanalysis.readthedocs.io/
 [tests]: https://github.com/rogercaminal/hamcontestanalysis/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/rogercaminal/hamcontestanalysis
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
-## Features
+<!-- ## Features
 
 - TODO
 
 ## Requirements
 
-- TODO
+- TODO -->
+
+## Introduction
+
+_HamContestAnalysis_ comprises a set of tools for radio amateurs dedicated to analyze contest with the maximum detail.
+
+This library is divided into two main components: a collection of functions and classes that allow to easily download public logs and process them for further analysis, as well as a dashboard that provides the user not only with a general view of the contest, but also with the possibility to compare between different call signs and/or years.
 
 ## Installation
 
-You can install _HamContestAnalysis_ via [pip] from [PyPI]:
+_HamContestAnalysis_ can be installed via [pip] from [PyPI]:
 
 ```console
 $ pip install hamcontestanalysis
 ```
 
 ## Usage
 
-Please see the [Command-line Reference] for details.
+Please see the [Command-line Reference] for technical details.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `hamcontestanalysis-1.0.0/pyproject.toml` & `hamcontestanalysis-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hamcontestanalysis"
-version = "1.0.0"
-description = "hca"
+version = "1.1.0"
+description = "Ham radio contest analysis tools"
 authors = ["Roger Caminal Armadans <roger.caminal@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rogercaminal/hamcontestanalysis"
 repository = "https://github.com/rogercaminal/hamcontestanalysis"
 documentation = "https://hamcontestanalysis.readthedocs.io"
 classifiers = [
@@ -23,14 +23,15 @@
 dynaconf = "3.1.12"
 pandas = "2.0.0"
 pyarrow = "12.0.1"
 pydantic = "1.10.7"
 pyhamtools = "0.8.7"
 python-dotenv = "1.0.1"
 typer = "0.9.0"
+sphinxcontrib-typer = "0.2.1"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/dashboard.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/dashboard.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from logging import getLogger
 
 from typer import Option
 from typer import Typer
 
 from hamcontestanalysis.modules.dashboard.contest_analysis import main as _main_contest
-from hamcontestanalysis.modules.dashboard.snr_analysis import main as _main_snr
 
 
 app = Typer(name="dashboard", add_completion=False)
 logger = getLogger(__name__)
 
 
 @app.command()
@@ -25,25 +24,7 @@
         "host = %s, port = %s",
         debug,
         host,
         port,
     )
 
     _main_contest(debug=debug, host=host, port=port)
-
-
-@app.command()
-def snr_analysis(
-    debug: bool = Option(False, "--debug", help="Debug the dashboard"),
-    host: str = Option("localhost", "--host", help="Host to run the dashboard"),
-    port: int = Option(8050, "--port", help="Port to run the dashboard"),
-) -> None:
-    """Dashboard main command line interface for RBN analysis."""
-    logger.info(
-        "Starting SNR dashboard with the following commands: Debug = %s, "
-        "host = %s, port = %s",
-        debug,
-        host,
-        port,
-    )
-
-    _main_snr(debug=debug, host=host, port=port)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/download.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/download.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/main.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/main.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/cli/plot.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/cli/plot.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/arrldx.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/arrldx.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/cqwpx.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/cqwpx.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/cqww.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/cqww.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/general.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,21 +143,20 @@
     return data
 
 
 def add_previous_calls_info(data: DataFrame) -> DataFrame:
     """Adds information about previous calls in other bands.
 
     It adds the following columns:
-    - minutes_from_previous_call: indicates the number of minutes since this
-        callsign previously called.
-    - band_transition_from_previous_call: the band that this callsign
-        previously called.
+    - minutes_from_previous_call: indicates the number of minutes since this callsign
+    previously called.
+    - band_transition_from_previous_call: the band that this callsign previously called.
 
     Args:
-        data (DataFrame): Data frame containing the log
+        data (DataFrame): Data frame containing the log.
 
     Returns:
         DataFrame: Dataframe with the new information added.
     """
     data = (
         data.join(
             data.query("is_valid")
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/commons/pandas/iaru.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/commons/pandas/iaru.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/__init__.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/base.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/base.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/contest.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/contest.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/settings.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/settings.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/config/storage.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/config/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 
 class StoragePathsSettings(BaseSettings):
     """S3 Paths Settings model."""
 
     raw_data: str
     raw_metadata: str
     raw_rbn: str
+    plots: str
     temporary: str
 
 
 class StorageSettings(BaseSettings):
     """Storage Settings model."""
 
     partitions: str
     prefix: str
     partitions_rbn: str
+    prefix_plots: str
+    partitions_plots: str
 
     @property
     def paths(self):
         """Render HamContestAnalysis paths from settings.
 
         This method renders the paths for types in 'optimisation', 'performance' and
         'temporary' by interpolating:
@@ -30,15 +33,16 @@
         the prefix via environment variables. This use case is needed on the staged
         executions to redirect S3 output on either environment.
         """
         return StoragePathsSettings(
             raw_data=(f"{self.prefix}/{self.partitions}/raw_data"),
             raw_metadata=(f"{self.prefix}/{self.partitions}/raw_metadata"),
             raw_rbn=(f"{self.prefix}/{self.partitions_rbn}/rbn"),
+            plots=(f"{self.prefix_plots}/{self.partitions_plots}"),
             temporary=f"{self.prefix}/temporary",
         )
 
     # pylint: disable=too-few-public-methods
     class Config:
         """Pydantic model config."""
 
-        env_prefix = "PYCA_STORAGE__"
+        env_prefix = "HCA_STORAGE__"
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/arrldx/storage_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/arrldx/storage_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/cqwpx/storage_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/cqwpx/storage_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/cqww/storage_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/cqww/storage_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/data_sink.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/data_sink.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/data_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/data_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/iaru/storage_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/iaru/storage_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/processed_contest_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/processed_contest_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/processed_rbn_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/processed_rbn_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/raw_contest_cabrillo.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/raw_contest_cabrillo.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/raw_contest_sink.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/raw_contest_sink.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/rbn/storage_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/rbn/storage_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/storage_sink.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/storage_sink.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/data/storage_source.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/data/storage_source.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/assets/css/test.css` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/assets/css/test.css`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/search.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/search.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_direction.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_direction.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_evolution.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_evolution.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_log.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_log.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_propagation.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_propagation.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rates.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rates.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rbn.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_rbn.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_summary.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/callbacks/tab_summary.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/navbar.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/navbar.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/search.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/search.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_direction.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_direction.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_evolution.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_evolution.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_log.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_log.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_propagation.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_propagation.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_rates.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_rates.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_rbn.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_rbn.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/components/tab_summary.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/components/tab_summary.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/dashboard/contest_analysis.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/dashboard/contest_analysis.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/download/data_manipulation.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/download/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/modules/download/main.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/modules/download/main.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/arrldx/plot_contest_evolution.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/iaru/plot_contest_evolution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""Plot ARRL DX contest evolution."""
+"""Plot IARU HF contest evolution."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import concat
 from pandas import to_datetime
@@ -34,24 +35,26 @@
         "mean",
     ],
     "mult_worth_qsos": ["mult_worth_qsos", "# QSOs equivalent to multiplier", "mean"],
 }
 
 
 class PlotContestEvolution(PlotBase):
-    """Plot ARRL DX evolution."""
+    """Plot IARU HF evolution."""
+
+    name = "iaru_evolution"
 
     def __init__(
         self,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         feature: str,
         time_bin_size: int = 1,
     ):
-        """Init methodof the class.
+        """Init method of the PlotCqWwScore class.
 
         Args:
             contest (str): Contest name
             mode (str): Mode of the contest
             callsigns_years (List[Tuple[str, int]]): List of callsign-year tuples
             feature (str): Feature to plot
             time_bin_size (int): Size of the time bin. Defaults to 1.
@@ -123,15 +126,18 @@
             },
             range_y=[0.0, _data[AVAILABLE_FEATURES[self.feature][0]].max() * 1.05],
         )
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_xaxes(title="Dummy contest datetime")
         fig.update_yaxes(
-            title=f"ARRL DX {AVAILABLE_FEATURES[self.feature][1]}", matches=None
+            title=f"IARU HF {AVAILABLE_FEATURES[self.feature][1]}", matches=None
         )
 
         if not save:
             return fig
-        po_plot(
-            fig, filename=f"iaru_evolution_{AVAILABLE_FEATURES[self.feature][0]}.html"
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(
+            self.prefix_plots, f"{self.name}_{AVAILABLE_FEATURES[self.feature][0]}.html"
         )
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_frequency.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_frequency.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import Optional
 
 from pandas import to_datetime
 from pandas import to_timedelta
 from plotly.express import scatter
 from plotly.graph_objects import Figure
 from plotly.offline import plot as po_plot
@@ -12,14 +13,16 @@
 from hamcontestanalysis.plots.plot_base import PlotBase
 from hamcontestanalysis.utils import BANDMAP
 
 
 class PlotFrequency(PlotBase):
     """Plot QSOs Hour."""
 
+    name = "frequency"
+
     def plot(self, save: bool = False) -> Optional[Figure]:
         """Create plot.
 
         Args:
             save (bool): Save file in html. Defaults to False.
 
         Returns:
@@ -48,8 +51,11 @@
         )
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_yaxes(title="Frequency", matches=None)
 
         if not save:
             return fig
-        po_plot(fig, filename="frequency.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_log_heatmap.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_log_heatmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from numpy import arange
 from numpy import floor
 from numpy import int64
@@ -21,14 +22,16 @@
 from hamcontestanalysis.plots.plot_base import PlotBase
 from hamcontestanalysis.utils import CONTINENTS
 
 
 class PlotLogHeatmap(PlotBase):
     """Plot Contest log heatmap."""
 
+    name = "log_heatmap"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         time_bin_size: int = 1,
         continents: Optional[List[str]] = None,
@@ -155,8 +158,11 @@
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_xaxes(title="Contest minute")
         fig.update_yaxes(title="Contest hour")
 
         if not save:
             return fig
-        po_plot(fig, filename="log_heatmap.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_minutes_from_previous_call.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_minutes_from_previous_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot minutes until next call."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from numpy import around
 from pandas import concat
 from plotly.express import line
@@ -13,14 +14,16 @@
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_base import PlotBase
 
 
 class PlotMinutesPreviousCall(PlotBase):
     """Plot Minutes from previous call histogram."""
 
+    name = "minutes_from_previous_call"
+
     def __init__(
         self,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         time_bin_size: int = 5,
         xaxis_max_value: int = 10,
     ):
@@ -89,8 +92,11 @@
                 "counts": "QSOs",
             },
         )
         fig.update_layout(template=PLOT_TEMPLATE)
 
         if not save:
             return fig
-        po_plot(fig, filename="cqww_minutes_from_previous_call.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_qso_direction.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_qso_direction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from numpy import arange
 from pandas import cut
 from plotly.express import line_polar
@@ -13,14 +14,16 @@
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_base import PlotBase
 
 
 class PlotQsoDirection(PlotBase):
     """Plot QSO direction."""
 
+    name = "qso_direction"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         contest_hours: List[float],
     ):
@@ -77,8 +80,11 @@
             f"{self.contest_hours[0]} <= hour < {self.contest_hours[1]}",
             markers=True,
         )
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
 
         if not save:
             return fig
-        po_plot(fig, filename="rate.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_qsos_hour.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_qsos_hour.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 from pandas import DataFrame
 from plotly.express import bar
@@ -15,14 +16,16 @@
 from hamcontestanalysis.utils import CONTINENTS
 from hamcontestanalysis.utils.calculations import custom_floor
 
 
 class PlotQsosHour(PlotBase):
     """Plot QSOs Hour."""
 
+    name = "qsos_hour"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         continents: Optional[List[str]] = None,
         time_bin_size: int = 60,
@@ -115,8 +118,11 @@
         )
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_xaxes(title="Contest hour")
         fig.update_yaxes(title="QSOs")
 
         if not save:
             return fig
-        po_plot(fig, filename="qsos_hour.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_rate.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_rate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import to_datetime
 from pandas import to_timedelta
@@ -14,14 +15,16 @@
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_base import PlotBase
 
 
 class PlotRate(PlotBase):
     """Plot Rate."""
 
+    name = "rate"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         time_bin_size: int = 1,
         target: str = "qsos",
@@ -86,8 +89,11 @@
         )
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_xaxes(title="Dummy contest datetime")
         fig.update_yaxes(title=f"QSOs / {self.time_bin}min")
 
         if not save:
             return fig
-        po_plot(fig, filename="rate.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/common/plot_rolling_rate.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/common/plot_rolling_rate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import to_datetime
 from pandas import to_timedelta
 from plotly.express import line
@@ -13,14 +14,16 @@
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_base import PlotBase
 
 
 class PlotRollingRate(PlotBase):
     """Plot Rate."""
 
+    name = "rolling_rate"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         time_bin_size: int = 1,
         target: str = "qsos",
@@ -85,8 +88,11 @@
         )
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_xaxes(title="Dummy contest datetime")
         fig.update_yaxes(title=f"QSOs / {self.time_bin}min (rolling sum)")
 
         if not save:
             return fig
-        po_plot(fig, filename="rolling_rate.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/cqwpx/plot_contest_evolution.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/cqwpx/plot_contest_evolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot CQ WPX contest evolution."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import concat
 from pandas import to_datetime
@@ -36,14 +37,16 @@
     "mult_worth_qsos": ["mult_worth_qsos", "# QSOs equivalent to multiplier", "mean"],
 }
 
 
 class PlotContestEvolution(PlotBase):
     """Plot CQ WPX evolution."""
 
+    name = "cqwpx_evolution"
+
     def __init__(
         self,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         feature: str,
         time_bin_size: int = 1,
     ):
@@ -128,10 +131,13 @@
         fig.update_xaxes(title="Dummy contest datetime")
         fig.update_yaxes(
             title=f"CQ WPX {AVAILABLE_FEATURES[self.feature][1]}", matches=None
         )
 
         if not save:
             return fig
-        po_plot(
-            fig, filename=f"cqwpx_evolution_{AVAILABLE_FEATURES[self.feature][0]}.html"
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(
+            self.prefix_plots, f"{self.name}_{AVAILABLE_FEATURES[self.feature][0]}.html"
         )
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/cqww/plot_contest_evolution.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/cqww/plot_contest_evolution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot CQ WW contest evolution."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import concat
 from pandas import to_datetime
@@ -36,14 +37,16 @@
     "mult_worth_qsos": ["mult_worth_qsos", "# QSOs equivalent to multiplier", "mean"],
 }
 
 
 class PlotContestEvolution(PlotBase):
     """Plot CQ WW evolution."""
 
+    name = "cqww_evolution"
+
     def __init__(
         self,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         feature: str,
         time_bin_size: int = 1,
     ):
@@ -127,10 +130,13 @@
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_yaxes(
             title=f"CQ WW {AVAILABLE_FEATURES[self.feature][1]}", matches=None
         )
 
         if not save:
             return fig
-        po_plot(
-            fig, filename=f"cqww_evolution_{AVAILABLE_FEATURES[self.feature][0]}.html"
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(
+            self.prefix_plots, f"{self.name}_{AVAILABLE_FEATURES[self.feature][0]}.html"
         )
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/iaru/plot_contest_evolution.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/arrldx/plot_contest_evolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""Plot IARU HF contest evolution."""
+"""Plot ARRL DX contest evolution."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import concat
 from pandas import to_datetime
@@ -34,24 +35,26 @@
         "mean",
     ],
     "mult_worth_qsos": ["mult_worth_qsos", "# QSOs equivalent to multiplier", "mean"],
 }
 
 
 class PlotContestEvolution(PlotBase):
-    """Plot IARU HF evolution."""
+    """Plot ARRL DX evolution."""
+
+    name = "arrldx_evolution"
 
     def __init__(
         self,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         feature: str,
         time_bin_size: int = 1,
     ):
-        """Init method of the PlotCqWwScore class.
+        """Init methodof the class.
 
         Args:
             contest (str): Contest name
             mode (str): Mode of the contest
             callsigns_years (List[Tuple[str, int]]): List of callsign-year tuples
             feature (str): Feature to plot
             time_bin_size (int): Size of the time bin. Defaults to 1.
@@ -123,15 +126,18 @@
             },
             range_y=[0.0, _data[AVAILABLE_FEATURES[self.feature][0]].max() * 1.05],
         )
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_xaxes(title="Dummy contest datetime")
         fig.update_yaxes(
-            title=f"IARU HF {AVAILABLE_FEATURES[self.feature][1]}", matches=None
+            title=f"ARRL DX {AVAILABLE_FEATURES[self.feature][1]}", matches=None
         )
 
         if not save:
             return fig
-        po_plot(
-            fig, filename=f"iaru_evolution_{AVAILABLE_FEATURES[self.feature][0]}.html"
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(
+            self.prefix_plots, f"{self.name}_{AVAILABLE_FEATURES[self.feature][0]}.html"
         )
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/plot_base.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/plot_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,30 +6,41 @@
 from typing import Optional
 from typing import Tuple
 
 from pandas import DataFrame
 from pandas import concat
 from plotly.graph_objects import Figure
 
+from hamcontestanalysis.config import get_settings
 from hamcontestanalysis.data.processed_contest_source import ProcessedContestDataSource
 
 
+settings = get_settings()
+
+
 class PlotBase(ABC):
     """Plot abstract base class.
 
     This abstract class serves as a base interface for the different plots,
     It mainly defines the `PlotBase.plot` method as the
     way to create a plotly object, implemented by each plot subclass.
     """
 
+    name: str
+
     def __init__(self, contest: str, mode: str, callsigns_years: List[Tuple[str, int]]):
         """Init method of the base class."""
         self.contest = contest
         self.mode = mode
         self.callsigns_years = callsigns_years
+        self.prefix_plots = settings.storage.paths.plots.format(
+            contest=self.contest,
+            mode=self.mode,
+            callsigns_years="__".join([f"{c}_{y}" for c, y in self.callsigns_years]),
+        )
         self._data = None
 
     @property
     def data(self):
         """Property of attribute data."""
         if not isinstance(self._data, DataFrame):
             self._data = self._get_inputs()
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/plot_rbn_base.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/plot_rbn_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,43 @@
 from typing import List
 from typing import Optional
 
 from pandas import DataFrame
 from pandas import concat
 from plotly.graph_objects import Figure
 
+from hamcontestanalysis.config import get_settings
 from hamcontestanalysis.data.processed_rbn_source import (
     ProcessedReverseBeaconDataSource,
 )
 
 
+settings = get_settings()
+
+
 class PlotReverseBeaconBase(ABC):
     """Plot RBN abstract base class.
 
     This abstract class serves as a base interface for the different plots,
     It mainly defines the `PlotBase.plot` method as the
     way to create a plotly object, implemented by each plot subclass.
     """
 
+    name: str
+
     def __init__(self, contest: str, mode: str, years: List[int]):
         """Init method of the base class."""
         self.contest = contest
         self.mode = mode
         self.years = years
+        self.prefix_plots = settings.storage.paths.plots.format(
+            contest=self.contest,
+            mode=self.mode,
+            callsigns_years="__".join(self.years),
+        )
         self._data = None
 
     @property
     def data(self):
         """Property of attribute data."""
         if not isinstance(self._data, DataFrame):
             self._data = self._get_inputs()
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_band_conditions.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_band_conditions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 
 from numpy import where
 from pandas import Grouper
 from plotly.express import line
 from plotly.graph_objects import Figure
@@ -14,14 +15,16 @@
 from hamcontestanalysis.plots.plot_rbn_base import PlotReverseBeaconBase
 from hamcontestanalysis.utils import BANDMAP
 
 
 class PlotBandConditions(PlotReverseBeaconBase):
     """Plot band conditions."""
 
+    name = "band_conditions"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         years: List[int],
         time_bin_size: int,
         reference: str,
@@ -108,8 +111,11 @@
             title=f"Reference: {self.reference} - % RBN spots per band and continent",
             template=PLOT_TEMPLATE,
         )
         fig.update_yaxes(title="% spots")
 
         if not save:
             return fig
-        po_plot(fig, filename="band_conditions.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_cw_speed.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_cw_speed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import concat
 from pandas import to_datetime
 from pandas import to_timedelta
 from plotly.express import scatter
 from plotly.graph_objects import Figure
 from plotly.offline import plot as po_plot
 
 from hamcontestanalysis.commons.pandas.general import hour_of_contest
+from hamcontestanalysis.config import get_settings
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_rbn_base import PlotReverseBeaconBase
 from hamcontestanalysis.utils import BANDMAP
 
 
+settings = get_settings()
+
+
 class PlotCwSpeed(PlotReverseBeaconBase):
     """Plot CW speed from RBN."""
 
+    name = "cw_speed"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         time_bin_size: int,
         bands: Optional[List[int]] = None,
@@ -42,14 +49,19 @@
             contest=contest, mode=mode, years=[y for (_, y) in callsigns_years]
         )
         self.callsigns_years = callsigns_years
         self.time_bin_size = time_bin_size
         self.bands = (
             [int(b) for b in bands] if bands is not None else list(BANDMAP.keys())
         )
+        self.prefix_plots = settings.storage.paths.plots.format(
+            contest=self.contest,
+            mode=self.mode,
+            callsigns_years="__".join([f"{c}_{y}" for c, y in self.callsigns_years]),
+        )
 
     def plot(self, save: bool = False) -> Optional[Figure]:
         """Create plot.
 
         Args:
             save (bool): Save file in html. Defaults to False.
 
@@ -111,7 +123,11 @@
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_yaxes(title="CW speed", matches=None)
 
         if not save:
             return fig
         po_plot(fig, filename="cw_speed.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_number_rbn_spots.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_snr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,124 @@
 """Plot QSO rate."""
 
+import os
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from pandas import Grouper
 from pandas import concat
 from pandas import to_datetime
 from pandas import to_timedelta
 from plotly.express import scatter
 from plotly.graph_objects import Figure
 from plotly.offline import plot as po_plot
 
 from hamcontestanalysis.commons.pandas.general import hour_of_contest
+from hamcontestanalysis.config import get_settings
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_rbn_base import PlotReverseBeaconBase
 from hamcontestanalysis.utils import BANDMAP
 
 
-class PlotNumberRbnSpots(PlotReverseBeaconBase):
+settings = get_settings()
+
+
+class PlotSnr(PlotReverseBeaconBase):
     """Plot SNR from RBN."""
 
+    name = "cw_snr"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         callsigns_years: List[Tuple[str, int]],
         time_bin_size: int,
         rx_continents: List[str],
-        bands: Optional[List[int]] = None,
     ):
         """Init method of the PlotBandConditions class.
 
         Args:
             contest (str): Contest name
             mode (str): Mode of the contest
-            years (List[int]): Years of the contest
             callsigns_years (List[Tuple[str, int]]): List of callsign-year tuples
             time_bin_size (int): Time bin size in minutes
             rx_continents (List[str]): Continents of the RX stations
-            bands (Optional[List[int]]): Bands to consider. Defaults to None.
         """
         super().__init__(
             contest=contest, mode=mode, years=[y for (_, y) in callsigns_years]
         )
         self.callsigns_years = callsigns_years
         self.time_bin_size = time_bin_size
         self.rx_continents = rx_continents
-        self.bands = (
-            [int(b) for b in bands] if bands is not None else list(BANDMAP.keys())
+        self.prefix_plots = settings.storage.paths.plots.format(
+            contest=self.contest,
+            mode=self.mode,
+            callsigns_years="__".join([f"{c}_{y}" for c, y in self.callsigns_years]),
         )
 
     def plot(self, save: bool = False) -> Optional[Figure]:
         """Create plot.
 
         Args:
             save (bool): Save file in html. Defaults to False.
 
         Returns:
             Optional[Figure]: Plotly figure
         """
         # Filter callsigns and years
         _data = []
         for callsign, year in self.callsigns_years:
-            _data.append(
-                self.data.query(f"(dx == '{callsign}') & (year == {year})").query(
-                    f"(band.isin({self.bands}))"
-                )
-            )
+            _data.append(self.data.query(f"(dx == '{callsign}') & (year == {year})"))
         _data = concat(_data)
 
         # Dummy datetime to compare
         _data = _data.pipe(
             func=hour_of_contest,
         ).assign(
             dummy_datetime=lambda x: to_datetime("2000-01-01")
             + to_timedelta(x["hour"], "H"),
             callsign_year=lambda x: x["dx"] + "(" + x["year"].astype(str) + ")",
         )
 
         # Groupby
-        do_dummy_datetime = len(self.data["year"].unique()) > 1
-        datetime_column_name = "dummy_datetime" if do_dummy_datetime else "datetime"
         _data = (
             _data.reset_index(drop=True)
             .query(f"(de_cont.isin({self.rx_continents}))")
             .groupby(
                 [
                     "callsign_year",
                     "band",
-                    Grouper(key=datetime_column_name, freq=f"{self.time_bin_size}Min"),
+                    Grouper(key="dummy_datetime", freq=f"{self.time_bin_size}Min"),
                 ],
                 as_index=False,
             )
-            .agg(db=("db", "count"))
-            .rename(columns={"db": "counts"})
+            .agg(db=("db", "mean"))
         )
 
         fig = scatter(
             _data,
-            x=datetime_column_name,
-            y="counts",
+            x="dummy_datetime",
+            y="db",
             color="callsign_year",
             facet_row="band",
             labels={
                 "callsign_year": "Callsign (year)",
                 "dummy_datetime": "Dummy contest datetime",
-                "datetime": "Contest datetime",
-                "counts": "# RBN spots",
+                "dB": "SNR (dB)",
                 "band": "Band",
             },
-            category_orders={"band": self.bands},
-            range_y=[0.0, _data["counts"].max() * 1.05],
+            category_orders={"band": list(BANDMAP.keys())},
+            range_y=[0.0, _data["db"].max() * 1.05],
         )
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
-        fig.update_yaxes(title="# RBN spots", matches=None)
+        fig.update_xaxes(title="Dummy contest datetime")
+        fig.update_yaxes(title="SNR (dB)", matches=None)
 
         if not save:
             return fig
-        po_plot(fig, filename="cw_rbn_spots.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/plots/rbn/plot_snr_band_continent.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/plots/rbn/plot_snr_band_continent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """Plot QSO rate."""
 
+import os
 from logging import getLogger
 from typing import List
 from typing import Optional
 
 import numpy as np
 from pandas import DataFrame
 from pandas import Grouper
 from pandas import date_range
 from pandas import merge
 from plotly.express import line
 from plotly.graph_objects import Figure
 from plotly.offline import plot as po_plot
 
+from hamcontestanalysis.config import get_settings
 from hamcontestanalysis.plots import PLOT_TEMPLATE
 from hamcontestanalysis.plots.plot_rbn_base import PlotReverseBeaconBase
 
 
 logger = getLogger(__name__)
+settings = get_settings()
 
 
 class PlotSnrBandContinent(PlotReverseBeaconBase):
     """Plot SNR from RBN in a grid of bands and continents."""
 
+    name = "cw_snr_band_continent"
+
     def __init__(
         self,
         contest: str,
         mode: str,
         bands: List[int],
         callsigns: List[str],
         year: int,
@@ -49,14 +54,19 @@
         self.bands = [int(b) for b in bands]
         self.time_bin_size = time_bin_size
         self.rx_continents = rx_continents
         self.smoothing = 2
         self.min_rx_spots_per_hour = 2
         self.filter_str = None
         self.closed_list_spotters = True
+        self.prefix_plots = settings.storage.paths.plots.format(
+            contest=self.contest,
+            mode=self.mode,
+            callsigns_years="__".join([f"{c}_{year}"] for c in self.callsigns),
+        )
 
     def _clean_dataset(self):
         _df = self.data.copy().assign(
             datetime_floor=lambda x: x["datetime"].dt.floor(freq="60min")
         )
 
         # Extra filter if needed
@@ -225,8 +235,11 @@
         )
 
         fig.update_layout(hovermode="x unified", template=PLOT_TEMPLATE)
         fig.update_traces(marker_size=4, line=dict(width=0.5))
 
         if not save:
             return fig
-        po_plot(fig, filename="cw_snr_band_continent.html")
+        if not os.path.exists(self.prefix_plots):
+            os.makedirs(self.prefix_plots)
+        filename = os.path.join(self.prefix_plots, f"{self.name}.html")
+        po_plot(fig, filename=filename)
```

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/settings/contest.yaml` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/settings/contest.yaml`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/settings/logging.yaml` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/settings/logging.yaml`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/arrldx/table_contest_log.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/arrldx/table_contest_log.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/arrldx/table_contest_summary.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/arrldx/table_contest_summary.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqwpx/table_contest_log.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqwpx/table_contest_log.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqwpx/table_contest_summary.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqwpx/table_contest_summary.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqww/table_contest_log.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqww/table_contest_log.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/cqww/table_contest_summary.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/cqww/table_contest_summary.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/iaru/table_contest_log.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/iaru/table_contest_log.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/iaru/table_contest_summary.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/iaru/table_contest_summary.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/tables/table_base.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/tables/table_base.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/calculations/contests.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/calculations/contests.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/dashboards/callbacks_manager.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/dashboards/callbacks_manager.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/src/hamcontestanalysis/utils/types/dataframe_types.py` & `hamcontestanalysis-1.1.0/src/hamcontestanalysis/utils/types/dataframe_types.py`

 * *Files identical despite different names*

### Comparing `hamcontestanalysis-1.0.0/PKG-INFO` & `hamcontestanalysis-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hamcontestanalysis
-Version: 1.0.0
-Summary: hca
+Version: 1.1.0
+Summary: Ham radio contest analysis tools
 Home-page: https://github.com/rogercaminal/hamcontestanalysis
 License: MIT
 Author: Roger Caminal Armadans
 Author-email: roger.caminal@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
@@ -20,24 +20,24 @@
 Requires-Dist: dash-bootstrap-components (==1.4.1)
 Requires-Dist: dynaconf (==3.1.12)
 Requires-Dist: pandas (==2.0.0)
 Requires-Dist: pyarrow (==12.0.1)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: pyhamtools (==0.8.7)
 Requires-Dist: python-dotenv (==1.0.1)
+Requires-Dist: sphinxcontrib-typer (==0.2.1)
 Requires-Dist: typer (==0.9.0)
 Project-URL: Changelog, https://github.com/rogercaminal/hamcontestanalysis/releases
 Project-URL: Documentation, https://hamcontestanalysis.readthedocs.io
 Project-URL: Repository, https://github.com/rogercaminal/hamcontestanalysis
 Description-Content-Type: text/markdown
 
 # HamContestAnalysis
 
 [![PyPI](https://img.shields.io/pypi/v/hamcontestanalysis.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/hamcontestanalysis.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/hamcontestanalysis)][python version]
 [![License](https://img.shields.io/pypi/l/hamcontestanalysis)][license]
 
 [![Read the documentation at https://hamcontestanalysis.readthedocs.io/](https://img.shields.io/readthedocs/hamcontestanalysis/latest.svg?label=Read%20the%20Docs)][read the docs]
 [![Tests](https://github.com/rogercaminal/hamcontestanalysis/workflows/Tests/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/rogercaminal/hamcontestanalysis/branch/main/graph/badge.svg)][codecov]
 
@@ -49,33 +49,39 @@
 [python version]: https://pypi.org/project/hamcontestanalysis
 [read the docs]: https://hamcontestanalysis.readthedocs.io/
 [tests]: https://github.com/rogercaminal/hamcontestanalysis/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/rogercaminal/hamcontestanalysis
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
-## Features
+<!-- ## Features
 
 - TODO
 
 ## Requirements
 
-- TODO
+- TODO -->
+
+## Introduction
+
+_HamContestAnalysis_ comprises a set of tools for radio amateurs dedicated to analyze contest with the maximum detail.
+
+This library is divided into two main components: a collection of functions and classes that allow to easily download public logs and process them for further analysis, as well as a dashboard that provides the user not only with a general view of the contest, but also with the possibility to compare between different call signs and/or years.
 
 ## Installation
 
-You can install _HamContestAnalysis_ via [pip] from [PyPI]:
+_HamContestAnalysis_ can be installed via [pip] from [PyPI]:
 
 ```console
 $ pip install hamcontestanalysis
 ```
 
 ## Usage
 
-Please see the [Command-line Reference] for details.
+Please see the [Command-line Reference] for technical details.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

