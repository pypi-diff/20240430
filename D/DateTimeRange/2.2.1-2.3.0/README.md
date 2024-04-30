# Comparing `tmp/DateTimeRange-2.2.1.tar.gz` & `tmp/datetimerange-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DateTimeRange-2.2.1.tar", last modified: Sun Apr  7 14:55:50 2024, max compression
+gzip compressed data, was "datetimerange-2.3.0.tar", last modified: Tue Apr 30 13:10:10 2024, max compression
```

## Comparing `DateTimeRange-2.2.1.tar` & `datetimerange-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/DateTimeRange.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9753 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 14:55:42.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1084 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      205 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9753 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7565 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/datetimerange/
--rw-rw-r--   0 root         (0) root         (0)      325 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      201 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/__version__.py
--rw-rw-r--   0 root         (0) root         (0)    33749 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/_core.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.325921 DateTimeRange-2.2.1/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.325921 DateTimeRange-2.2.1/docs/pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/docs/pages/introduction/
--rw-rw-r--   0 root         (0) root         (0)      214 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/docs/pages/introduction/summary.txt
--rw-rw-r--   0 root         (0) root         (0)     1517 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/requirements/
--rw-rw-r--   0 root         (0) root         (0)       64 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/requirements/docs_requirements.txt
--rw-rw-r--   0 root         (0) root         (0)       53 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/requirements/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)       41 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/requirements/test_requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3190 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/test/
--rw-rw-r--   0 root         (0) root         (0)    49719 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/test/test_dtr.py
--rw-rw-r--   0 root         (0) root         (0)     1523 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.889506 datetimerange-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.877506 datetimerange-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 13:09:39.000000 datetimerange-2.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 13:09:39.000000 datetimerange-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.877506 datetimerange-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-30 13:09:39.000000 datetimerange-2.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-30 13:09:39.000000 datetimerange-2.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-30 13:09:39.000000 datetimerange-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 13:09:39.000000 datetimerange-2.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-30 13:09:39.000000 datetimerange-2.3.0/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/DateTimeRange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-30 13:10:10.000000 datetimerange-2.3.0/DateTimeRange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-30 13:10:10.000000 datetimerange-2.3.0/DateTimeRange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:10:10.000000 datetimerange-2.3.0/DateTimeRange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:09:58.000000 datetimerange-2.3.0/DateTimeRange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 13:10:10.000000 datetimerange-2.3.0/DateTimeRange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 13:10:10.000000 datetimerange-2.3.0/DateTimeRange.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 13:09:39.000000 datetimerange-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 13:09:39.000000 datetimerange-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-30 13:09:39.000000 datetimerange-2.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-30 13:10:10.889506 datetimerange-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-30 13:09:39.000000 datetimerange-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.877506 datetimerange-2.3.0/datetimerange/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 13:09:39.000000 datetimerange-2.3.0/datetimerange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 13:09:39.000000 datetimerange-2.3.0/datetimerange/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-04-30 13:09:39.000000 datetimerange-2.3.0/datetimerange/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:09:39.000000 datetimerange-2.3.0/datetimerange/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.877506 datetimerange-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/make_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.881506 datetimerange-2.3.0/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/changelog_ref.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/docs/pages/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Add_elapsed_time_when_conversion _to_string.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Change_separator_of_the_converted_string.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Change_string_conversion_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Compare_time_ranges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Create_and_convert_to_string.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Create_from_a_string.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_datetime.timedelta.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_end_time_as_datetime.datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_end_time_as_string.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_iterator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_start_time_as_datetime.datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_start_time_as_string.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Get_timedelta_as_seconds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Make_a_subtracted_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Make_an_encompassed_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Make_an_intersected_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Move_the_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Set_end_time.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Set_start_time.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Set_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Test_whether_a_value_intersect_the_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Test_whether_a_value_within_the_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Test_whether_the_time_range_is_set.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Test_whether_the_time_range_is_valid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Truncate_time_range.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/Validate_time_inversion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/docs/pages/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/introduction/badges.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/introduction/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/introduction/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/introduction/summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/links.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/docs/pages/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/reference/datetimerange.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-30 13:09:39.000000 datetimerange-2.3.0/docs/pages/sponsors.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-30 13:09:39.000000 datetimerange-2.3.0/examples/DateTimeRange.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 13:09:39.000000 datetimerange-2.3.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 13:09:39.000000 datetimerange-2.3.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-30 13:09:39.000000 datetimerange-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 13:09:39.000000 datetimerange-2.3.0/requirements/docs_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 13:09:39.000000 datetimerange-2.3.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 13:09:39.000000 datetimerange-2.3.0/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:10:10.889506 datetimerange-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-30 13:09:39.000000 datetimerange-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:10:10.885506 datetimerange-2.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    51886 2024-04-30 13:09:39.000000 datetimerange-2.3.0/test/test_dtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-30 13:09:39.000000 datetimerange-2.3.0/tox.ini
```

### Comparing `DateTimeRange-2.2.1/DateTimeRange.egg-info/PKG-INFO` & `datetimerange-2.3.0/DateTimeRange.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DateTimeRange
-Version: 2.2.1
+Version: 2.3.0
 Summary: DateTimeRange is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 Home-page: https://github.com/thombashi/DateTimeRange
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
-Project-URL: Changlog, https://github.com/thombashi/DateTimeRange/releases
+Project-URL: Changelog, https://github.com/thombashi/DateTimeRange/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://datetimerange.rtfd.io/
 Project-URL: Funding, https://github.com/sponsors/thombashi
 Project-URL: Source, https://github.com/thombashi/DateTimeRange
 Project-URL: Tracker, https://github.com/thombashi/DateTimeRange/issues
 Keywords: datetimerange,datetime,time range
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -48,25 +48,25 @@
    :backlinks: top
    :depth: 2
 
 Summary
 =========
 `DateTimeRange <https://github.com/thombashi/DateTimeRange>`__ is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 
-|PyPI pkg ver| |conda pkg ver| |Supported Python versions| |CI status| |Test coverage| |CodeQL|
+|PyPI pkg ver| |conda pkg ver| |Supported Python ver| |CI status| |Test coverage| |CodeQL|
 
 .. |PyPI pkg ver| image:: https://badge.fury.io/py/DateTimeRange.svg
     :target: https://badge.fury.io/py/DateTimeRange
     :alt: PyPI package version
 
 .. |conda pkg ver| image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
     :target: https://anaconda.org/conda-forge/datetimerange
     :alt: conda-forge package version
 
-.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
     :target: https://pypi.org/project/DateTimeRange
     :alt: Supported Python versions
 
 .. |CI status| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
@@ -280,19 +280,27 @@
 
 Documentation
 ===============
 https://datetimerange.rtfd.io/
 
 Sponsors
 ====================================
-.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
-   :target: https://github.com/b4tman
-   :alt: Dmitry Belyaev (b4tman)
-.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+|chasbecker| |shiguredo| |b4tman| |Arturi0| |github|
+
+.. |chasbecker| image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
-   :alt: Charles Becker (chasbecker)
-.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :alt: ex-sponsor: Charles Becker (chasbecker)
+.. |shiguredo| image:: https://avatars.githubusercontent.com/u/2549434?s=48&v=4
+   :target: https://github.com/shiguredo
+   :alt: ex-sponsor: 時雨堂 (shiguredo)
+.. |b4tman| image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: onetime: Dmitry Belyaev (b4tman)
+.. |Arturi0| image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
    :target: https://github.com/Arturi0
-   :alt: Arturi0
+   :alt: onetime: Arturi0
+.. |github| image:: https://avatars.githubusercontent.com/u/9919?s=48&v=4
+   :target: https://github.com/github
+   :alt: onetime: GitHub (github)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DateTimeRange-2.2.1/LICENSE` & `datetimerange-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DateTimeRange-2.2.1/PKG-INFO` & `datetimerange-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DateTimeRange
-Version: 2.2.1
+Version: 2.3.0
 Summary: DateTimeRange is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 Home-page: https://github.com/thombashi/DateTimeRange
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
-Project-URL: Changlog, https://github.com/thombashi/DateTimeRange/releases
+Project-URL: Changelog, https://github.com/thombashi/DateTimeRange/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://datetimerange.rtfd.io/
 Project-URL: Funding, https://github.com/sponsors/thombashi
 Project-URL: Source, https://github.com/thombashi/DateTimeRange
 Project-URL: Tracker, https://github.com/thombashi/DateTimeRange/issues
 Keywords: datetimerange,datetime,time range
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -48,25 +48,25 @@
    :backlinks: top
    :depth: 2
 
 Summary
 =========
 `DateTimeRange <https://github.com/thombashi/DateTimeRange>`__ is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 
-|PyPI pkg ver| |conda pkg ver| |Supported Python versions| |CI status| |Test coverage| |CodeQL|
+|PyPI pkg ver| |conda pkg ver| |Supported Python ver| |CI status| |Test coverage| |CodeQL|
 
 .. |PyPI pkg ver| image:: https://badge.fury.io/py/DateTimeRange.svg
     :target: https://badge.fury.io/py/DateTimeRange
     :alt: PyPI package version
 
 .. |conda pkg ver| image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
     :target: https://anaconda.org/conda-forge/datetimerange
     :alt: conda-forge package version
 
-.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
     :target: https://pypi.org/project/DateTimeRange
     :alt: Supported Python versions
 
 .. |CI status| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
@@ -280,19 +280,27 @@
 
 Documentation
 ===============
 https://datetimerange.rtfd.io/
 
 Sponsors
 ====================================
-.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
-   :target: https://github.com/b4tman
-   :alt: Dmitry Belyaev (b4tman)
-.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+|chasbecker| |shiguredo| |b4tman| |Arturi0| |github|
+
+.. |chasbecker| image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
-   :alt: Charles Becker (chasbecker)
-.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :alt: ex-sponsor: Charles Becker (chasbecker)
+.. |shiguredo| image:: https://avatars.githubusercontent.com/u/2549434?s=48&v=4
+   :target: https://github.com/shiguredo
+   :alt: ex-sponsor: 時雨堂 (shiguredo)
+.. |b4tman| image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: onetime: Dmitry Belyaev (b4tman)
+.. |Arturi0| image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
    :target: https://github.com/Arturi0
-   :alt: Arturi0
+   :alt: onetime: Arturi0
+.. |github| image:: https://avatars.githubusercontent.com/u/9919?s=48&v=4
+   :target: https://github.com/github
+   :alt: onetime: GitHub (github)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DateTimeRange-2.2.1/README.rst` & `datetimerange-2.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
    :backlinks: top
    :depth: 2
 
 Summary
 =========
 `DateTimeRange <https://github.com/thombashi/DateTimeRange>`__ is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 
-|PyPI pkg ver| |conda pkg ver| |Supported Python versions| |CI status| |Test coverage| |CodeQL|
+|PyPI pkg ver| |conda pkg ver| |Supported Python ver| |CI status| |Test coverage| |CodeQL|
 
 .. |PyPI pkg ver| image:: https://badge.fury.io/py/DateTimeRange.svg
     :target: https://badge.fury.io/py/DateTimeRange
     :alt: PyPI package version
 
 .. |conda pkg ver| image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
     :target: https://anaconda.org/conda-forge/datetimerange
     :alt: conda-forge package version
 
-.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
     :target: https://pypi.org/project/DateTimeRange
     :alt: Supported Python versions
 
 .. |CI status| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
@@ -234,19 +234,27 @@
 
 Documentation
 ===============
 https://datetimerange.rtfd.io/
 
 Sponsors
 ====================================
-.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
-   :target: https://github.com/b4tman
-   :alt: Dmitry Belyaev (b4tman)
-.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+|chasbecker| |shiguredo| |b4tman| |Arturi0| |github|
+
+.. |chasbecker| image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
-   :alt: Charles Becker (chasbecker)
-.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :alt: ex-sponsor: Charles Becker (chasbecker)
+.. |shiguredo| image:: https://avatars.githubusercontent.com/u/2549434?s=48&v=4
+   :target: https://github.com/shiguredo
+   :alt: ex-sponsor: 時雨堂 (shiguredo)
+.. |b4tman| image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: onetime: Dmitry Belyaev (b4tman)
+.. |Arturi0| image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
    :target: https://github.com/Arturi0
-   :alt: Arturi0
+   :alt: onetime: Arturi0
+.. |github| image:: https://avatars.githubusercontent.com/u/9919?s=48&v=4
+   :target: https://github.com/github
+   :alt: onetime: GitHub (github)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DateTimeRange-2.2.1/datetimerange/_core.py` & `datetimerange-2.3.0/datetimerange/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,24 +361,52 @@
 
                 False
                 True
         """
 
         return all([self.start_datetime is not None, self.end_datetime is not None])
 
-    def validate_time_inversion(self) -> None:
+    def is_time_inversion(self, allow_timezone_mismatch: bool = True) -> bool:
         """
-        Check time inversion of the time range.
+        Check the time inversion of the time range.
+
+        :param bool allow_timezone_mismatch:
+            If |True|, ignore the timezone mismatch of the start and end time.
+
+        :return:
+            |True| if |attr_start_datetime| is bigger than |attr_end_datetime|.
+        """
+
+        if not self.is_set():
+            raise ValueError("range is not set")
+
+        assert self.start_datetime
+        assert self.end_datetime
+
+        if not allow_timezone_mismatch and self.start_datetime.tzinfo != self.end_datetime.tzinfo:
+            raise ValueError(f"timezone mismatch: start={self.start_datetime.tzinfo}, end={self.end_datetime.tzinfo}")
+
+        start_utc = self.start_datetime.astimezone(datetime.timezone.utc)
+        end_utc = self.end_datetime.astimezone(datetime.timezone.utc)
+
+        return start_utc > end_utc
+
+    def validate_time_inversion(self, allow_timezone_mismatch: bool = True) -> None:
+        """
+        Check the time inversion of the time range.
+
+        :param bool allow_timezone_mismatch:
+            If |True|, ignore the timezone mismatch of the start and end time.
 
         :raises ValueError:
             If |attr_start_datetime| is
             bigger than |attr_end_datetime|.
         :raises TypeError:
             Any one of |attr_start_datetime| and |attr_end_datetime|,
-            or both is inappropriate datetime value.
+            or both are inappropriate datetime values.
 
         :Sample Code:
             .. code:: python
 
                 from datetimerange import DateTimeRange
                 time_range = DateTimeRange("2015-03-22T10:10:00+0900", "2015-03-22T10:00:00+0900")
                 try:
@@ -394,18 +422,20 @@
         if not self.is_set():
             # for python2/3 compatibility
             raise TypeError
 
         assert self.start_datetime
         assert self.end_datetime
 
-        if self.start_datetime.tzinfo != self.end_datetime.tzinfo:
+        if not allow_timezone_mismatch and self.start_datetime.tzinfo != self.end_datetime.tzinfo:
             raise ValueError(f"timezone mismatch: start={self.start_datetime.tzinfo}, end={self.end_datetime.tzinfo}")
 
-        if self.start_datetime > self.end_datetime:
+        start_utc = self.start_datetime.astimezone(datetime.timezone.utc)
+        end_utc = self.end_datetime.astimezone(datetime.timezone.utc)
+        if start_utc > end_utc:
             raise ValueError(
                 "time inversion found: {:s} > {:s}".format(str(self.start_datetime), str(self.end_datetime))
             )
 
     def is_valid_timerange(self) -> bool:
         """
         :return:
@@ -662,48 +692,48 @@
                 2015-01-04 00:00:00+09:00
         """
 
         cmp_step_w_zero = _compare_timedelta(step, seconds=0)
         if cmp_step_w_zero == 0:
             raise ValueError("step must be not zero")
 
-        is_inversion = False
-        try:
-            self.validate_time_inversion()
-        except ValueError:
-            is_inversion = True
+        if not self.is_set():
+            raise ValueError("range is not set")
 
         assert self.start_datetime
         assert self.end_datetime
 
-        current_datetime = self.start_datetime
+        current_datetime = _normalize_datetime_value(self.start_datetime, self.timezone)
+        assert current_datetime
 
-        if not is_inversion:
+        if not self.is_time_inversion():
             if cmp_step_w_zero < 0:
                 raise ValueError(f"invalid step: expect greater than 0, actual={step}")
 
             while current_datetime <= self.end_datetime:
                 yield current_datetime
-                current_datetime = current_datetime + step
+                current_datetime = _normalize_datetime_value(current_datetime + step, self.timezone)
+                assert current_datetime
         else:
             if cmp_step_w_zero > 0:
                 raise ValueError(f"invalid step: expect less than 0, actual={step}")
 
             while current_datetime >= self.end_datetime:
                 yield current_datetime
-                current_datetime = current_datetime + step
+                current_datetime = _normalize_datetime_value(current_datetime + step, self.timezone)
+                assert current_datetime
 
     def intersection(
         self,
         x: "DateTimeRange",
         intersection_threshold: Union[datetime.timedelta, rdelta.relativedelta, None] = None,
     ) -> "DateTimeRange":
         """
         Create a new time range that overlaps the input and the current time range.
-        If no overlaps found, return a time range that set ``None`` for both start and end time.
+        If no overlaps are found, return a time range that sets ``None`` for both start and end time.
 
         :param DateTimeRange x:
             Value to compute intersection with the current time range.
         :param Union[datetime.timedelta, dateutil.relativedelta.relativedelta, None] intersection_threshold:
             Minimum time constraint that an intersection must have.
             Defaults to ``None`` (no constraint).
 
@@ -843,15 +873,15 @@
         ]
 
     def encompass(self, x: "DateTimeRange") -> "DateTimeRange":
         """
         Create a new time range that encompasses the input and the current time range.
 
         :param DateTimeRange x:
-            Value to compute encompass with the current time range.
+            Value to compute encompasses the current time range.
 
         :Sample Code:
             .. code:: python
 
                 from datetimerange import DateTimeRange
                 dtr0 = DateTimeRange("2015-03-22T10:00:00+0900", "2015-03-22T10:10:00+0900")
                 dtr1 = DateTimeRange("2015-03-22T10:05:00+0900", "2015-03-22T10:15:00+0900")
@@ -874,15 +904,15 @@
             end_datetime=max(self.end_datetime, x.end_datetime),
             start_time_format=self.start_time_format,
             end_time_format=self.end_time_format,
         )
 
     def truncate(self, percentage: float) -> None:
         """
-        Truncate ``percentage`` / 2 [%] of whole time from first and last time.
+        Truncate ``percentage`` / 2 [%] of the whole time from the first and last time.
 
         :param float percentage: Percentage of truncate.
 
         :Sample Code:
             .. code:: python
 
                 from datetimerange import DateTimeRange
@@ -917,15 +947,15 @@
 
     def split(self, separator: Union[str, datetime.datetime]) -> List["DateTimeRange"]:
         """
         Split the DateTimerange in two DateTimerange at a specific datetime.
 
         :param Union[str, datetime.datetime] separator:
             Date and time to split the DateTimeRange.
-            This value will be included for both of the ranges after split.
+            This value will be included for both of the ranges after the split.
 
         :Sample Code:
             .. code:: python
 
                 from datetimerange import DateTimeRange
                 dtr = DateTimeRange("2015-03-22T10:00:00+0900", "2015-03-22T10:10:00+0900")
                 dtr.split("2015-03-22T10:05:00+0900")
@@ -978,15 +1008,15 @@
         """Create a ``DateTimeRange`` instance from a datetime range text.
 
         :param str range_text:
             Input text that includes datetime range.
             e.g. ``2021-01-23T10:00:00+0400 - 2021-01-232T10:10:00+0400``
 
         :param str separator:
-            Regular expression that separating the ``range_text`` to start and end time.
+            Regular expression that separates the ``range_text`` to start and end time.
 
         :return: DateTimeRange
             Created instance.
         """
 
         datetime_ranges = re.split(separator, range_text.strip())
         if len(datetime_ranges) != 2:
```

### Comparing `DateTimeRange-2.2.1/pyproject.toml` & `datetimerange-2.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=61.0"]
+requires = [
+  "setuptools>=64",
+  "setuptools_scm>=7,<8; python_version<'3.8'",
+  "setuptools_scm>=8; python_version>='3.8'",
+]
+
+[tool.setuptools_scm]
+version_scheme = "guess-next-dev"
+local_scheme = "no-local-version"
 
 [tool.black]
 exclude = '''
 /(
       \.eggs
     | \.git
     | \.mypy_cache
@@ -28,16 +36,14 @@
 [tool.coverage.report]
 exclude_lines = [
   'except ImportError',
   'raise NotImplementedError',
   'pass',
   'ABCmeta',
   'abstractmethod',
-  'abstractproperty',
-  'abstractclassmethod',
   'warnings.warn',
 ]
 precision = 1
 show_missing = true
 
 [tool.isort]
 include_trailing_comma = true
```

### Comparing `DateTimeRange-2.2.1/setup.py` & `datetimerange-2.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,28 +41,27 @@
     tests_requires = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "docs_requirements.txt")) as f:
     docs_requires = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description=summary,
     package_data={MODULE_NAME.lower(): ["py.typed"]},
     include_package_data=True,
     keywords=["datetimerange", "datetime", "time range"],
     license=pkg_info["__license__"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     project_urls={
-        "Changlog": f"{REPOSITORY_URL:s}/releases",
+        "Changelog": f"{REPOSITORY_URL:s}/blob/master/CHANGELOG.md",
         "Documentation": f"https://{MODULE_NAME.lower():s}.rtfd.io/",
         "Funding": "https://github.com/sponsors/thombashi",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
     python_requires=">=3.7",
     install_requires=install_requires,
```

### Comparing `DateTimeRange-2.2.1/test/test_dtr.py` & `datetimerange-2.3.0/test/test_dtr.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import pytest
 import pytz
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta
 
 from datetimerange import DateTimeRange
+from datetimerange._core import _normalize_datetime_value
 
 
 TIMEZONE = "+0900"
 START_DATETIME_TEXT = "2015-03-22T10:00:00" + TIMEZONE
 END_DATETIME_TEXT = "2015-03-22T10:10:00" + TIMEZONE
 
 TEST_START_DATETIME = parse(START_DATETIME_TEXT)
@@ -519,14 +520,47 @@
             [DateTimeRange(None, None), False],
         ],
     )
     def test_normal(self, value, expected):
         assert value.is_set() == expected
 
 
+class TestDateTimeRange_is_time_inversion:
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            [DateTimeRange(TEST_START_DATETIME, TEST_END_DATETIME), False],
+            [DateTimeRange(TEST_START_DATETIME, TEST_START_DATETIME), False],
+            [DateTimeRange(TEST_END_DATETIME, TEST_START_DATETIME), True],
+        ],
+    )
+    def test_normal(self, value, expected):
+        assert value.is_time_inversion() == expected
+
+    def test_allow_timezone_mismatch(self):
+        dtr = DateTimeRange("2022-10-29 00:00:00+02:00", "2022-10-31 00:00:00+01:00")
+
+        assert not dtr.is_time_inversion(allow_timezone_mismatch=True)
+
+        with pytest.raises(ValueError):
+            dtr.is_time_inversion(allow_timezone_mismatch=False)
+
+    @pytest.mark.parametrize(
+        ["value"],
+        [
+            [DateTimeRange(None, None)],
+            [DateTimeRange(None, TEST_END_DATETIME)],
+            [DateTimeRange(TEST_START_DATETIME, None)],
+        ],
+    )
+    def test_exception(self, value):
+        with pytest.raises(ValueError):
+            value.is_time_inversion()
+
+
 class TestDateTimeRange_validate_time_inversion:
     @pytest.mark.parametrize(
         ["value"],
         [
             [DateTimeRange(TEST_START_DATETIME, TEST_END_DATETIME)],
             [DateTimeRange(TEST_START_DATETIME, TEST_START_DATETIME)],
         ],
@@ -546,14 +580,22 @@
             [DateTimeRange(TEST_START_DATETIME, None)],
         ],
     )
     def test_exception(self, value):
         with pytest.raises(TypeError):
             value.validate_time_inversion()
 
+    def test_allow_timezone_mismatch(self):
+        dtr = DateTimeRange("2022-10-29 00:00:00+02:00", "2022-10-31 00:00:00+01:00")
+
+        assert not dtr.is_time_inversion(allow_timezone_mismatch=True)
+
+        with pytest.raises(ValueError):
+            dtr.validate_time_inversion(allow_timezone_mismatch=False)
+
 
 class TestDateTimeRange_is_valid_timerange:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             [DateTimeRange(TEST_START_DATETIME, TEST_END_DATETIME), True],
             [DateTimeRange(TEST_END_DATETIME, TEST_START_DATETIME), False],
@@ -631,14 +673,27 @@
     )
     def test_normal(self, value, step, expected):
         results = list(value.range(step))
         assert len(results) == len(expected)
         for value_item, expected_item in zip(results, expected):
             assert value_item == expected_item
 
+    def test_normal_dst(self):
+        dtr = DateTimeRange("2022-10-29 00:00:00+02:00", "2022-10-31 00:00:00+01:00")
+        results = list(dtr.range(timedelta(days=1)))
+        timezone = pytz.timezone("Africa/Tripoli")
+        expected = [
+            _normalize_datetime_value(datetime(2022, 10, 29, 0, 0, 0), timezone=timezone),
+            _normalize_datetime_value(datetime(2022, 10, 30, 0, 0, 0), timezone=timezone),
+            _normalize_datetime_value(datetime(2022, 10, 31, 0, 0, 0), timezone=timezone),
+        ]
+        assert len(results) == len(expected)
+        for value_item, expected_item in zip(results, expected):
+            assert value_item == expected_item
+
     @pytest.mark.parametrize(
         ["value", "step", "expected"],
         [
             [
                 DateTimeRange(datetime(2015, 3, 22, 0, 0, 0), datetime(2015, 3, 22, 0, 1, 0)),
                 relativedelta(seconds=-60),
                 ValueError,
```

### Comparing `DateTimeRange-2.2.1/tox.ini` & `datetimerange-2.3.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,23 @@
     build>=1
     twine
     wheel
 commands =
     python -m build
     twine check dist/*.whl dist/*.tar.gz
 
+[testenv:changelog]
+skip_install = true
+deps =
+    pandoc
+allowlist_externals =
+    pandoc
+commands =
+    pandoc -s CHANGELOG.md -o docs/pages/CHANGELOG.rst
+
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
@@ -57,15 +66,15 @@
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
     isort>=5
     ruff>=0.3.5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
     ruff format
 
 [testenv:lint]
 extras =
     docs
     test
@@ -87,7 +96,13 @@
 
 [testenv:readme]
 changedir = docs
 extras =
     docs
 commands =
     python make_readme.py
+
+[testenv:release]
+deps =
+    releasecmd
+commands =
+    python setup.py release --sign --skip-uploading --verbose
```

