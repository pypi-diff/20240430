# Comparing `tmp/rtc-tools-2.6.1.tar.gz` & `tmp/rtc-tools-2.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-2.6.1.tar", last modified: Tue Mar  5 12:51:05 2024, max compression
+gzip compressed data, was "rtc-tools-2.7.0a1.tar", last modified: Tue Apr 30 07:11:19 2024, max compression
```

## Comparing `rtc-tools-2.6.1.tar` & `rtc-tools-2.7.0a1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.512678 rtc-tools-2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1182 2024-03-05 12:51:05.512678 rtc-tools-2.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4106 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-05 12:51:05.512678 rtc-tools-2.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2038 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.498679 rtc-tools-2.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.502679 rtc-tools-2.6.1/src/rtc_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-03-05 12:51:05.000000 rtc-tools-2.6.1/src/rtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2130 2024-03-05 12:51:05.000000 rtc-tools-2.6.1/src/rtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 12:51:05.000000 rtc-tools-2.6.1/src/rtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2024-03-05 12:51:05.000000 rtc-tools-2.6.1/src/rtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      164 2024-03-05 12:51:05.000000 rtc-tools-2.6.1/src/rtc_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-05 12:51:05.000000 rtc-tools-2.6.1/src/rtc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.512678 rtc-tools-2.6.1/src/rtctools/
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.504679 rtc-tools-2.6.1/src/rtctools/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/_internal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5310 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/_internal/alias_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/_internal/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/_internal/casadi_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/_internal/debug_check_helpers.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-03-05 12:51:05.512678 rtc-tools-2.6.1/src/rtctools/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.505679 rtc-tools-2.6.1/src/rtctools/data/
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5231 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.506679 rtc-tools-2.6.1/src/rtctools/data/interpolation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/interpolation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/interpolation/bspline.py
--rw-rw-rw-   0 root         (0) root         (0)     6106 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/interpolation/bspline1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1693 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/interpolation/bspline2d.py
--rw-rw-rw-   0 root         (0) root         (0)    19109 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/netcdf.py
--rw-rw-rw-   0 root         (0) root         (0)    45437 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/pi.py
--rw-rw-rw-   0 root         (0) root         (0)     9077 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/rtc.py
--rw-rw-rw-   0 root         (0) root         (0)    13206 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/data/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.510679 rtc-tools-2.6.1/src/rtctools/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   131343 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/collocated_integrated_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     8974 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/control_tree_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    17298 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/csv_lookup_table_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    12252 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    32999 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    43781 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/goal_programming_mixin_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6905 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/homotopy_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3116 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/initial_state_estimation_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11821 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/linearization_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     9087 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    14031 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/min_abs_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    17161 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/modelica_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7563 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/netcdf_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    44131 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)    11314 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/planning_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    25784 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/single_pass_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/optimization/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     4200 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/rtctoolsapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 12:51:05.511679 rtc-tools-2.6.1/src/rtctools/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6704 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/simulation/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     6209 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/simulation/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     9359 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/simulation/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    44556 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/simulation/simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     9075 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/src/rtctools/util.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2024-03-05 12:51:00.000000 rtc-tools-2.6.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.274591 rtc-tools-2.7.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-30 07:11:19.274591 rtc-tools-2.7.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4106 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-04-30 07:11:19.275591 rtc-tools-2.7.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.262591 rtc-tools-2.7.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.265591 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-30 07:11:19.000000 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-04-30 07:11:19.000000 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:11:19.000000 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-30 07:11:19.000000 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-30 07:11:19.000000 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-30 07:11:19.000000 rtc-tools-2.7.0a1/src/rtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.275591 rtc-tools-2.7.0a1/src/rtctools/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.267591 rtc-tools-2.7.0a1/src/rtctools/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/_internal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/_internal/alias_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/_internal/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/_internal/casadi_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/_internal/debug_check_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-30 07:11:19.275591 rtc-tools-2.7.0a1/src/rtctools/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.268591 rtc-tools-2.7.0a1/src/rtctools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.269591 rtc-tools-2.7.0a1/src/rtctools/data/interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/interpolation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/interpolation/bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/interpolation/bspline1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1693 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/interpolation/bspline2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    19109 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    45437 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/pi.py
+-rw-rw-rw-   0 root         (0) root         (0)     9077 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/rtc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13206 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/data/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.273591 rtc-tools-2.7.0a1/src/rtctools/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   131343 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/collocated_integrated_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     8974 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/control_tree_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    17298 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/csv_lookup_table_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    12252 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    32999 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    43781 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/goal_programming_mixin_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6905 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/homotopy_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/initial_state_estimation_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11821 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/linearization_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9087 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    14031 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/min_abs_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    17769 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/modelica_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7563 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/netcdf_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    44131 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)    11786 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/planning_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    25784 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/single_pass_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/optimization/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/rtctoolsapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:11:19.274591 rtc-tools-2.7.0a1/src/rtctools/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6704 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/simulation/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6209 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/simulation/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9831 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/simulation/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    48541 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/simulation/simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     9075 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/src/rtctools/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2024-04-30 07:11:14.000000 rtc-tools-2.7.0a1/versioneer.py
```

### Comparing `rtc-tools-2.6.1/COPYING.LESSER` & `rtc-tools-2.7.0a1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/PKG-INFO` & `rtc-tools-2.7.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.6.1
+Version: 2.7.0a1
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.6.1/README.md` & `rtc-tools-2.7.0a1/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/setup.py` & `rtc-tools-2.7.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtc_tools.egg-info/PKG-INFO` & `rtc-tools-2.7.0a1/src/rtc_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.6.1
+Version: 2.7.0a1
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.6.1/src/rtc_tools.egg-info/SOURCES.txt` & `rtc-tools-2.7.0a1/src/rtc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/_internal/alias_tools.py` & `rtc-tools-2.7.0a1/src/rtctools/_internal/alias_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/_internal/caching.py` & `rtc-tools-2.7.0a1/src/rtctools/_internal/caching.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/_internal/casadi_helpers.py` & `rtc-tools-2.7.0a1/src/rtctools/_internal/casadi_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/_internal/debug_check_helpers.py` & `rtc-tools-2.7.0a1/src/rtctools/_internal/debug_check_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/csv.py` & `rtc-tools-2.7.0a1/src/rtctools/data/csv.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/interpolation/bspline.py` & `rtc-tools-2.7.0a1/src/rtctools/data/interpolation/bspline.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/interpolation/bspline1d.py` & `rtc-tools-2.7.0a1/src/rtctools/data/interpolation/bspline1d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/interpolation/bspline2d.py` & `rtc-tools-2.7.0a1/src/rtctools/data/interpolation/bspline2d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/netcdf.py` & `rtc-tools-2.7.0a1/src/rtctools/data/netcdf.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/pi.py` & `rtc-tools-2.7.0a1/src/rtctools/data/pi.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/rtc.py` & `rtc-tools-2.7.0a1/src/rtctools/data/rtc.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/data/storage.py` & `rtc-tools-2.7.0a1/src/rtctools/data/storage.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/collocated_integrated_optimization_problem.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/collocated_integrated_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/control_tree_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/control_tree_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/csv_lookup_table_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/csv_lookup_table_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/csv_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/goal_programming_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/goal_programming_mixin_base.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/goal_programming_mixin_base.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/homotopy_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/homotopy_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/initial_state_estimation_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/initial_state_estimation_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/io_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/linearization_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/linearization_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/linearized_order_goal_programming_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/linearized_order_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/min_abs_goal_programming_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/min_abs_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/modelica_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/modelica_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,29 @@
             model_name = kwargs["model_name"]
         else:
             if hasattr(self, "model_name"):
                 model_name = self.model_name
             else:
                 model_name = self.__class__.__name__
 
-        self.__pymoca_model = pymoca.backends.casadi.api.transfer_model(
-            kwargs["model_folder"], model_name, self.compiler_options()
-        )
+        compiler_options = self.compiler_options()
+        logger.info(f"Loading/compiling model {model_name}.")
+        try:
+            self.__pymoca_model = pymoca.backends.casadi.api.transfer_model(
+                kwargs["model_folder"], model_name, compiler_options
+            )
+        except RuntimeError as error:
+            if compiler_options.get("cache", False):
+                raise error
+            compiler_options["cache"] = False
+            logger.warning(f"Loading model {model_name} using a cache file failed: {error}.")
+            logger.info(f"Compiling model {model_name}.")
+            self.__pymoca_model = pymoca.backends.casadi.api.transfer_model(
+                kwargs["model_folder"], model_name, compiler_options
+            )
 
         # Extract the CasADi MX variables used in the model
         self.__mx = {}
         self.__mx["time"] = [self.__pymoca_model.time]
         self.__mx["states"] = [v.symbol for v in self.__pymoca_model.states]
         self.__mx["derivatives"] = [v.symbol for v in self.__pymoca_model.der_states]
         self.__mx["algebraics"] = [v.symbol for v in self.__pymoca_model.alg_states]
```

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/netcdf_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/netcdf_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/optimization_problem.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/pi_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/pi_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -273,7 +273,20 @@
 
     @property
     def timeseries_export(self):
         """
         :class:`pi.Timeseries` object for holding the output data.
         """
         return self.__timeseries_export
+
+    def set_unit(self, variable: str, unit: str):
+        """
+        Set the unit of a time series.
+
+        :param variable:        Time series ID.
+        :param unit:            Unit.
+        """
+        assert hasattr(
+            self, "_PIMixin__timeseries_import"
+        ), "set_unit can only be called after read() in pre() has finished."
+        self.__timeseries_import.set_unit(variable, unit, 0)
+        self.__timeseries_export.set_unit(variable, unit, 0)
```

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/planning_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/planning_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/single_pass_goal_programming_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/single_pass_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/optimization/timeseries.py` & `rtc-tools-2.7.0a1/src/rtctools/optimization/timeseries.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/rtctoolsapp.py` & `rtc-tools-2.7.0a1/src/rtctools/rtctoolsapp.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/simulation/csv_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/simulation/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/simulation/io_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/simulation/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/src/rtctools/simulation/pi_mixin.py` & `rtc-tools-2.7.0a1/src/rtctools/simulation/pi_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -236,7 +236,20 @@
 
         self.__timeseries_import.set(variable, values, unit=unit)
         self.io.set_timeseries(variable, self.io.datetimes, values)
 
     def get_timeseries(self, variable):
         _, values = self.io.get_timeseries(variable)
         return values
+
+    def set_unit(self, variable: str, unit: str):
+        """
+        Set the unit of a time series.
+
+        :param variable:        Time series ID.
+        :param unit:            Unit.
+        """
+        assert hasattr(
+            self, "_PIMixin__timeseries_import"
+        ), "set_unit can only be called after read() in pre() has finished."
+        self.__timeseries_import.set_unit(variable, unit, 0)
+        self.__timeseries_export.set_unit(variable, unit, 0)
```

### Comparing `rtc-tools-2.6.1/src/rtctools/simulation/simulation_problem.py` & `rtc-tools-2.7.0a1/src/rtctools/simulation/simulation_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,29 @@
         else:
             if hasattr(self, "model_name"):
                 model_name = self.model_name
             else:
                 model_name = self.__class__.__name__
 
         # Load model from pymoca backend
-        self.__pymoca_model = pymoca.backends.casadi.api.transfer_model(
-            kwargs["model_folder"], model_name, self.compiler_options()
-        )
+        compiler_options = self.compiler_options()
+        logger.info(f"Loading/compiling model {model_name}.")
+        try:
+            self.__pymoca_model = pymoca.backends.casadi.api.transfer_model(
+                kwargs["model_folder"], model_name, compiler_options
+            )
+        except RuntimeError as error:
+            if compiler_options.get("cache", False):
+                raise error
+            compiler_options["cache"] = False
+            logger.warning(f"Loading model {model_name} using a cache file failed: {error}.")
+            logger.info(f"Compiling model {model_name}.")
+            self.__pymoca_model = pymoca.backends.casadi.api.transfer_model(
+                kwargs["model_folder"], model_name, compiler_options
+            )
 
         # Extract the CasADi MX variables used in the model
         self.__mx = {}
         self.__mx["time"] = [self.__pymoca_model.time]
         self.__mx["states"] = [v.symbol for v in self.__pymoca_model.states]
         self.__mx["derivatives"] = [v.symbol for v in self.__pymoca_model.der_states]
         self.__mx["algebraics"] = [v.symbol for v in self.__pymoca_model.alg_states]
@@ -315,14 +327,25 @@
             delay_expression_states.append(expression_symbol)
         return delay_expression_states
 
     def initialize(self, config_file=None):
         """
         Initialize state vector with default values
 
+        Initial values are first read from the given Modelica files.
+        If an initial value equals zero or is not provided by a Modelica file,
+        and the variable is not marked as fixed,
+        then the initial value is tried to be set with the initial_state method.
+        When using CSVMixin, this method by default looks for initial values
+        in an initial_state.csv file.
+        Furthermore, if a variable is not marked as fixed
+        and no initial value is given by the initial_state method,
+        the initial value can be overwritten using the seed method.
+        When a variable is marked as fixed, the initial value is only read from the Modelica file.
+
         :param config_file: Path to an initialization file.
         """
         if config_file:
             # TODO read start and stop time from config_file and call:
             # self.setup_experiment(start,stop)
             # for now, assume that setup_experiment was called beforehand
             raise NotImplementedError
@@ -389,76 +412,121 @@
         )
 
         # Assemble initial residuals and set values from start attributes into the state vector
         minimized_residuals = []
         for var in itertools.chain(self.__pymoca_model.states, self.__pymoca_model.alg_states):
             var_name = var.symbol.name()
             var_nominal = self.get_variable_nominal(var_name)
+            start_values = {}
 
             # Attempt to cast var.start to python type
+            start_value_is_symbolic = False
             mx_start = ca.MX(var.start)
             if mx_start.is_constant():
                 # cast var.start to python type
-                start_val = var.python_type(mx_start.to_DM())
+                start_value_pymoca = var.python_type(mx_start.to_DM())
+                if start_value_pymoca is not None and start_value_pymoca != 0:
+                    start_values["modelica"] = start_value_pymoca
             else:
-                # var.start is a symbolic expression with unknown value
-                start_val = None
+                start_value_is_symbolic = True
+                start_values["modelica"] = mx_start
 
-            if start_val == 0.0 and not var.fixed:
+            if not var.fixed:
                 # To make initialization easier, we allow setting initial states by providing
                 # timeseries with names that match a symbol in the model. We only check for this
                 # matching if the start and fixed attributes were left as default
                 try:
-                    start_val = self.initial_state()[var_name]
+                    start_values["initial_state"] = self.initial_state()[var_name]
                 except KeyError:
                     pass
                 else:
                     # An initial state was found- add it to the constrained residuals
                     logger.debug(
                         "Initialize: Added {} = {} to initial equations "
-                        "(found matching timeseries).".format(var_name, start_val)
+                        "(found matching timeseries).".format(
+                            var_name, start_values["initial_state"]
+                        )
                     )
                     # Set var to be fixed
                     var.fixed = True
 
             if not var.fixed:
                 # To make initialization easier, we allow setting initial guesses by providing
                 # timeseries with names that match a symbol in the model. We only check for this
                 # matching if the start and fixed attributes were left as default
                 try:
-                    start_val = self.seed()[var_name]
+                    start_values["seed"] = self.seed()[var_name]
                 except KeyError:
                     pass
                 else:
                     # An initial state was found- add it to the constrained residuals
                     logger.debug(
                         "Initialize: Added {} = {} as initial guess "
-                        "(found matching timeseries).".format(var_name, start_val)
+                        "(found matching timeseries).".format(var_name, start_values["seed"])
                     )
 
+            # Set the start value based on the different inputs.
+            if "seed" in start_values:
+                input_source = "seed"
+                source_description = "seed method"
+            elif "modelica" in start_values:
+                input_source = "modelica"
+                source_description = "modelica file"
+            elif "initial_state" in start_values:
+                input_source = "initial_state"
+                source_description = "initial_state method (typically reads initial_state.csv)"
+            else:
+                start_values["modelica"] = start_value_pymoca
+                input_source = "modelica"
+                source_description = "modelica file or default value"
+            start_val = start_values.get(input_source, None)
+            is_numeric = start_val is not None and not start_value_is_symbolic
+            numeric_start_val = start_val if is_numeric else 0.0
+            if len(start_values) > 1:
+                logger.warning(
+                    "Initialize: Multiple initial values for {} are provided: {}.".format(
+                        var_name, start_values
+                    )
+                    + " Value from {} will be used to continue.".format(source_description)
+                )
+
             # Attempt to set start_val in the state vector. Default to zero if unknown.
             try:
-                self.set_var(var_name, start_val if start_val is not None else 0.0)
+                self.set_var(var_name, numeric_start_val)
             except KeyError:
                 logger.warning(
                     "Initialize: {} not found in state vector. "
-                    "Initial value of {} not set.".format(var_name, start_val)
+                    "Initial value of {} not set.".format(var_name, numeric_start_val)
                 )
 
             # Add a residual for the difference between the state and its starting expression
-            start_expr = start_val if start_val is not None else var.start
+            start_expr = start_val
             if var.fixed:
                 # Set bounds to be equal to each other, such that IPOPT can
                 # turn the decision variable into a parameter.
+                if var.min != -np.inf or var.max != np.inf:
+                    logger.info(
+                        "Initialize: bounds of {} will be overwritten".format(var_name)
+                        + " by the start value given by {}.".format(source_description)
+                    )
                 var.min = start_expr
                 var.max = start_expr
             else:
                 # minimize residual
                 minimized_residuals.append((var.symbol - start_expr) / var_nominal)
 
+            # Check that the start_value is in between the variable bounds.
+            if start_val is not None and is_numeric:
+                if not (var.min <= start_val and start_val <= var.max):
+                    logger.warning(
+                        "Initialize: start value {} = {}".format(var_name, start_val)
+                        + " is not in between bounds {} and {}".format(var.min, var.max)
+                        + " and will be adjusted."
+                    )
+
         # Default start var for ders is zero
         for der_var in self.__mx["derivatives"]:
             self.set_var(der_var.name(), 0.0)
 
         # Residuals for initial values for the delay states / expressions.
         for delay_state, delay_argument in zip(model.delay_states, model.delay_arguments):
             expression_state = delay_state + "_expr"
@@ -606,15 +674,23 @@
 
         # Find initial state
         initial_state = solver(x0=guess, lbx=self.__lbx, ubx=self.__ubx, lbg=lbg, ubg=ubg)
 
         # If unsuccessful, stop.
         return_status = solver.stats()["return_status"]
         if return_status not in {"Solve_Succeeded", "Solved_To_Acceptable_Level"}:
-            raise Exception('Initialization Failed with return status "{}"'.format(return_status))
+            if return_status == "Infeasible_Problem_Detected":
+                message = (
+                    "Initialization Failed with return status: {}. ".format(return_status)
+                    + "This means no initial state could be found "
+                    + "that satisfies all equations and constraints."
+                )
+            else:
+                message = "Initialization Failed with return status: {}. ".format(return_status)
+            raise Exception(message)
 
         # Update state vector with initial conditions
         self.__state_vector[: self.__n_states] = initial_state["x"][: self.__n_states].T
 
         # make a copy of the initialized initial state vector in case we want to run the model again
         self.__initialized_state_vector = copy.deepcopy(self.__state_vector)
```

### Comparing `rtc-tools-2.6.1/src/rtctools/util.py` & `rtc-tools-2.7.0a1/src/rtctools/util.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.6.1/versioneer.py` & `rtc-tools-2.7.0a1/versioneer.py`

 * *Files identical despite different names*

