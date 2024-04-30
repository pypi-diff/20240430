# Comparing `tmp/tradedangerous-11.1.2.tar.gz` & `tmp/tradedangerous-11.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.1.2.tar", last modified: Mon Apr 29 19:11:58 2024, max compression
+gzip compressed data, was "tradedangerous-11.1.3.tar", last modified: Mon Apr 29 19:40:19 2024, max compression
```

## Comparing `tradedangerous-11.1.2.tar` & `tradedangerous-11.1.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.508146 tradedangerous-11.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.512146 tradedangerous-11.1.2/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.516146 tradedangerous-11.1.2/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.516146 tradedangerous-11.1.2/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.516146 tradedangerous-11.1.2/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    22484 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 19:11:08.000000 tradedangerous-11.1.2/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradegui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.649813 tradedangerous-11.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-29 19:40:19.649813 tradedangerous-11.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 19:40:19.649813 tradedangerous-11.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.633813 tradedangerous-11.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.637813 tradedangerous-11.1.3/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.641813 tradedangerous-11.1.3/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.641813 tradedangerous-11.1.3/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.645813 tradedangerous-11.1.3/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.645813 tradedangerous-11.1.3/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.645813 tradedangerous-11.1.3/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22883 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.649813 tradedangerous-11.1.3/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 19:39:27.000000 tradedangerous-11.1.3/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:40:19.649813 tradedangerous-11.1.3/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 19:40:19.000000 tradedangerous-11.1.3/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-29 19:39:04.000000 tradedangerous-11.1.3/tradegui.py
```

### Comparing `tradedangerous-11.1.2/LICENSE` & `tradedangerous-11.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/PKG-INFO` & `tradedangerous-11.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.2
+Version: 11.1.3
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.2/README.md` & `tradedangerous-11.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/setup.py` & `tradedangerous-11.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_bootstrap_commands.py` & `tradedangerous-11.1.3/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_bootstrap_plugins.py` & `tradedangerous-11.1.3/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_cache.py` & `tradedangerous-11.1.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_commands.py` & `tradedangerous-11.1.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_fs.py` & `tradedangerous-11.1.3/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_peek.py` & `tradedangerous-11.1.3/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_trade.py` & `tradedangerous-11.1.3/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_trade_run.py` & `tradedangerous-11.1.3/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tests/test_utils.py` & `tradedangerous-11.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/trade.py` & `tradedangerous-11.1.3/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/__init__.py` & `tradedangerous-11.1.3/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/cache.py` & `tradedangerous-11.1.3/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/cli.py` & `tradedangerous-11.1.3/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.1.3/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/__init__.py` & `tradedangerous-11.1.3/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/commandenv.py` & `tradedangerous-11.1.3/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/exceptions.py` & `tradedangerous-11.1.3/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/parsing.py` & `tradedangerous-11.1.3/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.1.3/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/commands/update_gui.py` & `tradedangerous-11.1.3/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/corrections.py` & `tradedangerous-11.1.3/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/csvexport.py` & `tradedangerous-11.1.3/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/edscupdate.py` & `tradedangerous-11.1.3/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/edsmupdate.py` & `tradedangerous-11.1.3/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/formatting.py` & `tradedangerous-11.1.3/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/fs.py` & `tradedangerous-11.1.3/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/gui.py` & `tradedangerous-11.1.3/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/jsonprices.py` & `tradedangerous-11.1.3/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/mapping.py` & `tradedangerous-11.1.3/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/mfd/__init__.py` & `tradedangerous-11.1.3/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.1.3/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.1.3/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.1.3/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/clipboard.py` & `tradedangerous-11.1.3/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/coord64.py` & `tradedangerous-11.1.3/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.1.3/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.1.3/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/eddb.py` & `tradedangerous-11.1.3/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/eddn.py` & `tradedangerous-11.1.3/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/edsc.py` & `tradedangerous-11.1.3/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/edsm.py` & `tradedangerous-11.1.3/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.1.3/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.1.3/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/misc/progress.py` & `tradedangerous-11.1.3/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/__init__.py` & `tradedangerous-11.1.3/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/eddblink_plug.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
 Import plugin that uses data files from 
 https://elite.tromador.com/ to update the Database.
 """
 from __future__ import annotations
+
+from pathlib import Path
+from .. import plugins, cache, transfers
+from ..misc import progress as pbar
+from ..plugins import PluginException
+
 import certifi
 import csv
 import datetime
-import json
 import os
+import requests
 import sqlite3
 import ssl
-import time
 import typing
 import locale
-
-from urllib import request
-from pathlib import Path
-
-from .. import plugins, cache, transfers
-from ..misc import progress as pbar
-from ..plugins import PluginException
+import platform
 
 
 if typing.TYPE_CHECKING:
     from typing import Optional
     from .. tradeenv import TradeEnv
 
 # Find the first English UTF-8 locale for use in parsing timestamps.
 LOCALE = None
-import platform
 if platform.system() == 'Windows':
     for lang in locale.windows_locale.values():
         if "en" in lang:
             LOCALE = lang
             break
 else:
     # for other operating systems
@@ -48,22 +46,14 @@
         "Please refer to your OS for instructions installing one."
     )
 # Constants
 BASE_URL = os.environ.get('TD_SERVER') or "https://elite.tromador.com/files/"
 CONTEXT=ssl.create_default_context(cafile=certifi.where())
 
 
-def _request_url(url, headers=None):
-    data = None
-    if headers:
-        data = bytes(json.dumps(headers), encoding="utf-8")
-    
-    return request.urlopen(request.Request(url, data=data), context=CONTEXT, timeout=90)
-
-
 class DecodingError(PluginException):
     pass
 
 
 def _file_line_count(from_file: Path, bufsize: int = 128 * 1024) -> int:
     """ counts the number of newline characters in a given file. """
     # Pre-allocate a buffer so we aren't putting pressure on the garbage collector.
@@ -176,45 +166,54 @@
     def now(self):
         return datetime.datetime.now()
     
     def downloadFile(self, path):
         """
         Fetch the latest dumpfile from the website if newer than local copy.
         """
-        def openURL(url):
-            return _request_url(url, headers = {'User-Agent': 'Trade-Dangerous'})
-        
         if path not in (self.liveListingsPath, self.listingsPath):
             localPath = Path(self.tdb.dataPath, path)
         else:
             localPath = Path(self.dataPath, path)
         
         url  = BASE_URL + str(path)
         
         self.tdenv.NOTE("Checking for update to '{}'.", path)
+        # Use an HTTP Request header to obtain the Last-Modified and Content-Length headers.
+        # Also, tell the server to give us the un-compressed length of the file by saying
+        # that >this< request only wants text.
+        headers = {"User-Agent": "Trade-Dangerous", "Accept-Encoding": "text"}
         try:
-            response = openURL(url)
+            response = requests.head(url, headers=headers, timeout=70)
         except Exception as e:  # pylint: disable=broad-exception-caught
-            self.tdenv.WARN("Problem with download:\n    URL: {}\n    Error: {}", BASE_URL + str(path), str(e))
+            self.tdenv.WARN("Problem with download:\n    URL: {}\n    Error: {}", url, str(e))
             return False
         
-        url_time = response.getheader("Last-Modified")
         locale.setlocale(locale.LC_ALL, LOCALE)
-        dumpModded = datetime.datetime.strptime(url_time, "%a, %d %b %Y %H:%M:%S %Z").timestamp()
+        last_modified = response.headers.get("last-modified")
+        dump_mod_time = datetime.datetime.strptime(last_modified, "%a, %d %b %Y %H:%M:%S %Z").timestamp()
         locale.setlocale(locale.LC_ALL, '')
         
         if Path.exists(localPath):
-            localModded = localPath.stat().st_mtime
-            if localModded >= dumpModded:
+            local_mod_time = localPath.stat().st_mtime
+            if local_mod_time >= dump_mod_time:
                 self.tdenv.DEBUG0("'{}': Dump is not more recent than Local.", path)
                 return False
         
+        # The server doesn't know the gzip'd length, and we won't see the gzip'd data,
+        # so we want the actual text-only length. Capture it here so we can tell the
+        # transfer mechanism how big the file is going to be.
+        length = response.headers.get("content-length")
+        
         self.tdenv.NOTE("Downloading file '{}'.", path)
-        transfers.download(self.tdenv, url, localPath)
-        os.utime(localPath, (dumpModded, dumpModded))
+        transfers.download(self.tdenv, url, localPath, chunkSize=16384, length=length)
+        
+        # Change the timestamps on the file so they match the website
+        os.utime(localPath, (dump_mod_time, dump_mod_time))
+        
         return True
     
     def purgeSystems(self):
         """
         Purges systems from the System table that do not have any stations claiming to be in them.
         Keeps table from becoming too large because of fleet carriers moving to unpopulated systems.
         """
@@ -351,14 +350,16 @@
         self.tdb.close()
         
         self.tdenv.NOTE("Finished processing market data. End time = {}", self.now())
     
     def run(self):
         self.tdenv.DEBUG2(f'Using "{LOCALE}" locale for parsing modified timestamps. Please include this information in any error reports.')
         
+        self.tdenv.ignoreUnknown = True
+        
         # Create the /eddb folder for downloading the source files if it doesn't exist.
         try:
             Path(str(self.dataPath)).mkdir()
         except FileExistsError:
             pass
         
         # Run 'listings' by default:
@@ -507,16 +508,14 @@
                 buildCache = True
         
         # Remake the .db files with the updated info.
         if buildCache:
             self.tdb.close()
             self.tdb.reloadCache()
         
-        self.tdenv.ignoreUnknown = True
-        
         if self.getOption("purge"):
             self.purgeSystems()
         
         if self.getOption("listings"):
             if self.downloadFile(self.listingsPath) or self.getOption("force"):
                 self.importListings(self.listingsPath)
             if self.downloadFile(self.liveListingsPath) or self.getOption("force"):
```

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.1.3/tradedangerous/plugins/spansh_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/prices.py` & `tradedangerous-11.1.3/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/submit-distances.py` & `tradedangerous-11.1.3/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/templates/Added.csv` & `tradedangerous-11.1.3/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.1.3/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.1.3/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/tools.py` & `tradedangerous-11.1.3/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/tradecalc.py` & `tradedangerous-11.1.3/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/tradedb.py` & `tradedangerous-11.1.3/tradedangerous/tradedb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1146,16 +1146,17 @@
         """
         
         stationByID = {}
         systemByID = self.systemByID
         self.tradingStationCount = 0
         # Fleet Carriers are station type 24.
         # Odyssey settlements are station type 25.
+        # Assume type 0 (Unknown) are also Fleet Carriers.
         # Storing as a list allows easy expansion if needed.
-        types = {'fleet-carrier':[24,],'odyssey':[25,],}
+        types = {'fleet-carrier':[24, 0,],'odyssey':[25,],}
         with closing(self.query(stmt)) as cur:
             for (
                 ID, systemID, name,
                 lsFromStar, market, blackMarket, shipyard,
                 maxPadSize, outfitting, rearm, refuel, repair, planetary, type_id
             ) in cur:
                 isFleet = 'Y' if int(type_id) in types['fleet-carrier'] else 'N'
```

### Comparing `tradedangerous-11.1.2/tradedangerous/tradeenv.py` & `tradedangerous-11.1.3/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/transfers.py` & `tradedangerous-11.1.3/tradedangerous/transfers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-import csv
-import json
-import time
+from __future__ import annotations
 
 from collections import deque
 from pathlib import Path
 from .tradeexcept import TradeException
 from .misc import progress as pbar
 from . import fs
 
+import csv
+import json
+import time
+import typing
+
 import requests
 
 
+if typing.TYPE_CHECKING:
+    import os  # for PathLike
+    from .tradeenv import TradeEnv
+    from typing import Optional, Union
+
+
 ######################################################################
 # Helpers
 
 class HTTP404(TradeException):
     pass
 
 def makeUnit(value):
@@ -27,20 +36,24 @@
     for unit in units:
         if unitSize <= 640:
             return "{:>5.01f}{}".format(unitSize, unit)
         unitSize /= 1024
     return None
 
 def download(
-            tdenv, url, localFile,
-            headers=None,
-            backup=False,
-            shebang=None,
-            chunkSize=4096,
-            timeout=90,
+            tdenv:      TradeEnv,
+            url:        str,
+            localFile:  os.PathLike,
+            headers:    Optional[dict] = None,
+            backup:     bool = False,
+            shebang:    Optional[str] = None,
+            chunkSize:  int = 4096,
+            timeout:    int = 90,
+            *,
+            length:     Optional[Union[int, str]] = None,
         ):
     """
     Fetch data from a URL and save the output
     to a local file. Returns the response headers.
     
     tdenv:
         TradeEnv we're working under
@@ -53,40 +66,43 @@
     
     headers:
         dict() of additional HTTP headers to send
     
     shebang:
         function to call on the first line
     """
-    
     tdenv.NOTE("Requesting {}".format(url))
+
+    if isinstance(length, str):
+        length = int(length)
+
     req = requests.get(url, headers=headers or None, stream=True, timeout=timeout)
     req.raise_for_status()
     
     encoding = req.headers.get('content-encoding', 'uncompress')
-    length = req.headers.get('content-length', None)
+    content_length = req.headers.get('content-length', length)
     transfer = req.headers.get('transfer-encoding', None)
-    if transfer != 'chunked':
+    if not length and transfer != 'chunked':
         # chunked transfer-encoding doesn't need a content-length
-        if length is None:
+        if content_length is None:
             print(req.headers)
             raise Exception("Remote server replied with invalid content-length.")
-        length = int(length)
-        if length <= 0:
+        content_length = int(content_length)
+        if content_length <= 0:
             raise TradeException(
                 "Remote server gave an empty response. Please try again later."
             )
 
     # if the file is being compressed by the server, the headers tell us the
     # length of the compressed data, but in our loop below we will be receiving
     # the uncompressed data, which should be larger, which will cause our
     # download indicators to sit at 100% for a really long time if the file is
     # heavily compressed and large (e.g spansh 1.5gb compressed vs 9GB uncompressed)
-    if encoding == "gzip" and length:
-        length *= 4
+    if length is None and encoding == "gzip" and content_length:
+        length = content_length * 3
     
     if tdenv.detail > 1:
         if length:
             tdenv.NOTE("Downloading {} {}ed data", makeUnit(length), encoding)
         else:
             tdenv.NOTE("Downloading {} {}ed data", transfer, encoding)
     tdenv.DEBUG0(str(req.headers).replace("{", "{{").replace("}", "}}"))
```

### Comparing `tradedangerous-11.1.2/tradedangerous/utils.py` & `tradedangerous-11.1.3/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradedangerous/version.py` & `tradedangerous-11.1.3/tradedangerous/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.1.2'
+__version__ = '11.1.3'
```

### Comparing `tradedangerous-11.1.2/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.1.3/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.2
+Version: 11.1.3
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.2/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.1.3/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.2/tradegui.py` & `tradedangerous-11.1.3/tradegui.py`

 * *Files identical despite different names*

