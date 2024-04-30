# Comparing `tmp/specvizitor-0.4.0.tar.gz` & `tmp/specvizitor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specvizitor-0.4.0.tar", max compression
+gzip compressed data, was "specvizitor-0.4.1.tar", max compression
```

## Comparing `specvizitor-0.4.0.tar` & `specvizitor-0.4.1.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1532 2023-10-23 08:53:53.000000 specvizitor-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1351 2024-04-17 13:19:22.727160 specvizitor-0.4.0/README.md
--rw-r--r--   0        0        0      903 2024-04-17 16:24:11.359970 specvizitor-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/__init__.py
--rw-r--r--   0        0        0       31 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/__main__.py
--rw-r--r--   0        0        0     1412 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/appdata.py
--rw-r--r--   0        0        0      136 2023-11-17 10:15:06.000000 specvizitor-0.4.0/specvizitor/config/__init__.py
--rw-r--r--   0        0        0      549 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/config/appearance.py
--rw-r--r--   0        0        0      316 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/config/cache.py
--rw-r--r--   0        0        0     1403 2024-04-12 18:36:53.235882 specvizitor-0.4.0/specvizitor/config/config.py
--rw-r--r--   0        0        0     2807 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/config/data_widgets.py
--rw-r--r--   0        0        0      242 2023-11-17 10:15:06.000000 specvizitor-0.4.0/specvizitor/config/spectral_lines.py
--rw-r--r--   0        0        0     2683 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward.svg
--rw-r--r--   0        0        0     2672 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1526 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward.svg
--rw-r--r--   0        0        0     2096 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/dark-mode.svg
--rw-r--r--   0        0        0     3408 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/gear.svg
--rw-r--r--   0        0        0     5541 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/reset-dock-state.svg
--rw-r--r--   0        0        0     2062 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/dark/star.svg
--rw-r--r--   0        0        0     2682 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward.svg
--rw-r--r--   0        0        0     2671 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1525 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward.svg
--rw-r--r--   0        0        0     2112 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/dark-mode.svg
--rw-r--r--   0        0        0     3409 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/gear.svg
--rw-r--r--   0        0        0     5540 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/reset-dock-state.svg
--rw-r--r--   0        0        0     2063 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/icons/light/star.svg
--rw-r--r--   0        0        0      347 2024-04-12 18:57:29.896161 specvizitor-0.4.0/specvizitor/data/presets/config.yml
--rw-r--r--   0        0        0     2197 2024-04-16 15:53:33.245075 specvizitor-0.4.0/specvizitor/data/presets/data_widgets.yml
--rw-r--r--   0        0        0       35 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/data/presets/legacy.txt
--rw-r--r--   0        0        0     1957 2024-04-03 13:06:15.000000 specvizitor-0.4.0/specvizitor/data/presets/spectral_lines.yml
--rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/io/__init__.py
--rw-r--r--   0        0        0     6617 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/io/catalog.py
--rw-r--r--   0        0        0     7098 2024-04-14 10:45:37.736696 specvizitor-0.4.0/specvizitor/io/inspection_data.py
--rw-r--r--   0        0        0    11659 2024-04-16 15:53:33.257075 specvizitor-0.4.0/specvizitor/io/viewer_data.py
--rw-r--r--   0        0        0     3878 2024-03-21 12:29:30.000000 specvizitor-0.4.0/specvizitor/main.py
--rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/plugins/__init__.py
--rw-r--r--   0        0        0      532 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/plugins/plugin_core.py
--rw-r--r--   0        0        0     2920 2024-04-03 17:18:45.000000 specvizitor-0.4.0/specvizitor/plugins/sviz-eiger.py
--rw-r--r--   0        0        0     6367 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/plugins/sviz-grizli.py
--rw-r--r--   0        0        0        1 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/utils/__init__.py
--rw-r--r--   0        0        0     1296 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/logs.py
--rw-r--r--   0        0        0     4388 2024-03-15 11:33:34.000000 specvizitor-0.4.0/specvizitor/utils/params.py
--rw-r--r--   0        0        0      954 2024-02-16 22:41:49.000000 specvizitor-0.4.0/specvizitor/utils/qt_tools.py
--rw-r--r--   0        0        0      972 2023-12-07 21:01:49.000000 specvizitor-0.4.0/specvizitor/utils/widgets/AbstractWidget.py
--rw-r--r--   0        0        0      521 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/ColorBar.py
--rw-r--r--   0        0        0     4447 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/FileBrowser.py
--rw-r--r--   0        0        0      713 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/MyViewBox.py
--rw-r--r--   0        0        0    12377 2024-03-21 13:18:35.000000 specvizitor-0.4.0/specvizitor/utils/widgets/ParamTable.py
--rw-r--r--   0        0        0     3465 2024-03-21 13:35:19.000000 specvizitor-0.4.0/specvizitor/utils/widgets/Section.py
--rw-r--r--   0        0        0      208 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/utils/widgets/__init__.py
--rw-r--r--   0        0        0    14987 2024-04-17 15:17:46.467357 specvizitor-0.4.0/specvizitor/widgets/DataViewer.py
--rw-r--r--   0        0        0     6898 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/Image2D.py
--rw-r--r--   0        0        0     3477 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/InspectionEditor.py
--rw-r--r--   0        0        0     4647 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/InspectionResults.py
--rw-r--r--   0        0        0    28172 2024-04-15 13:02:55.200442 specvizitor-0.4.0/specvizitor/widgets/MainWindow.py
--rw-r--r--   0        0        0     7916 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/NewFile.py
--rw-r--r--   0        0        0     5221 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/ObjectInfo.py
--rw-r--r--   0        0        0     3854 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/Plot1D.py
--rw-r--r--   0        0        0     2537 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/QuickSearch.py
--rw-r--r--   0        0        0    16112 2024-04-12 19:10:29.663993 specvizitor-0.4.0/specvizitor/widgets/Settings.py
--rw-r--r--   0        0        0     6390 2024-04-15 16:03:47.642782 specvizitor-0.4.0/specvizitor/widgets/SmartSlider.py
--rw-r--r--   0        0        0     4144 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/Subsets.py
--rw-r--r--   0        0        0     3454 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/TableColumns.py
--rw-r--r--   0        0        0     7099 2024-03-20 22:12:36.000000 specvizitor-0.4.0/specvizitor/widgets/ToolBar.py
--rw-r--r--   0        0        0    17618 2024-04-15 22:04:47.006961 specvizitor-0.4.0/specvizitor/widgets/ViewerElement.py
--rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.0/specvizitor/widgets/__init__.py
--rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 specvizitor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1532 2023-10-23 08:53:53.000000 specvizitor-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     1351 2024-04-17 13:19:22.727160 specvizitor-0.4.1/README.md
+-rw-r--r--   0        0        0      917 2024-04-30 08:46:26.717979 specvizitor-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/__init__.py
+-rw-r--r--   0        0        0       31 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/__main__.py
+-rw-r--r--   0        0        0     1412 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/appdata.py
+-rw-r--r--   0        0        0      136 2023-11-17 10:15:06.000000 specvizitor-0.4.1/specvizitor/config/__init__.py
+-rw-r--r--   0        0        0      549 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/config/appearance.py
+-rw-r--r--   0        0        0      316 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/config/cache.py
+-rw-r--r--   0        0        0     1403 2024-04-12 18:36:53.235882 specvizitor-0.4.1/specvizitor/config/config.py
+-rw-r--r--   0        0        0     2807 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/config/data_widgets.py
+-rw-r--r--   0        0        0      242 2023-11-17 10:15:06.000000 specvizitor-0.4.1/specvizitor/config/spectral_lines.py
+-rw-r--r--   0        0        0     2683 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-backward.svg
+-rw-r--r--   0        0        0     2672 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1526 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-forward.svg
+-rw-r--r--   0        0        0     2096 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/dark-mode.svg
+-rw-r--r--   0        0        0     3408 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/gear.svg
+-rw-r--r--   0        0        0     5541 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/reset-dock-state.svg
+-rw-r--r--   0        0        0     2062 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/dark/star.svg
+-rw-r--r--   0        0        0     2682 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/arrow-backward.svg
+-rw-r--r--   0        0        0     2671 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1525 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/arrow-forward.svg
+-rw-r--r--   0        0        0     2112 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/dark-mode.svg
+-rw-r--r--   0        0        0     3409 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/gear.svg
+-rw-r--r--   0        0        0     5540 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/reset-dock-state.svg
+-rw-r--r--   0        0        0     2063 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/icons/light/star.svg
+-rw-r--r--   0        0        0      347 2024-04-12 18:57:29.896161 specvizitor-0.4.1/specvizitor/data/presets/config.yml
+-rw-r--r--   0        0        0     2197 2024-04-16 15:53:33.245075 specvizitor-0.4.1/specvizitor/data/presets/data_widgets.yml
+-rw-r--r--   0        0        0       35 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/data/presets/legacy.txt
+-rw-r--r--   0        0        0     1957 2024-04-03 13:06:15.000000 specvizitor-0.4.1/specvizitor/data/presets/spectral_lines.yml
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/io/__init__.py
+-rw-r--r--   0        0        0     6617 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/io/catalog.py
+-rw-r--r--   0        0        0     7098 2024-04-14 10:45:37.736696 specvizitor-0.4.1/specvizitor/io/inspection_data.py
+-rw-r--r--   0        0        0    11659 2024-04-16 15:53:33.257075 specvizitor-0.4.1/specvizitor/io/viewer_data.py
+-rw-r--r--   0        0        0     3878 2024-04-18 11:04:24.109784 specvizitor-0.4.1/specvizitor/main.py
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/plugins/__init__.py
+-rw-r--r--   0        0        0      532 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/plugins/plugin_core.py
+-rw-r--r--   0        0        0     2920 2024-04-03 17:18:45.000000 specvizitor-0.4.1/specvizitor/plugins/sviz-eiger.py
+-rw-r--r--   0        0        0     6376 2024-04-23 11:41:51.995742 specvizitor-0.4.1/specvizitor/plugins/sviz-grizli.py
+-rw-r--r--   0        0        0        1 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/utils/__init__.py
+-rw-r--r--   0        0        0     1296 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/utils/logs.py
+-rw-r--r--   0        0        0     4388 2024-03-15 11:33:34.000000 specvizitor-0.4.1/specvizitor/utils/params.py
+-rw-r--r--   0        0        0      954 2024-02-16 22:41:49.000000 specvizitor-0.4.1/specvizitor/utils/qt_tools.py
+-rw-r--r--   0        0        0      972 2023-12-07 21:01:49.000000 specvizitor-0.4.1/specvizitor/utils/widgets/AbstractWidget.py
+-rw-r--r--   0        0        0      521 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/utils/widgets/ColorBar.py
+-rw-r--r--   0        0        0     4447 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/utils/widgets/FileBrowser.py
+-rw-r--r--   0        0        0      251 2024-04-26 16:55:06.369000 specvizitor-0.4.1/specvizitor/utils/widgets/MyQTextEdit.py
+-rw-r--r--   0        0        0      713 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/utils/widgets/MyViewBox.py
+-rw-r--r--   0        0        0    12419 2024-04-18 11:43:13.377630 specvizitor-0.4.1/specvizitor/utils/widgets/ParamTable.py
+-rw-r--r--   0        0        0     3465 2024-04-18 11:34:49.342627 specvizitor-0.4.1/specvizitor/utils/widgets/Section.py
+-rw-r--r--   0        0        0      245 2024-04-26 16:48:23.140262 specvizitor-0.4.1/specvizitor/utils/widgets/__init__.py
+-rw-r--r--   0        0        0    14987 2024-04-17 15:17:46.467357 specvizitor-0.4.1/specvizitor/widgets/DataViewer.py
+-rw-r--r--   0        0        0     6898 2024-04-18 12:07:07.104520 specvizitor-0.4.1/specvizitor/widgets/Image2D.py
+-rw-r--r--   0        0        0     3477 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/InspectionEditor.py
+-rw-r--r--   0        0        0     4740 2024-04-26 17:19:06.891585 specvizitor-0.4.1/specvizitor/widgets/InspectionResults.py
+-rw-r--r--   0        0        0    28169 2024-04-26 16:53:45.564016 specvizitor-0.4.1/specvizitor/widgets/MainWindow.py
+-rw-r--r--   0        0        0     7916 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/NewFile.py
+-rw-r--r--   0        0        0     5221 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/ObjectInfo.py
+-rw-r--r--   0        0        0     3854 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/Plot1D.py
+-rw-r--r--   0        0        0     2537 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/QuickSearch.py
+-rw-r--r--   0        0        0    16112 2024-04-18 11:36:24.447983 specvizitor-0.4.1/specvizitor/widgets/Settings.py
+-rw-r--r--   0        0        0     6390 2024-04-15 16:03:47.642782 specvizitor-0.4.1/specvizitor/widgets/SmartSlider.py
+-rw-r--r--   0        0        0     4144 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/Subsets.py
+-rw-r--r--   0        0        0     3454 2024-03-20 22:12:36.000000 specvizitor-0.4.1/specvizitor/widgets/TableColumns.py
+-rw-r--r--   0        0        0     7050 2024-04-26 15:57:26.096483 specvizitor-0.4.1/specvizitor/widgets/ToolBar.py
+-rw-r--r--   0        0        0    17618 2024-04-15 22:04:47.006961 specvizitor-0.4.1/specvizitor/widgets/ViewerElement.py
+-rw-r--r--   0        0        0        0 2023-10-23 08:53:53.000000 specvizitor-0.4.1/specvizitor/widgets/__init__.py
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 specvizitor-0.4.1/PKG-INFO
```

### Comparing `specvizitor-0.4.0/LICENSE.txt` & `specvizitor-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/README.md` & `specvizitor-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/pyproject.toml` & `specvizitor-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "specvizitor"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python GUI application for a visual inspection of astronomical spectroscopic data"
 authors = ["Ivan Kramarenko <im.kramarenko@gmail.com>", "Josephine Kerutt <>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ivkram/specvizitor"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-astropy = "6.0.0"
+astropy = ">=6.0.0"
 dacite = "1.8.1"
 dictdiffer = "0.9.0"
-pandas = "2.2.0"
+pandas = ">=2.2.0"
 pgcolorbar = "1.1.3"
-pillow = "10.2.0"
-platformdirs = "4.2.0"
+pillow = ">=10.2.0"
+platformdirs = ">=4.2.0"
 pyqt5 = "5.15.2"
 pyqtdarktheme = "2.1.0"
-pyqtgraph = "0.13.3"
+pyqtgraph = ">=0.13.3"
 qtpy = "2.4.1"
-rasterio = "1.3.9"
-scipy = "1.12.0"
+rasterio = ">=1.3.9"
+scipy = ">=1.12.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 sphinx-book-theme = "*"
```

### Comparing `specvizitor-0.4.0/specvizitor/appdata.py` & `specvizitor-0.4.1/specvizitor/appdata.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/config/appearance.py` & `specvizitor-0.4.1/specvizitor/config/appearance.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/config/config.py` & `specvizitor-0.4.1/specvizitor/config/config.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/config/data_widgets.py` & `specvizitor-0.4.1/specvizitor/config/data_widgets.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward-starred.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-backward.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward-starred.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/arrow-forward.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/dark-mode.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/gear.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/reset-dock-state.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/reset-view.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/screenshot.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/star-empty.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/dark/star.svg` & `specvizitor-0.4.1/specvizitor/data/icons/dark/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward-starred.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-backward.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward-starred.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/arrow-forward.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/dark-mode.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/gear.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/reset-dock-state.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/reset-view.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/screenshot.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/star-empty.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/icons/light/star.svg` & `specvizitor-0.4.1/specvizitor/data/icons/light/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/presets/data_widgets.yml` & `specvizitor-0.4.1/specvizitor/data/presets/data_widgets.yml`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/data/presets/spectral_lines.yml` & `specvizitor-0.4.1/specvizitor/data/presets/spectral_lines.yml`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/io/catalog.py` & `specvizitor-0.4.1/specvizitor/io/catalog.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/io/inspection_data.py` & `specvizitor-0.4.1/specvizitor/io/inspection_data.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/io/viewer_data.py` & `specvizitor-0.4.1/specvizitor/io/viewer_data.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/main.py` & `specvizitor-0.4.1/specvizitor/main.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/plugins/plugin_core.py` & `specvizitor-0.4.1/specvizitor/plugins/plugin_core.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/plugins/sviz-eiger.py` & `specvizitor-0.4.1/specvizitor/plugins/sviz-eiger.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/plugins/sviz-grizli.py` & `specvizitor-0.4.1/specvizitor/plugins/sviz-grizli.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             scale = 1 / flat
         scale[scale == np.inf] = np.nan
 
         spec_1d._axes.y.unit = (t['flux'] * scale).unit
         spec_1d.update_axis_labels()
 
         # update the plot
-        for label in ('flux', 'err'):
+        for label in ('flux', 'err', 'model'):
             plot_data_item = spec_1d.plot_data_items.get(label)
             if plot_data_item is None:
                 continue
 
             x_data, _ = plot_data_item.getData()
 
             y_data = spec_1d.get_plot_data(spec_1d.cfg.plots[label].y)
```

### Comparing `specvizitor-0.4.0/specvizitor/utils/logs.py` & `specvizitor-0.4.1/specvizitor/utils/logs.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/params.py` & `specvizitor-0.4.1/specvizitor/utils/params.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/qt_tools.py` & `specvizitor-0.4.1/specvizitor/utils/qt_tools.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/widgets/AbstractWidget.py` & `specvizitor-0.4.1/specvizitor/utils/widgets/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/widgets/ColorBar.py` & `specvizitor-0.4.1/specvizitor/utils/widgets/ColorBar.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/widgets/FileBrowser.py` & `specvizitor-0.4.1/specvizitor/utils/widgets/FileBrowser.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/widgets/MyViewBox.py` & `specvizitor-0.4.1/specvizitor/utils/widgets/MyViewBox.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/utils/widgets/ParamTable.py` & `specvizitor-0.4.1/specvizitor/utils/widgets/ParamTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,15 @@
         self._table.setTextElideMode(QtCore.Qt.ElideLeft)
         self._table.horizontalHeader().setStretchLastSection(True)
         self._table.setHorizontalHeaderLabels(self._header)
 
         self._table.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self._table.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
         self._table.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self._table.setMinimumHeight(250)
 
         self._create_table_items()
         self._set_table_items()
 
         self._table.selectionModel().selectionChanged.connect(self.selection_changed_action)
 
         self._add_button.clicked.connect(self._add_row_dialog)
```

### Comparing `specvizitor-0.4.0/specvizitor/utils/widgets/Section.py` & `specvizitor-0.4.1/specvizitor/utils/widgets/Section.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/DataViewer.py` & `specvizitor-0.4.1/specvizitor/widgets/DataViewer.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/Image2D.py` & `specvizitor-0.4.1/specvizitor/widgets/Image2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         if self.has_defined_levels:
             limits_cfg = self.cfg.color_bar.limits
             if limits_cfg.type not in self.ALLOWED_CBAR_LIMS:
                 logger.error(f'Unknown type of colorbar limits: {limits_cfg}.'
                              f'Supported types: {self.ALLOWED_CBAR_LIMS}')
             else:
                 if limits_cfg.type == 'minmax':
-                    l1, l2 = np.nanmin(self.data), np.nanmin(self.data)
+                    l1, l2 = np.nanmin(self.data), np.nanmax(self.data)
                 elif limits_cfg.type == 'zscale':
                     l1, l2 = ZScaleInterval().get_limits(self.data)
                 else:
                     l1 = limits_cfg.min if limits_cfg.min is not None else np.nanmin(self.data)
                     l2 = limits_cfg.max if limits_cfg.max is not None else np.nanmax(self.data)
 
                 self.set_default_levels((l1, l2))
```

### Comparing `specvizitor-0.4.0/specvizitor/widgets/InspectionEditor.py` & `specvizitor-0.4.1/specvizitor/widgets/InspectionEditor.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/InspectionResults.py` & `specvizitor-0.4.1/specvizitor/widgets/InspectionResults.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from qtpy import QtCore, QtWidgets
 
 from ..config import config
 from ..io.inspection_data import InspectionData, REDSHIFT_FILL_VALUE
-from ..utils.widgets import AbstractWidget
+from ..utils.widgets import AbstractWidget, MyQTextEdit
 
 
 class InspectionResults(AbstractWidget):
     data_collected = QtCore.Signal(float, str, dict)
     edit_button_clicked = QtCore.Signal()
 
     def __init__(self, cfg: config.InspectionResults, parent=None):
@@ -16,22 +16,25 @@
 
         self._redshift_widget: QtWidgets.QLabel | None = None
         self._spacer: QtWidgets.QWidget | None = None
         self._clear_redshift: QtWidgets.QPushButton | None = None
         self._separator: QtWidgets.QFrame | None = None
 
         self._checkbox_widgets: dict[str, QtWidgets.QCheckBox] | None = None
-        self._comments_widget: QtWidgets.QTextEdit | None = None
+        self._comments_widget: MyQTextEdit | None = None
 
         self._edit_fields: QtWidgets.QPushButton | None = None
 
         super().__init__(parent=parent)
         self.setEnabled(False)
         self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
 
+        # add shortcuts
+        QtWidgets.QShortcut("E", self, self._comments_widget.setFocus)
+
     def _create_checkbox_widgets(self, review: InspectionData | None = None):
         if self._checkbox_widgets is not None:
             for w in self._checkbox_widgets.values():
                 w.deleteLater()
 
         flags = self.cfg.default_flags if review is None else review.flag_columns
 
@@ -53,15 +56,15 @@
         self._spacer.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
         self._clear_redshift = QtWidgets.QPushButton("Clear", self)
 
         self._separator = QtWidgets.QFrame(self)
         self._separator.setFrameShape(QtWidgets.QFrame.HLine)
 
         self._create_checkbox_widgets()
-        self._comments_widget = QtWidgets.QTextEdit(self)
+        self._comments_widget = MyQTextEdit(self)
         self._comments_widget.setPlaceholderText('Comment')
         self._comments_widget.setMinimumWidth(90)
 
         self._edit_fields = QtWidgets.QPushButton("Edit...", self)
         self._edit_fields.clicked.connect(self.edit_button_clicked.emit)
 
         self._clear_redshift.clicked.connect(self.clear_redshift_value)
```

### Comparing `specvizitor-0.4.0/specvizitor/widgets/MainWindow.py` & `specvizitor-0.4.1/specvizitor/widgets/MainWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         self._file.addAction(self._quit)
 
         self._view = self._menu.addMenu("&View")
 
         self._reset_view = QtWidgets.QAction("Reset View")
         self._reset_view.setEnabled(False)
         self._reset_view.triggered.connect(self._data_viewer.view_reset.emit)
-        self._reset_view.setShortcut('F5')
+        self._reset_view.setShortcut('R')
         self._view.addAction(self._reset_view)
 
         self._reset_dock_layout = QtWidgets.QAction("Reset Layout")
         self._reset_dock_layout.setEnabled(False)
         self._reset_dock_layout.triggered.connect(self._data_viewer.init_docks)
         self._view.addAction(self._reset_dock_layout)
 
@@ -219,15 +219,15 @@
         self._view.addAction(self._zen)
 
         self._view.addSeparator()
 
         self._fullscreen = QtWidgets.QAction("Fullscreen")
         self._fullscreen.triggered.connect(lambda:
                                            self._exit_fullscreen() if self.isFullScreen() else self._enter_fullscreen())
-        self._fullscreen.setShortcut('F11')
+        self._fullscreen.setShortcut('F')
         self._view.addAction(self._fullscreen)
 
         self._widgets = self._menu.addMenu("&Widgets")
 
         self._add_widget = QtWidgets.QAction("Add...")
         self._add_widget.setEnabled(False)
         self._widgets.addAction(self._add_widget)
```

### Comparing `specvizitor-0.4.0/specvizitor/widgets/NewFile.py` & `specvizitor-0.4.1/specvizitor/widgets/NewFile.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/ObjectInfo.py` & `specvizitor-0.4.1/specvizitor/widgets/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/Plot1D.py` & `specvizitor-0.4.1/specvizitor/widgets/Plot1D.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/QuickSearch.py` & `specvizitor-0.4.1/specvizitor/widgets/QuickSearch.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/Settings.py` & `specvizitor-0.4.1/specvizitor/widgets/Settings.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/SmartSlider.py` & `specvizitor-0.4.1/specvizitor/widgets/SmartSlider.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/Subsets.py` & `specvizitor-0.4.1/specvizitor/widgets/Subsets.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/TableColumns.py` & `specvizitor-0.4.1/specvizitor/widgets/TableColumns.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/specvizitor/widgets/ToolBar.py` & `specvizitor-0.4.1/specvizitor/widgets/ToolBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 
         # create a `screenshot` button
         self._screenshot_button = QtWidgets.QAction(self)
         self._screenshot_button.setToolTip('Take a screenshot')
 
         # create a `reset view` button
         self._reset_view_button = QtWidgets.QAction(self)
-        self._reset_view_button.setShortcut('R')
         self._reset_view_button.setToolTip('Reset the view')
 
         # create a `reset layout` button
         self._reset_layout_button = QtWidgets.QAction(self)
         self._reset_layout_button.setToolTip('Reset the layout')
 
         for b in self._viewer_connected_buttons:
```

### Comparing `specvizitor-0.4.0/specvizitor/widgets/ViewerElement.py` & `specvizitor-0.4.1/specvizitor/widgets/ViewerElement.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.4.0/PKG-INFO` & `specvizitor-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: specvizitor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python GUI application for a visual inspection of astronomical spectroscopic data
 Home-page: https://github.com/ivkram/specvizitor
 License: BSD-3-Clause
 Author: Ivan Kramarenko
 Author-email: im.kramarenko@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astropy (==6.0.0)
+Requires-Dist: astropy (>=6.0.0)
 Requires-Dist: dacite (==1.8.1)
 Requires-Dist: dictdiffer (==0.9.0)
-Requires-Dist: pandas (==2.2.0)
+Requires-Dist: pandas (>=2.2.0)
 Requires-Dist: pgcolorbar (==1.1.3)
-Requires-Dist: pillow (==10.2.0)
-Requires-Dist: platformdirs (==4.2.0)
+Requires-Dist: pillow (>=10.2.0)
+Requires-Dist: platformdirs (>=4.2.0)
 Requires-Dist: pyqt5 (==5.15.2)
 Requires-Dist: pyqtdarktheme (==2.1.0)
-Requires-Dist: pyqtgraph (==0.13.3)
+Requires-Dist: pyqtgraph (>=0.13.3)
 Requires-Dist: qtpy (==2.4.1)
-Requires-Dist: rasterio (==1.3.9)
-Requires-Dist: scipy (==1.12.0)
+Requires-Dist: rasterio (>=1.3.9)
+Requires-Dist: scipy (>=1.12.0)
 Project-URL: Repository, https://github.com/ivkram/specvizitor
 Description-Content-Type: text/markdown
 
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 Specvizitor is a Python GUI application for a visual inspection of astronomical spectroscopic data. The main goal is to provide a flexible tool for inspecting **large** and **homogeneous** spectroscopic samples of galaxies. This includes but not limited to [wide-field slitless spectroscopic (WFSS)](https://jwst-docs.stsci.edu/methods-and-roadmaps/jwst-wide-field-slitless-spectroscopy) data from the James Webb Space Telescope (JWST). Originally developed for the JWST Cycle 1 program "[FRESCO](https://jwst-fresco.astro.unige.ch)", this software can be easily adapted for a variety of spectroscopic data sets represented in standard data formats used in the astronomy community (FITS, ASCII, etc.).
```

