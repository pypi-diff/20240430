# Comparing `tmp/qteasy-1.2.2.tar.gz` & `tmp/qteasy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qteasy-1.2.2.tar", last modified: Sun Apr 28 16:37:03 2024, max compression
+gzip compressed data, was "qteasy-1.2.3.tar", last modified: Tue Apr 30 14:05:51 2024, max compression
```

## Comparing `qteasy-1.2.2.tar` & `qteasy-1.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.539524 qteasy-1.2.2/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.2/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    29111 2024-04-28 16:37:03.539268 qteasy-1.2.2/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    25387 2024-04-28 16:32:22.000000 qteasy-1.2.2/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-04-28 16:32:22.000000 qteasy-1.2.2/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.526354 qteasy-1.2.2/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-04-28 16:32:22.000000 qteasy-1.2.2/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-27 10:02:20.000000 qteasy-1.2.2/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.2/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-04-23 05:23:43.000000 qteasy-1.2.2/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142505 2024-04-28 16:28:11.000000 qteasy-1.2.2/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   111230 2024-04-27 14:57:02.000000 qteasy-1.2.2/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   390977 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.2/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-21 23:36:55.000000 qteasy-1.2.2/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-27 10:02:29.000000 qteasy-1.2.2/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.2/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.2.2/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.2.2/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.2/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-04-28 16:28:11.000000 qteasy-1.2.2/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   156061 2024-04-28 16:28:11.000000 qteasy-1.2.2/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-04-23 13:23:43.000000 qteasy-1.2.2/qteasy/trader_cli.py
--rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-04-23 05:23:43.000000 qteasy-1.2.2/qteasy/trader_tui.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 14:28:39.000000 qteasy-1.2.2/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.2/qteasy/tsfuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)      840 2024-04-23 05:23:43.000000 qteasy-1.2.2/qteasy/tui_style.tcss
--rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-04-27 14:12:34.000000 qteasy-1.2.2/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.2/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.538688 qteasy-1.2.2/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    29111 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.2/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      195 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-28 16:37:03.000000 qteasy-1.2.2/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-04-28 16:37:03.539881 qteasy-1.2.2/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.2/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-28 16:37:03.538414 qteasy-1.2.2/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-04-27 14:13:03.000000 qteasy-1.2.2/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.2/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.2/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.2/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.2/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.2/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.2/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-28 16:28:11.000000 qteasy-1.2.2/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-28 14:32:18.000000 qteasy-1.2.2/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.2/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    40797 2024-04-28 16:28:11.000000 qteasy-1.2.2/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.2/tests/test_trading.py
--rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-04-23 05:23:43.000000 qteasy-1.2.2/tests/test_tui.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.2/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.2/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.2/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.698964 qteasy-1.2.3/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.3/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-04-30 14:05:51.698882 qteasy-1.2.3/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24211 2024-04-30 14:05:38.000000 qteasy-1.2.3/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-04-30 14:05:38.000000 qteasy-1.2.3/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.694169 qteasy-1.2.3/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-04-30 14:05:38.000000 qteasy-1.2.3/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-29 15:26:18.000000 qteasy-1.2.3/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.3/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-04-23 05:23:43.000000 qteasy-1.2.3/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142505 2024-04-29 14:37:23.000000 qteasy-1.2.3/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   111306 2024-04-30 14:05:38.000000 qteasy-1.2.3/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   390965 2024-04-30 14:05:38.000000 qteasy-1.2.3/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.3/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-21 23:36:55.000000 qteasy-1.2.3/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-29 15:26:18.000000 qteasy-1.2.3/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.3/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.2.3/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.2.3/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.3/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-04-29 14:37:23.000000 qteasy-1.2.3/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   156061 2024-04-29 14:37:23.000000 qteasy-1.2.3/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/trader_cli.py
+-rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-04-23 05:23:43.000000 qteasy-1.2.3/qteasy/trader_tui.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-29 15:26:18.000000 qteasy-1.2.3/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.3/qteasy/tsfuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)      840 2024-04-23 05:23:43.000000 qteasy-1.2.3/qteasy/tui_style.tcss
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-04-27 14:12:34.000000 qteasy-1.2.3/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.3/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.698346 qteasy-1.2.3/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.3/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      195 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-04-30 14:05:51.699233 qteasy-1.2.3/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.3/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.698191 qteasy-1.2.3/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-04-27 14:13:03.000000 qteasy-1.2.3/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.3/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.3/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.3/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.3/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.3/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.3/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-29 14:37:23.000000 qteasy-1.2.3/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-28 14:32:18.000000 qteasy-1.2.3/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.3/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    40797 2024-04-29 14:37:23.000000 qteasy-1.2.3/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.3/tests/test_trading.py
+-rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_tui.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.3/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.3/tests/test_visual.py
```

### Comparing `qteasy-1.2.2/LICENSE` & `qteasy-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/PKG-INFO` & `qteasy-1.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -106,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.2`
+- Latest Version: `1.2.3`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -125,34 +125,34 @@
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_5_2.png)
+![png](docs/source/img/output_5_2.png)
 
 ### **创建交易策略**
 
 - 提供几十种内置交易策略，可以直接搭积木式使用
 - 快速创建自定义交易策略，灵活设置可调参数
 - 交易策略的回测、优化、评价，可视化输出回测结果
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_14_3.png)
+![png](docs/source/img/output_14_3.png)
 
 ### **实盘交易模拟**
 - 读取实时市场数据，实盘运行交易策略
 - 生成交易信号，模拟交易结果
 - 跟踪记录交易日志、股票持仓、账户资金变化等信息
 - 随时查看交易过程，检查盈亏情况
 - 手动控制交易进程、调整交易参数，手动下单
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
+![png](docs/source/examples/img/trader_app_1.png)  
+![png](docs/source/examples/img/trader_app_2.png)  
+![png](docs/source/examples/img/trader_app_light_theme.png) 
 
 ## 安装
 
 ```bash
 $ pip install qteasy
 ```
 
@@ -192,15 +192,15 @@
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
 import qteasy as qt
-print(qt.__version__)
+qt.__version__
 ```
 
 ### 配置本地数据源
 
 为了使用`qteasy`，需要大量的金融历史数据，所有的历史数据都必须首先保存在本地，如果本地没有历史数据，那么`qteasy`的许多功能就无法执行。
 
 `qteasy`默认通过`tushare`金融数据包来获取大量的金融数据，用户需要自行申请API Token，获取相应的权限和积分（详情参考：https://tushare.pro/document/2）
@@ -288,15 +288,15 @@
 股票的数据下载后，使用`qt.candle()`可以显示股票数据K线图。
 
 ```python
 import qteasy as qt
 data = qt.candle('000300.SH', start='2021-06-01', end='2021-8-01', asset_type='IDX')
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_5_2.png)
+![png](docs/source/img/output_5_2.png)
     
 `qteasy`的K线图函数`candle`支持通过六位数股票/指数代码查询准确的证券代码，也支持通过股票、指数名称显示K线图
 `qt.candle()`支持功能如下：
 - 显示股票、基金、期货的K线
 - 显示复权价格
 - 显示分钟、 周或月K线 
 - 显示不同移动均线以及MACD/KDJ等指标
@@ -314,23 +314,23 @@
 qt.candle('中国电信', start = '20211021', freq='30min', adj='b')
 # 期货K线，三条移动均线分别为9天、12天、26天
 qt.candle('沪铜主力', start = '20211021', mav=[9, 12, 26])
 # 场外基金净值曲线图，复权净值，不显示移动均线
 qt.candle('000001.OF', start='20200101', asset_type='FD', adj='b', mav=[])
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_1.png)
+![png](docs/source/img/output_3_1.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_7_2.png)
+![png](docs/source/img/output_7_2.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_8_3.png)
+![png](docs/source/img/output_8_3.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_4.png)
+![png](docs/source/img/output_3_4.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_5.png)
+![png](docs/source/img/output_3_5.png)
     
 
 生成的K线图可以是一个交互式动态K线图（请注意，K线图基于`matplotlib`绘制，在使用不同的终端时，显示功能有所区别，某些终端并不支持
 动态图表，详情请参阅 [matplotlib文档](https://matplotlib.org/stable/users/explain/backends.html)
 
 
 在使用动态K线图时，用户可以用鼠标和键盘控制K线图的显示范围：
@@ -338,15 +338,15 @@
 - 鼠标在图表上左右拖动：可以移动K线图显示更早或更晚的K线
 - 鼠标滚轮在图表上滚动，可以缩小或放大K线图的显示范围
 - 通过键盘左右方向键，可以移动K线图的显示范围显示更早或更晚的K线
 - 通过键盘上下键，可以缩小或放大K线图的显示范围
 - 在K线图上双击鼠标，可以切换不同的均线类型
 - 在K线图的指标区域双击，可以切换不同的指标类型：MACD，RSI，DEMA
 
-![gif](https://raw.githubusercontent.com/shepherdpp/qteasy/qt_dev/img/output_dyna_plot.gif)
+![gif](docs/source/img/output_dyna_plot.gif)
 
 关于`DataSource`对象的更多详细介绍，请参见[qteasy文档](https://qteasy.readthedocs.io)
 
 
 ###  创建一个投资策略
 
 `qteasy`中的所有交易策略都是由`qteast.Operator`（交易员）对象来实现回测和运行的，`Operator`对象是一个策略容器，一个交易员可以同时
@@ -472,15 +472,15 @@
 250 day volatility:               0.138
 Max drawdown:                    11.92% 
     peak / valley:        2022-08-17 / 2022-10-31
     recovered on:         Not recovered!
 
 ===========END OF REPORT=============
 ```
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_21_1.png)
+![png](docs/source/img/output_21_1.png)
 
 ### 交易策略的参数调优
 
 交易策略的表现与参数有关，如果输入不同的参数，策略回报相差会非常大。`qteasy`可以用多种不同的优化算法，帮助搜索最优的策略参数，
 
 要使用策略优化功能，需要设置交易策略的优化标记`opt_tag=1`，并配置环境变量`mode=2`即可:
 
@@ -521,15 +521,15 @@
 27   (103, 84, 70)     1.0      1.0    74.84 114,731.44 14.7%     -3.5%     8.8%
 28  (143, 103, 49)     1.0      1.0    74.33 116,453.26 16.5%     -3.5%     4.3%
 29   (129, 92, 56)     1.0      1.0    74.55 118,811.58 18.8%     -3.5%     4.3%
 
 ===========END OF REPORT=============
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_24_1.png)   
+![png](docs/source/img/output_24_1.png)   
 将优化后的参数应用到策略中，并再次回测，可以看到结果明显提升：
 
 ```python
 op.set_parameter('dma', pars=(143, 99, 32))
 res = op.run(
         mode=1,                         # 历史回测模式
         asset_pool='000300.SH',         # 投资资产池
@@ -541,22 +541,22 @@
         cost_rate_sell=0.0001,          # 卖出费率
         visual=True,                    # 打印可视化回测图表
         trade_log=True,                 # 打印交易日志
 )
 ```
 结果如下：
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_26_1.png)   
+![png](docs/source/img/output_26_1.png)   
 
 
 关于策略优化结果的更多解读、以及更多优化参数的介绍，请参见详细文档
 
 ### 部署并开始交易策略的实盘运行
 
-`qteasy`提供了在命令行环境中运行的一个简单实盘交易程序，在配置好Operator对象并设置好策略后，自动定期运行、自动盯盘、自动下载实时数据并根据策略结果生成交易指令，模拟交易过程并记录交易结果。
+在配置好Operator对象并设置好策略后，`qteasy`可以自动定期运行、自动盯盘、自动下载实时数据并根据策略结果生成交易指令，模拟交易过程并记录交易结果。
 
 在`Operator`中设置好交易策略，并配置好交易参数后，可以直接启动实盘交易：
 
 ```python
 import qteasy as qt
 
 # 创建一个交易策略alpha
@@ -587,19 +587,19 @@
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
         live_trade_ui_type='tui',  # 使用TUI界面监控实盘交易，默认使用CLI界面
 )
 
 qt.run(op)
 ```
-qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
+`qteasy`的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
-为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
+为了对策略运行过程进行监控，同时与`qteasy`进行互动，`qteasy`提供了两种不同的交互界面：
 
 - **`TraderShell`** 交互式命令行界面，可以在命令行中输入命令，查看交易日志、查看持仓、查看账户资金变化等信息：
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+![png](docs/source/img/output_27_1.png)  
+![png](docs/source/img/output_27_3.png) 
 - **`TraderApp`** (v1.2.0新增) 交互式图形界面，可以在图形界面中查看交易日志、查看持仓、查看账户资金变化等信息
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png) 
+![png](docs/source/examples/img/trader_app_light_theme.png) 
+![png](docs/source/examples/img/trader_app_2.png) 
 
 上面两种方式都可以在实盘运行时使用，根据qteasy的配置参数进入不同的交互界，关于更多实盘运行的介绍，请参见[`QTEASY`文档](https://qteasy.readthedocs.io)
```

### Comparing `qteasy-1.2.2/README.md` & `qteasy-1.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.2`
+- Latest Version: `1.2.3`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -61,34 +61,34 @@
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_5_2.png)
+![png](docs/source/img/output_5_2.png)
 
 ### **创建交易策略**
 
 - 提供几十种内置交易策略，可以直接搭积木式使用
 - 快速创建自定义交易策略，灵活设置可调参数
 - 交易策略的回测、优化、评价，可视化输出回测结果
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_14_3.png)
+![png](docs/source/img/output_14_3.png)
 
 ### **实盘交易模拟**
 - 读取实时市场数据，实盘运行交易策略
 - 生成交易信号，模拟交易结果
 - 跟踪记录交易日志、股票持仓、账户资金变化等信息
 - 随时查看交易过程，检查盈亏情况
 - 手动控制交易进程、调整交易参数，手动下单
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
+![png](docs/source/examples/img/trader_app_1.png)  
+![png](docs/source/examples/img/trader_app_2.png)  
+![png](docs/source/examples/img/trader_app_light_theme.png) 
 
 ## 安装
 
 ```bash
 $ pip install qteasy
 ```
 
@@ -128,15 +128,15 @@
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
 import qteasy as qt
-print(qt.__version__)
+qt.__version__
 ```
 
 ### 配置本地数据源
 
 为了使用`qteasy`，需要大量的金融历史数据，所有的历史数据都必须首先保存在本地，如果本地没有历史数据，那么`qteasy`的许多功能就无法执行。
 
 `qteasy`默认通过`tushare`金融数据包来获取大量的金融数据，用户需要自行申请API Token，获取相应的权限和积分（详情参考：https://tushare.pro/document/2）
@@ -224,15 +224,15 @@
 股票的数据下载后，使用`qt.candle()`可以显示股票数据K线图。
 
 ```python
 import qteasy as qt
 data = qt.candle('000300.SH', start='2021-06-01', end='2021-8-01', asset_type='IDX')
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_5_2.png)
+![png](docs/source/img/output_5_2.png)
     
 `qteasy`的K线图函数`candle`支持通过六位数股票/指数代码查询准确的证券代码，也支持通过股票、指数名称显示K线图
 `qt.candle()`支持功能如下：
 - 显示股票、基金、期货的K线
 - 显示复权价格
 - 显示分钟、 周或月K线 
 - 显示不同移动均线以及MACD/KDJ等指标
@@ -250,23 +250,23 @@
 qt.candle('中国电信', start = '20211021', freq='30min', adj='b')
 # 期货K线，三条移动均线分别为9天、12天、26天
 qt.candle('沪铜主力', start = '20211021', mav=[9, 12, 26])
 # 场外基金净值曲线图，复权净值，不显示移动均线
 qt.candle('000001.OF', start='20200101', asset_type='FD', adj='b', mav=[])
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_1.png)
+![png](docs/source/img/output_3_1.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_7_2.png)
+![png](docs/source/img/output_7_2.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_8_3.png)
+![png](docs/source/img/output_8_3.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_4.png)
+![png](docs/source/img/output_3_4.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_5.png)
+![png](docs/source/img/output_3_5.png)
     
 
 生成的K线图可以是一个交互式动态K线图（请注意，K线图基于`matplotlib`绘制，在使用不同的终端时，显示功能有所区别，某些终端并不支持
 动态图表，详情请参阅 [matplotlib文档](https://matplotlib.org/stable/users/explain/backends.html)
 
 
 在使用动态K线图时，用户可以用鼠标和键盘控制K线图的显示范围：
@@ -274,15 +274,15 @@
 - 鼠标在图表上左右拖动：可以移动K线图显示更早或更晚的K线
 - 鼠标滚轮在图表上滚动，可以缩小或放大K线图的显示范围
 - 通过键盘左右方向键，可以移动K线图的显示范围显示更早或更晚的K线
 - 通过键盘上下键，可以缩小或放大K线图的显示范围
 - 在K线图上双击鼠标，可以切换不同的均线类型
 - 在K线图的指标区域双击，可以切换不同的指标类型：MACD，RSI，DEMA
 
-![gif](https://raw.githubusercontent.com/shepherdpp/qteasy/qt_dev/img/output_dyna_plot.gif)
+![gif](docs/source/img/output_dyna_plot.gif)
 
 关于`DataSource`对象的更多详细介绍，请参见[qteasy文档](https://qteasy.readthedocs.io)
 
 
 ###  创建一个投资策略
 
 `qteasy`中的所有交易策略都是由`qteast.Operator`（交易员）对象来实现回测和运行的，`Operator`对象是一个策略容器，一个交易员可以同时
@@ -408,15 +408,15 @@
 250 day volatility:               0.138
 Max drawdown:                    11.92% 
     peak / valley:        2022-08-17 / 2022-10-31
     recovered on:         Not recovered!
 
 ===========END OF REPORT=============
 ```
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_21_1.png)
+![png](docs/source/img/output_21_1.png)
 
 ### 交易策略的参数调优
 
 交易策略的表现与参数有关，如果输入不同的参数，策略回报相差会非常大。`qteasy`可以用多种不同的优化算法，帮助搜索最优的策略参数，
 
 要使用策略优化功能，需要设置交易策略的优化标记`opt_tag=1`，并配置环境变量`mode=2`即可:
 
@@ -457,15 +457,15 @@
 27   (103, 84, 70)     1.0      1.0    74.84 114,731.44 14.7%     -3.5%     8.8%
 28  (143, 103, 49)     1.0      1.0    74.33 116,453.26 16.5%     -3.5%     4.3%
 29   (129, 92, 56)     1.0      1.0    74.55 118,811.58 18.8%     -3.5%     4.3%
 
 ===========END OF REPORT=============
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_24_1.png)   
+![png](docs/source/img/output_24_1.png)   
 将优化后的参数应用到策略中，并再次回测，可以看到结果明显提升：
 
 ```python
 op.set_parameter('dma', pars=(143, 99, 32))
 res = op.run(
         mode=1,                         # 历史回测模式
         asset_pool='000300.SH',         # 投资资产池
@@ -477,22 +477,22 @@
         cost_rate_sell=0.0001,          # 卖出费率
         visual=True,                    # 打印可视化回测图表
         trade_log=True,                 # 打印交易日志
 )
 ```
 结果如下：
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_26_1.png)   
+![png](docs/source/img/output_26_1.png)   
 
 
 关于策略优化结果的更多解读、以及更多优化参数的介绍，请参见详细文档
 
 ### 部署并开始交易策略的实盘运行
 
-`qteasy`提供了在命令行环境中运行的一个简单实盘交易程序，在配置好Operator对象并设置好策略后，自动定期运行、自动盯盘、自动下载实时数据并根据策略结果生成交易指令，模拟交易过程并记录交易结果。
+在配置好Operator对象并设置好策略后，`qteasy`可以自动定期运行、自动盯盘、自动下载实时数据并根据策略结果生成交易指令，模拟交易过程并记录交易结果。
 
 在`Operator`中设置好交易策略，并配置好交易参数后，可以直接启动实盘交易：
 
 ```python
 import qteasy as qt
 
 # 创建一个交易策略alpha
@@ -523,19 +523,19 @@
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
         live_trade_ui_type='tui',  # 使用TUI界面监控实盘交易，默认使用CLI界面
 )
 
 qt.run(op)
 ```
-qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
+`qteasy`的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
-为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
+为了对策略运行过程进行监控，同时与`qteasy`进行互动，`qteasy`提供了两种不同的交互界面：
 
 - **`TraderShell`** 交互式命令行界面，可以在命令行中输入命令，查看交易日志、查看持仓、查看账户资金变化等信息：
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+![png](docs/source/img/output_27_1.png)  
+![png](docs/source/img/output_27_3.png) 
 - **`TraderApp`** (v1.2.0新增) 交互式图形界面，可以在图形界面中查看交易日志、查看持仓、查看账户资金变化等信息
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png) 
+![png](docs/source/examples/img/trader_app_light_theme.png) 
+![png](docs/source/examples/img/trader_app_2.png) 
 
 上面两种方式都可以在实盘运行时使用，根据qteasy的配置参数进入不同的交互界，关于更多实盘运行的介绍，请参见[`QTEASY`文档](https://qteasy.readthedocs.io)
```

### Comparing `qteasy-1.2.2/pyproject.toml` & `qteasy-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
```

### Comparing `qteasy-1.2.2/qteasy/__init__.py` & `qteasy-1.2.3/qteasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
 # qteasy版本信息
-__version__ = '1.2.1'
+__version__ = '1.2.3'
 version_info = Namespace(
         major=1,
         minor=2,
         patch=2,
         short=(1, 2),
-        full=(1, 2, 2),
-        string='1.2.2',
-        tuple=('1', '2', '2'),
+        full=(1, 2, 3),
+        string='1.2.3',
+        tuple=('1', '2', '3'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.2.2/qteasy/_arg_validators.py` & `qteasy-1.2.3/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/backtest.py` & `qteasy-1.2.3/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/blender.py` & `qteasy-1.2.3/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/broker.py` & `qteasy-1.2.3/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/built_in.py` & `qteasy-1.2.3/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/core.py` & `qteasy-1.2.3/qteasy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -691,14 +691,18 @@
             保存数据到本地时，为了减少文件/数据库读取次数，将下载的数据累计一定数量后
             再批量保存到本地，chunk_size即批量，默认值100
 
     Returns
     -------
     None
 
+    Examples
+    --------
+    >>> refill_data_source(tables='stock_basic')
+
     """
     from .database import DataSource
     if data_source is None:
         data_source = qteasy.QT_DATA_SOURCE
     if not isinstance(data_source, DataSource):
         raise TypeError(f'A DataSource object must be passed, got {type(data_source)} instead.')
     print(f'Filling data source {data_source} ...')
```

### Comparing `qteasy-1.2.2/qteasy/database.py` & `qteasy-1.2.3/qteasy/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -5144,15 +5144,15 @@
                             time_remain = sec_to_duration((total - completed) * time_elapsed / completed,
                                                           estimation=True, short_form=False)
                             progress_bar(completed, total, f'<{table}:{list(cur_kwargs.values())[0]}>'
                                                            f'{total_written}wrtn/{time_remain} left')
 
                         total_written += self.update_table_data(table, dnld_data)
                 else:
-                    progress_bar(0, total, f'<{table}:{all_kwargs}> estimating time left...')
+                    progress_bar(0, total, f'<{table}> estimating time left...')
                     for kwargs in all_kwargs:
                         df = self.fetch_history_table_data(table, channel='tushare', **kwargs)
                         completed += 1
                         if completed % chunk_size:
                             dnld_data = pd.concat([dnld_data, df])
                         else:
                             dnld_data = pd.concat([dnld_data, df])
@@ -5161,14 +5161,15 @@
                         total_written += rows_affected
                         time_elapsed = time.time() - st
                         time_remain = sec_to_duration(
                                 (total - completed) * time_elapsed / completed,
                                 estimation=True,
                                 short_form=False
                         )
+
                         if (download_batch_interval != 0) and (completed % download_batch_size == 0):
                             progress_bar(completed, total, f'<{table}:{list(kwargs.values())[0]}>'
                                                            f'{total_written}wrtn/Pausing for '
                                                            f'{download_batch_interval} sec...')
                             time.sleep(download_batch_interval)
                         else:
                             progress_bar(completed, total, f'<{table}:{list(kwargs.values())[0]}>'
```

### Comparing `qteasy-1.2.2/qteasy/emfuncs.py` & `qteasy-1.2.3/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/evaluate.py` & `qteasy-1.2.3/qteasy/evaluate.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/finance.py` & `qteasy-1.2.3/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/history.py` & `qteasy-1.2.3/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/optimization.py` & `qteasy-1.2.3/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/qt_operator.py` & `qteasy-1.2.3/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/space.py` & `qteasy-1.2.3/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/strategy.py` & `qteasy-1.2.3/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/tafuncs.py` & `qteasy-1.2.3/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/trade_recording.py` & `qteasy-1.2.3/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/trader.py` & `qteasy-1.2.3/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/trader_cli.py` & `qteasy-1.2.3/qteasy/trader_cli.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/trader_tui.py` & `qteasy-1.2.3/qteasy/trader_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/trading_util.py` & `qteasy-1.2.3/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/tsfuncs.py` & `qteasy-1.2.3/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/tui_style.tcss` & `qteasy-1.2.3/qteasy/tui_style.tcss`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/utilfuncs.py` & `qteasy-1.2.3/qteasy/utilfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy/visual.py` & `qteasy-1.2.3/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/qteasy.egg-info/PKG-INFO` & `qteasy-1.2.3/qteasy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -106,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.2`
+- Latest Version: `1.2.3`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -125,34 +125,34 @@
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_5_2.png)
+![png](docs/source/img/output_5_2.png)
 
 ### **创建交易策略**
 
 - 提供几十种内置交易策略，可以直接搭积木式使用
 - 快速创建自定义交易策略，灵活设置可调参数
 - 交易策略的回测、优化、评价，可视化输出回测结果
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_14_3.png)
+![png](docs/source/img/output_14_3.png)
 
 ### **实盘交易模拟**
 - 读取实时市场数据，实盘运行交易策略
 - 生成交易信号，模拟交易结果
 - 跟踪记录交易日志、股票持仓、账户资金变化等信息
 - 随时查看交易过程，检查盈亏情况
 - 手动控制交易进程、调整交易参数，手动下单
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
+![png](docs/source/examples/img/trader_app_1.png)  
+![png](docs/source/examples/img/trader_app_2.png)  
+![png](docs/source/examples/img/trader_app_light_theme.png) 
 
 ## 安装
 
 ```bash
 $ pip install qteasy
 ```
 
@@ -192,15 +192,15 @@
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
 import qteasy as qt
-print(qt.__version__)
+qt.__version__
 ```
 
 ### 配置本地数据源
 
 为了使用`qteasy`，需要大量的金融历史数据，所有的历史数据都必须首先保存在本地，如果本地没有历史数据，那么`qteasy`的许多功能就无法执行。
 
 `qteasy`默认通过`tushare`金融数据包来获取大量的金融数据，用户需要自行申请API Token，获取相应的权限和积分（详情参考：https://tushare.pro/document/2）
@@ -288,15 +288,15 @@
 股票的数据下载后，使用`qt.candle()`可以显示股票数据K线图。
 
 ```python
 import qteasy as qt
 data = qt.candle('000300.SH', start='2021-06-01', end='2021-8-01', asset_type='IDX')
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_5_2.png)
+![png](docs/source/img/output_5_2.png)
     
 `qteasy`的K线图函数`candle`支持通过六位数股票/指数代码查询准确的证券代码，也支持通过股票、指数名称显示K线图
 `qt.candle()`支持功能如下：
 - 显示股票、基金、期货的K线
 - 显示复权价格
 - 显示分钟、 周或月K线 
 - 显示不同移动均线以及MACD/KDJ等指标
@@ -314,23 +314,23 @@
 qt.candle('中国电信', start = '20211021', freq='30min', adj='b')
 # 期货K线，三条移动均线分别为9天、12天、26天
 qt.candle('沪铜主力', start = '20211021', mav=[9, 12, 26])
 # 场外基金净值曲线图，复权净值，不显示移动均线
 qt.candle('000001.OF', start='20200101', asset_type='FD', adj='b', mav=[])
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_1.png)
+![png](docs/source/img/output_3_1.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_7_2.png)
+![png](docs/source/img/output_7_2.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_8_3.png)
+![png](docs/source/img/output_8_3.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_4.png)
+![png](docs/source/img/output_3_4.png)
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_3_5.png)
+![png](docs/source/img/output_3_5.png)
     
 
 生成的K线图可以是一个交互式动态K线图（请注意，K线图基于`matplotlib`绘制，在使用不同的终端时，显示功能有所区别，某些终端并不支持
 动态图表，详情请参阅 [matplotlib文档](https://matplotlib.org/stable/users/explain/backends.html)
 
 
 在使用动态K线图时，用户可以用鼠标和键盘控制K线图的显示范围：
@@ -338,15 +338,15 @@
 - 鼠标在图表上左右拖动：可以移动K线图显示更早或更晚的K线
 - 鼠标滚轮在图表上滚动，可以缩小或放大K线图的显示范围
 - 通过键盘左右方向键，可以移动K线图的显示范围显示更早或更晚的K线
 - 通过键盘上下键，可以缩小或放大K线图的显示范围
 - 在K线图上双击鼠标，可以切换不同的均线类型
 - 在K线图的指标区域双击，可以切换不同的指标类型：MACD，RSI，DEMA
 
-![gif](https://raw.githubusercontent.com/shepherdpp/qteasy/qt_dev/img/output_dyna_plot.gif)
+![gif](docs/source/img/output_dyna_plot.gif)
 
 关于`DataSource`对象的更多详细介绍，请参见[qteasy文档](https://qteasy.readthedocs.io)
 
 
 ###  创建一个投资策略
 
 `qteasy`中的所有交易策略都是由`qteast.Operator`（交易员）对象来实现回测和运行的，`Operator`对象是一个策略容器，一个交易员可以同时
@@ -472,15 +472,15 @@
 250 day volatility:               0.138
 Max drawdown:                    11.92% 
     peak / valley:        2022-08-17 / 2022-10-31
     recovered on:         Not recovered!
 
 ===========END OF REPORT=============
 ```
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_21_1.png)
+![png](docs/source/img/output_21_1.png)
 
 ### 交易策略的参数调优
 
 交易策略的表现与参数有关，如果输入不同的参数，策略回报相差会非常大。`qteasy`可以用多种不同的优化算法，帮助搜索最优的策略参数，
 
 要使用策略优化功能，需要设置交易策略的优化标记`opt_tag=1`，并配置环境变量`mode=2`即可:
 
@@ -521,15 +521,15 @@
 27   (103, 84, 70)     1.0      1.0    74.84 114,731.44 14.7%     -3.5%     8.8%
 28  (143, 103, 49)     1.0      1.0    74.33 116,453.26 16.5%     -3.5%     4.3%
 29   (129, 92, 56)     1.0      1.0    74.55 118,811.58 18.8%     -3.5%     4.3%
 
 ===========END OF REPORT=============
 ```
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_24_1.png)   
+![png](docs/source/img/output_24_1.png)   
 将优化后的参数应用到策略中，并再次回测，可以看到结果明显提升：
 
 ```python
 op.set_parameter('dma', pars=(143, 99, 32))
 res = op.run(
         mode=1,                         # 历史回测模式
         asset_pool='000300.SH',         # 投资资产池
@@ -541,22 +541,22 @@
         cost_rate_sell=0.0001,          # 卖出费率
         visual=True,                    # 打印可视化回测图表
         trade_log=True,                 # 打印交易日志
 )
 ```
 结果如下：
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_26_1.png)   
+![png](docs/source/img/output_26_1.png)   
 
 
 关于策略优化结果的更多解读、以及更多优化参数的介绍，请参见详细文档
 
 ### 部署并开始交易策略的实盘运行
 
-`qteasy`提供了在命令行环境中运行的一个简单实盘交易程序，在配置好Operator对象并设置好策略后，自动定期运行、自动盯盘、自动下载实时数据并根据策略结果生成交易指令，模拟交易过程并记录交易结果。
+在配置好Operator对象并设置好策略后，`qteasy`可以自动定期运行、自动盯盘、自动下载实时数据并根据策略结果生成交易指令，模拟交易过程并记录交易结果。
 
 在`Operator`中设置好交易策略，并配置好交易参数后，可以直接启动实盘交易：
 
 ```python
 import qteasy as qt
 
 # 创建一个交易策略alpha
@@ -587,19 +587,19 @@
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
         live_trade_ui_type='tui',  # 使用TUI界面监控实盘交易，默认使用CLI界面
 )
 
 qt.run(op)
 ```
-qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
+`qteasy`的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
-为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
+为了对策略运行过程进行监控，同时与`qteasy`进行互动，`qteasy`提供了两种不同的交互界面：
 
 - **`TraderShell`** 交互式命令行界面，可以在命令行中输入命令，查看交易日志、查看持仓、查看账户资金变化等信息：
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+![png](docs/source/img/output_27_1.png)  
+![png](docs/source/img/output_27_3.png) 
 - **`TraderApp`** (v1.2.0新增) 交互式图形界面，可以在图形界面中查看交易日志、查看持仓、查看账户资金变化等信息
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png) 
+![png](docs/source/examples/img/trader_app_light_theme.png) 
+![png](docs/source/examples/img/trader_app_2.png) 
 
 上面两种方式都可以在实盘运行时使用，根据qteasy的配置参数进入不同的交互界，关于更多实盘运行的介绍，请参见[`QTEASY`文档](https://qteasy.readthedocs.io)
```

### Comparing `qteasy-1.2.2/qteasy.egg-info/SOURCES.txt` & `qteasy-1.2.3/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/setup.cfg` & `qteasy-1.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.2.2
+version = 1.2.3
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
```

### Comparing `qteasy-1.2.2/tests/test_broker.py` & `qteasy-1.2.3/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_cashplan.py` & `qteasy-1.2.3/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_config.py` & `qteasy-1.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_core_sub_funcs.py` & `qteasy-1.2.3/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_cost.py` & `qteasy-1.2.3/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_datasource.py` & `qteasy-1.2.3/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_eastmoney.py` & `qteasy-1.2.3/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_evaluations.py` & `qteasy-1.2.3/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_fast_experiments.py` & `qteasy-1.2.3/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_historypanel.py` & `qteasy-1.2.3/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_loop.py` & `qteasy-1.2.3/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_operator_and_strategy.py` & `qteasy-1.2.3/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_qt.py` & `qteasy-1.2.3/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_space.py` & `qteasy-1.2.3/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_ta_funcs.py` & `qteasy-1.2.3/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_trader.py` & `qteasy-1.2.3/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_trader_shell.py` & `qteasy-1.2.3/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_trading.py` & `qteasy-1.2.3/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_tui.py` & `qteasy-1.2.3/tests/test_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_tushare.py` & `qteasy-1.2.3/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_utilityfuncs.py` & `qteasy-1.2.3/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.2/tests/test_visual.py` & `qteasy-1.2.3/tests/test_visual.py`

 * *Files identical despite different names*

