# Comparing `tmp/freezeyt-1.1.0.tar.gz` & `tmp/freezeyt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freezeyt-1.1.0.tar", last modified: Tue Nov  7 17:07:30 2023, max compression
+gzip compressed data, was "freezeyt-1.1.1.tar", last modified: Tue Apr 30 15:51:45 2024, max compression
```

## Comparing `freezeyt-1.1.0.tar` & `freezeyt-1.1.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-11-07 17:07:30.221760 freezeyt-1.1.0/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1073 2023-08-15 15:14:45.000000 freezeyt-1.1.0/LICENCE.MIT
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    32158 2023-11-07 17:07:30.221760 freezeyt-1.1.0/PKG-INFO
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    30573 2023-10-31 17:59:01.000000 freezeyt-1.1.0/README.md
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-11-07 17:07:30.209760 freezeyt-1.1.0/freezeyt/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      664 2023-11-07 17:03:06.000000 freezeyt-1.1.0/freezeyt/__init__.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)       38 2021-12-07 17:37:42.000000 freezeyt-1.1.0/freezeyt/__main__.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1188 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/actions.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     5286 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/cli.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2524 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/compat.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      959 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/dictsaver.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      833 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/encoding.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2538 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/extra_files.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2792 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/filesaver.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    26554 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/freezer.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2115 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/hooks.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     6672 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/middleware.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3542 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/mimetype_check.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     4424 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/plugins.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      837 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/saver.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      338 2023-08-08 16:47:37.000000 freezeyt-1.1.0/freezeyt/status_handlers.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      258 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/types.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3056 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/url_finders.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     7778 2023-11-07 16:19:28.000000 freezeyt-1.1.0/freezeyt/util.py
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-11-07 17:07:30.210760 freezeyt-1.1.0/freezeyt.egg-info/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    32158 2023-11-07 17:07:30.000000 freezeyt-1.1.0/freezeyt.egg-info/PKG-INFO
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1531 2023-11-07 17:07:30.000000 freezeyt-1.1.0/freezeyt.egg-info/SOURCES.txt
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)        1 2023-11-07 17:07:30.000000 freezeyt-1.1.0/freezeyt.egg-info/dependency_links.txt
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)       47 2023-11-07 17:07:30.000000 freezeyt-1.1.0/freezeyt.egg-info/entry_points.txt
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)        1 2021-08-18 17:35:45.000000 freezeyt-1.1.0/freezeyt.egg-info/not-zip-safe
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)      271 2023-11-07 17:07:30.000000 freezeyt-1.1.0/freezeyt.egg-info/requires.txt
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)        9 2023-11-07 17:07:30.000000 freezeyt-1.1.0/freezeyt.egg-info/top_level.txt
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      382 2023-11-07 16:19:28.000000 freezeyt-1.1.0/pyproject.toml
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1147 2023-11-07 17:07:30.222760 freezeyt-1.1.0/setup.cfg
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)       38 2023-03-07 18:15:23.000000 freezeyt-1.1.0/setup.py
-drwxr-xr-x   0 pviktori  (1000) pviktori  (1000)        0 2023-11-07 17:07:30.219760 freezeyt-1.1.0/tests/
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1583 2023-08-15 16:54:48.000000 freezeyt-1.1.0/tests/test_add_port.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      952 2023-08-08 16:47:37.000000 freezeyt-1.1.0/tests/test_cancel_tasks.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     5211 2022-11-15 18:42:52.000000 freezeyt-1.1.0/tests/test_check_mimetype.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     2172 2022-04-19 18:19:45.000000 freezeyt-1.1.0/tests/test_cleanup.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    11183 2023-08-08 16:47:37.000000 freezeyt-1.1.0/tests/test_click_cli.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)      981 2021-12-07 18:34:53.000000 freezeyt-1.1.0/tests/test_concurrency.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     4737 2023-11-07 16:19:28.000000 freezeyt-1.1.0/tests/test_config.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1121 2021-12-07 17:37:42.000000 freezeyt-1.1.0/tests/test_encoding.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     4995 2022-10-04 16:37:58.000000 freezeyt-1.1.0/tests/test_expected_output.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     7085 2023-11-07 16:19:28.000000 freezeyt-1.1.0/tests/test_extra_files.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     2686 2022-01-25 19:03:13.000000 freezeyt-1.1.0/tests/test_get_css_links.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3229 2023-08-22 17:04:39.000000 freezeyt-1.1.0/tests/test_get_html_links.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1016 2022-04-19 18:19:45.000000 freezeyt-1.1.0/tests/test_get_mimetype.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     4240 2023-08-08 16:23:35.000000 freezeyt-1.1.0/tests/test_gh_pages.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    11635 2023-08-15 15:14:13.000000 freezeyt-1.1.0/tests/test_hooks.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2950 2023-08-22 17:04:39.000000 freezeyt-1.1.0/tests/test_import_variable_from_module.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1958 2023-09-05 16:15:16.000000 freezeyt-1.1.0/tests/test_is_external.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2444 2023-10-31 17:59:01.000000 freezeyt-1.1.0/tests/test_logging.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    10680 2023-10-31 17:59:01.000000 freezeyt-1.1.0/tests/test_middleware.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     4967 2023-08-22 17:04:39.000000 freezeyt-1.1.0/tests/test_mime_db_mimetype.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      717 2023-08-08 16:23:35.000000 freezeyt-1.1.0/tests/test_mimetype_checker.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     1240 2022-04-19 17:05:20.000000 freezeyt-1.1.0/tests/test_multierror.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     1898 2023-09-05 16:25:19.000000 freezeyt-1.1.0/tests/test_parse_absolute_url.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)      961 2023-08-08 16:23:35.000000 freezeyt-1.1.0/tests/test_plugins.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     2212 2022-01-25 19:03:13.000000 freezeyt-1.1.0/tests/test_reason.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     2873 2023-08-08 16:23:35.000000 freezeyt-1.1.0/tests/test_remove_output_dir.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     5092 2023-08-08 16:47:37.000000 freezeyt-1.1.0/tests/test_status_handlers.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3720 2023-08-22 17:04:39.000000 freezeyt-1.1.0/tests/test_testutil.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)    10214 2023-08-22 17:04:39.000000 freezeyt-1.1.0/tests/test_url_finders.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     3438 2023-08-22 16:00:07.000000 freezeyt-1.1.0/tests/test_url_to_path.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)      841 2022-05-03 16:47:25.000000 freezeyt-1.1.0/tests/test_version.py
--rw-rw-r--   0 pviktori  (1000) pviktori  (1000)     3499 2022-01-25 19:03:13.000000 freezeyt-1.1.0/tests/test_wsgi.py
--rw-r--r--   0 pviktori  (1000) pviktori  (1000)     4145 2023-11-07 16:19:28.000000 freezeyt-1.1.0/tests/testutil.py
+drwxr-xr-x   0 encukou   (1000) encukou   (1000)        0 2024-04-30 15:51:45.338029 freezeyt-1.1.1/
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1073 2024-01-09 16:32:47.000000 freezeyt-1.1.1/LICENCE.MIT
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    32322 2024-04-30 15:51:45.338029 freezeyt-1.1.1/PKG-INFO
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    30720 2024-01-09 16:32:47.000000 freezeyt-1.1.1/README.md
+drwxr-xr-x   0 encukou   (1000) encukou   (1000)        0 2024-04-30 15:51:45.336028 freezeyt-1.1.1/freezeyt/
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      664 2024-04-30 15:49:52.000000 freezeyt-1.1.1/freezeyt/__init__.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)       38 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/__main__.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1492 2024-03-19 16:29:27.000000 freezeyt-1.1.1/freezeyt/actions.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     5595 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/cli.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2641 2024-04-30 15:27:27.000000 freezeyt-1.1.1/freezeyt/compat.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2238 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/dictsaver.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      869 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/encoding.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2566 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/extra_files.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3110 2024-03-19 16:29:27.000000 freezeyt-1.1.1/freezeyt/filesaver.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    27760 2024-04-30 15:39:23.000000 freezeyt-1.1.1/freezeyt/freezer.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2487 2024-03-19 16:29:27.000000 freezeyt-1.1.1/freezeyt/hooks.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     6952 2024-04-30 15:27:27.000000 freezeyt-1.1.1/freezeyt/middleware.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3825 2024-03-19 16:29:27.000000 freezeyt-1.1.1/freezeyt/mimetype_check.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     4858 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/plugins.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      888 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/saver.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      338 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/status_handlers.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      660 2024-04-30 15:27:27.000000 freezeyt-1.1.1/freezeyt/types.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3070 2024-01-09 16:32:47.000000 freezeyt-1.1.1/freezeyt/url_finders.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     8215 2024-04-30 15:27:27.000000 freezeyt-1.1.1/freezeyt/util.py
+drwxr-xr-x   0 encukou   (1000) encukou   (1000)        0 2024-04-30 15:51:45.337029 freezeyt-1.1.1/freezeyt.egg-info/
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    32322 2024-04-30 15:51:45.000000 freezeyt-1.1.1/freezeyt.egg-info/PKG-INFO
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1555 2024-04-30 15:51:45.000000 freezeyt-1.1.1/freezeyt.egg-info/SOURCES.txt
+-rw-r--r--   0 encukou   (1000) encukou   (1000)        1 2024-04-30 15:51:45.000000 freezeyt-1.1.1/freezeyt.egg-info/dependency_links.txt
+-rw-r--r--   0 encukou   (1000) encukou   (1000)       47 2024-04-30 15:51:45.000000 freezeyt-1.1.1/freezeyt.egg-info/entry_points.txt
+-rw-r--r--   0 encukou   (1000) encukou   (1000)        1 2024-01-16 17:25:16.000000 freezeyt-1.1.1/freezeyt.egg-info/not-zip-safe
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      288 2024-04-30 15:51:45.000000 freezeyt-1.1.1/freezeyt.egg-info/requires.txt
+-rw-r--r--   0 encukou   (1000) encukou   (1000)        9 2024-04-30 15:51:45.000000 freezeyt-1.1.1/freezeyt.egg-info/top_level.txt
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      442 2024-01-09 16:32:47.000000 freezeyt-1.1.1/pyproject.toml
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1168 2024-04-30 15:51:45.338029 freezeyt-1.1.1/setup.cfg
+-rw-r--r--   0 encukou   (1000) encukou   (1000)       38 2024-01-09 16:32:47.000000 freezeyt-1.1.1/setup.py
+drwxr-xr-x   0 encukou   (1000) encukou   (1000)        0 2024-04-30 15:51:45.337029 freezeyt-1.1.1/tests/
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1583 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_add_port.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      952 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_cancel_tasks.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     5211 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_check_mimetype.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2172 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_cleanup.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    11183 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_click_cli.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      981 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_concurrency.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     5209 2024-04-30 15:46:55.000000 freezeyt-1.1.1/tests/test_config.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     5469 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_dictsaver.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1121 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_encoding.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     4995 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_expected_output.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     7178 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_extra_files.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2686 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_get_css_links.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3229 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_get_html_links.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1016 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_get_mimetype.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     4240 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_gh_pages.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    11635 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_hooks.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2950 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_import_variable_from_module.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1958 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_is_external.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2444 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_logging.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    10680 2024-04-30 15:27:27.000000 freezeyt-1.1.1/tests/test_middleware.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     4967 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_mime_db_mimetype.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      717 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_mimetype_checker.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1240 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_multierror.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     1898 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_parse_absolute_url.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      961 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_plugins.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2212 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_reason.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     2873 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_remove_output_dir.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     5092 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_status_handlers.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3768 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_testutil.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)    10214 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_url_finders.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3438 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_url_to_path.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)      841 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/test_version.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     3499 2024-04-30 15:27:27.000000 freezeyt-1.1.1/tests/test_wsgi.py
+-rw-r--r--   0 encukou   (1000) encukou   (1000)     4177 2024-01-09 16:32:47.000000 freezeyt-1.1.1/tests/testutil.py
```

### Comparing `freezeyt-1.1.0/LICENCE.MIT` & `freezeyt-1.1.1/LICENCE.MIT`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/PKG-INFO` & `freezeyt-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freezeyt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generate static web pages from WSGI apps
 Home-page: https://github.com/encukou/freezeyt
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -35,15 +35,15 @@
 Requires-Dist: flask; extra == "blog"
 Requires-Dist: markdown-it-py; extra == "blog"
 Requires-Dist: pygments; extra == "blog"
 Provides-Extra: typecheck
 Requires-Dist: mypy; extra == "typecheck"
 Requires-Dist: types-click; extra == "typecheck"
 Requires-Dist: types-PyYAML; extra == "typecheck"
-Requires-Dist: types-html5lib; extra == "typecheck"
+Requires-Dist: types-html5lib>=1.1.11.20240228; extra == "typecheck"
 
 # freezeyt
 
 Static web page generator created by the Czech Python community.
 
 
 ## What this does
@@ -299,16 +299,16 @@
 
 ```yaml
 extra_pages:
     - /extra/
     - /extra2.html
 ```
 
-Freezeyt will freeze these pages in addition to those it
-finds by following links.
+Freezeyt will handle these pages as if it found them by following links.
+(For example, by default it will follow links in extra pages.)
 
 Extra pages may also be given on the command line,
 e.g. `--extra-page /extra/ --extra-page /extra2.html`.
 The lists from CLI and the config file are merged together.
 
 You can also specify extra pages using a Python generator,
 specified using a module name and function name as follows:
@@ -337,14 +337,17 @@
 
 
 ### Extra files
 
 Extra files to be included in the output can be specified,
 along with their content.
 
+These files are not considered part of the app; freezeyt will not try to find
+links in them.
+
 This is useful for configuration of your static server.
 (For pages that are part of your website, we recommend
 adding them to your application rather than as extra files.)
 
 If you specify backslashes in `url part`, `freezeyt` convert them to forward slashes.
 
 For example, the following config will add 3 files to
```

### Comparing `freezeyt-1.1.0/README.md` & `freezeyt-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -256,16 +256,16 @@
 
 ```yaml
 extra_pages:
     - /extra/
     - /extra2.html
 ```
 
-Freezeyt will freeze these pages in addition to those it
-finds by following links.
+Freezeyt will handle these pages as if it found them by following links.
+(For example, by default it will follow links in extra pages.)
 
 Extra pages may also be given on the command line,
 e.g. `--extra-page /extra/ --extra-page /extra2.html`.
 The lists from CLI and the config file are merged together.
 
 You can also specify extra pages using a Python generator,
 specified using a module name and function name as follows:
@@ -294,14 +294,17 @@
 
 
 ### Extra files
 
 Extra files to be included in the output can be specified,
 along with their content.
 
+These files are not considered part of the app; freezeyt will not try to find
+links in them.
+
 This is useful for configuration of your static server.
 (For pages that are part of your website, we recommend
 adding them to your application rather than as extra files.)
 
 If you specify backslashes in `url part`, `freezeyt` convert them to forward slashes.
 
 For example, the following config will add 3 files to
```

### Comparing `freezeyt-1.1.0/freezeyt/__init__.py` & `freezeyt-1.1.1/freezeyt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from freezeyt.util import InfiniteRedirection, ExternalURLError, RelativeURLError, UnexpectedStatus, MultiError
 from freezeyt.filesaver import DirectoryExistsError
 from freezeyt.freezer import default_url_to_path as url_to_path
 from freezeyt.middleware import Middleware
 from freezeyt.types import Config
 
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 __all__ = [
     'freeze',
     'freeze_async',
     'url_to_path',
     'Middleware',
     'DirectoryExistsError',
```

### Comparing `freezeyt-1.1.0/freezeyt/cli.py` & `freezeyt-1.1.1/freezeyt/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Command-Line Interface for freezeyt"""
 
 import sys
 import shutil
+from typing import Optional, TextIO, List
 
 import click
 import yaml
 
 from freezeyt import freeze, MultiError
 from freezeyt.util import import_variable_from_module
+from freezeyt.compat import Literal
 
 
 @click.command()
 @click.argument('app', required=False)
 @click.argument('dest_path', required=False, type=click.Path(file_okay=False))
 @click.option('-o', '--output', type=click.Path(file_okay=False),
               help='Absolute or relative path to the output directory')
@@ -34,17 +36,26 @@
 @click.option('--gh-pages/--no-gh-pages', 'gh_pages',
               default=None,
               help='If activated and freeze was successful, create git gh-pages branch in output folder and commit all files to that branch.')
 @click.option('-x', '--fail-fast/--no-fail-fast',
               default=None,
               help='Stop on the first error')
 def main(
-    app, dest_path, output, prefix,
-    extra_pages, config_file, config_var, progress, cleanup, gh_pages, fail_fast
-):
+    app: str,
+    dest_path: str,
+    output: Optional[str],
+    prefix: Optional[str],
+    extra_pages: Optional[List[str]],
+    config_file: Optional[TextIO],
+    config_var: Optional[str],
+    progress: Optional[Literal['none', 'bar', 'log']],
+    cleanup: Optional[bool],
+    gh_pages: Optional[str],
+    fail_fast: Optional[bool],
+) -> None:
     """
     APP
         Name of the Python web app module which will be frozen.
 
     DEST_PATH
         Absolute or relative path to the directory to which the files
     will be frozen.
@@ -55,15 +66,15 @@
         python -m freezeyt demo_app build -c config.yaml
     """
     if config_file and config_var:
         raise click.UsageError(
             "Can't pass configuration both in a file and in a variable."
         )
 
-    elif config_file != None:
+    elif config_file is not None:
         config = yaml.safe_load(config_file)
         if not isinstance(config, dict):
             raise SyntaxError(
                     f'File {config_file.name} is not a YAML dictionary.'
                     )
 
     elif config_var is not None:
```

### Comparing `freezeyt-1.1.0/freezeyt/compat.py` & `freezeyt-1.1.1/freezeyt/compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 """Utilities for compatibility with older versions of Python
 """
 
 import sys
 import asyncio
 import shutil
-from typing import TYPE_CHECKING
+from typing import TypeVar, Coroutine, Any, Optional
 
-if sys.version_info >= (3, 8) or TYPE_CHECKING:
+T = TypeVar('T')
+
+
+if sys.version_info >= (3, 8):
     from typing import Literal
+else:
+    from typing_extensions import Literal
 
 
 if sys.version_info >= (3, 11):
     import wsgiref.types
     StartResponse = wsgiref.types.StartResponse
     WSGIEnvironment = wsgiref.types.WSGIEnvironment
     WSGIApplication = wsgiref.types.WSGIApplication
 else:
     import typing
     StartResponse = typing.Callable
     WSGIEnvironment = dict
     WSGIApplication = typing.Any
 
 
-def asyncio_run(awaitable):
-    """asyncio.run for Python 3.6"""
-    try:
-        aio_run = asyncio.run
-    except AttributeError:
-        # Python 3.6
+if sys.version_info < (3, 7):
+    def asyncio_run(awaitable):
+        """asyncio.run for Python 3.6"""
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(awaitable)
         # We should also call loop.close() here, but that would mean
         # the event loop can't be used in other code:
         # * when using freezeyt as a library, and
         # * in our own tests.
         # So, we cheat a bit and don't call close().
         # (Python 3.6 support is ending soon, anyway.)
-    else:
-        return aio_run(awaitable)
+else:
+    asyncio_run = asyncio.run
 
 
-def asyncio_create_task(coroutine, name):
+def asyncio_create_task(
+    coroutine: 'Coroutine[Any, Any, T]',
+    name: 'Optional[str]',
+) -> 'asyncio.Task[T]':
     """asyncio.create_task for Python 3.6 & 3.7"""
     if sys.version_info < (3, 7):
         # Python 3.6
         return asyncio.ensure_future(coroutine)
     elif sys.version_info < (3, 8):
         # Python 3.7
         return asyncio.create_task(coroutine)
     else:
         return asyncio.create_task(coroutine, name=name)
 
 
-def get_running_loop():
+def get_running_loop() -> asyncio.AbstractEventLoop:
     try:
         get_loop = asyncio.get_running_loop
     except AttributeError:
         # Python 3.6
         return asyncio.get_event_loop()
     else:
         return get_loop()
```

### Comparing `freezeyt-1.1.0/freezeyt/encoding.py` & `freezeyt-1.1.1/freezeyt/encoding.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from urllib.parse import unquote
 
 # See doc/encoding-notes.txt for notes on the string encodings.
 
-def decode_input_path(s):
+def decode_input_path(s: str) -> str:
     r"""Decodes a path from URL (text) for internal use
 
     Examples:
         /čau/☺フ → /čau/☺フ
         /%C4%8Dau → /čau
         /%8Dau → '/\udc8dau'
     """
     return unquote(s, errors='surrogateescape')
 
 
-def encode_wsgi_path(s):
+def encode_wsgi_path(s: str) -> str:
     """Encodes an URL path from internal format for use in WSGI"""
 
     bytestring = s.encode('utf-8', errors='surrogateescape')
     return bytestring.decode('latin-1')
 
 
-def encode_file_path(s):
+def encode_file_path(s: str) -> str:
     """Encodes an URL path from internal format for use in disk filenames"""
     # This doesn't change the string.
     # But, if we ever change the internal representation of paths, we'll
     # need to change the 3 functions here that deal with it
     return s
```

### Comparing `freezeyt-1.1.0/freezeyt/extra_files.py` & `freezeyt-1.1.1/freezeyt/extra_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     )
             else:
                 raise TypeError(
                     'extra_files values must be bytes, str or mappings;'
                     + f' got a {type(content).__name__}'
                 )
 
-def get_url_parts_from_directory(url_part, path):
+def get_url_parts_from_directory(url_part: str, path: Path) -> Iterator[str]:
     """Yield the names of all files in `path`, prefixed by `url_part`.
 
     If `path` is a directory, yield all of its contents recursively.
     """
     if path.is_dir():
         for subpath in path.iterdir():
             yield from get_url_parts_from_directory(
```

### Comparing `freezeyt-1.1.0/freezeyt/filesaver.py` & `freezeyt-1.1.1/freezeyt/filesaver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 import os
 import stat
+from pathlib import Path, PurePosixPath
 
 from . import compat
 from .saver import Saver
+from .types import AbsoluteURL
+
+from typing import Callable, Iterable, BinaryIO
 
 
 class DirectoryExistsError(Exception):
     """Attempt to overwrite directory that doesn't contain freezeyt output"""
 
 
 class FileSaver(Saver):
     """Outputs frozen pages as files on the filesystem.
 
     base - Filesystem base path (eg. /tmp/)
     prefix - Base URL to deploy web app in production
         (eg. url_parse('http://example.com:8000/foo/')
     """
     @staticmethod
-    def add_write_flag(function, path, exception):
+    def add_write_flag(
+        function: Callable[[str], None],
+        path: str,
+        exception: BaseException,
+    ) -> None:
         """A function that adds a write attribute/flag for a path where such an attribute is missing. This function is not necessary on Linux, but on Windows, attempting to delete a file where such an attribute is missing will raise an exception.
-        
+
         Function parameters are:
         function: function which raised the exception,
         path: path name passed to function,
         excinfo: exception information returned by sys.exc_info()
         """
         if not os.access(path, os.W_OK):
             os.chmod(path, os.stat(path).st_mode | stat.S_IWRITE)
-            function(path)
+            return function(path)
         else:
             raise exception
-    
-    def __init__(self, base_path, prefix):
+
+    def __init__(self, base_path: Path, prefix: AbsoluteURL):
         self.base_path = base_path.resolve()
         self.prefix = prefix
 
-    async def prepare(self):
+    async def prepare(self) -> None:
         if self.base_path.exists():
             has_files = list(self.base_path.iterdir())
             has_index = self.base_path.joinpath('index.html').exists()
             if has_files and not has_index:
                 raise DirectoryExistsError(
                     f'Will not overwrite directory {self.base_path}: it '
                     + 'contains files that do not look like a frozen website. '
                     + 'If you are sure, remove the directory before running '
                     + 'freezeyt.'
                 )
-            
+
             compat.rmtree(self.base_path, onexc=self.add_write_flag)
 
-    async def save_to_filename(self, filename, content_iterable):
+    async def save_to_filename(
+        self,
+        filename: PurePosixPath,
+        content_iterable: Iterable[bytes],
+    ) -> None:
         absolute_filename = self.base_path / filename
         assert self.base_path in absolute_filename.parents
 
         loop = compat.get_running_loop()
 
         absolute_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(absolute_filename, "wb") as f:
             for item in content_iterable:
                 await loop.run_in_executor(None, f.write, item)
 
-    async def open_filename(self, filename):
+    async def open_filename(self, filename: PurePosixPath) -> BinaryIO:
         absolute_filename = self.base_path / filename
         assert self.base_path in absolute_filename.parents
 
         return open(absolute_filename, 'rb')
 
-    async def finish(self, success: bool, cleanup: bool):
+    async def finish(self, success: bool, cleanup: bool) -> None:
         """Delete incomplete directory after a failed freeze."""
         if not success and cleanup and self.base_path.exists():
             compat.rmtree(self.base_path)
```

### Comparing `freezeyt-1.1.0/freezeyt/freezer.py` & `freezeyt-1.1.1/freezeyt/freezer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
 from pathlib import Path, PurePosixPath
 import io
 import itertools
 import functools
 import dataclasses
 from typing import Callable, Optional, Mapping, Set, Generator, Dict, Union
-from typing import Tuple, List, TypeVar
-import enum
+from typing import Tuple, List, TypeVar, Any
 import asyncio
 import inspect
 import re
 import urllib.parse
 
 from werkzeug.datastructures import Headers
 from werkzeug.http import parse_options_header, parse_list_header
@@ -20,37 +19,42 @@
 from freezeyt.encoding import encode_wsgi_path, decode_input_path
 from freezeyt.encoding import encode_file_path
 from freezeyt.filesaver import FileSaver
 from freezeyt.dictsaver import DictSaver
 from freezeyt.util import parse_absolute_url, is_external, urljoin
 from freezeyt.util import import_variable_from_module
 from freezeyt.util import InfiniteRedirection, ExternalURLError
-from freezeyt.util import UnexpectedStatus, MultiError, AbsoluteURL
+from freezeyt.util import UnexpectedStatus, MultiError, AbsoluteURL, TaskStatus
 from freezeyt.compat import asyncio_run, asyncio_create_task
 from freezeyt.compat import StartResponse, WSGIEnvironment, WSGIApplication
 from freezeyt import hooks
 from freezeyt.saver import Saver
 from freezeyt.middleware import Middleware
 from freezeyt.actions import ActionFunction
 from freezeyt.url_finders import UrlFinder
 from freezeyt.extra_files import get_extra_files, get_url_parts_from_directory
+from freezeyt.types import Config, SaverResult, WSGIHeaderList
+from freezeyt.types import WSGIExceptionInfo
 
 
 MAX_RUNNING_TASKS = 100
 
 # HTTP status description for status_handlers:
 # 3 digits, or 1 digit and 'xx'.
 STATUS_KEY_RE = re.compile('^[0-9]([0-9]{2}|xx)$')
 
 
-def freeze(app: Optional[WSGIApplication], config):
+def freeze(app: Optional[WSGIApplication], config: Config) -> SaverResult:
     return asyncio_run(freeze_async(app, config))
 
 
-async def freeze_async(app: Optional[WSGIApplication], config):
+async def freeze_async(
+    app: Optional[WSGIApplication],
+    config: Config,
+) -> SaverResult:
     freezer = Freezer(app, config)
     try:
         await freezer.prepare()
         freezer.call_hook('start', freezer.freeze_info)
         await freezer.handle_urls()
         await freezer.handle_redirects()
         return await freezer.finish()
@@ -66,43 +70,49 @@
 
 
 K = TypeVar('K')
 Func = TypeVar('Func', bound=Callable)
 
 def parse_handlers(
     handlers: Mapping[K, Union[str, Func]],
-    default_module: Optional[str]=None
+    default_module: Optional[str]=None,
+    label: str="Handler",
 ) -> Dict[K, Func]:
+    """Map handler/action as callable
+    """
     result = {}
+
     for key, handler_or_name in handlers.items():
         if isinstance(handler_or_name, str):
             handler = import_variable_from_module(
-                handler_or_name, default_module_name=default_module
+                handler_or_name,
+                default_module_name=default_module
             )
         else:
             handler = handler_or_name
+
         if not callable(handler):
             raise TypeError(
-                "Handler for {key!r} in configuration must be a string or a callable,"
-                + f" not {type(handler)}!"
+                f"{label} for {key!r} in configuration must be "
+                + f"a string or a callable, not a {type(handler)}!"
             )
 
         result[key] = handler
 
     return result
 
 
 def default_url_to_path(path: str) -> str:
     if path.endswith('/') or not path:
         path = path + 'index.html'
     return encode_file_path(path)
 
 
 def get_path_from_url(
-    prefix: AbsoluteURL, url: AbsoluteURL, url_to_path,
+    prefix: AbsoluteURL, url: AbsoluteURL, url_to_path: Callable[[str], str],
 ) -> PurePosixPath:
     """Return the disk path to which `url` should be saved.
 
     `url_to_path` is the function given in the config. It takes a string
     and returns a string.
 
     Both arguments should be results of parse_absolute_url.
@@ -111,17 +121,15 @@
         raise ValueError(f'external url {url}')
 
     path = url.path
 
     if path.startswith(prefix.path):
         path = path[len(prefix.path):]
 
-    result = url_to_path(path)
-
-    result = PurePosixPath(result)
+    result = PurePosixPath(url_to_path(path))
 
     if result.is_absolute():
         url_text = urllib.parse.urlunsplit(url)
         raise ValueError(
             f"Path may not be absolute: {result}(from {url_text})"
         )
     assert '.' not in result.parts
@@ -129,45 +137,47 @@
         url_text = urllib.parse.urlunsplit(url)
         raise ValueError(
             f"Path may not contain /../ segment: {result}(from {url_text})"
         )
 
     return result
 
-class TaskStatus(enum.Enum):
-    IN_PROGRESS = "Currently being handled"
-    REDIRECTING = "Waiting for target of redirection"
-    DONE = "Saved"
-    FAILED = "Raised an exception"
-
 @dataclasses.dataclass
 class Task:
     path: PurePosixPath
     urls: "Set[AbsoluteURL]"
     freezer: "Freezer"
     response_headers: Optional[Headers] = None
     response_status: Optional[str] = None
     redirects_to: "Optional[Task]" = None
     reasons: set = dataclasses.field(default_factory=set)
     asyncio_task: "Optional[asyncio.Task]" = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<Task for {self.path}, {self.status.name}>"
 
     def get_a_url(self) -> AbsoluteURL:
         """Get an arbitrary one of the task's URLs."""
         return next(iter(self.urls))
 
     @property
     def status(self) -> TaskStatus:
         for status, collection in self.freezer.task_collections.items():
             if self.path in collection:
                 return status
         raise ValueError(f'Task not registered with freezer: {self}')
 
+    def update_status(self, old_status, new_status):
+        assert self.status == old_status
+        old_collection = self.freezer.task_collections[old_status]
+        del old_collection[self.path]
+        new_collection = self.freezer.task_collections[new_status]
+        assert self.path not in new_collection
+        new_collection[self.path] = self
+
 class IsARedirect(BaseException):
     """Raised when a page redirects and freezing it should be postponed"""
 
 class IgnorePage(BaseException):
     """Raised when freezing a page should be ignored"""
 
 class VersionMismatch(ValueError):
@@ -196,26 +206,29 @@
     task_collections: Dict[TaskStatus, TaskCollection]
     done_tasks: TaskCollection
     redirecting_tasks: TaskCollection
     inprogress_tasks: TaskCollection
     failed_tasks: TaskCollection
     extra_pages: ExtraPagesConfig
     hooks: Dict[str, List[Callable]]
-    url_to_path: Union[str, Callable[[str], str]]
+    url_to_path: Callable[[str], str]
+    fail_fast: bool
 
     url_finders: Dict[str, UrlFinder]
     status_handlers: Dict[str, ActionFunction]
 
-    def __init__(self, app: Optional[WSGIApplication], config: dict):
-        self.config = config
+    def __init__(self, app: Optional[WSGIApplication], config: Config):
+        self.config = dict(config)
+        del config  # we always want to use `self.config` from now on
+
         self.check_version(self.config.get('version'))
 
         self.freeze_info = hooks.FreezeInfo(self)
 
-        app_config = config.get('app')
+        app_config = self.config.get('app')
         if app is None:
             if app_config is None:
                 raise ValueError("Application is required")
 
             if isinstance(app_config, str):
                 # config file/variable or command line argument
                 app = import_variable_from_module(
@@ -225,76 +238,81 @@
                 # config variable - app as object
                 app = app_config
         else:
             if app_config is not None:
                 raise ValueError("Application is specified both as parameter and in configuration")
             app = app
 
-        self.app = Middleware(app, config)
+        # The original app, to be passed back to the user when needed
+        self.user_app = app
+
+        # The app we call, wrapped in Middleware
+        self.app = Middleware(app, self.config)
 
         self.fail_fast = self.config.get('fail_fast', False)
 
         if self.config.get("gh_pages", False):
-            plugins = config.setdefault('plugins', [])
+            plugins = self.config.setdefault('plugins', [])
             if 'freezeyt.plugins:GHPagesPlugin' not in plugins:
                 plugins.append('freezeyt.plugins:GHPagesPlugin')
         if self.config.get("gh_pages", False) is False:
-            plugins = config.setdefault('plugins', [])
+            plugins = self.config.setdefault('plugins', [])
             if 'freezeyt.plugins:GHPagesPlugin' in plugins:
                 plugins.remove('freezeyt.plugins:GHPagesPlugin')
 
         CONFIG_DATA = (
             ('extra_pages', ()),
             ('url_to_path', default_url_to_path)
         )
         for attr_name, default in CONFIG_DATA:
-            setattr(self, attr_name, config.get(attr_name, default))
+            setattr(self, attr_name, self.config.get(attr_name, default))
 
         if isinstance(self.url_to_path, str):
             self.url_to_path = import_variable_from_module(self.url_to_path)
 
-        if config.get('use_default_url_finders', True):
+        if self.config.get('use_default_url_finders', True):
             _url_finders = dict(
-                DEFAULT_URL_FINDERS, **config.get('url_finders', {})
+                DEFAULT_URL_FINDERS, **self.config.get('url_finders', {})
             )
         else:
-            _url_finders = config.get('url_finders', {})
+            _url_finders = self.config.get('url_finders', {})
 
         self.url_finders = parse_handlers(
-            _url_finders, default_module='freezeyt.url_finders'
+            _url_finders, default_module='freezeyt.url_finders', label="URL finder"
         )
 
-        _status_handlers = config.get('status_handlers', {})
+        _status_handlers = self.config.get('status_handlers', {})
         for key in _status_handlers:
             if not STATUS_KEY_RE.fullmatch(key):
                 raise ValueError(
-                    'Status descriptions must be strings with 3 digits or one '
-                    + f'digit and "xx", got f{key!r}'
+                    "Status description must be string with three digits (e.g. 200)"
+                    + " or a status group, one digit with 'xx' (e.g. 2xx),"
+                    + f" got f{key!r}"
                 )
 
         self.status_handlers = parse_handlers(
-            _status_handlers, default_module='freezeyt.actions'
+            _status_handlers, default_module='freezeyt.actions', label="Status handler"
         )
 
-        prefix = config.get('prefix', 'http://localhost:8000/')
+        prefix = self.config.get('prefix', 'http://localhost:8000/')
 
         # Decode path in the prefix URL.
         # Save the parsed version of prefix as self.prefix
         prefix_parsed = parse_absolute_url(prefix)
         decoded_path = decode_input_path(prefix_parsed.path)
         if not decoded_path.endswith('/'):
             raise ValueError('prefix must end with /')
         self.prefix = prefix_parsed._replace(path=decoded_path)
 
-        output = config['output']
+        output = self.config['output']
         if isinstance(output, str):
             output = {'type': 'dir', 'dir': output}
 
         if output['type'] == 'dict':
-            self.saver = DictSaver(self.prefix)
+            self.saver = DictSaver()
         elif output['type'] == 'dir':
             try:
                 output_dir = output['dir']
             except KeyError:
                 raise ValueError("output directory not specified")
             self.saver = FileSaver(Path(output_dir), self.prefix)
         else:
@@ -316,57 +334,57 @@
         }
         if "//" in prefix_parsed.path:
             self.warnings.append(
                 f"Freezeyt reduces multiple consecutive slashes in {prefix!r} to one"
             )
 
         self.hooks = {}
-        for name, funcs in config.get('hooks', {}).items():
+        for name, funcs in self.config.get('hooks', {}).items():
             for func in funcs:
                 if isinstance(func, str):
                     func = import_variable_from_module(func)
                 self.add_hook(name, func)
 
-        for plugin in config.get('plugins', {}):
+        for plugin in self.config.get('plugins', {}):
             if isinstance(plugin, str):
                 plugin = import_variable_from_module(plugin)
             plugin(self.freeze_info)
 
         self.semaphore = asyncio.Semaphore(MAX_RUNNING_TASKS)
 
 
-    def check_version(self, config_version):
+    def check_version(self, config_version: Union[str, float, None]) -> None:
         if config_version is None:
             return
         if not isinstance(config_version, float):
             main_version = str(config_version).split(".")[0]
         else:
             raise VersionMismatch("The specified version has to be string or int i.e. 1, 1.1 or '1', '1.1'.")
 
         current_version = freezeyt.__version__.split(".")[0]
         if main_version != current_version:
             raise VersionMismatch("The specified version does not match the freezeyt main version.")
 
-    def add_hook(self, hook_name, func):
+    def add_hook(self, hook_name: str, func: Callable) -> None:
         self.hooks.setdefault(hook_name, []).append(func)
 
-    async def cancel_tasks(self):
+    async def cancel_tasks(self) -> None:
         cancelled_atasks = []
         while self.inprogress_tasks:
             path, task = self.inprogress_tasks.popitem()
             assert task.asyncio_task is not None
             task.asyncio_task.cancel()
             cancelled_atasks.append(task.asyncio_task)
         for atask in cancelled_atasks:
             try:
                 await atask
             except asyncio.CancelledError:
                 pass
 
-    async def finish(self):
+    async def finish(self) -> SaverResult:
         success = not self.failed_tasks
         cleanup = self.config.get("cleanup", True)
         result = await self.saver.finish(success, cleanup)
         if success:
             self.call_hook('success', self.freeze_info)
 
             for task in self.done_tasks.values():
@@ -391,15 +409,18 @@
         """Add a task to freeze the given URL
 
         If no task is added (e.g. for external URLs), return None.
         """
         task = self._add_task(url, external_ok=external_ok, reason=reason)
         if task and task.asyncio_task is None:
             coroutine = self.handle_one_task(task)
-            task.asyncio_task = asyncio_create_task(coroutine, name=task.path)
+            task.asyncio_task = asyncio_create_task(
+                coroutine,
+                name=str(task.path),
+            )
         return task
 
     def _add_task(
         self,
         url: AbsoluteURL,
         *,
         external_ok: bool = False,
@@ -423,48 +444,57 @@
             # Here, this means the task wasn't found.
             task = Task(path, {url}, self)
             self.inprogress_tasks[path] = task
         if reason:
             task.reasons.add(reason)
         return task
 
-    async def prepare(self):
+    async def prepare(self) -> None:
         """Preparatory method for creating tasks and preparing the saver."""
         # prepare the tasks
         self.add_task(self.prefix, reason='site root (homepage)')
         for url_part, kind, content_or_path in get_extra_files(self.config):
             if kind == 'content':
                 # join part with path, otherwise filename 'http:' overwrite prefix
                 assert self.prefix.path.endswith('/')
                 assert not url_part.startswith('/')
                 url_part = self.prefix.path + url_part
                 self.add_task(
                     urljoin(self.prefix, url_part),
                     reason="from extra_files",
                 )
             elif kind == 'path':
+                assert isinstance(content_or_path, Path)
                 for part in get_url_parts_from_directory(
                     url_part, content_or_path
                 ):
                 # join part with path, otherwise filename 'http:' overwrite prefix
                     assert self.prefix.path.endswith('/')
                     assert not url_part.startswith('/')
                     part = self.prefix.path + part
                     self.add_task(
                         urljoin(self.prefix, part),
                         reason="from extra_files",
                     )
+            else:
+                raise ValueError(kind)
         self._add_extra_pages(self.prefix, self.extra_pages)
 
         # and at the end prepare the saver
-        await self.saver.prepare()
+        return await self.saver.prepare()
 
     def start_response(
-        self, task, url, wsgi_write, status, headers, exc_info=None,
-    ):
+        self,
+        task: Task,
+        url: AbsoluteURL,
+        wsgi_write: Func,
+        status: str,
+        headers: WSGIHeaderList,
+        exc_info: WSGIExceptionInfo = None,
+    ) -> Func:
         """WSGI start_response hook
 
         The application we are freezing will call this method
         and supply the status, headers, exc_info arguments.
         (self and wsgi_write are provided by freezeyt.)
 
         See: https://www.python.org/dev/peps/pep-3333/#the-start-response-callable
@@ -511,15 +541,19 @@
             raise IgnorePage()
         elif status_action == 'follow':
             raise IsARedirect()
         else:
             raise UnexpectedStatus(url, status)
 
 
-    def _add_extra_pages(self, prefix, extras: ExtraPagesConfig):
+    def _add_extra_pages(
+        self,
+        prefix: AbsoluteURL,
+        extras: ExtraPagesConfig,
+    ) -> None:
         """Add URLs of extra pages from config.
 
         Handles both literal URLs and generators.
         """
         for extra in extras:
             if isinstance(extra, dict):
                 try:
@@ -527,43 +561,42 @@
                 except KeyError:
                     raise ValueError(
                         'extra_pages must be strings or dicts with '
                         + f'a "generator" key, not `{extra}`'
                     )
                 if isinstance(generator, str):
                     generator = import_variable_from_module(generator)
-                self._add_extra_pages(prefix, generator(self.app))
+                self._add_extra_pages(prefix, generator(self.user_app))
             elif isinstance(extra, str):
                 url = urljoin(prefix, decode_input_path(extra))
                 try:
                     self.add_task(
                         url,
                         reason='extra page',
                     )
                 except ExternalURLError:
                     raise ExternalURLError(f'External URL specified in extra_pages: {url}')
             else:
                 generator = extra
-                self._add_extra_pages(prefix, generator(self.app))
+                self._add_extra_pages(prefix, generator(self.user_app))
 
-    async def handle_urls(self):
+    async def handle_urls(self) -> None:
         while self.inprogress_tasks:
             # Get an item from self.inprogress_tasks.
             # Since this is a dict, we can't do self.inprogress_tasks[0];
             # and since we don't want to change it we can't use pop().
             # So, start iterating over it, and break the loop immediately
             # when we get the first item.
             for path, task in self.inprogress_tasks.items():
                 break
             assert task.asyncio_task is not None
             try:
                 await task.asyncio_task
             except Exception as exc:
-                del self.inprogress_tasks[task.path]
-                self.failed_tasks[task.path] = task
+                task.update_status(TaskStatus.IN_PROGRESS, TaskStatus.FAILED)
                 self.call_hook('page_failed', hooks.TaskInfo(task))
                 if self.fail_fast:
                     raise exc
             if path in self.inprogress_tasks:
                 raise ValueError(f'{task} is in_progress after it was handled')
 
     @needs_semaphore
@@ -620,16 +653,15 @@
         # Call the application. All calls to write (wsgi_write_data.append)
         # must be done as part of this call.
         try:
             result_iterable = self.app(environ, start_response)
         except IsARedirect:
             return
         except IgnorePage:
-            del self.inprogress_tasks[task.path]
-            self.done_tasks[task.path] = task
+            task.update_status(TaskStatus.IN_PROGRESS, TaskStatus.DONE)
             return
 
         try:
             # Combine the list of data from write() with the returned
             # iterable object.
             full_result = itertools.chain(
                 wsgi_write_data,
@@ -683,42 +715,39 @@
                         raise ValueError(f'Invalid Link header: {link!r}')
                     new_url = urljoin(url, link_text)
                     self.add_task(
                         new_url, external_ok=True,
                         reason=f'Link header from: {task.path}',
                     )
 
-        del self.inprogress_tasks[task.path]
-        self.done_tasks[task.path] = task
+        task.update_status(TaskStatus.IN_PROGRESS, TaskStatus.DONE)
 
         self.call_hook('page_frozen', hooks.TaskInfo(task))
 
     @needs_semaphore
-    async def handle_redirects(self):
+    async def handle_redirects(self) -> None:
         """Save copies of target pages for redirect_policy='follow'"""
         while self.redirecting_tasks:
             saved_something = False
             for key, task in list(self.redirecting_tasks.items()):
                 assert task.redirects_to is not None
                 if task.redirects_to.status == TaskStatus.FAILED:
                     # Don't process redirects to a failed pages
-                    del self.redirecting_tasks[key]
-                    self.done_tasks[task.path] = task
+                    task.update_status(TaskStatus.REDIRECTING, TaskStatus.DONE)
                     continue
                 if task.redirects_to.status != TaskStatus.DONE:
                     continue
 
                 with await self.saver.open_filename(task.redirects_to.path) as f:
                     await self.saver.save_to_filename(task.path, f)
                 self.call_hook('page_frozen', hooks.TaskInfo(task))
-                del self.redirecting_tasks[key]
-                self.done_tasks[task.path] = task
+                task.update_status(TaskStatus.REDIRECTING, TaskStatus.DONE)
                 saved_something = True
             if not saved_something:
                 # Get some task (the first one we get by iteration) for the
                 # error message.
                 for task in self.redirecting_tasks.values():
                     raise InfiniteRedirection(task)
 
-    def call_hook(self, hook_name, *arguments):
+    def call_hook(self, hook_name: str, *arguments: Any) -> None:
         for hook in self.hooks.get(hook_name, ()):
             hook(*arguments)
```

### Comparing `freezeyt-1.1.0/freezeyt/hooks.py` & `freezeyt-1.1.1/freezeyt/hooks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,84 @@
-from typing import Iterable
+from typing import Iterable, Callable, Optional, TYPE_CHECKING
 import urllib.parse
 
 from freezeyt.util import parse_absolute_url
 
+
+if TYPE_CHECKING:
+    from freezeyt.freezer import Freezer, Task
+
 class TaskInfo:
     """Public information about a task that's being saved"""
-    def __init__(self, task):
+    def __init__(self, task: 'Task'):
         self._task = task
         self._freezer = task.freezer
 
-    def get_a_url(self):
+    def get_a_url(self) -> str:
         """Return a URL of this page"""
         return urllib.parse.urlunsplit(self._task.get_a_url())
 
     @property
-    def path(self):
+    def path(self) -> str:
         """The relative path the content is saved to"""
         return str(self._task.path)
 
     @property
-    def freeze_info(self):
+    def freeze_info(self) -> 'FreezeInfo':
         return self._freezer.freeze_info
 
     @property
-    def exception(self):
-        if self._task.asyncio_task.done():
-            return self._task.asyncio_task.exception()
+    def exception(self) -> Optional[BaseException]:
+        aio_task = self._task.asyncio_task
+        if aio_task is None:
+            return None
+        if aio_task.done():
+            return aio_task.exception()
         else:
             return None
 
     @property
     def reasons(self) -> Iterable[str]:
         """A list of strings explaining why the given page was visited.
 
         New entries may be added as the freezing goes on.
         """
         return sorted(self._task.reasons)
 
 
 class FreezeInfo:
-    def __init__(self, freezer):
+    """Public information about a freezer"""
+
+    def __init__(self, freezer: 'Freezer'):
         self._freezer = freezer
 
-    def add_url(self, url, reason=None):
+    def add_url(self, url: str, reason: Optional[str] = None) -> None:
         self._freezer.add_task(parse_absolute_url(url), reason=reason)
 
-    def add_hook(self, hook_name, func):
+    def add_hook(self, hook_name: str, func: Callable) -> None:
         self._freezer.add_hook(hook_name, func)
 
     @property
-    def fail_fast(self):
+    def fail_fast(self) -> bool:
         return self._freezer.fail_fast
 
     @property
-    def total_task_count(self):
+    def total_task_count(self) -> int:
         return sum(
             len(tasks) for tasks in self._freezer.task_collections.values()
         )
 
     @property
-    def done_task_count(self):
+    def done_task_count(self) -> int:
         # Import TaskStatus here to avoid a circular import
         # (since freezer imports hooks)
         from freezeyt.freezer import TaskStatus
         return (
             len(self._freezer.task_collections[TaskStatus.FAILED])
             + len(self._freezer.task_collections[TaskStatus.DONE])
         )
 
     @property
-    def failed_task_count(self):
+    def failed_task_count(self) -> int:
         # Import TaskStatus here, see done_task_count
         from freezeyt.freezer import TaskStatus
         return len(self._freezer.task_collections[TaskStatus.FAILED])
```

### Comparing `freezeyt-1.1.0/freezeyt/middleware.py` & `freezeyt-1.1.1/freezeyt/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Iterable
+from typing import Iterable, Callable
 import io
 
 from werkzeug.wrappers import Response
 from werkzeug.exceptions import NotFound, Forbidden, MethodNotAllowed
 from werkzeug.routing import Map, Rule, RequestRedirect
 from werkzeug.security import safe_join
 from werkzeug.utils import send_file
 
 from freezeyt.compat import StartResponse, WSGIEnvironment, WSGIApplication
 from freezeyt.mimetype_check import MimetypeChecker
 from freezeyt.extra_files import get_extra_files
+from freezeyt.types import Config, WSGIHeaderList, WSGIExceptionInfo
 
 
 class Middleware:
-    def __init__(self, app: WSGIApplication, config):
+    def __init__(self, app: WSGIApplication, config: Config):
         self.app = app
         self.mimetype_checker = MimetypeChecker(config)
         self.url_map = Map()
         for url_part, kind, content_or_path in get_extra_files(config):
             if '<' in url_part:
                 raise NotImplementedError("the extra file URL cannot include '<'")
             if kind == 'content':
@@ -124,22 +125,29 @@
             except OSError:
                 # This could have several different behaviors,
                 # see https://github.com/encukou/freezeyt/issues/331
                 # For now, return a 404
                 response = NotFound()
             return response(environ, server_start_response)
 
-        def mw_start_response(status, headers, exc_info=None):
+        def mw_start_response(
+            status: str,
+            headers: WSGIHeaderList,
+            exc_info: WSGIExceptionInfo = None,
+        ) -> Callable[[bytes], object]:
             result = server_start_response(status, headers, exc_info)
             self.mimetype_checker.check(path_info, headers)
             return result
 
         return self.app(environ, mw_start_response)
 
-    def  handle_non_get(self, environ, server_start_response):
+    def handle_non_get(
+        self, environ: WSGIEnvironment,
+        server_start_response: StartResponse,
+    ) -> Iterable[bytes]:
         # Handle requests other than GET. These can't come from Freezeyt.
         if not self.static_mode:
             # Normally, pass all other requests to the app unchanged.
             return self.app(environ, server_start_response)
 
         # In static mode, disallow everything but GET, HEAD, OPTIONS.
 
@@ -160,14 +168,14 @@
             return []
         elif environ['REQUEST_METHOD'] == 'OPTIONS':
             # For OPTIONS, give our own response
             # (The status should be '204 No Content', but according to
             # MDN, some browsers misinterpret that, so '200' is safer.)
             server_start_response(
                 '200 No Content',
-                {'Allow': 'GET, HEAD, OPTIONS'},
+                [('Allow', 'GET, HEAD, OPTIONS')],
             )
             return []
         else:
             # Disallow other methods
             response = MethodNotAllowed()
             return response(environ, server_start_response)
```

### Comparing `freezeyt-1.1.0/freezeyt/mimetype_check.py` & `freezeyt-1.1.1/freezeyt/mimetype_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from mimetypes import guess_type
 import json
-from typing import Optional, List, Mapping, Dict
+from typing import Optional, List, Mapping, Dict, Callable
 import functools
 from pathlib import PurePosixPath
 
 from werkzeug.datastructures import Headers
 from werkzeug.http import parse_options_header
 
 from freezeyt.util import WrongMimetypeError
 from freezeyt.util import import_variable_from_module
+from freezeyt.types import Config, WSGIHeaderList
 
 
+GetMimetypeFunction = Callable[[str], Optional[List[str]]]
+
 class MimetypeChecker:
-    def __init__(self, config):
+    default_mimetype: str
+    get_mimetype: GetMimetypeFunction
+
+    def __init__(self, config: Config):
         self.default_mimetype = config.get(
             'default_mimetype', 'application/octet-stream')
         get_mimetype = config.get('get_mimetype', default_mimetype)
         mime_db_file = config.get('mime_db_file', None)
 
         if mime_db_file:
             with open(mime_db_file) as file:
@@ -26,23 +32,23 @@
             get_mimetype = functools.partial(mime_db_mimetype, mime_db)
 
         if isinstance(get_mimetype, str):
             get_mimetype = import_variable_from_module(get_mimetype)
 
         self.get_mimetype = get_mimetype
 
-    def check(self, url, headers):
+    def check(self, url: str, headers: WSGIHeaderList) -> None:
         check_mimetype(
             url,
             headers,
             self.default_mimetype,
             get_mimetype=self.get_mimetype,
         )
 
-    def guess_mimetype(self, url):
+    def guess_mimetype(self, url: str) -> str:
         """Return a single best guess of the mimetype for url"""
         types = self.get_mimetype(url)
         if types is None:
             return self.default_mimetype
         return types[0]
 
 
@@ -54,31 +60,33 @@
     if file_mimetype is None:
         return None
     else:
         return [file_mimetype]
 
 
 def check_mimetype(
-    url_path, headers,
-    default='application/octet-stream', *, get_mimetype=default_mimetype,
-):
+    url_path: str,
+    headers: WSGIHeaderList,
+    default: str = 'application/octet-stream',
+    *,
+    get_mimetype: GetMimetypeFunction = default_mimetype,
+) -> None:
     """Ensure mimetype sent from headers with file mimetype guessed
     from its suffix.
     Raise WrongMimetypeError if they don't match.
     """
     if url_path.endswith('/'):
         # Directories get saved as index.html
         url_path = 'index.html'
     file_mimetypes = get_mimetype(url_path)
     if file_mimetypes is None:
         file_mimetypes = [default]
 
-    headers = Headers(headers)
     headers_mimetype, encoding = parse_options_header(
-        headers.get('Content-Type')
+        Headers(headers).get('Content-Type')
     )
 
     if isinstance(file_mimetypes, str):
         raise TypeError("get_mimetype result must not be a string")
 
     if headers_mimetype.lower() not in (m.lower() for m in file_mimetypes):
         raise WrongMimetypeError(file_mimetypes, headers_mimetype, url_path)
```

### Comparing `freezeyt-1.1.0/freezeyt/plugins.py` & `freezeyt-1.1.1/freezeyt/plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,105 @@
 import traceback
 import sys
 from subprocess import check_output, CalledProcessError, STDOUT
 from textwrap import dedent
+from typing import List
 
 import enlighten
 import click
 
+from freezeyt.hooks import FreezeInfo, TaskInfo
+from freezeyt.filesaver import FileSaver
+
 class GitCommandError(ValueError):
     """An exception occurred while executing git commands."""
 
 class ProgressBarPlugin:
     bar_format = '{percentage:3.0f}%▕{bar}▏{elapsed}, {rate:.2f} pg/s'
-    def __init__(self, freeze_info):
+    def __init__(self, freeze_info: FreezeInfo):
         self.manager = enlighten.get_manager()
         self.counter = self.manager.counter(
             total=100, color='red', bar_format=self.bar_format)
         self.failure_counter = self.counter
         self.success_counter = self.counter.add_subcounter('cyan')
         freeze_info.add_hook('page_frozen', self.update_bar)
         freeze_info.add_hook('page_failed', self.update_bar)
 
-    def update_bar(self, task_info):
+    def update_bar(self, task_info: TaskInfo) -> None:
         self.counter.total = task_info.freeze_info.total_task_count
         self.counter.count = task_info.freeze_info.done_task_count
         self.success_counter.count = (
             task_info.freeze_info.done_task_count
             - task_info.freeze_info.failed_task_count
         )
         self.counter.update(0)
 
 class LogPlugin:
-    def __init__(self, freeze_info):
+    def __init__(self, freeze_info: FreezeInfo):
         freeze_info.add_hook('page_frozen', self.page_frozen)
         freeze_info.add_hook('page_failed', self.page_failed)
 
-    def _summary(self, freeze_info):
+    def _summary(self, freeze_info: FreezeInfo) -> str:
         total = freeze_info.total_task_count
         failed = freeze_info.failed_task_count
         done = freeze_info.done_task_count
         progress = done / total
         result = [
             f'[{done:{len(str(total))}d}/{total}, ~{progress:3.0%}'
         ]
         if failed:
             result.append(f', {failed} errors')
         result.append(']')
         return ''.join(result)
 
-    def page_frozen(self, task_info):
+    def page_frozen(self, task_info: TaskInfo) -> None:
         summary = click.style(self._summary(task_info.freeze_info), fg='cyan')
         click.echo(f'{summary} {task_info.path}', file=sys.stderr)
 
-    def page_failed(self, task_info):
+    def page_failed(self, task_info: TaskInfo) -> None:
         summary = click.style(self._summary(task_info.freeze_info), fg='red')
         click.echo(f'{summary} ERROR in {task_info.path}', file=sys.stderr)
         exc = task_info.exception
+        assert exc is not None
         if not task_info._freezer.freeze_info.fail_fast:
             traceback.print_exception(type(exc), exc, exc.__traceback__)
 
 class GHPagesPlugin:
-    def __init__(self, freeze_info):
+    def __init__(self, freeze_info: FreezeInfo):
         if freeze_info._freezer.prefix.path != "/":
             raise ValueError("When using the Github Pages plugin, you can't specify a path in the prefix, so github can't handle it.")
+        if not isinstance(freeze_info._freezer.saver, FileSaver):
+            raise ValueError("When using the Github Pages plugin, you must save to a directory.")
         self.base_path = freeze_info._freezer.saver.base_path
-        self.prefix_host = freeze_info._freezer.prefix.hostname
+        hostname = freeze_info._freezer.prefix.hostname
+        assert hostname is not None
+        self.prefix_host = hostname
         freeze_info.add_hook('success', self.github_pages)
 
-    def github_pages(self, freeze_info):
+    def github_pages(self, freeze_info: FreezeInfo) -> None:
         if self.base_path.exists():
             (self.base_path / "CNAME").write_text(self.prefix_host)
             (self.base_path / ".nojekyll").write_text("")
-            try:
-                sp_params = {"stderr": STDOUT,
-                             "cwd": self.base_path,
-                             "env": {   "GIT_CONFIG_NOSYSTEM": "1",
-                                        "GIT_AUTHOR_NAME": "gh_pages",
-                                        "GIT_AUTHOR_EMAIL": "gh@mail.invalid",
-                                        "GIT_COMMITTER_NAME": "gh_pages",
-                                        "GIT_COMMITTER_EMAIL": "gh@mail.invalid"
-                                    }
-                             }
-                check_output(["git", "init", "-b", "gh-pages"], **sp_params)
-                check_output(["git", "add", "."], **sp_params)
+            def run_git(command: List[str]) -> None:
                 check_output(
-                    ["git", "commit", "-m", "added all freezed files"], **sp_params)
+                    command,
+                    stderr=STDOUT,
+                    cwd=self.base_path,
+                    env={
+                        "GIT_CONFIG_NOSYSTEM": "1",
+                        "GIT_AUTHOR_NAME": "gh_pages",
+                        "GIT_AUTHOR_EMAIL": "gh@mail.invalid",
+                        "GIT_COMMITTER_NAME": "gh_pages",
+                        "GIT_COMMITTER_EMAIL": "gh@mail.invalid",
+                    },
+                )
+            try:
+                run_git(["git", "init", "-b", "gh-pages"])
+                run_git(["git", "add", "."])
+                run_git(["git", "commit", "-m", "added all freezed files"])
             except CalledProcessError as e:
                 raise GitCommandError(f"""
                       Freezing was successful, but a problem occurs during the execution of one of commands for creating git gh-pages branch:
                       command: {e.cmd}
                       captured standard output with error:
                       {e.stdout.decode()}""")
             else:
```

### Comparing `freezeyt-1.1.0/freezeyt/saver.py` & `freezeyt-1.1.1/freezeyt/saver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
 from pathlib import PurePosixPath
-from typing import BinaryIO, Any, Iterable
+from typing import BinaryIO, Iterable
+
+from freezeyt.types import SaverResult
 
 class Saver(abc.ABC):
-    async def prepare(self):
+    async def prepare(self) -> None:
         """Initialize the saver."""
 
     @abc.abstractmethod
     async def save_to_filename(
         self,
         filename: PurePosixPath,
         content_iterable: "Iterable[bytes]",
@@ -17,14 +19,14 @@
     @abc.abstractmethod
     async def open_filename(
         self,
         filename: PurePosixPath,
     ) -> BinaryIO:
         """Open the given path for reading bytes"""
 
-    async def finish(self, success: bool, cleanup: bool) -> Any:
+    async def finish(self, success: bool, cleanup: bool) -> SaverResult:
         """Clean up after a freeze and return the result, if any.
 
         success: true if the freeze was successful
         cleanup: If true, clean up after failed freezes
         """
         return None
```

### Comparing `freezeyt-1.1.0/freezeyt/url_finders.py` & `freezeyt-1.1.1/freezeyt/url_finders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import xml.etree.ElementTree
-from typing import Iterable, BinaryIO, List, Optional, Tuple, Callable
+from typing import Iterable, BinaryIO, Optional, Callable
 from typing import Coroutine, Union, Any, TYPE_CHECKING
 
 import html5lib
 import cssutils
 
 from werkzeug.datastructures import Headers
 from werkzeug.http import parse_options_header
 
 from . import compat
 from .util import process_pool_executor
+from .types import WSGIHeaderList
 
 
-_Headers = Optional[List[Tuple[str, str]]]
+_Headers = Optional[WSGIHeaderList]
 UrlFinder = Callable[
     [BinaryIO, str, _Headers],
     Union[Iterable[str], Coroutine[Any, Any, Iterable[str]]],
 ]
 
 
 def _get_css_links(
```

### Comparing `freezeyt-1.1.0/freezeyt/util.py` & `freezeyt-1.1.1/freezeyt/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 import importlib
 import concurrent.futures
 import urllib.parse
-from typing import Sequence, TYPE_CHECKING
+from typing import Sequence, TYPE_CHECKING, List, Optional, Any
+import enum
 
 from werkzeug.urls import uri_to_iri
 
 from freezeyt.compat import _MultiErrorBase, HAVE_EXCEPTION_GROUP
 from freezeyt.encoding import decode_input_path
 from freezeyt.types import AbsoluteURL
 
 
 if TYPE_CHECKING:
     from freezeyt.hooks import TaskInfo
+    from freezeyt.freezer import Task
 
 
 process_pool_executor = concurrent.futures.ProcessPoolExecutor()
 
 
 class InfiniteRedirection(Exception):
     """Infinite redirection was detected with redirect_policy='follow'"""
-    def __init__(self, task):
+    def __init__(self, task: 'Task'):
+        redirects_to = task.redirects_to
+        assert redirects_to is not None
         super().__init__(
-            f'{task.get_a_url()} redirects to {task.redirects_to.get_a_url()},'
+            f'{task.get_a_url()} redirects to {redirects_to.get_a_url()},'
             + ' which was not frozen (most likely because of infinite redirection)'
         )
 
 class ExternalURLError(ValueError):
     """Unexpected external URL specified"""
 
 class RelativeURLError(ValueError):
     """Absolute URL was expected"""
 
 class UnsupportedSchemeError(ValueError):
     """Raised for URLs with unsupported schemes"""
 
 class UnexpectedStatus(ValueError):
     """The application returned an unexpected status code for a page"""
-    def __init__(self, url, status):
+    def __init__(self, url: AbsoluteURL, status: str):
         self.url = urllib.parse.urlunsplit(url)
         self.status = status
         message = str(status)
         super().__init__(message)
 
 class WrongMimetypeError(ValueError):
     """MIME type does not match file extension"""
-    def __init__(self, expected, got, url_path):
+    def __init__(self, expected: List[str], got: str, url_path: str):
         super().__init__(
             f"Content-type {got!r} is different from allowed MIME types {expected}"
             + f" guessed from '{url_path}'"
         )
 
 class MultiError(_MultiErrorBase):
     """Contains multiple errors"""
@@ -79,14 +83,21 @@
         self.tasks = [TaskInfo(t) for t in tasks]
         return self
 
     def derive(self, excs):
         return MultiError([e._freezeyt_exception_task for e in excs])
 
 
+class TaskStatus(enum.Enum):
+    IN_PROGRESS = "Currently being handled"
+    REDIRECTING = "Waiting for target of redirection"
+    DONE = "Saved"
+    FAILED = "Raised an exception"
+
+
 def is_external(parsed_url: AbsoluteURL, prefix: AbsoluteURL) -> bool:
     """Return true if the given URL is within a web app at `prefix`
     """
     if parsed_url.scheme not in ('http', 'https'):
         # We know the prefix has a supported scheme.
         # If parsed_url has a different scheme, it must be external.
         return True
@@ -164,15 +175,19 @@
     except UnsupportedSchemeError:
         # If this has a scheme other than http and https,
         # it's an external url; we don't need the port in it.
         return AbsoluteURL(result)
 
 
 def import_variable_from_module(
-    name, *, default_module_name=None, default_variable_name=None):
+    name: str,
+    *,
+    default_module_name: Optional[str] = None,
+    default_variable_name: Optional[str] = None,
+) -> Any:
     """Import a variable from a named module
 
     Given a name like "package.module:namespace.variable":
     - import module "package.module"
     - get the attribute "namespace" from the module
     - return the attribute "variable" from the "namespace" object
```

### Comparing `freezeyt-1.1.0/freezeyt.egg-info/PKG-INFO` & `freezeyt-1.1.1/freezeyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freezeyt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generate static web pages from WSGI apps
 Home-page: https://github.com/encukou/freezeyt
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -35,15 +35,15 @@
 Requires-Dist: flask; extra == "blog"
 Requires-Dist: markdown-it-py; extra == "blog"
 Requires-Dist: pygments; extra == "blog"
 Provides-Extra: typecheck
 Requires-Dist: mypy; extra == "typecheck"
 Requires-Dist: types-click; extra == "typecheck"
 Requires-Dist: types-PyYAML; extra == "typecheck"
-Requires-Dist: types-html5lib; extra == "typecheck"
+Requires-Dist: types-html5lib>=1.1.11.20240228; extra == "typecheck"
 
 # freezeyt
 
 Static web page generator created by the Czech Python community.
 
 
 ## What this does
@@ -299,16 +299,16 @@
 
 ```yaml
 extra_pages:
     - /extra/
     - /extra2.html
 ```
 
-Freezeyt will freeze these pages in addition to those it
-finds by following links.
+Freezeyt will handle these pages as if it found them by following links.
+(For example, by default it will follow links in extra pages.)
 
 Extra pages may also be given on the command line,
 e.g. `--extra-page /extra/ --extra-page /extra2.html`.
 The lists from CLI and the config file are merged together.
 
 You can also specify extra pages using a Python generator,
 specified using a module name and function name as follows:
@@ -337,14 +337,17 @@
 
 
 ### Extra files
 
 Extra files to be included in the output can be specified,
 along with their content.
 
+These files are not considered part of the app; freezeyt will not try to find
+links in them.
+
 This is useful for configuration of your static server.
 (For pages that are part of your website, we recommend
 adding them to your application rather than as extra files.)
 
 If you specify backslashes in `url part`, `freezeyt` convert them to forward slashes.
 
 For example, the following config will add 3 files to
```

### Comparing `freezeyt-1.1.0/freezeyt.egg-info/SOURCES.txt` & `freezeyt-1.1.1/freezeyt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 tests/test_add_port.py
 tests/test_cancel_tasks.py
 tests/test_check_mimetype.py
 tests/test_cleanup.py
 tests/test_click_cli.py
 tests/test_concurrency.py
 tests/test_config.py
+tests/test_dictsaver.py
 tests/test_encoding.py
 tests/test_expected_output.py
 tests/test_extra_files.py
 tests/test_get_css_links.py
 tests/test_get_html_links.py
 tests/test_get_mimetype.py
 tests/test_gh_pages.py
```

### Comparing `freezeyt-1.1.0/setup.cfg` & `freezeyt-1.1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 	flask
 	markdown-it-py
 	pygments
 typecheck = 
 	mypy
 	types-click
 	types-PyYAML
-	types-html5lib
+	
+	types-html5lib >= 1.1.11.20240228
 
 [options.entry_points]
 console_scripts = 
 	freezeyt = freezeyt.cli:main
 
 [egg_info]
 tag_build =
```

### Comparing `freezeyt-1.1.0/tests/test_add_port.py` & `freezeyt-1.1.1/tests/test_add_port.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_cancel_tasks.py` & `freezeyt-1.1.1/tests/test_cancel_tasks.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_check_mimetype.py` & `freezeyt-1.1.1/tests/test_check_mimetype.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_cleanup.py` & `freezeyt-1.1.1/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_click_cli.py` & `freezeyt-1.1.1/tests/test_click_cli.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_concurrency.py` & `freezeyt-1.1.1/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_config.py` & `freezeyt-1.1.1/tests/test_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 
 def test_func_to_dict(tmp_path):
     config = {**freeze_config, 'output': {'type': 'dict'}}
 
     result = freeze(app, config)
 
+    assert result is not None
+
     print(result)
     assert sorted(result) == [
         '.nojekyll', 'CNAME', 'bin_range.dat', 'config',
         'index.html', 'smile.png', 'smile2.png'
     ]
 
 
@@ -119,21 +121,33 @@
             'extra_pages': ['http://external.example/foo.html'],
         }
 
         with pytest.raises(ExternalURLError):
             freeze(module.app, freeze_config)
 
 
-def test_external_extra_files_generator(tmp_path):
-    def gen(app):
-        yield 'http://external.example/foo.html'
+def generate_extra_page(app):
+    assert app.is_the_fixture_app_2pages
+    yield 'http://external.example/foo.html'
+
+def test_external_extra_files_generator_as_function(tmp_path):
+    with context_for_test('app_2pages') as module:
+        freeze_config = {
+            'output': {'type': 'dict'},
+            'extra_pages': [generate_extra_page],
+        }
+
+        with pytest.raises(ExternalURLError):
+            freeze(module.app, freeze_config)
+
+def test_external_extra_files_generator_from_string(tmp_path):
     with context_for_test('app_2pages') as module:
         freeze_config = {
             'output': {'type': 'dict'},
-            'extra_pages': [gen],
+            'extra_pages': [{'generator': f'{__name__}:generate_extra_page'}],
         }
 
         with pytest.raises(ExternalURLError):
             freeze(module.app, freeze_config)
 
 def my_url_to_path(path):
     return {
```

### Comparing `freezeyt-1.1.0/tests/test_encoding.py` & `freezeyt-1.1.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_expected_output.py` & `freezeyt-1.1.1/tests/test_expected_output.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_extra_files.py` & `freezeyt-1.1.1/tests/test_extra_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         'extra_files': extra_file,
         'output': {'type': 'dict'},
     }
 
     with context_for_test('app_simple') as module:
         result = freeze(module.app, config)
 
+    assert result is not None
+
     # pop to simplify syntax of expected dict
     # index.html is root page for app_simple, not useful for this test
     result.pop('index.html')
 
     assert result == expected
 
 EXTRA_FILE_DOT = {
@@ -80,14 +82,16 @@
         'extra_files': extra_file,
         'output': {'type': 'dict'},
     }
 
     with context_for_test('app_simple') as module:
         result = freeze(module.app, config)
 
+    assert result is not None
+
     # pop to simplify syntax of expected dict
     # index.html is root page for app_simple, not useful for this test
     result.pop('index.html')
 
     assert result == expected
 
 
@@ -104,14 +108,16 @@
         'extra_files': extra_file,
         'output': {'type': 'dict'},
     }
 
     with context_for_test('app_simple') as module:
         result = freeze(module.app, config)
 
+    assert result is not None
+
     # pop to simplify syntax of expected dict
     # index.html is root page for app_simple, not useful for this test
     result.pop('index.html')
 
     assert result == expected
 
 EXTRA_FILE_WITH_PREFIX = {
```

### Comparing `freezeyt-1.1.0/tests/test_get_css_links.py` & `freezeyt-1.1.1/tests/test_get_css_links.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_get_html_links.py` & `freezeyt-1.1.1/tests/test_get_html_links.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_get_mimetype.py` & `freezeyt-1.1.1/tests/test_get_mimetype.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_gh_pages.py` & `freezeyt-1.1.1/tests/test_gh_pages.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_hooks.py` & `freezeyt-1.1.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_import_variable_from_module.py` & `freezeyt-1.1.1/tests/test_import_variable_from_module.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_is_external.py` & `freezeyt-1.1.1/tests/test_is_external.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_logging.py` & `freezeyt-1.1.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_middleware.py` & `freezeyt-1.1.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_mime_db_mimetype.py` & `freezeyt-1.1.1/tests/test_mime_db_mimetype.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_mimetype_checker.py` & `freezeyt-1.1.1/tests/test_mimetype_checker.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_multierror.py` & `freezeyt-1.1.1/tests/test_multierror.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_parse_absolute_url.py` & `freezeyt-1.1.1/tests/test_parse_absolute_url.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_plugins.py` & `freezeyt-1.1.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_reason.py` & `freezeyt-1.1.1/tests/test_reason.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_remove_output_dir.py` & `freezeyt-1.1.1/tests/test_remove_output_dir.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_status_handlers.py` & `freezeyt-1.1.1/tests/test_status_handlers.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_testutil.py` & `freezeyt-1.1.1/tests/test_testutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import PurePosixPath
+from typing import NoReturn
 
 import pytest
 
 from freezeyt import MultiError
 from freezeyt.freezer import Task
 from freezeyt.hooks import TaskInfo
 from freezeyt.compat import asyncio_run, asyncio_create_task
@@ -38,17 +39,17 @@
     path1.write_text('A')
     path2.write_text('B')
 
     with pytest.raises(AssertionError):
         assert_dirs_same(dir1, dir2)
 
 
-async def create_failing_task():
+async def create_failing_task() -> Task:
     """Create a fake freezeyt task that failed with an AssertionError"""
-    async def fail():
+    async def fail() -> NoReturn:
         """coroutine that fails"""
         raise AssertionError()
     # Create an asyncio task
     asyncio_task = asyncio_create_task(fail(), name='test')
     # Wait for it to be done (catching the AssertionError)
     with pytest.raises(AssertionError):
         await asyncio_task
```

### Comparing `freezeyt-1.1.0/tests/test_url_finders.py` & `freezeyt-1.1.1/tests/test_url_finders.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_url_to_path.py` & `freezeyt-1.1.1/tests/test_url_to_path.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_version.py` & `freezeyt-1.1.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/test_wsgi.py` & `freezeyt-1.1.1/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `freezeyt-1.1.0/tests/testutil.py` & `freezeyt-1.1.1/tests/testutil.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,21 +39,21 @@
             module = importlib.import_module(module_name)
         yield module
     finally:
         sys.modules.clear()
         sys.modules.update(original_modules)
 
 
-def assert_dirs_same(got: Path, expected: Path):
+def assert_dirs_same(got: Path, expected: Path) -> None:
     cmp = filecmp.dircmp(got, expected, ignore=[])
     cmp.report_full_closure()
     assert_cmp_same(cmp)
 
 
-def assert_cmp_same(cmp):
+def assert_cmp_same(cmp: filecmp.dircmp) -> None:
     print('assert_cmp_same', cmp.left, cmp.right)
 
     if cmp.left_only:
         raise AssertionError(f'Extra files frozen: {cmp.left_only}')
 
     if cmp.right_only:
         raise AssertionError(f'Files not frozen: {cmp.right_only}')
```

