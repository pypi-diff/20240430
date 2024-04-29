# Comparing `tmp/pyufunc-0.2.5.tar.gz` & `tmp/pyufunc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyufunc-0.2.5.tar", last modified: Sat Mar 30 22:40:10 2024, max compression
+gzip compressed data, was "pyufunc-0.2.6.tar", last modified: Mon Apr 29 23:52:33 2024, max compression
```

## Comparing `pyufunc-0.2.5.tar` & `pyufunc-0.2.6.tar`

### file list

```diff
@@ -1,108 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.230758 pyufunc-0.2.5/
--rw-rw-rw-   0        0        0     1085 2024-02-29 19:16:47.000000 pyufunc-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     7404 2024-03-30 22:40:10.229389 pyufunc-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6142 2024-03-30 18:56:09.000000 pyufunc-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.034491 pyufunc-0.2.5/pyufunc/
--rw-rw-rw-   0        0        0     7579 2024-03-30 18:56:36.000000 pyufunc-0.2.5/pyufunc/__init__.py
--rw-rw-rw-   0        0        0     3907 2024-03-30 22:39:18.000000 pyufunc-0.2.5/pyufunc/pkg_configs.py
--rw-rw-rw-   0        0        0    19242 2024-03-30 22:31:23.000000 pyufunc-0.2.5/pyufunc/pkg_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.071642 pyufunc-0.2.5/pyufunc/util_ai/
--rw-rw-rw-   0        0        0      288 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_ai/__init__.py
--rw-rw-rw-   0        0        0      281 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_ai/_open_cv.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_ai/_pytorch.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_ai/_scikitlearn.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_ai/_scipy.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_ai/_tensorflow.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.087271 pyufunc-0.2.5/pyufunc/util_common/
--rw-rw-rw-   0        0        0      704 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_common/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_common/_google_numpy_docstring.py
--rw-rw-rw-   0        0        0     2910 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_common/_password_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.105833 pyufunc-0.2.5/pyufunc/util_data_processing/
--rw-rw-rw-   0        0        0      570 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_data_processing/__init__.py
--rw-rw-rw-   0        0        0      965 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_data_processing/_common.py
--rw-rw-rw-   0        0        0      281 2024-03-13 08:40:41.000000 pyufunc-0.2.5/pyufunc/util_data_processing/_data_cleaning.py
--rw-rw-rw-   0        0        0     1541 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_data_processing/_dict.py
--rw-rw-rw-   0        0        0     3263 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_data_processing/_list.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_data_processing/_str.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.108878 pyufunc-0.2.5/pyufunc/util_datetime/
--rw-rw-rw-   0        0        0      881 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_datetime/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-03-13 08:35:33.000000 pyufunc-0.2.5/pyufunc/util_datetime/_dt_format.py
--rw-rw-rw-   0        0        0    13578 2024-03-30 22:08:01.000000 pyufunc-0.2.5/pyufunc/util_datetime/_dt_group.py
--rw-rw-rw-   0        0        0     3986 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_datetime/_dt_time_difference.py
--rw-rw-rw-   0        0        0     2919 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_datetime/_dt_timezone.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.124508 pyufunc-0.2.5/pyufunc/util_fullstack/
--rw-rw-rw-   0        0        0      288 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_fullstack/__init__.py
--rw-rw-rw-   0        0        0      280 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_fullstack/_database.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_fullstack/_django.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_fullstack/_django_restapi.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_fullstack/_fastapi.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_fullstack/_flask.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.142060 pyufunc-0.2.5/pyufunc/util_geo/
--rw-rw-rw-   0        0        0     1054 2024-03-02 22:46:11.000000 pyufunc-0.2.5/pyufunc/util_geo/__init__.py
--rw-rw-rw-   0        0        0      281 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_geo/_geo_area.py
--rw-rw-rw-   0        0        0     6902 2024-03-30 22:01:15.000000 pyufunc-0.2.5/pyufunc/util_geo/_geo_circle.py
--rw-rw-rw-   0        0        0      283 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_geo/_geo_common.py
--rw-rw-rw-   0        0        0    14474 2024-03-30 22:05:08.000000 pyufunc-0.2.5/pyufunc/util_geo/_geo_distance.py
--rw-rw-rw-   0        0        0     6828 2024-03-03 04:39:49.000000 pyufunc-0.2.5/pyufunc/util_geo/_gmns.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.144135 pyufunc-0.2.5/pyufunc/util_git_pypi/
--rw-rw-rw-   0        0        0      178 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_git_pypi/__init__.py
--rw-rw-rw-   0        0        0    26454 2024-03-03 06:19:17.000000 pyufunc-0.2.5/pyufunc/util_git_pypi/_github.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_git_pypi/_gitlab.py
--rw-rw-rw-   0        0        0     2368 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_git_pypi/_pypi.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.144135 pyufunc-0.2.5/pyufunc/util_git_pypi/static/
--rw-rw-rw-   0        0        0      281 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_git_pypi/static/__init__.py
--rw-rw-rw-   0        0        0   483581 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_git_pypi/static/user-agent-strings.json
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.144135 pyufunc-0.2.5/pyufunc/util_gui/
--rw-rw-rw-   0        0        0      292 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.163088 pyufunc-0.2.5/pyufunc/util_img/
--rw-rw-rw-   0        0        0      930 2024-03-29 23:58:07.000000 pyufunc-0.2.5/pyufunc/util_img/__init__.py
--rw-rw-rw-   0        0        0     2414 2024-03-29 20:39:50.000000 pyufunc-0.2.5/pyufunc/util_img/_img_cvt.py
--rw-rw-rw-   0        0        0    17095 2024-03-30 22:19:27.000000 pyufunc-0.2.5/pyufunc/util_img/_img_operate.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.174872 pyufunc-0.2.5/pyufunc/util_log/
--rw-rw-rw-   0        0        0      288 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_log/__init__.py
--rw-rw-rw-   0        0        0     2296 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_log/log.txt
--rw-rw-rw-   0        0        0     1907 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_log/log_config.py
--rw-rw-rw-   0        0        0    25658 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_log/loga.py
--rw-rw-rw-   0        0        0     8529 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_log/logutils.py
--rw-rw-rw-   0        0        0     2749 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_log/te.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.174872 pyufunc-0.2.5/pyufunc/util_network/
--rw-rw-rw-   0        0        0      366 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_network/__init__.py
--rw-rw-rw-   0        0        0      839 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_network/_network.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.174872 pyufunc-0.2.5/pyufunc/util_office/
--rw-rw-rw-   0        0        0      379 2024-03-13 03:39:04.000000 pyufunc-0.2.5/pyufunc/util_office/__init__.py
--rw-rw-rw-   0        0        0     8546 2024-03-13 04:02:55.000000 pyufunc-0.2.5/pyufunc/util_office/_email.py
--rw-rw-rw-   0        0        0      323 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_office/_pdf.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_office/_printer.py
--rw-rw-rw-   0        0        0      305 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_office/_word.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.198456 pyufunc-0.2.5/pyufunc/util_optimization/
--rw-rw-rw-   0        0        0      288 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_optimization/__init__.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_optimization/_cplex.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_optimization/_cvxpy.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_optimization/_gurobi.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_optimization/_pyomo.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.207749 pyufunc-0.2.5/pyufunc/util_pathio/
--rw-rw-rw-   0        0        0     1317 2024-03-29 20:25:29.000000 pyufunc-0.2.5/pyufunc/util_pathio/__init__.py
--rw-rw-rw-   0        0        0      309 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_pathio/_argparse.py
--rw-rw-rw-   0        0        0     7449 2024-03-29 20:23:22.000000 pyufunc-0.2.5/pyufunc/util_pathio/_io.py
--rw-rw-rw-   0        0        0     8024 2024-03-29 19:49:39.000000 pyufunc-0.2.5/pyufunc/util_pathio/_path.py
--rw-rw-rw-   0        0        0     1896 2024-03-30 22:17:39.000000 pyufunc-0.2.5/pyufunc/util_pathio/_platform.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.207749 pyufunc-0.2.5/pyufunc/util_test/
--rw-rw-rw-   0        0        0      288 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_test/__init__.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_test/_pytest.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_test/_unittest.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.207749 pyufunc-0.2.5/pyufunc/util_vis/
--rw-rw-rw-   0        0        0      288 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_vis/__init__.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_vis/bivis.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_vis/matplotlib.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_vis/plotly.py
--rw-rw-rw-   0        0        0      276 2024-02-29 19:16:47.000000 pyufunc-0.2.5/pyufunc/util_vis/pyecharts.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.071642 pyufunc-0.2.5/pyufunc.egg-info/
--rw-rw-rw-   0        0        0     7404 2024-03-30 22:40:09.000000 pyufunc-0.2.5/pyufunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2676 2024-03-30 22:40:09.000000 pyufunc-0.2.5/pyufunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 22:40:09.000000 pyufunc-0.2.5/pyufunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-30 22:40:09.000000 pyufunc-0.2.5/pyufunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 22:40:10.230758 pyufunc-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2493 2024-02-29 19:16:47.000000 pyufunc-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:40:10.223370 pyufunc-0.2.5/tests/
--rw-rw-rw-   0        0        0     2948 2024-02-29 19:16:47.000000 pyufunc-0.2.5/tests/test_dp_list.py
--rw-rw-rw-   0        0        0     3186 2024-02-29 19:16:47.000000 pyufunc-0.2.5/tests/test_pathio_io.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.077571 pyufunc-0.2.6/
+-rw-rw-rw-   0        0        0     1085 2024-02-29 19:16:48.000000 pyufunc-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     7599 2024-04-29 23:52:33.077571 pyufunc-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6337 2024-04-18 17:27:13.000000 pyufunc-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:32.971207 pyufunc-0.2.6/pyufunc/
+-rw-rw-rw-   0        0        0     8255 2024-04-22 23:47:24.000000 pyufunc-0.2.6/pyufunc/__init__.py
+-rw-rw-rw-   0        0        0     4460 2024-04-29 23:52:22.000000 pyufunc-0.2.6/pyufunc/pkg_configs.py
+-rw-rw-rw-   0        0        0    21148 2024-04-21 17:52:09.000000 pyufunc-0.2.6/pyufunc/pkg_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.010098 pyufunc-0.2.6/pyufunc/util_ai/
+-rw-rw-rw-   0        0        0      944 2024-04-12 19:27:45.000000 pyufunc-0.2.6/pyufunc/util_ai/__init__.py
+-rw-rw-rw-   0        0        0     7948 2024-04-12 19:27:45.000000 pyufunc-0.2.6/pyufunc/util_ai/_error_measurement.py
+-rw-rw-rw-   0        0        0      281 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_ai/_open_cv.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_ai/_pytorch.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_ai/_scikitlearn.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_ai/_scipy.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_ai/_tensorflow.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.012719 pyufunc-0.2.6/pyufunc/util_algorithm/
+-rw-rw-rw-   0        0        0      571 2024-04-12 20:38:51.000000 pyufunc-0.2.6/pyufunc/util_algorithm/__init__.py
+-rw-rw-rw-   0        0        0     9957 2024-04-12 23:17:02.000000 pyufunc-0.2.6/pyufunc/util_algorithm/_sort.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.012719 pyufunc-0.2.6/pyufunc/util_common/
+-rw-rw-rw-   0        0        0      704 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_common/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_common/_google_numpy_docstring.py
+-rw-rw-rw-   0        0        0     2910 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_common/_password_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.012719 pyufunc-0.2.6/pyufunc/util_data_processing/
+-rw-rw-rw-   0        0        0      570 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_data_processing/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_data_processing/_common.py
+-rw-rw-rw-   0        0        0      281 2024-03-13 08:40:42.000000 pyufunc-0.2.6/pyufunc/util_data_processing/_data_cleaning.py
+-rw-rw-rw-   0        0        0     1541 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_data_processing/_dict.py
+-rw-rw-rw-   0        0        0     3263 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_data_processing/_list.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_data_processing/_str.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.012719 pyufunc-0.2.6/pyufunc/util_datetime/
+-rw-rw-rw-   0        0        0      881 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_datetime/__init__.py
+-rw-rw-rw-   0        0        0     1831 2024-04-22 23:51:11.000000 pyufunc-0.2.6/pyufunc/util_datetime/_dt_format.py
+-rw-rw-rw-   0        0        0    13578 2024-03-30 22:08:02.000000 pyufunc-0.2.6/pyufunc/util_datetime/_dt_group.py
+-rw-rw-rw-   0        0        0     3986 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_datetime/_dt_time_difference.py
+-rw-rw-rw-   0        0        0     2919 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_datetime/_dt_timezone.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.025101 pyufunc-0.2.6/pyufunc/util_fullstack/
+-rw-rw-rw-   0        0        0      288 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_fullstack/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_fullstack/_database.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_fullstack/_django.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_fullstack/_django_restapi.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_fullstack/_fastapi.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_fullstack/_flask.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.032454 pyufunc-0.2.6/pyufunc/util_geo/
+-rw-rw-rw-   0        0        0     1891 2024-04-22 23:31:29.000000 pyufunc-0.2.6/pyufunc/util_geo/__init__.py
+-rw-rw-rw-   0        0        0    13937 2024-04-14 22:33:48.000000 pyufunc-0.2.6/pyufunc/util_geo/_coordinate_coversion.py
+-rw-rw-rw-   0        0        0      281 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_geo/_geo_area.py
+-rw-rw-rw-   0        0        0     6902 2024-03-30 22:01:16.000000 pyufunc-0.2.6/pyufunc/util_geo/_geo_circle.py
+-rw-rw-rw-   0        0        0      283 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_geo/_geo_common.py
+-rw-rw-rw-   0        0        0    14474 2024-03-30 22:05:10.000000 pyufunc-0.2.6/pyufunc/util_geo/_geo_distance.py
+-rw-rw-rw-   0        0        0     8087 2024-04-23 00:01:58.000000 pyufunc-0.2.6/pyufunc/util_geo/_gmns.py
+-rw-rw-rw-   0        0        0      309 2024-04-23 00:02:35.000000 pyufunc-0.2.6/pyufunc/util_geo/_gmns_load.py
+-rw-rw-rw-   0        0        0     2171 2024-04-12 21:02:27.000000 pyufunc-0.2.6/pyufunc/util_geo/_shortest_path.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.032454 pyufunc-0.2.6/pyufunc/util_git_pypi/
+-rw-rw-rw-   0        0        0      178 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_git_pypi/__init__.py
+-rw-rw-rw-   0        0        0    26454 2024-03-03 06:19:18.000000 pyufunc-0.2.6/pyufunc/util_git_pypi/_github.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_git_pypi/_gitlab.py
+-rw-rw-rw-   0        0        0     2368 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_git_pypi/_pypi.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.032454 pyufunc-0.2.6/pyufunc/util_git_pypi/static/
+-rw-rw-rw-   0        0        0      281 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_git_pypi/static/__init__.py
+-rw-rw-rw-   0        0        0   483581 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_git_pypi/static/user-agent-strings.json
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.032454 pyufunc-0.2.6/pyufunc/util_gui/
+-rw-rw-rw-   0        0        0      292 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.032454 pyufunc-0.2.6/pyufunc/util_img/
+-rw-rw-rw-   0        0        0      883 2024-04-14 22:37:23.000000 pyufunc-0.2.6/pyufunc/util_img/__init__.py
+-rw-rw-rw-   0        0        0     2398 2024-04-14 22:36:08.000000 pyufunc-0.2.6/pyufunc/util_img/_img_cvt.py
+-rw-rw-rw-   0        0        0    17063 2024-04-15 00:20:59.000000 pyufunc-0.2.6/pyufunc/util_img/_img_operate.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.059043 pyufunc-0.2.6/pyufunc/util_log/
+-rw-rw-rw-   0        0        0      288 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_log/__init__.py
+-rw-rw-rw-   0        0        0     2296 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_log/log.txt
+-rw-rw-rw-   0        0        0     1907 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_log/log_config.py
+-rw-rw-rw-   0        0        0    25658 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_log/loga.py
+-rw-rw-rw-   0        0        0     8529 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_log/logutils.py
+-rw-rw-rw-   0        0        0     2749 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_log/te.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.061697 pyufunc-0.2.6/pyufunc/util_network/
+-rw-rw-rw-   0        0        0      366 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_network/__init__.py
+-rw-rw-rw-   0        0        0      839 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_network/_network.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.064695 pyufunc-0.2.6/pyufunc/util_office/
+-rw-rw-rw-   0        0        0      379 2024-03-13 03:39:06.000000 pyufunc-0.2.6/pyufunc/util_office/__init__.py
+-rw-rw-rw-   0        0        0     8546 2024-04-22 23:48:23.000000 pyufunc-0.2.6/pyufunc/util_office/_email.py
+-rw-rw-rw-   0        0        0      323 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_office/_pdf.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_office/_printer.py
+-rw-rw-rw-   0        0        0      305 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_office/_word.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.066747 pyufunc-0.2.6/pyufunc/util_optimization/
+-rw-rw-rw-   0        0        0      288 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_optimization/__init__.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_optimization/_cplex.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_optimization/_cvxpy.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_optimization/_gurobi.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_optimization/_pyomo.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.066747 pyufunc-0.2.6/pyufunc/util_pathio/
+-rw-rw-rw-   0        0        0     1311 2024-04-21 16:13:47.000000 pyufunc-0.2.6/pyufunc/util_pathio/__init__.py
+-rw-rw-rw-   0        0        0      309 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_pathio/_argparse.py
+-rw-rw-rw-   0        0        0     7449 2024-03-29 20:23:24.000000 pyufunc-0.2.6/pyufunc/util_pathio/_io.py
+-rw-rw-rw-   0        0        0     8021 2024-04-21 16:05:29.000000 pyufunc-0.2.6/pyufunc/util_pathio/_path.py
+-rw-rw-rw-   0        0        0     1896 2024-03-30 22:17:40.000000 pyufunc-0.2.6/pyufunc/util_pathio/_platform.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.077571 pyufunc-0.2.6/pyufunc/util_test/
+-rw-rw-rw-   0        0        0      288 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_test/__init__.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_test/_pytest.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_test/_unittest.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.077571 pyufunc-0.2.6/pyufunc/util_vis/
+-rw-rw-rw-   0        0        0      288 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_vis/__init__.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_vis/bivis.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_vis/matplotlib.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_vis/plotly.py
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:16:48.000000 pyufunc-0.2.6/pyufunc/util_vis/pyecharts.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:32.998379 pyufunc-0.2.6/pyufunc.egg-info/
+-rw-rw-rw-   0        0        0     7599 2024-04-29 23:52:32.000000 pyufunc-0.2.6/pyufunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2889 2024-04-29 23:52:32.000000 pyufunc-0.2.6/pyufunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 23:52:32.000000 pyufunc-0.2.6/pyufunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 23:52:32.000000 pyufunc-0.2.6/pyufunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 23:52:33.077571 pyufunc-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2493 2024-02-29 19:16:48.000000 pyufunc-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 23:52:33.077571 pyufunc-0.2.6/tests/
+-rw-rw-rw-   0        0        0     2948 2024-02-29 19:16:48.000000 pyufunc-0.2.6/tests/test_dp_list.py
+-rw-rw-rw-   0        0        0     3186 2024-02-29 19:16:48.000000 pyufunc-0.2.6/tests/test_pathio_io.py
```

### Comparing `pyufunc-0.2.5/LICENSE` & `pyufunc-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/PKG-INFO` & `pyufunc-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyufunc
-Version: 0.2.5
+Version: 0.2.6
 Summary: PyUFunc consolidates frequently used utility functions from various libraries into one cohesive package
 Home-page: https://github.com/xyluo25/pyufunc
 Author: Mr. Xiangyong Luo, Dr. Xuesong Simon Zhou
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 License: MIT License
 Project-URL: Homepage, https://github.com/xyluo25/pyufunc
 Project-URL: Bug Tracker, https://github.com/xyluo25/pyufunc/issues
@@ -39,15 +39,15 @@
 2. **Modularity and Extensibility:** pyufunc is structured with modularity in mind. Each utility function is a standalone entity, allowing you to cherry-pick the ones you need without introducing unnecessary dependencies. Furthermore, the package is designed to be extensible, making it effortless to contribute your own utility functions and enrich the community.
 3. **Robust Collection of Utility Functions:** pyufunc offers a versatile assortment of utility functions, carefully crafted and thoroughly tested to meet industry standards. The package covers diverse domains, including data manipulation, file handling, string operations, mathematical functions, and much more.
 4. **Regular Updates and Maintenance:** Our team is dedicated to providing regular updates, ensuring that pyufunc remains compatible with the latest Python releases and industry best practices. We actively welcome community feedback and continually refine the package to meet developers' evolving requirements.
 5. **Time and Effort Savings:** With pyufunc, you can avoid reinventing the wheel by leveraging pre-existing, widely used utility functions. This saves you time and effort in writing custom utility functions and allows you to focus on the core aspects of your project.
 
 Let pyufunc take care of the repetitive tasks while you focus on building remarkable Python applications. Empower your projects with the efficiency and elegance that comes with pyufunc - your all-inclusive Python utility toolkit. Happy coding!
 
-🚀️ **No Extra dependencies will be installed to your environment unless use of functions that need certain dependency, the function will automatically install required package when you run it.**
+🚀️ **No dependencies will be installed to your environment unless use of functions that need certain dependency, the function will automatically install required package when you run it.**
 
 ## Existing Utility Functions Categorized by Functionality
 
 - [utility_function_by_category.md](https://github.com/xyluo25/pyufunc/blob/main/utility_function_by_category.md)
 
 ## Existing Utility Functions Categorized by Keywords
 
@@ -112,12 +112,17 @@
 
 For more information about the ways you can contribute to pyufunc, visit [PyUFunc GitHub](https://github.com/xyluo25/pyufunc). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
 
 ## Comprehensive Review of Utility Function Packages
 
 - [utility_function_package_review.md](https://github.com/xyluo25/pyufunc/blob/main/utility_function_package_review.md)
 
+## How to Cite
+
+If you use pyufunc in your work and research, please use the following entry:
+Luo, X. and Zhou, X. (2024, February 18). PYUFUNC. Retrieved from https://github.com/xyluo25/pyufunc
+
 ## ACKNOWLEDGMENT
 
 This open-source package is supported by National Science Foundation under grant no. TIP-2303748 titled, "[POSE: Phase II: CONNECT: Consortium of Open-source Planning Models for Next-generation Equitable and Efficient Communities and Transportation](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303748&HistoricalAwards=false)"
 
 Thank you to everyone who has contributed to the list of packages mentioned above. Your contributions have significantly enriched our open-source community. If any code violates your licensing agreements, please don't hesitate to [Contact developers](mailto:luoxiangyong01@gmail.com).
```

### Comparing `pyufunc-0.2.5/README.md` & `pyufunc-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 2. **Modularity and Extensibility:** pyufunc is structured with modularity in mind. Each utility function is a standalone entity, allowing you to cherry-pick the ones you need without introducing unnecessary dependencies. Furthermore, the package is designed to be extensible, making it effortless to contribute your own utility functions and enrich the community.
 3. **Robust Collection of Utility Functions:** pyufunc offers a versatile assortment of utility functions, carefully crafted and thoroughly tested to meet industry standards. The package covers diverse domains, including data manipulation, file handling, string operations, mathematical functions, and much more.
 4. **Regular Updates and Maintenance:** Our team is dedicated to providing regular updates, ensuring that pyufunc remains compatible with the latest Python releases and industry best practices. We actively welcome community feedback and continually refine the package to meet developers' evolving requirements.
 5. **Time and Effort Savings:** With pyufunc, you can avoid reinventing the wheel by leveraging pre-existing, widely used utility functions. This saves you time and effort in writing custom utility functions and allows you to focus on the core aspects of your project.
 
 Let pyufunc take care of the repetitive tasks while you focus on building remarkable Python applications. Empower your projects with the efficiency and elegance that comes with pyufunc - your all-inclusive Python utility toolkit. Happy coding!
 
-🚀️ **No Extra dependencies will be installed to your environment unless use of functions that need certain dependency, the function will automatically install required package when you run it.**
+🚀️ **No dependencies will be installed to your environment unless use of functions that need certain dependency, the function will automatically install required package when you run it.**
 
 ## Existing Utility Functions Categorized by Functionality
 
 - [utility_function_by_category.md](https://github.com/xyluo25/pyufunc/blob/main/utility_function_by_category.md)
 
 ## Existing Utility Functions Categorized by Keywords
 
@@ -85,12 +85,17 @@
 
 For more information about the ways you can contribute to pyufunc, visit [PyUFunc GitHub](https://github.com/xyluo25/pyufunc). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
 
 ## Comprehensive Review of Utility Function Packages
 
 - [utility_function_package_review.md](https://github.com/xyluo25/pyufunc/blob/main/utility_function_package_review.md)
 
+## How to Cite
+
+If you use pyufunc in your work and research, please use the following entry:
+Luo, X. and Zhou, X. (2024, February 18). PYUFUNC. Retrieved from https://github.com/xyluo25/pyufunc
+
 ## ACKNOWLEDGMENT
 
 This open-source package is supported by National Science Foundation under grant no. TIP-2303748 titled, "[POSE: Phase II: CONNECT: Consortium of Open-source Planning Models for Next-generation Equitable and Efficient Communities and Transportation](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303748&HistoricalAwards=false)"
 
 Thank you to everyone who has contributed to the list of packages mentioned above. Your contributions have significantly enriched our open-source community. If any code violates your licensing agreements, please don't hesitate to [Contact developers](mailto:luoxiangyong01@gmail.com).
```

### Comparing `pyufunc-0.2.5/pyufunc/__init__.py` & `pyufunc-0.2.6/pyufunc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # import modules with same name from different folder in python
 from __future__ import absolute_import
 from itertools import chain
 
 # import all modules
 from .util_ai import *  # machine learning functions
+from .util_algorithm import *  # algorithm functions
 from .util_common import *  # unclassified functions are here
 from .util_data_processing import *  # data processing functions including algorithms
 from .util_datetime import *  # datetime functions
 from .util_fullstack import *  # fullstack functions, including front end and back end
 from .util_geo import *  # geographic functions
 from .util_git_pypi import *  # git and pypi functions
 from .util_gui import *  # GUI functions
@@ -25,18 +26,20 @@
 from .util_optimization import *  # optimization functions
 from .util_pathio import *  # path and IO functions
 from .util_test import *  # test functions
 from .util_vis import *  # visualization functions
 
 # import package configurations and utilities
 from .pkg_configs import *
-from .pkg_configs import FUNC_KEYWORD
+from .pkg_configs import config_FUNC_KEYWORD as FUNC_KEYWORD
 from .pkg_utils import *
 
+# prepare FUNC_CATEGORY for show_util_func_by_category
 import pyufunc.util_ai as __util_ai
+import pyufunc.util_algorithm as __util_algo
 import pyufunc.util_common as __util_common
 import pyufunc.util_data_processing as __util_data_processing
 import pyufunc.util_datetime as __util_datetime
 import pyufunc.util_fullstack as __util_fullstack
 import pyufunc.util_geo as __util_geo
 import pyufunc.util_git_pypi as __util_git_pypi
 import pyufunc.util_gui as __util_gui
@@ -46,17 +49,18 @@
 import pyufunc.util_office as __util_office
 import pyufunc.util_optimization as __util_optimization
 import pyufunc.util_pathio as __util_pathio
 import pyufunc.util_test as __util_test
 import pyufunc.util_vis as __util_vis
 import pyufunc.pkg_utils as __pkg_utils
 
-# **** specify the available utility functions by category **** #
+# specify the available utility functions by category
 FUNC_CATEGORY = {
     "util_ai"             : __util_ai.__all__,
+    "util_algorithm"      : __util_algo.__all__,
     "util_common"         : __util_common.__all__,
     "util_data_processing": __util_data_processing.__all__,
     "util_datetime"       : __util_datetime.__all__,
     "util_fullstack"      : __util_fullstack.__all__,
     "util_geo"            : __util_geo.__all__,
     "util_git_pypi"       : __util_git_pypi.__all__,
     "util_gui"            : __util_gui.__all__,
@@ -103,19 +107,19 @@
 
     res_str_head = "Available utility functions in pyUFunc"
     res_str_by_category = ""
     func_count = 0
     for util_category in FUNC_CATEGORY:
         if FUNC_CATEGORY[util_category]:
             res_str_by_category += f"\n- {util_category}:\n"
-            for func in FUNC_CATEGORY[util_category]:
+            for func in sorted(FUNC_CATEGORY[util_category], key=str.lower):
                 res_str_by_category += f"  - {func}\n"
                 func_count += 1
 
-    res_str = res_str_head + f" ({func_count}):\n" + res_str_by_category
+    res_str = f"{res_str_head} ({func_count}):\n{res_str_by_category}"
 
     if verbose:
         print(res_str)
         return None
     return res_str
 
 
@@ -139,33 +143,42 @@
            ** requires
 
         -- show:
            ** show_numpy_docstring_style
            ** show_available_utility_func
     """
 
-    for func_str in list(chain.from_iterable(FUNC_CATEGORY.values())):
+    all_func_str = sorted(list(chain.from_iterable(FUNC_CATEGORY.values())), key=str.lower)
+    for func_str in all_func_str:
+        # get the prefix and suffix of the function name
         prefix = func_str.split("_")[0]
-        if prefix in FUNC_KEYWORD:
+        suffix = func_str.split("_")[-1]
+
+        # if the prefix is not in FUNC_KEYWORD, add it
+        if prefix in FUNC_KEYWORD and func_str not in FUNC_KEYWORD[prefix]:
             FUNC_KEYWORD[prefix].append(func_str)
+        elif suffix in FUNC_KEYWORD and func_str not in FUNC_KEYWORD[suffix]:
+            FUNC_KEYWORD[suffix].append(func_str)
         else:
             FUNC_KEYWORD["non-keywords"].append(func_str)
 
     res_str_head = "Available utility functions in pyUFunc"
     res_str_by_keyword = ""
     func_count = 0
 
     for keyword in FUNC_KEYWORD:
         if FUNC_KEYWORD[keyword]:
             res_str_by_keyword += f"\n- {keyword}:\n"
+
+            # add unique function names to the string
             for func in FUNC_KEYWORD[keyword]:
                 res_str_by_keyword += f"  - {func}\n"
                 func_count += 1
 
-    res_str = res_str_head + f" ({func_count}):\n" + res_str_by_keyword
+    res_str = f"{res_str_head} ({func_count}):\n{res_str_by_keyword}"
 
     if verbose:
         print(res_str)
         return None
     return res_str
 
 
@@ -196,14 +209,14 @@
         if keyword.lower() in func_str.lower():
             res_str_by_keyword += f"  \n{func_count + 1}. {func_str}\n"
             res_str_lst.append(func_str)
             func_count += 1
 
     if verbose:
         res_str_head = f"Available functions by keyword: {keyword}"
-        res_str = res_str_head + f" ({func_count}):\n" + res_str_by_keyword
+        res_str = f"{res_str_head} ({func_count}):\n{res_str_by_keyword}"
 
         print(res_str)
         return ""
     return res_str_lst
 
 __all__ = list(chain(*FUNC_CATEGORY.values()))
```

### Comparing `pyufunc-0.2.5/pyufunc/pkg_configs.py` & `pyufunc-0.2.6/pyufunc/pkg_configs.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 import os
 from pyufunc.util_pathio._path import path2linux
 
 # ############## Package Configurations ############## #
-pkg_version = "0.2.5"
+pkg_version = "0.2.6"
 pkg_name = "pyufunc"
 pkg_author = "Mr. Xiangyong Luo, Dr. Xuesong Simon Zhou"
 pkg_email = "luoxiangyong01@gmail.com, xzhou74@asu.edu"
 
 # ############## Logging Configurations ############## #
-logging_config = {
+config_logging = {
     # system logging
     "is_log": True,
 
     # logging default folder
     "log_folder": path2linux(os.path.join(os.getcwd(), "syslogs")),
 
     # logging
@@ -29,15 +29,15 @@
     "log_fmt": "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 
     # default log date format
     "log_datefmt": "%Y-%m-%d %H:%M:%S",
 }
 
 # ############### Date Time Format Configuration ############### #
-pkg_datetime_fmt = {
+config_datetime_fmt = {
 
     # 0 "YYYY-MM-DD", 2023-07-09
     # 1 "YYYY-MM-DD HH:MM:SS", 2023-07-09 11:11:11
     # 2 "YYYY-MM-DD HH:MM:SS.MS", 2023-07-09 11:11:11.123456
     0 : "%Y-%m-%d",
     1 : "%Y-%m-%d %H:%M:%S",
     2 : "%Y-%m-%d %H:%M:%S.%f",
@@ -57,15 +57,15 @@
     8 : "%d/%m/%Y %H:%M:%S.%f",
 
     9 : "%H:%M:%S",  # "HH:MM:SS", 11:11:11
     10 : "%H:%M:%S.%f",  # "HH:MM:SS.MS", 11:11:11.123456
 }
 
 # ############### Function Keywords Configuration ############### #
-FUNC_KEYWORD = {
+config_FUNC_KEYWORD = {
     "non-keywords": [],
     "show"        : [],
     "get"         : [],
     "generate"    : [],
     "create"      : [],
     "find"        : [],
     "calc"        : [],
@@ -78,18 +78,20 @@
     "split"       : [],
     "fmt"         : [],
     "cvt"         : [],
     "is"          : [],
     "proj"        : [],
     "github"      : [],
     "pypi"        : [],
+    "error"       : [],
+    "sort"        : [],
 }
 
 # ############### Email Configuration ############### #
-email_config = {
+config_email = {
     'gmail.com': {
         'smtp': ('smtp.gmail.com', 587),
         'pop3': ('pop.gmail.com', 995)},
     'office365.com': {
         'smtp': ('smtp.office365.com', 587),
         'pop3': ('outlook.office365.com', 995)},
     'outlook.com': {
@@ -119,7 +121,16 @@
     '163.com': {
         'smtp': ('smtp.163.com', 465),
         'pop3': ('pop.163.com', 995)},
     'asu.edu': {
         'smtp': ('smtp.gmail.edu', 587),
         'pop3': ('pop.gmail.edu', 995)},
 }
+
+# ############### GMNS: General Modeling Network Specification configuration #
+config_gmns = {
+    # specify required fields for node.csv and poi.csv and zone.csv (optional)
+    "node_required_fields": ["node_id", "x_coord", "y_coord",
+                             "activity_type", "is_boundary", "poi_id"],
+    "poi_required_fields": ["poi_id", "building", "centroid", "area", "geometry"],
+    "link_required_fields": ["link_id", "from_node_id", "to_node_id", "length", "lanes"],
+}
```

### Comparing `pyufunc-0.2.5/pyufunc/pkg_utils.py` & `pyufunc-0.2.6/pyufunc/pkg_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # specify the available utility functions for importing all
 __all__ = [
     "import_package",
     "requires",
     "func_running_time",
     "func_time",
     "run_parallel",
+    "end_of_life",
     "get_user_defined_func",
     "is_user_defined_func",
     "is_module_importable",
 ]
 
 
 def import_package(pkg_name: Union[str, tuple, list],
@@ -40,21 +41,23 @@
 
     Location:
         The function defined in pyufunc/pkg_utils.py.
 
     Args:
         package_name (str): the package name, it can be a string or tuple or list.
             if it's a string, it's the package name for both installation and import.
+
             if it's a tuple or list, it has two elements:
-                first element is the package name, for pip or conda installation
-                second element is the package name, for import the package
-            eg: "numpy" or "numpy==1.19.5".
-            eg. ("pillow", "PIL"),
-            eg. ["pillow==8.3.1", "PIL"]
-            eg. ["opencv-python", "cv2"]
+                first element is the package name, for pip or conda installation;
+                second element is the package name, for import the package;
+
+            eg: "numpy" or "numpy==1.19.5";
+            eg: ("pillow", "PIL");
+            eg: ["pillow==8.3.1", "PIL"];
+            eg: ["opencv-python", "cv2"];
         options (list, optional): the installation optional inputs,
             eg: '--force-reinstall', '--ignore-installed'. Defaults to ["--user"].
         verbose (bool, optional): print the error message if the package is not available.
             Defaults to True.
 
     Returns:
         object: the imported package
@@ -67,19 +70,22 @@
 
     Examples:
         >>> numpy = import_package("numpy") # equal to "import numpy as numpy"
         >>> np = import_package("numpy")  # equal to "import numpy as np"
 
         # not existed
         >>> numpy = import_package("numpy")
-            :numpy not existed in current env, installing...
+
+        :numpy not existed in current env, installing...
 
         # specify the version
+
         >>> numpy = import_package("numpy==1.19.5")
-            :Package numpy==1.19.5 not existed in current env, installing...
+
+        :Package numpy==1.19.5 not existed in current env, installing...
 
         # different name for installation and import
         >>> PIL = import_package(("pillow", "PIL"))
         >>> cv2 = import_package(["opencv-python", "cv2"])
         >>> cv2 = import_package(["opencv-python", "cv2"], options=["--force-reinstall"])
         >>> cv2 = import_package(["opencv-python==4.9.0.80", "cv2"])
     """
@@ -106,16 +112,15 @@
 
         if verbose:
             print(f"  :installing {module_name}...")
 
         # install package to current environment
         outputs = []
         try:
-            all_args = [sys.executable, '-m', 'pip',
-                        'install', *options, module_name]
+            all_args = [sys.executable, '-m', 'pip', 'install', *options, module_name]
 
             result = subprocess.run(
                 all_args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
             stdout = result.stdout.decode('utf-8')
             stderr = result.stderr.decode('utf-8')
             outputs.extend((stdout, stderr))
@@ -175,21 +180,20 @@
             INFO Begin to run function: func …
             main function...
             INFO Finished running function: func, total: 3s
     """
 
     @wraps(func)
     def inner(*args, **kwargs):
-        print(f'  :INFO: begin to run function: {func.__name__} …')
+        # print(f'  :INFO: begin to run function: {func.__name__} …')
         time_start = datetime.datetime.now()
         res = func(*args, **kwargs)
         time_diff = datetime.datetime.now() - time_start
         print(
-            f'  :INFO: finished running function: {func.__name__}, total: {time_diff.seconds}s')
-        print()
+            f'  :INFO: finished function: {func.__name__}, total: {time_diff.seconds}s \n')
         return res
 
     return inner
 
 
 def func_time(func: object) -> object:
     """A decorator to measure the time of a function or class method.
@@ -219,21 +223,20 @@
             INFO Begin to run function: func …
             main function...
             INFO Finished running function: func, total: 3s
     """
 
     @wraps(func)
     def inner(*args, **kwargs):
-        print(f'  :INFO: begin to run function: {func.__name__} …')
+        # print(f'  :INFO: begin to run function: {func.__name__} …')
         time_start = datetime.datetime.now()
         res = func(*args, **kwargs)
         time_diff = datetime.datetime.now() - time_start
         print(
-            f'  :INFO: finished running function: {func.__name__}, total: {time_diff.seconds}s')
-        print()
+            f'  :INFO: finished function: {func.__name__}, total: {time_diff.seconds}s \n')
         return res
 
     return inner
 
 
 def get_user_defined_func(module: object = sys.modules[__name__]) -> list:
     """list all user-defined functions in a module.
@@ -295,35 +298,35 @@
     except Exception as e:
         # Handle other possible exceptions, such as the function being a built-in method of a built-in type
         print(f"  :Info: could not determine the {func_obj} is user-defined: {e}")
         return False
 
     # Check if the function is defined in the script's main file or a user-defined module
     # This is a simple check and might need to be adjusted based on your project structure
-    if "site-packages" in func_file or "python" in func_file.lower():
-        # The function is likely imported from an installed package or the standard library
-        return False
-
-    return True  # The function is likely user-defined
+    return "site-packages" not in func_file and "python" not in func_file.lower()
 
 
 def is_module_importable(module_name: str) -> bool:
     """Safely import a module and return a boolean. If the module is not importable, return False.
 
     Args:
-        modname (str): the module name to import.
+        module_name (str): the module name to import.
 
     Returns:
         bool: True if the module is importable, False otherwise.
 
     Note:
         This function is useful to check if a module is installed in the current environment.
 
     Examples:
-
+        >>> from pyufunc import is_module_importable
+        >>> is_module_importable("numpy")
+        True
+        >>> is_module_importable("unknown_module")
+        False
     """
 
     # TDD, test-driven development: check inputs
     assert isinstance(module_name, str), "The input module name should be a string."
 
     try:
         exec(f"import {module_name}")
@@ -342,51 +345,54 @@
     Args:
         *args: the required dependencies to run the function.
             if argument is a string, module and import are the same.
             if argument is a tuple or list, it has two elements:
                 first element is the module name, for pip or conda installation;
                 second element is the import name, for import the module;
         **kwargs: the optional arguments, including verbose and auto_install.
-            verbose (bool, optional): print the processing message.
-                Defaults to True.
+            verbose (bool, optional): print the processing message. Defaults to True.
             auto_install (bool, optional): install the missing dependencies automatically.
                 Defaults to False.
 
     Returns:
         object: the decorated function.
 
     Note:
         user can parse the verbose and auto_install options to control the behavior of the decorator.
         verbose: print the error message if the dependencies are not available.
             Default is True.
+
         auto_install: install the missing dependencies automatically.
             Default is True.
 
         eg: @requires("numpy", "pandas", verbose=False)
         eg: @requires("numpy", "pandas", verbose=True, auto_install=True)
         eg: @requires("numpy", "pandas", verbose=False, auto_install=True)
         eg: @requires(("pillow", "PIL"), "pandas", verbose=True, auto_install=True)
 
     Examples:
 
         # Example 1: the function will not run if the dependencies are not available
+
         >>> @requires("numpy", "pandas", "unknown_module", verbose=True, auto_install=False)
             def my_function():
-                return "I'm running!"
+               return "I'm running!"
 
         >>> my_function()
-            Error: missing dependencies: ['numpy', 'pandas'], please install them first.
-            not running the function: my_function
+        Error: missing dependencies: ['numpy', 'pandas'], please install them first.
+        not running the function: my_function
 
         # Example 2: the function will run if the dependencies are available
+
         >>> @requires("numpy", "pandas", verbose=True, auto_install=True)
             def my_function():
                 return "I'm running!"
+
         >>> my_function()
-            "I'm running!"
+        "I'm running!"
 
     """
 
     # get the verbose option, default is True
     # the verbose option is used to print the error message
     verbose = kwargs.get("verbose", True)
     auto_install = kwargs.get("auto_install", False)
@@ -518,7 +524,60 @@
     with Pool(num_processors) as pool:
         if chunksize == 0:
             results = pool.map(func, iterable)
         else:
             results = pool.map(func, iterable, chunksize=chunksize)
 
     return results
+
+
+def end_of_life(func: object = None, **kwargs) -> object:
+    """A decorator to mark the end of life of a function or class method.
+    It's useful to use this function to remind users to avoid using the deprecated functions.
+
+    Args:
+        *args: the required dependencies to run the function.
+            if argument is a string, module and import are the same.
+            if argument is a tuple or list, it has two elements:
+                first element is the module name, for pip or conda installation;
+                second element is the import name, for import the module;
+        **kwargs: the optional arguments, including message.
+            message (str, optional): the additional message to the users.
+
+    Returns:
+        object: the decorated function.
+
+    Examples:
+        >>> from pyufunc import end_of_life
+        >>> @end_of_life
+            def my_func():
+                return "I'm running!"
+        >>> my_func()
+          :Warning: my_func is deprecated and will be removed in the future.
+        I'm running!
+
+        >>>@end_of_life(message="Please use the new function instead.")
+           def my_func():
+              return "I'm running!"
+        >>> my_func()
+            :Warning: my_func is deprecated and will be removed in the future.
+            :Please use the new function instead.
+        I'm running!
+    """
+
+    # kwargs from decorator
+    # print("kwargs: ", kwargs)
+    message = kwargs.get("message", None)
+
+    def inner(func_obj: object) -> object:
+        @wraps(func_obj)
+        def wrapper(*args, **kwargs):
+            # kwargs from function
+            print(f"  :Warning: {func_obj.__name__} is deprecated and will be removed in the future version.")
+
+            if message:
+                print(f"  :{message}")
+
+            return func_obj(*args, **kwargs)
+        return wrapper
+
+    return inner(func) if func else inner
```

### Comparing `pyufunc-0.2.5/pyufunc/util_common/__init__.py` & `pyufunc-0.2.6/pyufunc/util_common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_common/_google_numpy_docstring.py` & `pyufunc-0.2.6/pyufunc/util_common/_google_numpy_docstring.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_common/_password_generator.py` & `pyufunc-0.2.6/pyufunc/util_common/_password_generator.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_data_processing/__init__.py` & `pyufunc-0.2.6/pyufunc/util_data_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_data_processing/_common.py` & `pyufunc-0.2.6/pyufunc/util_data_processing/_common.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_data_processing/_dict.py` & `pyufunc-0.2.6/pyufunc/util_data_processing/_dict.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_data_processing/_list.py` & `pyufunc-0.2.6/pyufunc/util_data_processing/_list.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_datetime/__init__.py` & `pyufunc-0.2.6/pyufunc/util_datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_datetime/_dt_format.py` & `pyufunc-0.2.6/pyufunc/util_datetime/_dt_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # Contact Info: luoxiangyong01@gmail.com
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 
 import datetime
 from typing import Union
-from pyufunc.pkg_configs import pkg_datetime_fmt
+from pyufunc.pkg_configs import config_datetime_fmt
 
 
 def fmt_dt_to_str(dt: Union[datetime.datetime, str] = datetime.datetime.now(),
                   format_seq: int = 1) -> str:
     """Format datetime to datetime string
 
     Args:
         dt (datetime, optional): the datetime to be formatted. Defaults to datetime.datetime.now().
         format_seq (int): the format of the datetime. Defaults to 0 ("%Y-%m-%d %H:%M:%S").
 
     See Also:
-        pyufunc.pkg_configs.pkg_datetime_fmt : pre-defined datetime string formats
+        pyufunc.pkg_configs.config_datetime_fmt : pre-defined datetime string formats
 
     Returns:
         str : the formatted datetime string
 
     Example:
         >>> from pyufunc import fmt_dt_to_str
         >>> fmt_dt_to_str()
@@ -36,17 +36,17 @@
 
     # check if the dt is a string
     if isinstance(dt, str):
         # convert input datetime string to datetime object
         dt = datetime.datetime.strptime(dt, "%Y-%m-%d %H:%M:%S")
 
     # pre-defined datetime string formats: pyufunc.pkg_configs.pkg_dt_fmt_seq
-    if format_seq not in pkg_datetime_fmt:
+    if format_seq not in config_datetime_fmt:
         print("The format_seq is not valid. use format_seq = 0 as the default format: %Y-%m-%d %H:%M:%S")
-        return dt.strftime(pkg_datetime_fmt[1])
+        return dt.strftime(config_datetime_fmt[1])
 
     try:
-        return dt.strftime(pkg_datetime_fmt[format_seq])
+        return dt.strftime(config_datetime_fmt[format_seq])
     except Exception as e:
         print(e)
         print("Cannot convert the datetime to the specified format. return the original datetime.")
         return dt
```

### Comparing `pyufunc-0.2.5/pyufunc/util_datetime/_dt_group.py` & `pyufunc-0.2.6/pyufunc/util_datetime/_dt_group.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_datetime/_dt_time_difference.py` & `pyufunc-0.2.6/pyufunc/util_datetime/_dt_time_difference.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_datetime/_dt_timezone.py` & `pyufunc-0.2.6/pyufunc/util_datetime/_dt_timezone.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_geo/_geo_circle.py` & `pyufunc-0.2.6/pyufunc/util_geo/_geo_circle.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_geo/_geo_distance.py` & `pyufunc-0.2.6/pyufunc/util_geo/_geo_distance.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_geo/_gmns.py` & `pyufunc-0.2.6/pyufunc/util_geo/_gmns.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         boundary_flag: The boundary flag of the node. = 1 (current node is boundary node)
         zone_id: The zone ID. default == -1, only three conditions to become an activity node
                 1) POI node, 2) is_boundary node(freeway),  3) residential in activity_type
         poi_id: The POI ID of the node. default = -1; to be assigned to a POI ID after reading poi.csv
         activity_type: The activity type of the node. provided from osm2gmns such as motoway, residential, ...
         activity_location_tab: The activity location tab of the node.
         geometry: The geometry of the node. based on wkt format.
+        as_dict: The method to convert the node to a dictionary.
+        to_networkx: The method to convert the node to a networkx node tuple format. (id, attr_dict)
     """
     id: int = 0
     x_coord: float = 0
     y_coord: float = 0
     production: float = 0
     attraction: float = 0
     boundary_flag: int = 0
@@ -43,14 +45,19 @@
     activity_type: str = ''
     activity_location_tab: str = ''
     geometry: str = ''
 
     def as_dict(self):
         return asdict(self)
 
+    def to_networkx(self) -> tuple:
+        # covert to networkx node
+        # networkx.add_nodes_from([(id, attr_dict), ])
+        return (self.id, self.as_dict())
+
 
 @dataclass
 class Link:
     """A link in the network.
 
     Attributes:
         id: The link ID.
@@ -61,14 +68,17 @@
         lanes: The lanes of the link.
         dir_flag: The direction flag of the link.
         free_speed: The free speed of the link.
         capacity: The capacity of the link.
         link_type: The type of the link.
         link_type_name: The name of the link type.
         geometry: The geometry of the link. based on wkt format.
+        as_dict: The method to convert the link to a dictionary.
+        to_networkx: The method to convert the link to a networkx edge tuple format. (from_node_id, to_node_id, attr_dict)
+
     """
 
     id: int = 0
     name: str = ""
     from_node_id: int = -1
     to_node_id: int = -1
     length: float = -1
@@ -79,31 +89,39 @@
     link_type: int = -1
     link_type_name: str = ""
     geometry: str = ""
     allowed_uses: str = ""
     from_biway: int = 1
     is_link: bool = True
 
+
     def as_dict(self):
         return asdict(self)
 
+    def to_networkx(self) -> tuple:
+        # convert to networkx edge
+        # networkx.add_edges_from([(from_node_id, to_node_id, attr_dict), ])
+        return (self.from_node_id, self.to_node_id, {**self.as_dict(), **{"weight": self.length}})
+
 
 @dataclass
 class POI:
     """A POI in the network.
 
     Attributes:
         id: The POI ID.
         x_coord: The x coordinate of the POI.
         y_coord: The y coordinate of the POI.
         count: The count of the POI. Total POI values for this POI node or POI zone
         area: The area of the POI. Total area of polygon for this POI zone. unit is square meter
         poi_type: The type of the POI. Default is empty string
         geometry: The polygon of the POI. based on wkt format. Default is empty string
         zone_id: The zone ID. mapping from zone
+        as_dict: The method to convert the POI to a dictionary.
+        to_networkx: The method to convert the POI to a networkx node tuple format. (id, attr_dict)
     """
 
     id: int = 0
     x_coord: float = 0
     y_coord: float = 0
     count: int = 1
     area: list = field(default_factory=list)
@@ -111,14 +129,19 @@
     trip_rate: dict = field(default_factory=dict)
     geometry: str = ''
     zone_id: int = 0
 
     def as_dict(self):
         return asdict(self)
 
+    def to_networkx(self) -> tuple:
+        # convert to networkx node
+        # networkx.add_nodes_from([(id, attr_dict), ])
+        return (self.id, self.as_dict())
+
 
 @dataclass
 class Zone:
     """A zone in the network.
 
     Attributes:
         id: The zone ID.
@@ -133,14 +156,15 @@
         node_id_list: Node IDs which belong to this zone.
         poi_id_list: The POIs which belong to this zone.
         production: The production of the zone.
         attraction: The attraction of the zone.
         production_fixed: The fixed production of the zone (implement different models).
         attraction_fixed: The fixed attraction of the zone (implement different models).
         geometry: The geometry of the zone. based on wkt format
+        as_dict: The method to convert the zone to a dictionary.
     """
 
     id: int = 0
     name: str = ''
     centroid_x: float = 0
     centroid_y: float = 0
     centroid: str = ""
@@ -180,14 +204,15 @@
         path_cost: The path cost. default = 0
 
         b_generated: The flag of whether the agent is generated. default = False
         b_complete_trip: The flag of whether the agent completes the trip. default = False
 
         geometry: The geometry of the agent. based on wkt format. default = ''
         departure_time: The departure time of the agent. unit is second. default = 0
+        as_dict: The method to convert the agent to a dictionary.
     """
 
     id: int = 0
     agent_type: str = ''
     o_zone_id: int = 0
     d_zone_id: int = 0
     o_zone_name: str = ''
```

### Comparing `pyufunc-0.2.5/pyufunc/util_git_pypi/_github.py` & `pyufunc-0.2.6/pyufunc/util_git_pypi/_github.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_git_pypi/_pypi.py` & `pyufunc-0.2.6/pyufunc/util_git_pypi/_pypi.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_git_pypi/static/user-agent-strings.json` & `pyufunc-0.2.6/pyufunc/util_git_pypi/static/user-agent-strings.json`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_img/__init__.py` & `pyufunc-0.2.6/pyufunc/util_img/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 ##############################################################
 # Created Date: Thursday, February 15th 2024
 # Contact Info: luoxiangyong01@gmail.com
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 from ._img_cvt import (
-    cvt_img_to_bytes,
-    cvt_PIL_img_to_bytes,
-    cvt_img_bytes_to_PIL_img,
+    img_to_bytes,
+    img_PIL_to_bytes,
+    img_bytes_to_PIL,
 )
 
 from ._img_operate import (
     is_PIL_img,
     is_CV_img,
-    cvt_img_PIL_to_CV,
-    cvt_img_CV_to_PIL,
+    img_PIL_to_CV,
+    img_CV_to_PIL,
     img_translate,
     img_rotate,
     img_rotate_bound,
     img_resize,
     img_show
 )
 
 __all__ = [
     # _img_cvt
-    "cvt_img_to_bytes",
-    "cvt_PIL_img_to_bytes",
-    "cvt_img_bytes_to_PIL_img",
+    "img_to_bytes",
+    "img_PIL_to_bytes",
+    "img_bytes_to_PIL",
 
     # _img_rotate
     "is_PIL_img",
     "is_CV_img",
-    "cvt_img_PIL_to_CV",
-    "cvt_img_CV_to_PIL",
+    "img_PIL_to_CV",
+    "img_CV_to_PIL",
     "img_translate",
     "img_rotate",
     "img_rotate_bound",
     "img_resize",
-    "img_show"
+    "img_show",
 
 ]
```

### Comparing `pyufunc-0.2.5/pyufunc/util_img/_img_cvt.py` & `pyufunc-0.2.6/pyufunc/util_img/_img_cvt.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # https://stackoverflow.com/questions/61384752/how-to-type-hint-with-an-optional-import
 if TYPE_CHECKING:
     # check the support version of python
     # https://pillow.readthedocs.io/en/stable/installation.html
     from PIL import Image
 
 
-def cvt_img_to_bytes(img_path: str) -> bytes:
+def img_to_bytes(img_path: str) -> bytes:
     """Convert image to bytes
 
     Args:
         img_path (str): image path, include all image format, e.g. .jpg, .png, .bmp, .gif, etc.
 
     Returns:
         bytes: the image bytes
@@ -34,15 +34,15 @@
         with open(img_path, 'rb') as f:
             img_b = f.read()
     except Exception:
         img_b = bytes("", encoding='utf-8')
     return img_b
 
 
-def cvt_PIL_img_to_bytes(img: Image) -> bytes:
+def img_PIL_to_bytes(img: Image) -> bytes:
     """Convert PIL image to bytes
 
     Args:
         img (Image): PIL image object
 
     Returns:
         bytes: the image bytes
@@ -58,15 +58,15 @@
         img_b = io.BytesIO()
         img.save(img_b, format='JPEG')
         return img_b.getvalue()
     except Exception:
         return bytes("", encoding='utf-8')
 
 
-def cvt_img_bytes_to_PIL_img(img_b: bytes) -> Image:
+def img_bytes_to_PIL(img_b: bytes) -> Image:
     """Convert image bytes to PIL image
 
     Args:
         img_b (bytes): image bytes
 
     Returns:
         Image: PIL image object
```

### Comparing `pyufunc-0.2.5/pyufunc/util_img/_img_operate.py` & `pyufunc-0.2.6/pyufunc/util_img/_img_operate.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     import_package("numpy", verbose=False)
     import numpy as np
 
     return isinstance(img, np.ndarray)
 
 
 @requires("numpy", ("opencv-python", "cv2"), ("pillow", "PIL"), verbose=False)
-def cvt_img_PIL_to_CV(img: Image.Image) -> np.ndarray:
+def img_PIL_to_CV(img: Image.Image) -> np.ndarray:
     """Convert PIL image to CV image
 
     Args:
         img (Image.Image): PIL image object
 
     Returns:
         np.ndarray: CV image array
@@ -101,15 +101,15 @@
     import cv2
     from PIL import Image
 
     return cv2.cvtColor(np.array(img), cv2.COLOR_RGB2BGR)
 
 
 @requires("numpy", ("opencv-python", "cv2"), ("pillow", "PIL"), verbose=False)
-def cvt_img_CV_to_PIL(img: np.ndarray) -> Image.Image:
+def img_CV_to_PIL(img: np.ndarray) -> Image.Image:
     """Convert CV image to PIL image
 
     Args:
         img (np.ndarray): CV image array
 
     Returns:
         Image.Image: PIL image object
@@ -175,15 +175,15 @@
             img = cv2.imread(img)
         except Exception as e:
             raise Exception(f"Error: {e}") from e
 
     # check if the input image is a PIL image
     # if it is a PIL image, convert it to a CV image
     if isinstance(img, Image.Image):
-        img = cvt_img_PIL_to_CV(img)
+        img = img_PIL_to_CV(img)
 
     # get the height and width of image
     height, width = img.shape[:2]
 
     # get the translation matrix
     M = np.float32([[1, 0, dx], [0, 1, dy]])
     img_t = cv2.warpAffine(img, M, (width, height))
@@ -242,15 +242,15 @@
         try:
             img = cv2.imread(img)
         except Exception as e:
             raise Exception(f"Error: {e}") from e
 
     # check if the input image is a PIL image
     if isinstance(img, Image.Image):
-        img = cvt_img_PIL_to_CV(img)
+        img = img_PIL_to_CV(img)
 
     # get the height and width of image
     height, width = img.shape[:2]
 
     # if center is None, set center to the center of image
     img_center = (width // 2, height // 2)
 
@@ -322,15 +322,15 @@
         try:
             img = cv2.imread(img)
         except Exception as e:
             raise Exception(f"Error: {e}") from e
 
     # check if the input image is a PIL image
     if isinstance(img, Image.Image):
-        img = cvt_img_PIL_to_CV(img)
+        img = img_PIL_to_CV(img)
 
     # get the height and width of image
     height, width = img.shape[:2]
 
     # get the center of image
     center_x, center_y = width / 2, height / 2
 
@@ -405,15 +405,15 @@
         try:
             img = cv2.imread(img)
         except Exception as e:
             raise Exception(f"Error: {e}") from e
 
     # check if the input image is a PIL image
     if isinstance(img, Image.Image):
-        img = cvt_img_PIL_to_CV(img)
+        img = img_PIL_to_CV(img)
 
     # set the default interpolation method
     if inter is None:
         inter = cv2.INTER_AREA
 
     # get the height and width of image
     img_height, img_width = img.shape[:2]
@@ -481,21 +481,21 @@
             img_cv = cv2.imread(img)
             img_pil = Image.open(img)
         except Exception as e:
             raise Exception(f"Error: {e}") from e
 
     # check if the input image is a PIL image
     if isinstance(img, Image.Image):
-        img_cv = cvt_img_PIL_to_CV(img)
+        img_cv = img_PIL_to_CV(img)
         img_pil = img
 
     # check if the input image is a CV image
     if isinstance(img, np.ndarray):
         img_cv = img
-        img_pil = cvt_img_CV_to_PIL(img)
+        img_pil = img_CV_to_PIL(img)
 
     if is_PIL_show:
         if verbose:
             print("  Show image using PIL, if you want to show the image using OpenCV, set is_PIL_show=False")
 
         img_pil.show()
         return None
```

### Comparing `pyufunc-0.2.5/pyufunc/util_log/log.txt` & `pyufunc-0.2.6/pyufunc/util_log/log.txt`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_log/log_config.py` & `pyufunc-0.2.6/pyufunc/util_log/log_config.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_log/loga.py` & `pyufunc-0.2.6/pyufunc/util_log/loga.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_log/logutils.py` & `pyufunc-0.2.6/pyufunc/util_log/logutils.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_log/te.py` & `pyufunc-0.2.6/pyufunc/util_log/te.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_network/_network.py` & `pyufunc-0.2.6/pyufunc/util_network/_network.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_office/_email.py` & `pyufunc-0.2.6/pyufunc/util_office/_email.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from email.mime.audio import MIMEAudio
 from email.mime.base import MIMEBase
 from email import encoders
 
 # For guessing MIME type based on file name extension
 import mimetypes
 
-from pyufunc.pkg_configs import email_config
+from pyufunc.pkg_configs import config_email
 from pyufunc.util_pathio._path import path2linux
 
 
 def is_valid_email(email: str) -> bool:
     """check if the email is valid
 
     Args:
@@ -133,15 +133,15 @@
     if bcc and not isinstance(bcc, list):
         raise ValueError("bcc should be a list or a string of email addresses")
     if bcc and not all(is_valid_email(email) for email in bcc):
         raise ValueError(f"Invalid email address: {bcc}")
 
     # get email configurations from send_from
     email_from_domain = send_from.split("@")[-1]
-    email_config_domain = email_config.get(email_from_domain.lower())
+    email_config_domain = config_email.get(email_from_domain.lower())
     if not email_config_domain:
         raise ValueError(f"Unknown email provider: {email_from_domain}")
 
     smtp_server, smtp_port = email_config_domain.get("smtp")
 
     # Create a multipart message
     msg = MIMEMultipart()
```

### Comparing `pyufunc-0.2.5/pyufunc/util_pathio/__init__.py` & `pyufunc-0.2.6/pyufunc/util_pathio/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                   create_tempfile,
                   remove_file,
                   add_dir_to_env
                   )
 from ._path import (path2linux,
                     path2uniform,
                     get_filenames_by_ext,
-                    check_files_existence,
+                    check_files_in_dir,
                     check_filename,
                     generate_unique_filename
                     )
 from ._platform import (check_platform,
                         is_windows,
                         is_linux,
                         is_mac)
@@ -35,15 +35,15 @@
     "remove_file",
     "add_dir_to_env",
 
     # path
     'path2linux',
     'path2uniform',
     "get_filenames_by_ext",
-    "check_files_existence",
+    "check_files_in_dir",
     "check_filename",
     "generate_unique_filename",
 
     # platform
     "check_platform",
     "is_windows",
     "is_linux",
```

### Comparing `pyufunc-0.2.5/pyufunc/util_pathio/_io.py` & `pyufunc-0.2.6/pyufunc/util_pathio/_io.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc/util_pathio/_path.py` & `pyufunc-0.2.6/pyufunc/util_pathio/_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     if file_ext[0] in {None, "*", "all"}:
         return [path2linux(os.path.join(dir_path, file)) for file in os.listdir(dir_path)]
 
     return [path2linux(os.path.join(dir_path, file)) for file in os.listdir(dir_path)
             if file.endswith(file_ext)]
 
 
-def check_files_existence(filenames: list[str | Path], dir_path: str | Path = "", incl_subdir: bool = False) -> bool:
+def check_files_in_dir(filenames: list[str | Path], dir_path: str | Path = "", incl_subdir: bool = False) -> bool:
     """Check if provided list of files exist in the given directory
 
     Location:
         pyufunc/pathio/_path.py
 
     References:
         https://github.com/xyluo25/utdf2gmns (Apache)
```

### Comparing `pyufunc-0.2.5/pyufunc/util_pathio/_platform.py` & `pyufunc-0.2.6/pyufunc/util_pathio/_platform.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/pyufunc.egg-info/PKG-INFO` & `pyufunc-0.2.6/pyufunc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyufunc
-Version: 0.2.5
+Version: 0.2.6
 Summary: PyUFunc consolidates frequently used utility functions from various libraries into one cohesive package
 Home-page: https://github.com/xyluo25/pyufunc
 Author: Mr. Xiangyong Luo, Dr. Xuesong Simon Zhou
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 License: MIT License
 Project-URL: Homepage, https://github.com/xyluo25/pyufunc
 Project-URL: Bug Tracker, https://github.com/xyluo25/pyufunc/issues
@@ -39,15 +39,15 @@
 2. **Modularity and Extensibility:** pyufunc is structured with modularity in mind. Each utility function is a standalone entity, allowing you to cherry-pick the ones you need without introducing unnecessary dependencies. Furthermore, the package is designed to be extensible, making it effortless to contribute your own utility functions and enrich the community.
 3. **Robust Collection of Utility Functions:** pyufunc offers a versatile assortment of utility functions, carefully crafted and thoroughly tested to meet industry standards. The package covers diverse domains, including data manipulation, file handling, string operations, mathematical functions, and much more.
 4. **Regular Updates and Maintenance:** Our team is dedicated to providing regular updates, ensuring that pyufunc remains compatible with the latest Python releases and industry best practices. We actively welcome community feedback and continually refine the package to meet developers' evolving requirements.
 5. **Time and Effort Savings:** With pyufunc, you can avoid reinventing the wheel by leveraging pre-existing, widely used utility functions. This saves you time and effort in writing custom utility functions and allows you to focus on the core aspects of your project.
 
 Let pyufunc take care of the repetitive tasks while you focus on building remarkable Python applications. Empower your projects with the efficiency and elegance that comes with pyufunc - your all-inclusive Python utility toolkit. Happy coding!
 
-🚀️ **No Extra dependencies will be installed to your environment unless use of functions that need certain dependency, the function will automatically install required package when you run it.**
+🚀️ **No dependencies will be installed to your environment unless use of functions that need certain dependency, the function will automatically install required package when you run it.**
 
 ## Existing Utility Functions Categorized by Functionality
 
 - [utility_function_by_category.md](https://github.com/xyluo25/pyufunc/blob/main/utility_function_by_category.md)
 
 ## Existing Utility Functions Categorized by Keywords
 
@@ -112,12 +112,17 @@
 
 For more information about the ways you can contribute to pyufunc, visit [PyUFunc GitHub](https://github.com/xyluo25/pyufunc). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
 
 ## Comprehensive Review of Utility Function Packages
 
 - [utility_function_package_review.md](https://github.com/xyluo25/pyufunc/blob/main/utility_function_package_review.md)
 
+## How to Cite
+
+If you use pyufunc in your work and research, please use the following entry:
+Luo, X. and Zhou, X. (2024, February 18). PYUFUNC. Retrieved from https://github.com/xyluo25/pyufunc
+
 ## ACKNOWLEDGMENT
 
 This open-source package is supported by National Science Foundation under grant no. TIP-2303748 titled, "[POSE: Phase II: CONNECT: Consortium of Open-source Planning Models for Next-generation Equitable and Efficient Communities and Transportation](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303748&HistoricalAwards=false)"
 
 Thank you to everyone who has contributed to the list of packages mentioned above. Your contributions have significantly enriched our open-source community. If any code violates your licensing agreements, please don't hesitate to [Contact developers](mailto:luoxiangyong01@gmail.com).
```

### Comparing `pyufunc-0.2.5/pyufunc.egg-info/SOURCES.txt` & `pyufunc-0.2.6/pyufunc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 pyufunc/pkg_configs.py
 pyufunc/pkg_utils.py
 pyufunc.egg-info/PKG-INFO
 pyufunc.egg-info/SOURCES.txt
 pyufunc.egg-info/dependency_links.txt
 pyufunc.egg-info/top_level.txt
 pyufunc/util_ai/__init__.py
+pyufunc/util_ai/_error_measurement.py
 pyufunc/util_ai/_open_cv.py
 pyufunc/util_ai/_pytorch.py
 pyufunc/util_ai/_scikitlearn.py
 pyufunc/util_ai/_scipy.py
 pyufunc/util_ai/_tensorflow.py
+pyufunc/util_algorithm/__init__.py
+pyufunc/util_algorithm/_sort.py
 pyufunc/util_common/__init__.py
 pyufunc/util_common/_google_numpy_docstring.py
 pyufunc/util_common/_password_generator.py
 pyufunc/util_data_processing/__init__.py
 pyufunc/util_data_processing/_common.py
 pyufunc/util_data_processing/_data_cleaning.py
 pyufunc/util_data_processing/_dict.py
@@ -31,19 +34,22 @@
 pyufunc/util_fullstack/__init__.py
 pyufunc/util_fullstack/_database.py
 pyufunc/util_fullstack/_django.py
 pyufunc/util_fullstack/_django_restapi.py
 pyufunc/util_fullstack/_fastapi.py
 pyufunc/util_fullstack/_flask.py
 pyufunc/util_geo/__init__.py
+pyufunc/util_geo/_coordinate_coversion.py
 pyufunc/util_geo/_geo_area.py
 pyufunc/util_geo/_geo_circle.py
 pyufunc/util_geo/_geo_common.py
 pyufunc/util_geo/_geo_distance.py
 pyufunc/util_geo/_gmns.py
+pyufunc/util_geo/_gmns_load.py
+pyufunc/util_geo/_shortest_path.py
 pyufunc/util_git_pypi/__init__.py
 pyufunc/util_git_pypi/_github.py
 pyufunc/util_git_pypi/_gitlab.py
 pyufunc/util_git_pypi/_pypi.py
 pyufunc/util_git_pypi/static/__init__.py
 pyufunc/util_git_pypi/static/user-agent-strings.json
 pyufunc/util_gui/__init__.py
```

### Comparing `pyufunc-0.2.5/setup.py` & `pyufunc-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/tests/test_dp_list.py` & `pyufunc-0.2.6/tests/test_dp_list.py`

 * *Files identical despite different names*

### Comparing `pyufunc-0.2.5/tests/test_pathio_io.py` & `pyufunc-0.2.6/tests/test_pathio_io.py`

 * *Files identical despite different names*

