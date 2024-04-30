# Comparing `tmp/pkscreener-0.44.20240429.314.tar.gz` & `tmp/pkscreener-0.44.20240430.315.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240429.314.tar", last modified: Mon Apr 29 13:19:54 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240430.315.tar", last modified: Tue Apr 30 10:30:21 2024, max compression
```

## Comparing `pkscreener-0.44.20240429.314.tar` & `pkscreener-0.44.20240430.315.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/
--rw-rw-rw-   0        0        0     1086 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.894821 pkscreener-0.44.20240429.314/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7288 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29455 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20421 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   116796 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51669 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    81840 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-29 13:19:46.000000 pkscreener-0.44.20240429.314/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123016 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    41457 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25897 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.894821 pkscreener-0.44.20240429.314/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:30:21.948394 pkscreener-0.44.20240430.315/
+-rw-rw-rw-   0        0        0     1086 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-30 10:30:21.948394 pkscreener-0.44.20240430.315/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 10:30:21.932773 pkscreener-0.44.20240430.315/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:30:21.948394 pkscreener-0.44.20240430.315/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25815 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7288 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29455 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20421 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   116796 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51669 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82018 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-30 10:30:11.000000 pkscreener-0.44.20240430.315/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123078 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25897 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:30:21.932773 pkscreener-0.44.20240430.315/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-30 10:30:21.000000 pkscreener-0.44.20240430.315/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-30 10:30:21.000000 pkscreener-0.44.20240430.315/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:30:21.000000 pkscreener-0.44.20240430.315/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-30 10:30:21.000000 pkscreener-0.44.20240430.315/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-30 10:30:21.000000 pkscreener-0.44.20240430.315/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-30 10:30:21.000000 pkscreener-0.44.20240430.315/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-30 10:30:21.948394 pkscreener-0.44.20240430.315/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-30 10:25:44.000000 pkscreener-0.44.20240430.315/setup.py
```

### Comparing `pkscreener-0.44.20240429.314/LICENSE` & `pkscreener-0.44.20240430.315/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/LICENSE-Others` & `pkscreener-0.44.20240430.315/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/PKG-INFO` & `pkscreener-0.44.20240430.315/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240429.314
+Version: 0.44.20240430.315
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240429.314.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240430.315.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240429.314/README.md` & `pkscreener-0.44.20240430.315/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240429.314/pkscreener/__init__.py` & `pkscreener-0.44.20240430.315/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,18 @@
             if userArgs is not None and userArgs.v:
                 os.environ["RUNNER"]="LOCAL_RUN_SCANNER"
             return
         elif (userArgs is not None and userArgs.runintradayanalysis):
             return
         if clearAlways or OutputControls().enableMultipleLineOutput:
             if platform.system() == "Windows":
+                # os.system('color 0f') # sets the background to black with white forerground
                 os.system("cls")
             else:
+                # os.system('setterm -background black -foreground white -store')
                 os.system("clear")
         try:
             if clearAlways or OutputControls().enableMultipleLineOutput:
                 art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
                 OutputControls().printOutput(art.encode('utf-8').decode(STD_ENCODING), enableMultipleLineOutput=True)
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
```

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/classes/keys.py` & `pkscreener-0.44.20240430.315/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/courbd.ttf` & `pkscreener-0.44.20240430.315/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/globals.py` & `pkscreener-0.44.20240430.315/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 test_messages_queue = []
 strategyFilter=[]
 listStockCodes = None
 tasks_queue = None
 results_queue = None
 consumers = None
 logging_queue = None
+mp_manager = None
 
 def finishScreening(
     downloadOnly,
     testing,
     stockDictPrimary,
     configManager,
     loadCount,
@@ -637,15 +638,15 @@
     )
     listStockCodes = prepareStocksForScreening(testing=False, downloadOnly=False, listStockCodes=None,indexOption=indexOption)
     stockDictPrimary,stockDictSecondary = loadDatabaseOrFetch(downloadOnly=False, listStockCodes=listStockCodes, menuOption=menuOption,indexOption=indexOption)
     PKScanRunner.refreshDatabase(consumers,stockDictPrimary,stockDictSecondary)
 
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
-    global listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDictPrimary, stockDictSecondary, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
+    global mp_manager, listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDictPrimary, stockDictSecondary, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
     start_time = 0
     testing = False if userArgs is None else (userArgs.testbuild and userArgs.prodbuild)
     testBuild = False if userArgs is None else (userArgs.testbuild and not testing)
     downloadOnly = False if userArgs is None else userArgs.download
     startupoptions = None if userArgs is None else userArgs.options
@@ -654,20 +655,22 @@
     userPassedArgs = userArgs
     options = []
     strategyFilter=[]
     if keyboardInterruptEventFired:
         return None, None
     screenCounter = multiprocessing.Value("i", 1)
     screenResultsCounter = multiprocessing.Value("i", 0)
+    if mp_manager is None:
+        mp_manager = multiprocessing.Manager()
     if keyboardInterruptEvent is None and not keyboardInterruptEventFired:
-        keyboardInterruptEvent = multiprocessing.Manager().Event()
+        keyboardInterruptEvent = mp_manager.Event()
     keyboardInterruptEventFired = False
     if stockDictPrimary is None:
-        stockDictPrimary = multiprocessing.Manager().dict()
-        stockDictSecondary = multiprocessing.Manager().dict()
+        stockDictPrimary = mp_manager.dict()
+        stockDictSecondary = mp_manager.dict()
         loadCount = 0
     endOfdayCandles = None
     minRSI = 0
     maxRSI = 100
     insideBarToLookback = 7
     respChartPattern = None
     daysForLowestVolume = 30
```

### Comparing `pkscreener-0.44.20240429.314/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240430.315/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240430.315/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     Application,
     CallbackQueryHandler,
     CommandHandler,
     ContextTypes,
     ConversationHandler,
     MessageHandler,
     filters,
+    CallbackContext
 )
 
 # Enable logging
 logging.basicConfig(
     format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 # set higher logging level for httpx to avoid all GET and POST requests being logged
@@ -163,15 +164,16 @@
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
     if data not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     midSkip = "1" if data == "X" else "N"
-    skipMenus = INDEX_SKIP_MENUS.append(midSkip)
+    skipMenus = [midSkip]
+    skipMenus.extend(INDEX_SKIP_MENUS)
     menuText = (
         m1.renderForMenu(
             m0.find(data),
             skip=skipMenus,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         .replace("     ", "")
@@ -216,15 +218,15 @@
         if str(selection[1]).isnumeric():
             # It's only level 2
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_1_TO_7,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\nN > More options"
+            menuText = menuText + "\n\nN > More options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_1_TO_7,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("N", "More Options", 2))
@@ -233,15 +235,15 @@
     elif len(selection) == 3:
         if selection[2] == "N":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_8_TO_13,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\nP > Previous Options"
+            menuText = menuText + "\n\nP > Previous Options"
             menuText = menuText + "\nM > More Options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_8_TO_13,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
@@ -249,15 +251,15 @@
             mns.append(menu().create("M", "More Options", 2))
         elif selection[2] == "M":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_14_TO_19,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\nP > Previous Options"
+            menuText = menuText + "\n\nP > Previous Options"
             menuText = menuText + "\n>> More Options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_14_TO_19,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
@@ -265,15 +267,15 @@
             mns.append(menu().create(">>", "More Options", 2))
         elif selection[2] == ">>":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_20_TO_27,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\nP > Previous Options"
+            menuText = menuText + "\n\nP > Previous Options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_20_TO_27,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("P", "Previous Options", 2))
@@ -865,14 +867,59 @@
                     )
                     for mnu3 in cmds3:
                         p3 = mnu3.menuKey.upper()
                         application.add_handler(
                             CommandHandler(f"{p0}_{p1}_{p2}_{p3}", command_handler)
                         )
 
+# def send_stuff(context: CallbackContext):
+#   job = context.job
+
+#   keyboard = [ 
+#     [   
+#         InlineKeyboardButton("NEVER", callback_data="NEVER"),
+#         InlineKeyboardButton("UNLIKELY", callback_data="UNLIKELY")
+#     ],  
+#     [   
+#         InlineKeyboardButton("MEH", callback_data="MEH"),
+#         InlineKeyboardButton("MAYBE", callback_data="MAYBE")
+#     ],  
+#     [   
+#         InlineKeyboardButton("YES", callback_data="YES"),
+#         InlineKeyboardButton("ABSOLUTELY", callback_data="ABSOLUTELY")
+#     ],  
+#     [   
+#         InlineKeyboardButton("RATHER NOT SAY", callback_data="UNKNOWN")
+#     ]   
+#   ]
+
+#   reply_markup = InlineKeyboardMarkup(keyboard)
+
+#   context.bot.send_photo(job.context, photo=open(PATH+thefile, 'rb'))
+#   # return values of send_message are saved in the 'msg' var
+#   msg = context.bot.send_message(job.context, text='RATE', reply_markup=reply_markup)
+
+#   # the following job is created every time the send_stuff function is called
+#   context.job_queue.run_once(
+#     callback=cleanup,
+#     when=5,
+#     context=msg,
+#     name='cleanup'
+#   )
+
+# # the function called by the job
+# def cleanup(context: CallbackContext):
+#   job = context.job
+
+#   context.bot.edit_message_text(
+#     chat_id=job.context.chat.id,
+#     text='NO ANSWER PROVIDED',
+#     message_id=job.context.message_id
+#   )
+
 
 def runpkscreenerbot() -> None:
     """Run the bot."""
     # Create the Application and pass it your bot's token.
     global chat_idADMIN, Channel_Id
     Channel_Id, TOKEN, chat_idADMIN, GITHUB_TOKEN = get_secrets()
     # TOKEN = '1234567'
```

### Comparing `pkscreener-0.44.20240429.314/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240430.315/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240430.315/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240429.314
+Version: 0.44.20240430.315
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240429.314.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240430.315.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.314/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240429.314/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240430.315/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.314/setup.py` & `pkscreener-0.44.20240430.315/setup.py`

 * *Files identical despite different names*

