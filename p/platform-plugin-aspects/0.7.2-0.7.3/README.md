# Comparing `tmp/platform_plugin_aspects-0.7.2.tar.gz` & `tmp/platform_plugin_aspects-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.7.2.tar", last modified: Fri Apr 19 16:22:31 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.7.3.tar", last modified: Tue Apr 30 18:32:46 2024, max compression
```

## Comparing `platform_plugin_aspects-0.7.2.tar` & `platform_plugin_aspects-0.7.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.472232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.472232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.513849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.517849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.517849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.517849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.517849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.517849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.513849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.517849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.513849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 18:32:46.000000 platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 18:32:46.521849 platform_plugin_aspects-0.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-04-30 18:32:43.000000 platform_plugin_aspects-0.7.3/setup.py
```

### Comparing `platform_plugin_aspects-0.7.2/CHANGELOG.rst` & `platform_plugin_aspects-0.7.3/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.3 - 2024-04-30
+******************
+
+Fixed
+=====
+
+* Fixed UUID generation for localized Superset assets, which caused embedded
+  dashboards to fail to load when localized.
+
 0.7.2 - 2024-04-19
 ******************
 
 Fixed
 =====
 
 * Fixed cms url configuration
```

### Comparing `platform_plugin_aspects-0.7.2/PKG-INFO` & `platform_plugin_aspects-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.2
+Version: 0.7.3
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
-License: AGPL 3.0
+License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock
 Requires-Dist: celery
 Requires-Dist: django_crum
 Requires-Dist: djangorestframework
@@ -211,17 +212,14 @@
 
 .. _Slack invitation: https://openedx.org/slack
 .. _community Slack workspace: https://openedx.slack.com/
 
 License
 *******
 
-The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted.
-
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 Contributing
 ************
 
 Contributions are very welcome.
 Please read `How To Contribute <https://openedx.org/r/how-to-contribute>`_ for details.
@@ -276,14 +274,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.3 - 2024-04-30
+******************
+
+Fixed
+=====
+
+* Fixed UUID generation for localized Superset assets, which caused embedded
+  dashboards to fail to load when localized.
+
 0.7.2 - 2024-04-19
 ******************
 
 Fixed
 =====
 
 * Fixed cms url configuration
```

### Comparing `platform_plugin_aspects-0.7.2/README.rst` & `platform_plugin_aspects-0.7.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -177,17 +177,14 @@
 
 .. _Slack invitation: https://openedx.org/slack
 .. _community Slack workspace: https://openedx.slack.com/
 
 License
 *******
 
-The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted.
-
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 Contributing
 ************
 
 Contributions are very welcome.
 Please read `How To Contribute <https://openedx.org/r/how-to-contribute>`_ for details.
```

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/extensions/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,21 @@
         """
         course = context["course"]
         dashboards = settings.ASPECTS_INSTRUCTOR_DASHBOARDS
 
         user = get_current_user()
 
         user_language = (
-            get_model("user_preference").get_value(user, "pref-lang") or "en_US"
+            get_model("user_preference").get_value(user, "pref-lang") or "en"
         )
-        formatted_language = user_language.replace("-", "_")
-        if formatted_language not in settings.SUPERSET_DASHBOARD_LOCALES:
-            formatted_language = "en_US"
+        formatted_language = user_language.lower().replace("-", "_")
+        if formatted_language not in [
+            loc.lower().replace("-", "_") for loc in settings.SUPERSET_DASHBOARD_LOCALES
+        ]:
+            formatted_language = "en"
 
         context["course_id"] = course.id
         context = generate_superset_context(
             context,
             dashboards=dashboards,
             language=formatted_language,
         )
```

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/settings/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             "name": "Instructor Dashboard",
             "slug": "instructor-dashboard",
             "uuid": "1d6bf904-f53f-47fd-b1c9-6cd7e284d286",
             "allow_translations": True,
         },
     ]
     settings.SUPERSET_EXTRA_FILTERS_FORMAT = []
-    settings.SUPERSET_DASHBOARD_LOCALES = ["en_US"]
+    settings.SUPERSET_DASHBOARD_LOCALES = ["en"]
     settings.EVENT_SINK_CLICKHOUSE_BACKEND_CONFIG = {
         # URL to a running ClickHouse server's HTTP interface. ex: https://foo.openedx.org:8443/ or
         # http://foo.openedx.org:8123/ . Note that we only support the ClickHouse HTTP interface
         # to avoid pulling in more dependencies to the platform than necessary.
         "url": "http://clickhouse:8123",
         "username": "ch_cms",
         "password": "password",
```

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,8 +264,9 @@
 
 def get_localized_uuid(base_uuid, language):
     """
     Generate an idempotent uuid.
     """
     base_uuid = uuid.UUID(base_uuid)
     base_namespace = uuid.uuid5(base_uuid, "superset")
-    return str(uuid.uuid5(base_namespace, language))
+    normalized_language = language.lower().replace("-", "_")
+    return str(uuid.uuid5(base_namespace, normalized_language))
```

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.2
+Version: 0.7.3
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
-License: AGPL 3.0
+License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock
 Requires-Dist: celery
 Requires-Dist: django_crum
 Requires-Dist: djangorestframework
@@ -211,17 +212,14 @@
 
 .. _Slack invitation: https://openedx.org/slack
 .. _community Slack workspace: https://openedx.slack.com/
 
 License
 *******
 
-The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted.
-
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 Contributing
 ************
 
 Contributions are very welcome.
 Please read `How To Contribute <https://openedx.org/r/how-to-contribute>`_ for details.
@@ -276,14 +274,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.3 - 2024-04-30
+******************
+
+Fixed
+=====
+
+* Fixed UUID generation for localized Superset assets, which caused embedded
+  dashboards to fail to load when localized.
+
 0.7.2 - 2024-04-19
 ******************
 
 Fixed
 =====
 
 * Fixed cms url configuration
```

### Comparing `platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.7.3/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.2/requirements/constraints.txt` & `platform_plugin_aspects-0.7.3/requirements/constraints.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,7 +6,9 @@
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # Common constraints for edx repos
 -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+
+backports.zoneinfo;python_version<"3.9"
```

### Comparing `platform_plugin_aspects-0.7.2/setup.py` & `platform_plugin_aspects-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,26 +157,27 @@
     packages=find_packages(
         include=["platform_plugin_aspects", "platform_plugin_aspects.*"],
         exclude=["*tests"],
     ),
     include_package_data=True,
     install_requires=load_requirements("requirements/base.in"),
     python_requires=">=3.8",
-    license="AGPL 3.0",
+    license="Apache 2.0",
     zip_safe=False,
     keywords="Python edx",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Django",
-        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+        "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         "lms.djangoapp": [
             "platform_plugin_aspects = platform_plugin_aspects.apps:PlatformPluginAspectsConfig",
         ],
         "cms.djangoapp": [
             "platform_plugin_aspects = platform_plugin_aspects.apps:PlatformPluginAspectsConfig",
```

