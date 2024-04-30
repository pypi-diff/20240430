# Comparing `tmp/pkscreener-0.44.20240429.305.tar.gz` & `tmp/pkscreener-0.44.20240429.314.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240429.305.tar", last modified: Mon Apr 29 05:49:51 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240429.314.tar", last modified: Mon Apr 29 13:19:54 2024, max compression
```

## Comparing `pkscreener-0.44.20240429.305.tar` & `pkscreener-0.44.20240429.314.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:49:51.554782 pkscreener-0.44.20240429.305/
--rw-rw-rw-   0        0        0     1086 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-29 05:49:51.554782 pkscreener-0.44.20240429.305/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 05:49:51.539155 pkscreener-0.44.20240429.305/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:49:51.554782 pkscreener-0.44.20240429.305/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7288 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29455 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20421 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   116796 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51535 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    81840 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-29 05:49:42.000000 pkscreener-0.44.20240429.305/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123016 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    41457 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25522 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:49:51.539155 pkscreener-0.44.20240429.305/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-29 05:49:51.000000 pkscreener-0.44.20240429.305/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-29 05:49:51.000000 pkscreener-0.44.20240429.305/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:49:51.000000 pkscreener-0.44.20240429.305/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-29 05:49:51.000000 pkscreener-0.44.20240429.305/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 05:49:51.000000 pkscreener-0.44.20240429.305/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-29 05:49:51.000000 pkscreener-0.44.20240429.305/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-29 05:49:51.554782 pkscreener-0.44.20240429.305/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-29 05:45:15.000000 pkscreener-0.44.20240429.305/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/
+-rw-rw-rw-   0        0        0     1086 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.894821 pkscreener-0.44.20240429.314/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25815 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7288 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29455 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20421 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   116796 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51669 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    81840 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-29 13:19:46.000000 pkscreener-0.44.20240429.314/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123016 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    41457 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25897 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:19:54.894821 pkscreener-0.44.20240429.314/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-29 13:19:54.000000 pkscreener-0.44.20240429.314/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-29 13:19:54.910444 pkscreener-0.44.20240429.314/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-29 13:15:57.000000 pkscreener-0.44.20240429.314/setup.py
```

### Comparing `pkscreener-0.44.20240429.305/LICENSE` & `pkscreener-0.44.20240429.314/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/LICENSE-Others` & `pkscreener-0.44.20240429.314/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/PKG-INFO` & `pkscreener-0.44.20240429.314/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240429.305
+Version: 0.44.20240429.314
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240429.305.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240429.314.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240429.305/README.md` & `pkscreener-0.44.20240429.314/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240429.305/pkscreener/__init__.py` & `pkscreener-0.44.20240429.314/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,17 @@
                     processedData = processedData.head(len(intraday_processedData))
                     intraday_processedData = intraday_processedData.head(len(processedData))
                     data = data.tail(len(intraday_data))
                     intraday_data = intraday_data.tail(len(data))
                     # Indexes won't match. Hence, we'd need to fallback on tolist
                     processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
                     fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
+                else:
+                    processedData.loc[:,"RSIi"] = np.nan
+                    fullData.loc[:,"RSIi"] = np.nan
 
             def returnLegibleData(exceptionMessage=None):
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     raise ScreeningStatistics.EligibilityConditionNotMet(exceptionMessage)
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
```

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/classes/keys.py` & `pkscreener-0.44.20240429.314/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/courbd.ttf` & `pkscreener-0.44.20240429.314/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/globals.py` & `pkscreener-0.44.20240429.314/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240429.314/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240429.314/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240429.314/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # Pyinstaller compile Windows: pyinstaller --onefile --icon=screenshots\icon.ico pkscreener\pkscreenercli.py  --hidden-import cmath --hidden-import talib.stream --hidden-import numpy --hidden-import pandas --hidden-import alive-progress
 # Pyinstaller compile Linux  : pyinstaller --onefile --icon=screenshots/icon.ico pkscreener/pkscreenercli.py  --hidden-import cmath --hidden-import talib.stream --hidden-import numpy --hidden-import pandas --hidden-import alive-progress
 import warnings
 warnings.simplefilter("ignore", UserWarning,append=True)
 import argparse
 import builtins
 import logging
+import json
 import traceback
 import datetime
 # Keep module imports prior to classes
 import os
 import sys
 import tempfile
 os.environ["PYTHONWARNINGS"]="ignore::UserWarning"
@@ -196,14 +197,20 @@
 argParser.add_argument(
     "--runintradayanalysis",
     action="store_true",
     help="Run analysis for morning vs EoD LTP values",
     required=False,
 )
 argParser.add_argument(
+    "--simulate",
+    type=json.loads, # '{"isTrading":true,"currentDateTime":"2024-04-29 09:35:38"}'
+    help="Simulate various conditions",
+    required=False,
+)
+argParser.add_argument(
     "-t",
     "--testbuild",
     action="store_true",
     help="Run in test-build mode",
     required=False,
 )
 argParser.add_argument(
@@ -469,14 +476,18 @@
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild and args.answerdefault is None:
             input("Press <Enter> to continue...")
     else:
         if "PKDevTools_Default_Log_Level" in os.environ.keys():
             del os.environ['PKDevTools_Default_Log_Level']
             # os.environ["PKDevTools_Default_Log_Level"] = str(log.logging.NOTSET)
+    if args.simulate:
+        os.environ["simulation"] = json.dumps(args.simulate)
+    elif "simulation" in os.environ.keys():
+        del os.environ['simulation']
     # Import other dependency here because if we import them at the top
     # multiprocessing behaves in unpredictable ways
     import pkscreener.classes.Utility as Utility
 
     configManager.default_logger = default_logger()
     if originalStdOut is None:
         # Clear only if this is the first time it's being called from some
```

### Comparing `pkscreener-0.44.20240429.305/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240429.314/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240429.305
+Version: 0.44.20240429.314
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240429.305.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240429.314.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.304/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240429.305/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240429.305/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240429.314/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240429.305/setup.py` & `pkscreener-0.44.20240429.314/setup.py`

 * *Files identical despite different names*

