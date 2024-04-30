# Comparing `tmp/tinybird-cli-3.9.1.dev4.tar.gz` & `tmp/tinybird-cli-3.9.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.9.1.dev4.tar", last modified: Mon Apr 29 10:41:53 2024, max compression
+gzip compressed data, was "tinybird-cli-3.9.1.dev5.tar", last modified: Tue Apr 30 07:04:29 2024, max compression
```

## Comparing `tinybird-cli-3.9.1.dev4.tar` & `tinybird-cli-3.9.1.dev5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/
--rw-r--r--   0 root         (0) root         (0)    68632 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.524615 tinybird-cli-3.9.1.dev4/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-29 10:41:52.000000 tinybird-cli-3.9.1.dev4/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.524615 tinybird-cli-3.9.1.dev4/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59638 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41589 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.526615 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    31660 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.526615 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    68632 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.310853 tinybird-cli-3.9.1.dev5/
+-rw-r--r--   0 root         (0) root         (0)    68737 2024-04-30 07:04:29.309853 tinybird-cli-3.9.1.dev5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 07:04:29.310853 tinybird-cli-3.9.1.dev5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.306853 tinybird-cli-3.9.1.dev5/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-30 07:04:28.000000 tinybird-cli-3.9.1.dev5/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.306853 tinybird-cli-3.9.1.dev5/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   212518 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59638 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41589 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.308853 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    31660 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.308853 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.309853 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    68737 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.9.1.dev4/PKG-INFO` & `tinybird-cli-3.9.1.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev4
+Version: 3.9.1.dev5
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,14 +14,19 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ----------
 
+3.9.1.dev5
+************
+
+- `Added` support for adding multiple tokens when pushing a `.datasource` file
+
 
 3.9.1.dev4
 ************
 
 - `Fixed` s3 iamrole connection creation will not fail when `pbcopy` dependency is not available
 
 3.9.1.dev3
```

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/ch_utils/constants.py` & `tinybird-cli-3.9.1.dev5/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/ch_utils/engine.py` & `tinybird-cli-3.9.1.dev5/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/check_pypi.py` & `tinybird-cli-3.9.1.dev5/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/client.py` & `tinybird-cli-3.9.1.dev5/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/config.py` & `tinybird-cli-3.9.1.dev5/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/connectors.py` & `tinybird-cli-3.9.1.dev5/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/context.py` & `tinybird-cli-3.9.1.dev5/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/datafile.py` & `tinybird-cli-3.9.1.dev5/tinybird/datafile.py`

 * *Files 0% similar despite different names*

```diff
@@ -7636,5647 +7636,5648 @@
 0001dd30: 2020 2020 2020 2020 2020 2074 6f6b 656e             token
 0001dd40: 5f6e 616d 6520 3d20 746b 5b22 746f 6b65  _name = tk["toke
 0001dd50: 6e5f 6e61 6d65 225d 0a20 2020 2020 2020  n_name"].       
 0001dd60: 2020 2020 2074 203d 2061 7761 6974 2063       t = await c
 0001dd70: 6c69 656e 742e 6765 745f 746f 6b65 6e5f  lient.get_token_
 0001dd80: 6279 5f6e 616d 6528 746f 6b65 6e5f 6e61  by_name(token_na
 0001dd90: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0001dda0: 6966 2074 3a0a 2020 2020 2020 2020 2020  if t:.          
-0001ddb0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-0001ddc0: 2020 2020 6966 206e 6f74 2074 3a0a 2020      if not t:.  
-0001ddd0: 2020 2020 2020 2020 2020 746f 6b65 6e5f            token_
-0001dde0: 6e61 6d65 203d 2074 6b5b 2274 6f6b 656e  name = tk["token
-0001ddf0: 5f6e 616d 6522 5d0a 2020 2020 2020 2020  _name"].        
-0001de00: 2020 2020 636c 6963 6b2e 6563 686f 2846      click.echo(F
-0001de10: 6565 6462 6163 6b4d 616e 6167 6572 2e69  eedbackManager.i
-0001de20: 6e66 6f5f 6372 6561 7465 5f6e 6f74 5f66  nfo_create_not_f
-0001de30: 6f75 6e64 5f74 6f6b 656e 2874 6f6b 656e  ound_token(token
-0001de40: 3d74 6f6b 656e 5f6e 616d 6529 290a 2020  =token_name)).  
-0001de50: 2020 2020 2020 2020 2020 2320 4453 203d            # DS =
-0001de60: 3d20 746f 6b65 6e5f 6f72 6967 696e 2e4f  = token_origin.O
-0001de70: 7269 6769 6e73 2e44 4154 4153 4f55 5243  rigins.DATASOURC
-0001de80: 450a 2020 2020 2020 2020 2020 2020 6177  E.            aw
-0001de90: 6169 7420 636c 6965 6e74 2e63 7265 6174  ait client.creat
-0001dea0: 655f 746f 6b65 6e28 746f 6b65 6e5f 6e61  e_token(token_na
-0001deb0: 6d65 2c20 6622 4441 5441 534f 5552 4345  me, f"DATASOURCE
-0001dec0: 533a 7b74 6b5b 2770 6572 6d69 7373 696f  S:{tk['permissio
-0001ded0: 6e73 275d 7d3a 7b64 735f 6e61 6d65 7d22  ns']}:{ds_name}"
-0001dee0: 2c20 2244 5322 2c20 6473 5f6e 616d 6529  , "DS", ds_name)
-0001def0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0001df00: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-0001df10: 2e65 6368 6f28 4665 6564 6261 636b 4d61  .echo(FeedbackMa
-0001df20: 6e61 6765 722e 696e 666f 5f63 7265 6174  nager.info_creat
-0001df30: 655f 666f 756e 645f 746f 6b65 6e28 746f  e_found_token(to
-0001df40: 6b65 6e3d 746f 6b65 6e5f 6e61 6d65 2929  ken=token_name))
-0001df50: 0a20 2020 2020 2020 2020 2020 2073 636f  .            sco
-0001df60: 7065 7320 3d20 5b66 2244 4154 4153 4f55  pes = [f"DATASOU
-0001df70: 5243 4553 3a7b 746b 5b27 7065 726d 6973  RCES:{tk['permis
-0001df80: 7369 6f6e 7327 5d7d 3a7b 6473 5f6e 616d  sions']}:{ds_nam
-0001df90: 657d 225d 0a20 2020 2020 2020 2020 2020  e}"].           
-0001dfa0: 2066 6f72 2078 2069 6e20 745b 2273 636f   for x in t["sco
-0001dfb0: 7065 7322 5d3a 0a20 2020 2020 2020 2020  pes"]:.         
+0001dda0: 6966 206e 6f74 2074 3a0a 2020 2020 2020  if not t:.      
+0001ddb0: 2020 2020 2020 2020 2020 746f 6b65 6e5f            token_
+0001ddc0: 6e61 6d65 203d 2074 6b5b 2274 6f6b 656e  name = tk["token
+0001ddd0: 5f6e 616d 6522 5d0a 2020 2020 2020 2020  _name"].        
+0001dde0: 2020 2020 2020 2020 636c 6963 6b2e 6563          click.ec
+0001ddf0: 686f 2846 6565 6462 6163 6b4d 616e 6167  ho(FeedbackManag
+0001de00: 6572 2e69 6e66 6f5f 6372 6561 7465 5f6e  er.info_create_n
+0001de10: 6f74 5f66 6f75 6e64 5f74 6f6b 656e 2874  ot_found_token(t
+0001de20: 6f6b 656e 3d74 6f6b 656e 5f6e 616d 6529  oken=token_name)
+0001de30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001de40: 2020 2320 4453 203d 3d20 746f 6b65 6e5f    # DS == token_
+0001de50: 6f72 6967 696e 2e4f 7269 6769 6e73 2e44  origin.Origins.D
+0001de60: 4154 4153 4f55 5243 450a 2020 2020 2020  ATASOURCE.      
+0001de70: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0001de80: 636c 6965 6e74 2e63 7265 6174 655f 746f  client.create_to
+0001de90: 6b65 6e28 746f 6b65 6e5f 6e61 6d65 2c20  ken(token_name, 
+0001dea0: 6622 4441 5441 534f 5552 4345 533a 7b74  f"DATASOURCES:{t
+0001deb0: 6b5b 2770 6572 6d69 7373 696f 6e73 275d  k['permissions']
+0001dec0: 7d3a 7b64 735f 6e61 6d65 7d22 2c20 2244  }:{ds_name}", "D
+0001ded0: 5322 2c20 6473 5f6e 616d 6529 0a20 2020  S", ds_name).   
+0001dee0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001def0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001df00: 6c69 636b 2e65 6368 6f28 4665 6564 6261  lick.echo(Feedba
+0001df10: 636b 4d61 6e61 6765 722e 696e 666f 5f63  ckManager.info_c
+0001df20: 7265 6174 655f 666f 756e 645f 746f 6b65  reate_found_toke
+0001df30: 6e28 746f 6b65 6e3d 746f 6b65 6e5f 6e61  n(token=token_na
+0001df40: 6d65 2929 0a20 2020 2020 2020 2020 2020  me)).           
+0001df50: 2020 2020 2073 636f 7065 7320 3d20 5b66       scopes = [f
+0001df60: 2244 4154 4153 4f55 5243 4553 3a7b 746b  "DATASOURCES:{tk
+0001df70: 5b27 7065 726d 6973 7369 6f6e 7327 5d7d  ['permissions']}
+0001df80: 3a7b 6473 5f6e 616d 657d 225d 0a20 2020  :{ds_name}"].   
+0001df90: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001dfa0: 2078 2069 6e20 745b 2273 636f 7065 7322   x in t["scopes"
+0001dfb0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
 0001dfc0: 2020 2020 2020 2073 6320 3d20 785b 2274         sc = x["t
 0001dfd0: 7970 6522 5d20 6966 2022 7265 736f 7572  ype"] if "resour
 0001dfe0: 6365 2220 6e6f 7420 696e 2078 2065 6c73  ce" not in x els
 0001dff0: 6520 6622 7b78 5b27 7479 7065 275d 7d3a  e f"{x['type']}:
 0001e000: 7b78 5b27 7265 736f 7572 6365 275d 7d22  {x['resource']}"
 0001e010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e020: 2073 636f 7065 732e 6170 7065 6e64 2873   scopes.append(s
-0001e030: 6329 0a20 2020 2020 2020 2020 2020 2061  c).            a
-0001e040: 7761 6974 2063 6c69 656e 742e 616c 7465  wait client.alte
-0001e050: 725f 746f 6b65 6e73 2874 6f6b 656e 5f6e  r_tokens(token_n
-0001e060: 616d 652c 2073 636f 7065 7329 0a0a 2020  ame, scopes)..  
-0001e070: 2020 7472 793a 0a20 2020 2020 2020 2065    try:.        e
-0001e080: 7869 7374 696e 675f 6473 203d 2061 7761  xisting_ds = awa
-0001e090: 6974 2063 6c69 656e 742e 6765 745f 6461  it client.get_da
-0001e0a0: 7461 736f 7572 6365 2864 735f 6e61 6d65  tasource(ds_name
-0001e0b0: 290a 2020 2020 2020 2020 6461 7461 736f  ).        dataso
-0001e0c0: 7572 6365 5f65 7869 7374 7320 3d20 5472  urce_exists = Tr
-0001e0d0: 7565 0a20 2020 2065 7863 6570 7420 446f  ue.    except Do
-0001e0e0: 6573 4e6f 7445 7869 7374 4578 6365 7074  esNotExistExcept
-0001e0f0: 696f 6e3a 0a20 2020 2020 2020 2064 6174  ion:.        dat
-0001e100: 6173 6f75 7263 655f 6578 6973 7473 203d  asource_exists =
-0001e110: 2046 616c 7365 0a0a 2020 2020 6966 206e   False..    if n
-0001e120: 6f74 2064 6174 6173 6f75 7263 655f 6578  ot datasource_ex
-0001e130: 6973 7473 206f 7220 666f 726b 5f64 6f77  ists or fork_dow
-0001e140: 6e73 7472 6561 6d20 6f72 2066 6f72 6b3a  nstream or fork:
-0001e150: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-0001e160: 3d20 6473 5b22 7061 7261 6d73 225d 0a20  = ds["params"]. 
-0001e170: 2020 2020 2020 2070 6172 616d 735b 2262         params["b
-0001e180: 7261 6e63 685f 6d6f 6465 225d 203d 2022  ranch_mode"] = "
-0001e190: 666f 726b 2220 6966 2066 6f72 6b5f 646f  fork" if fork_do
-0001e1a0: 776e 7374 7265 616d 206f 7220 666f 726b  wnstream or fork
-0001e1b0: 2065 6c73 6520 224e 6f6e 6522 0a0a 2020   else "None"..  
-0001e1c0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0001e1d0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0001e1e0: 2020 2020 2020 2020 2020 2020 7061 7261              para
-0001e1f0: 6d73 2e67 6574 2822 7365 7276 6963 6522  ms.get("service"
-0001e200: 2920 696e 2050 5245 5649 4557 5f43 4f4e  ) in PREVIEW_CON
-0001e210: 4e45 4354 4f52 5f53 4552 5649 4345 530a  NECTOR_SERVICES.
-0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e230: 616e 6420 7061 7261 6d73 2e67 6574 2822  and params.get("
-0001e240: 636f 6e6e 6563 746f 7222 290a 2020 2020  connector").    
-0001e250: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001e260: 7061 7261 6d73 2e67 6574 2822 6275 636b  params.get("buck
-0001e270: 6574 5f75 7269 2229 0a20 2020 2020 2020  et_uri").       
-0001e280: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0001e290: 2020 2020 2020 2020 6461 7461 203d 2061          data = a
-0001e2a0: 7761 6974 2063 6c69 656e 742e 7072 6576  wait client.prev
-0001e2b0: 6965 775f 6275 636b 6574 2870 6172 616d  iew_bucket(param
-0001e2c0: 735b 2263 6f6e 6e65 6374 6f72 225d 2c20  s["connector"], 
-0001e2d0: 7061 7261 6d73 5b22 6275 636b 6574 5f75  params["bucket_u
-0001e2e0: 7269 225d 290a 2020 2020 2020 2020 2020  ri"]).          
-0001e2f0: 2020 2020 2020 6966 2064 6174 613a 0a20        if data:. 
-0001e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e310: 2020 2066 696c 6573 203d 2064 6174 612e     files = data.
-0001e320: 6765 7428 2266 696c 6573 222c 205b 5d29  get("files", [])
-0001e330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e340: 2020 2020 2069 6620 6c65 6e28 6669 6c65       if len(file
-0001e350: 7329 203e 2030 3a0a 2020 2020 2020 2020  s) > 0:.        
+0001e020: 2020 2020 2073 636f 7065 732e 6170 7065       scopes.appe
+0001e030: 6e64 2873 6329 0a20 2020 2020 2020 2020  nd(sc).         
+0001e040: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+0001e050: 656e 742e 616c 7465 725f 746f 6b65 6e73  ent.alter_tokens
+0001e060: 2874 6f6b 656e 5f6e 616d 652c 2073 636f  (token_name, sco
+0001e070: 7065 7329 0a0a 2020 2020 7472 793a 0a20  pes)..    try:. 
+0001e080: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
+0001e090: 6473 203d 2061 7761 6974 2063 6c69 656e  ds = await clien
+0001e0a0: 742e 6765 745f 6461 7461 736f 7572 6365  t.get_datasource
+0001e0b0: 2864 735f 6e61 6d65 290a 2020 2020 2020  (ds_name).      
+0001e0c0: 2020 6461 7461 736f 7572 6365 5f65 7869    datasource_exi
+0001e0d0: 7374 7320 3d20 5472 7565 0a20 2020 2065  sts = True.    e
+0001e0e0: 7863 6570 7420 446f 6573 4e6f 7445 7869  xcept DoesNotExi
+0001e0f0: 7374 4578 6365 7074 696f 6e3a 0a20 2020  stException:.   
+0001e100: 2020 2020 2064 6174 6173 6f75 7263 655f       datasource_
+0001e110: 6578 6973 7473 203d 2046 616c 7365 0a0a  exists = False..
+0001e120: 2020 2020 6966 206e 6f74 2064 6174 6173      if not datas
+0001e130: 6f75 7263 655f 6578 6973 7473 206f 7220  ource_exists or 
+0001e140: 666f 726b 5f64 6f77 6e73 7472 6561 6d20  fork_downstream 
+0001e150: 6f72 2066 6f72 6b3a 0a20 2020 2020 2020  or fork:.       
+0001e160: 2070 6172 616d 7320 3d20 6473 5b22 7061   params = ds["pa
+0001e170: 7261 6d73 225d 0a20 2020 2020 2020 2070  rams"].        p
+0001e180: 6172 616d 735b 2262 7261 6e63 685f 6d6f  arams["branch_mo
+0001e190: 6465 225d 203d 2022 666f 726b 2220 6966  de"] = "fork" if
+0001e1a0: 2066 6f72 6b5f 646f 776e 7374 7265 616d   fork_downstream
+0001e1b0: 206f 7220 666f 726b 2065 6c73 6520 224e   or fork else "N
+0001e1c0: 6f6e 6522 0a0a 2020 2020 2020 2020 7472  one"..        tr
+0001e1d0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
+0001e1e0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+0001e1f0: 2020 2020 7061 7261 6d73 2e67 6574 2822      params.get("
+0001e200: 7365 7276 6963 6522 2920 696e 2050 5245  service") in PRE
+0001e210: 5649 4557 5f43 4f4e 4e45 4354 4f52 5f53  VIEW_CONNECTOR_S
+0001e220: 4552 5649 4345 530a 2020 2020 2020 2020  ERVICES.        
+0001e230: 2020 2020 2020 2020 616e 6420 7061 7261          and para
+0001e240: 6d73 2e67 6574 2822 636f 6e6e 6563 746f  ms.get("connecto
+0001e250: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
+0001e260: 2020 2020 616e 6420 7061 7261 6d73 2e67      and params.g
+0001e270: 6574 2822 6275 636b 6574 5f75 7269 2229  et("bucket_uri")
+0001e280: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+0001e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2a0: 6461 7461 203d 2061 7761 6974 2063 6c69  data = await cli
+0001e2b0: 656e 742e 7072 6576 6965 775f 6275 636b  ent.preview_buck
+0001e2c0: 6574 2870 6172 616d 735b 2263 6f6e 6e65  et(params["conne
+0001e2d0: 6374 6f72 225d 2c20 7061 7261 6d73 5b22  ctor"], params["
+0001e2e0: 6275 636b 6574 5f75 7269 225d 290a 2020  bucket_uri"]).  
+0001e2f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001e300: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+0001e310: 2020 2020 2020 2020 2020 2066 696c 6573             files
+0001e320: 203d 2064 6174 612e 6765 7428 2266 696c   = data.get("fil
+0001e330: 6573 222c 205b 5d29 0a20 2020 2020 2020  es", []).       
+0001e340: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001e350: 6c65 6e28 6669 6c65 7329 203e 2030 3a0a  len(files) > 0:.
 0001e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e370: 6669 6c65 5f6e 616d 6520 3d20 6669 6c65  file_name = file
-0001e380: 735b 305d 2e67 6574 2822 6e61 6d65 222c  s[0].get("name",
-0001e390: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
-0001e3a0: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-0001e3b0: 656e 7369 6f6e 203d 2066 696c 655f 6e61  ension = file_na
-0001e3c0: 6d65 2e73 706c 6974 2822 2e22 295b 2d31  me.split(".")[-1
-0001e3d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001e3e0: 2020 2020 2020 2020 2020 7661 6c69 645f            valid_
-0001e3f0: 666f 726d 6174 7320 3d20 5b22 6373 7622  formats = ["csv"
-0001e400: 2c20 226e 646a 736f 6e22 2c20 2270 6172  , "ndjson", "par
-0001e410: 7175 6574 225d 0a20 2020 2020 2020 2020  quet"].         
-0001e420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001e430: 6620 6578 7465 6e73 696f 6e20 6e6f 7420  f extension not 
-0001e440: 696e 2076 616c 6964 5f66 6f72 6d61 7473  in valid_formats
-0001e450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e460: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0001e470: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
-0001e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e490: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-0001e4a0: 6565 6462 6163 6b4d 616e 6167 6572 2e65  eedbackManager.e
-0001e4b0: 7272 6f72 5f66 6f72 6d61 7428 6578 7465  rror_format(exte
-0001e4c0: 6e73 696f 6e3d 6578 7465 6e73 696f 6e2c  nsion=extension,
-0001e4d0: 2076 616c 6964 5f66 6f72 6d61 7473 3d76   valid_formats=v
-0001e4e0: 616c 6964 5f66 6f72 6d61 7473 290a 2020  alid_formats).  
-0001e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e500: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e520: 2020 2020 7061 7261 6d73 5b22 666f 726d      params["form
-0001e530: 6174 225d 203d 2065 7874 656e 7369 6f6e  at"] = extension
-0001e540: 0a0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-0001e550: 7461 736f 7572 6365 203d 2028 6177 6169  tasource = (awai
-0001e560: 7420 636c 6965 6e74 2e64 6174 6173 6f75  t client.datasou
-0001e570: 7263 655f 6372 6561 7465 5f66 726f 6d5f  rce_create_from_
-0001e580: 6465 6669 6e69 7469 6f6e 2870 6172 616d  definition(param
-0001e590: 7329 292e 6765 7428 2264 6174 6173 6f75  s)).get("datasou
-0001e5a0: 7263 6522 2c20 7b7d 290a 2020 2020 2020  rce", {}).      
-0001e5b0: 2020 2020 2020 6966 2022 746f 6b65 6e73        if "tokens
-0001e5c0: 2220 696e 2064 7320 616e 6420 6473 5b22  " in ds and ds["
-0001e5d0: 746f 6b65 6e73 225d 3a0a 2020 2020 2020  tokens"]:.      
-0001e5e0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0001e5f0: 6d61 6e61 6765 5f74 6f6b 656e 7328 290a  manage_tokens().
-0001e600: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001e610: 2273 6861 7265 645f 7769 7468 2220 696e  "shared_with" in
-0001e620: 2064 7320 616e 6420 6473 5b22 7368 6172   ds and ds["shar
-0001e630: 6564 5f77 6974 6822 5d3a 0a20 2020 2020  ed_with"]:.     
-0001e640: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0001e650: 7420 7573 6572 5f74 6f6b 656e 3a0a 2020  t user_token:.  
-0001e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e670: 2020 636c 6963 6b2e 6563 686f 2846 6565    click.echo(Fee
-0001e680: 6462 6163 6b4d 616e 6167 6572 2e69 6e66  dbackManager.inf
-0001e690: 6f5f 736b 6970 7069 6e67 5f73 6861 7265  o_skipping_share
-0001e6a0: 645f 7769 7468 5f65 6e74 7279 2829 290a  d_with_entry()).
-0001e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001e6d0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0001e6e0: 7368 6172 655f 616e 645f 756e 7368 6172  share_and_unshar
-0001e6f0: 655f 6461 7461 736f 7572 6365 280a 2020  e_datasource(.  
-0001e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e710: 2020 2020 2020 636c 6965 6e74 2c0a 2020        client,.  
-0001e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e730: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
-0001e740: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e750: 2020 2020 2020 2020 2020 7573 6572 5f74            user_t
-0001e760: 6f6b 656e 2c0a 2020 2020 2020 2020 2020  oken,.          
-0001e770: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-0001e780: 726b 7370 6163 6573 5f63 7572 7265 6e74  rkspaces_current
-0001e790: 5f73 6861 7265 645f 7769 7468 3d5b 5d2c  _shared_with=[],
-0001e7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e7b0: 2020 2020 2020 2020 2077 6f72 6b73 7061           workspa
-0001e7c0: 6365 735f 746f 5f73 6861 7265 3d64 735b  ces_to_share=ds[
-0001e7d0: 2273 6861 7265 645f 7769 7468 225d 2c0a  "shared_with"],.
-0001e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7f0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-0001e800: 7773 3d63 7572 7265 6e74 5f77 732c 0a20  ws=current_ws,. 
-0001e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e820: 2020 2029 0a0a 2020 2020 2020 2020 6578     )..        ex
-0001e830: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0001e840: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001e850: 2072 6169 7365 2063 6c69 636b 2e43 6c69   raise click.Cli
-0001e860: 636b 4578 6365 7074 696f 6e28 4665 6564  ckException(Feed
-0001e870: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
-0001e880: 725f 6372 6561 7469 6e67 5f64 6174 6173  r_creating_datas
-0001e890: 6f75 7263 6528 6572 726f 723d 7374 7228  ource(error=str(
-0001e8a0: 6529 2929 0a20 2020 2020 2020 2072 6574  e))).        ret
-0001e8b0: 7572 6e0a 0a20 2020 2069 6620 6e6f 7420  urn..    if not 
-0001e8c0: 666f 7263 653a 0a20 2020 2020 2020 2072  force:.        r
-0001e8d0: 6169 7365 2063 6c69 636b 2e43 6c69 636b  aise click.Click
-0001e8e0: 4578 6365 7074 696f 6e28 4665 6564 6261  Exception(Feedba
-0001e8f0: 636b 4d61 6e61 6765 722e 6572 726f 725f  ckManager.error_
-0001e900: 6461 7461 736f 7572 6365 5f61 6c72 6561  datasource_alrea
-0001e910: 6479 5f65 7869 7374 7328 6461 7461 736f  dy_exists(dataso
-0001e920: 7572 6365 3d64 735f 6e61 6d65 2929 0a0a  urce=ds_name))..
-0001e930: 2020 2020 6966 2064 732e 6765 7428 2273      if ds.get("s
-0001e940: 6861 7265 645f 7769 7468 222c 205b 5d29  hared_with", [])
-0001e950: 206f 7220 6578 6973 7469 6e67 5f64 732e   or existing_ds.
-0001e960: 6765 7428 2273 6861 7265 645f 7769 7468  get("shared_with
-0001e970: 222c 205b 5d29 3a0a 2020 2020 2020 2020  ", []):.        
-0001e980: 6966 206e 6f74 2075 7365 725f 746f 6b65  if not user_toke
-0001e990: 6e3a 0a20 2020 2020 2020 2020 2020 2063  n:.            c
-0001e9a0: 6c69 636b 2e65 6368 6f28 4665 6564 6261  lick.echo(Feedba
-0001e9b0: 636b 4d61 6e61 6765 722e 696e 666f 5f73  ckManager.info_s
-0001e9c0: 6b69 7070 696e 675f 7368 6172 6564 5f77  kipping_shared_w
-0001e9d0: 6974 685f 656e 7472 7928 2929 0a20 2020  ith_entry()).   
-0001e9e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001e9f0: 2020 2020 2020 2061 7761 6974 2073 6861         await sha
-0001ea00: 7265 5f61 6e64 5f75 6e73 6861 7265 5f64  re_and_unshare_d
-0001ea10: 6174 6173 6f75 7263 6528 0a20 2020 2020  atasource(.     
-0001ea20: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-0001ea30: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0001ea40: 2020 2065 7869 7374 696e 675f 6473 2c0a     existing_ds,.
-0001ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea60: 7573 6572 5f74 6f6b 656e 2c0a 2020 2020  user_token,.    
-0001ea70: 2020 2020 2020 2020 2020 2020 6578 6973              exis
-0001ea80: 7469 6e67 5f64 732e 6765 7428 2273 6861  ting_ds.get("sha
-0001ea90: 7265 645f 7769 7468 222c 205b 5d29 2c0a  red_with", []),.
-0001eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eab0: 6473 2e67 6574 2822 7368 6172 6564 5f77  ds.get("shared_w
-0001eac0: 6974 6822 2c20 5b5d 292c 0a20 2020 2020  ith", []),.     
-0001ead0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0001eae0: 6e74 5f77 732c 0a20 2020 2020 2020 2020  nt_ws,.         
-0001eaf0: 2020 2029 0a0a 2020 2020 616c 7465 725f     )..    alter_
-0001eb00: 7265 7370 6f6e 7365 203d 204e 6f6e 650a  response = None.
-0001eb10: 2020 2020 616c 7465 725f 6572 726f 725f      alter_error_
-0001eb20: 6d65 7373 6167 6520 3d20 4e6f 6e65 0a20  message = None. 
-0001eb30: 2020 206e 6577 5f64 6573 6372 6970 7469     new_descripti
-0001eb40: 6f6e 203d 204e 6f6e 650a 2020 2020 6e65  on = None.    ne
-0001eb50: 775f 7363 6865 6d61 203d 204e 6f6e 650a  w_schema = None.
-0001eb60: 2020 2020 6e65 775f 696e 6469 6365 7320      new_indices 
-0001eb70: 3d20 4e6f 6e65 0a20 2020 206e 6577 5f74  = None.    new_t
-0001eb80: 746c 203d 204e 6f6e 650a 0a20 2020 2074  tl = None..    t
-0001eb90: 7279 3a0a 2020 2020 2020 2020 6966 2064  ry:.        if d
-0001eba0: 6174 6173 6f75 7263 655f 6578 6973 7473  atasource_exists
-0001ebb0: 2061 6e64 2064 735b 2270 6172 616d 7322   and ds["params"
-0001ebc0: 5d5b 2264 6573 6372 6970 7469 6f6e 225d  ]["description"]
-0001ebd0: 2021 3d20 6578 6973 7469 6e67 5f64 735b   != existing_ds[
-0001ebe0: 2264 6573 6372 6970 7469 6f6e 225d 3a0a  "description"]:.
-0001ebf0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0001ec00: 6465 7363 7269 7074 696f 6e20 3d20 6473  description = ds
-0001ec10: 5b22 7061 7261 6d73 225d 5b22 6465 7363  ["params"]["desc
-0001ec20: 7269 7074 696f 6e22 5d0a 0a20 2020 2020  ription"]..     
-0001ec30: 2020 2069 6620 6461 7461 736f 7572 6365     if datasource
-0001ec40: 5f65 7869 7374 7320 616e 6420 6473 5b22  _exists and ds["
-0001ec50: 7061 7261 6d73 225d 2e67 6574 2822 656e  params"].get("en
-0001ec60: 6769 6e65 5f74 746c 2229 2021 3d20 6578  gine_ttl") != ex
-0001ec70: 6973 7469 6e67 5f64 735b 2265 6e67 696e  isting_ds["engin
-0001ec80: 6522 5d2e 6765 7428 2274 746c 2229 3a0a  e"].get("ttl"):.
-0001ec90: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0001eca0: 7474 6c20 3d20 6473 5b22 7061 7261 6d73  ttl = ds["params
-0001ecb0: 225d 2e67 6574 2822 656e 6769 6e65 5f74  "].get("engine_t
-0001ecc0: 746c 222c 2022 6661 6c73 6522 290a 0a20  tl", "false").. 
-0001ecd0: 2020 2020 2020 2023 2053 6368 656d 6120         # Schema 
-0001ece0: 6669 7865 6420 6279 2074 6865 206b 6166  fixed by the kaf
-0001ecf0: 6b61 2063 6f6e 6e65 6374 6f72 0a20 2020  ka connector.   
-0001ed00: 2020 2020 2069 6620 6461 7461 736f 7572       if datasour
-0001ed10: 6365 5f65 7869 7374 7320 616e 6420 280a  ce_exists and (.
-0001ed20: 2020 2020 2020 2020 2020 2020 6473 5b22              ds["
-0001ed30: 7061 7261 6d73 225d 5b22 7363 6865 6d61  params"]["schema
-0001ed40: 225d 2e72 6570 6c61 6365 2822 2022 2c20  "].replace(" ", 
-0001ed50: 2222 2920 213d 2065 7869 7374 696e 675f  "") != existing_
-0001ed60: 6473 5b22 7363 6865 6d61 225d 5b22 7371  ds["schema"]["sq
-0001ed70: 6c5f 7363 6865 6d61 225d 2e72 6570 6c61  l_schema"].repla
-0001ed80: 6365 2822 2022 2c20 2222 290a 2020 2020  ce(" ", "").    
-0001ed90: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-0001eda0: 2020 206e 6577 5f73 6368 656d 6120 3d20     new_schema = 
-0001edb0: 6473 5b22 7061 7261 6d73 225d 5b22 7363  ds["params"]["sc
-0001edc0: 6865 6d61 225d 0a0a 2020 2020 2020 2020  hema"]..        
-0001edd0: 6966 2064 6174 6173 6f75 7263 655f 6578  if datasource_ex
-0001ede0: 6973 7473 3a0a 2020 2020 2020 2020 2020  ists:.          
-0001edf0: 2020 6e65 7720 3d20 5b61 7364 6963 7428    new = [asdict(
-0001ee00: 696e 6465 7829 2066 6f72 2069 6e64 6578  index) for index
-0001ee10: 2069 6e20 6473 2e67 6574 2822 7061 7261   in ds.get("para
-0001ee20: 6d73 222c 207b 7d29 2e67 6574 2822 696e  ms", {}).get("in
-0001ee30: 6465 7865 735f 6c69 7374 222c 205b 5d29  dexes_list", [])
-0001ee40: 5d0a 2020 2020 2020 2020 2020 2020 6578  ].            ex
-0001ee50: 6973 7469 6e67 203d 2065 7869 7374 696e  isting = existin
-0001ee60: 675f 6473 2e67 6574 2822 696e 6465 7865  g_ds.get("indexe
-0001ee70: 7322 2c20 5b5d 290a 2020 2020 2020 2020  s", []).        
-0001ee80: 2020 2020 6e65 772e 736f 7274 286b 6579      new.sort(key
-0001ee90: 3d6c 616d 6264 6120 783a 2078 5b22 6e61  =lambda x: x["na
-0001eea0: 6d65 225d 290a 2020 2020 2020 2020 2020  me"]).          
-0001eeb0: 2020 6578 6973 7469 6e67 2e73 6f72 7428    existing.sort(
-0001eec0: 6b65 793d 6c61 6d62 6461 2078 3a20 785b  key=lambda x: x[
-0001eed0: 226e 616d 6522 5d29 0a20 2020 2020 2020  "name"]).       
-0001eee0: 2020 2020 2069 6620 6c65 6e28 6578 6973       if len(exis
-0001eef0: 7469 6e67 2920 213d 206c 656e 286e 6577  ting) != len(new
-0001ef00: 2920 6f72 2061 6e79 285b 2864 2c20 6432  ) or any([(d, d2
-0001ef10: 2920 666f 7220 642c 2064 3220 696e 207a  ) for d, d2 in z
-0001ef20: 6970 286e 6577 2c20 6578 6973 7469 6e67  ip(new, existing
-0001ef30: 2920 6966 2064 2021 3d20 6432 5d29 3a0a  ) if d != d2]):.
-0001ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef50: 6e65 775f 696e 6469 6365 7320 3d20 6473  new_indices = ds
-0001ef60: 2e67 6574 2822 7061 7261 6d73 222c 207b  .get("params", {
-0001ef70: 7d29 2e67 6574 2822 696e 6465 7865 7322  }).get("indexes"
-0001ef80: 2920 6f72 2022 3022 0a20 2020 2020 2020  ) or "0".       
-0001ef90: 2069 6620 6e65 775f 6465 7363 7269 7074   if new_descript
-0001efa0: 696f 6e20 6f72 206e 6577 5f73 6368 656d  ion or new_schem
-0001efb0: 6120 6f72 206e 6577 5f74 746c 206f 7220  a or new_ttl or 
-0001efc0: 286e 6577 5f69 6e64 6963 6573 2069 7320  (new_indices is 
-0001efd0: 6e6f 7420 4e6f 6e65 2920 616e 6420 286e  not None) and (n
-0001efe0: 6f74 2066 6f72 6b5f 646f 776e 7374 7265  ot fork_downstre
-0001eff0: 616d 206f 7220 6e6f 7420 666f 726b 293a  am or not fork):
-0001f000: 0a20 2020 2020 2020 2020 2020 2061 6c74  .            alt
-0001f010: 6572 5f72 6573 706f 6e73 6520 3d20 6177  er_response = aw
-0001f020: 6169 7420 636c 6965 6e74 2e61 6c74 6572  ait client.alter
-0001f030: 5f64 6174 6173 6f75 7263 6528 0a20 2020  _datasource(.   
-0001f040: 2020 2020 2020 2020 2020 2020 2064 735f               ds_
-0001f050: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0001f060: 2020 2020 2020 6e65 775f 7363 6865 6d61        new_schema
-0001f070: 3d6e 6577 5f73 6368 656d 612c 0a20 2020  =new_schema,.   
-0001f080: 2020 2020 2020 2020 2020 2020 2064 6573               des
-0001f090: 6372 6970 7469 6f6e 3d6e 6577 5f64 6573  cription=new_des
-0001f0a0: 6372 6970 7469 6f6e 2c0a 2020 2020 2020  cription,.      
-0001f0b0: 2020 2020 2020 2020 2020 7474 6c3d 6e65            ttl=ne
-0001f0c0: 775f 7474 6c2c 0a20 2020 2020 2020 2020  w_ttl,.         
-0001f0d0: 2020 2020 2020 2064 7279 5f72 756e 3d54         dry_run=T
-0001f0e0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0001f0f0: 2020 2020 2069 6e64 6578 6573 3d6e 6577       indexes=new
-0001f100: 5f69 6e64 6963 6573 2c0a 2020 2020 2020  _indices,.      
-0001f110: 2020 2020 2020 290a 2020 2020 6578 6365        ).    exce
-0001f120: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0001f130: 653a 0a20 2020 2020 2020 2069 6620 2254  e:.        if "T
-0001f140: 6865 7265 2077 6572 6520 6e6f 206f 7065  here were no ope
-0001f150: 7261 7469 6f6e 7320 746f 2070 6572 666f  rations to perfo
-0001f160: 726d 2220 696e 2073 7472 2865 293a 0a20  rm" in str(e):. 
-0001f170: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-0001f180: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001f190: 2020 2020 2020 2020 2020 616c 7465 725f            alter_
-0001f1a0: 6572 726f 725f 6d65 7373 6167 6520 3d20  error_message = 
-0001f1b0: 7374 7228 6529 0a0a 2020 2020 6966 2061  str(e)..    if a
-0001f1c0: 6c74 6572 5f72 6573 706f 6e73 653a 0a20  lter_response:. 
-0001f1d0: 2020 2020 2020 2069 6620 6769 745f 7265         if git_re
-0001f1e0: 6c65 6173 6520 616e 6420 6e6f 7420 736b  lease and not sk
-0001f1f0: 6970 5f63 6f6e 6669 726d 6174 696f 6e3a  ip_confirmation:
-0001f200: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-0001f210: 636b 2e65 6368 6f28 4665 6564 6261 636b  ck.echo(Feedback
-0001f220: 4d61 6e61 6765 722e 696e 666f 5f63 7573  Manager.info_cus
-0001f230: 746f 6d5f 6465 706c 6f79 6d65 6e74 2829  tom_deployment()
-0001f240: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
-0001f250: 6963 6b2e 6563 686f 2822 2a2a 2a2a 2a2a  ick.echo("******
-0001f260: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0001e370: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
+0001e380: 6520 3d20 6669 6c65 735b 305d 2e67 6574  e = files[0].get
+0001e390: 2822 6e61 6d65 222c 2022 2229 0a20 2020  ("name", "").   
+0001e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3b0: 2020 2020 2065 7874 656e 7369 6f6e 203d       extension =
+0001e3c0: 2066 696c 655f 6e61 6d65 2e73 706c 6974   file_name.split
+0001e3d0: 2822 2e22 295b 2d31 5d0a 2020 2020 2020  (".")[-1].      
+0001e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3f0: 2020 7661 6c69 645f 666f 726d 6174 7320    valid_formats 
+0001e400: 3d20 5b22 6373 7622 2c20 226e 646a 736f  = ["csv", "ndjso
+0001e410: 6e22 2c20 2270 6172 7175 6574 225d 0a20  n", "parquet"]. 
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 2020 2020 2069 6620 6578 7465 6e73         if extens
+0001e440: 696f 6e20 6e6f 7420 696e 2076 616c 6964  ion not in valid
+0001e450: 5f66 6f72 6d61 7473 3a0a 2020 2020 2020  _formats:.      
+0001e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e470: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+0001e480: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
+0001e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4a0: 2020 2020 2020 2046 6565 6462 6163 6b4d         FeedbackM
+0001e4b0: 616e 6167 6572 2e65 7272 6f72 5f66 6f72  anager.error_for
+0001e4c0: 6d61 7428 6578 7465 6e73 696f 6e3d 6578  mat(extension=ex
+0001e4d0: 7465 6e73 696f 6e2c 2076 616c 6964 5f66  tension, valid_f
+0001e4e0: 6f72 6d61 7473 3d76 616c 6964 5f66 6f72  ormats=valid_for
+0001e4f0: 6d61 7473 290a 2020 2020 2020 2020 2020  mats).          
+0001e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e510: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001e520: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0001e530: 6d73 5b22 666f 726d 6174 225d 203d 2065  ms["format"] = e
+0001e540: 7874 656e 7369 6f6e 0a0a 2020 2020 2020  xtension..      
+0001e550: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
+0001e560: 203d 2028 6177 6169 7420 636c 6965 6e74   = (await client
+0001e570: 2e64 6174 6173 6f75 7263 655f 6372 6561  .datasource_crea
+0001e580: 7465 5f66 726f 6d5f 6465 6669 6e69 7469  te_from_definiti
+0001e590: 6f6e 2870 6172 616d 7329 292e 6765 7428  on(params)).get(
+0001e5a0: 2264 6174 6173 6f75 7263 6522 2c20 7b7d  "datasource", {}
+0001e5b0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001e5c0: 2022 746f 6b65 6e73 2220 696e 2064 7320   "tokens" in ds 
+0001e5d0: 616e 6420 6473 5b22 746f 6b65 6e73 225d  and ds["tokens"]
+0001e5e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001e5f0: 2020 6177 6169 7420 6d61 6e61 6765 5f74    await manage_t
+0001e600: 6f6b 656e 7328 290a 0a20 2020 2020 2020  okens()..       
+0001e610: 2020 2020 2069 6620 2273 6861 7265 645f       if "shared_
+0001e620: 7769 7468 2220 696e 2064 7320 616e 6420  with" in ds and 
+0001e630: 6473 5b22 7368 6172 6564 5f77 6974 6822  ds["shared_with"
+0001e640: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0001e650: 2020 2069 6620 6e6f 7420 7573 6572 5f74     if not user_t
+0001e660: 6f6b 656e 3a0a 2020 2020 2020 2020 2020  oken:.          
+0001e670: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+0001e680: 6563 686f 2846 6565 6462 6163 6b4d 616e  echo(FeedbackMan
+0001e690: 6167 6572 2e69 6e66 6f5f 736b 6970 7069  ager.info_skippi
+0001e6a0: 6e67 5f73 6861 7265 645f 7769 7468 5f65  ng_shared_with_e
+0001e6b0: 6e74 7279 2829 290a 2020 2020 2020 2020  ntry()).        
+0001e6c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6e0: 2020 6177 6169 7420 7368 6172 655f 616e    await share_an
+0001e6f0: 645f 756e 7368 6172 655f 6461 7461 736f  d_unshare_dataso
+0001e700: 7572 6365 280a 2020 2020 2020 2020 2020  urce(.          
+0001e710: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+0001e720: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
+0001e730: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0001e740: 7461 736f 7572 6365 2c0a 2020 2020 2020  tasource,.      
+0001e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e760: 2020 7573 6572 5f74 6f6b 656e 2c0a 2020    user_token,.  
+0001e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e780: 2020 2020 2020 776f 726b 7370 6163 6573        workspaces
+0001e790: 5f63 7572 7265 6e74 5f73 6861 7265 645f  _current_shared_
+0001e7a0: 7769 7468 3d5b 5d2c 0a20 2020 2020 2020  with=[],.       
+0001e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7c0: 2077 6f72 6b73 7061 6365 735f 746f 5f73   workspaces_to_s
+0001e7d0: 6861 7265 3d64 735b 2273 6861 7265 645f  hare=ds["shared_
+0001e7e0: 7769 7468 225d 2c0a 2020 2020 2020 2020  with"],.        
+0001e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e800: 6375 7272 656e 745f 7773 3d63 7572 7265  current_ws=curre
+0001e810: 6e74 5f77 732c 0a20 2020 2020 2020 2020  nt_ws,.         
+0001e820: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001e830: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0001e840: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+0001e850: 2020 2020 2020 2020 2072 6169 7365 2063           raise c
+0001e860: 6c69 636b 2e43 6c69 636b 4578 6365 7074  lick.ClickExcept
+0001e870: 696f 6e28 4665 6564 6261 636b 4d61 6e61  ion(FeedbackMana
+0001e880: 6765 722e 6572 726f 725f 6372 6561 7469  ger.error_creati
+0001e890: 6e67 5f64 6174 6173 6f75 7263 6528 6572  ng_datasource(er
+0001e8a0: 726f 723d 7374 7228 6529 2929 0a20 2020  ror=str(e))).   
+0001e8b0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0001e8c0: 2069 6620 6e6f 7420 666f 7263 653a 0a20   if not force:. 
+0001e8d0: 2020 2020 2020 2072 6169 7365 2063 6c69         raise cli
+0001e8e0: 636b 2e43 6c69 636b 4578 6365 7074 696f  ck.ClickExceptio
+0001e8f0: 6e28 4665 6564 6261 636b 4d61 6e61 6765  n(FeedbackManage
+0001e900: 722e 6572 726f 725f 6461 7461 736f 7572  r.error_datasour
+0001e910: 6365 5f61 6c72 6561 6479 5f65 7869 7374  ce_already_exist
+0001e920: 7328 6461 7461 736f 7572 6365 3d64 735f  s(datasource=ds_
+0001e930: 6e61 6d65 2929 0a0a 2020 2020 6966 2064  name))..    if d
+0001e940: 732e 6765 7428 2273 6861 7265 645f 7769  s.get("shared_wi
+0001e950: 7468 222c 205b 5d29 206f 7220 6578 6973  th", []) or exis
+0001e960: 7469 6e67 5f64 732e 6765 7428 2273 6861  ting_ds.get("sha
+0001e970: 7265 645f 7769 7468 222c 205b 5d29 3a0a  red_with", []):.
+0001e980: 2020 2020 2020 2020 6966 206e 6f74 2075          if not u
+0001e990: 7365 725f 746f 6b65 6e3a 0a20 2020 2020  ser_token:.     
+0001e9a0: 2020 2020 2020 2063 6c69 636b 2e65 6368         click.ech
+0001e9b0: 6f28 4665 6564 6261 636b 4d61 6e61 6765  o(FeedbackManage
+0001e9c0: 722e 696e 666f 5f73 6b69 7070 696e 675f  r.info_skipping_
+0001e9d0: 7368 6172 6564 5f77 6974 685f 656e 7472  shared_with_entr
+0001e9e0: 7928 2929 0a20 2020 2020 2020 2065 6c73  y()).        els
+0001e9f0: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+0001ea00: 7761 6974 2073 6861 7265 5f61 6e64 5f75  wait share_and_u
+0001ea10: 6e73 6861 7265 5f64 6174 6173 6f75 7263  nshare_datasourc
+0001ea20: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0001ea30: 2020 2063 6c69 656e 742c 0a20 2020 2020     client,.     
+0001ea40: 2020 2020 2020 2020 2020 2065 7869 7374             exist
+0001ea50: 696e 675f 6473 2c0a 2020 2020 2020 2020  ing_ds,.        
+0001ea60: 2020 2020 2020 2020 7573 6572 5f74 6f6b          user_tok
+0001ea70: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
+0001ea80: 2020 2020 6578 6973 7469 6e67 5f64 732e      existing_ds.
+0001ea90: 6765 7428 2273 6861 7265 645f 7769 7468  get("shared_with
+0001eaa0: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
+0001eab0: 2020 2020 2020 2020 6473 2e67 6574 2822          ds.get("
+0001eac0: 7368 6172 6564 5f77 6974 6822 2c20 5b5d  shared_with", []
+0001ead0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001eae0: 2020 2063 7572 7265 6e74 5f77 732c 0a20     current_ws,. 
+0001eaf0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001eb00: 2020 616c 7465 725f 7265 7370 6f6e 7365    alter_response
+0001eb10: 203d 204e 6f6e 650a 2020 2020 616c 7465   = None.    alte
+0001eb20: 725f 6572 726f 725f 6d65 7373 6167 6520  r_error_message 
+0001eb30: 3d20 4e6f 6e65 0a20 2020 206e 6577 5f64  = None.    new_d
+0001eb40: 6573 6372 6970 7469 6f6e 203d 204e 6f6e  escription = Non
+0001eb50: 650a 2020 2020 6e65 775f 7363 6865 6d61  e.    new_schema
+0001eb60: 203d 204e 6f6e 650a 2020 2020 6e65 775f   = None.    new_
+0001eb70: 696e 6469 6365 7320 3d20 4e6f 6e65 0a20  indices = None. 
+0001eb80: 2020 206e 6577 5f74 746c 203d 204e 6f6e     new_ttl = Non
+0001eb90: 650a 0a20 2020 2074 7279 3a0a 2020 2020  e..    try:.    
+0001eba0: 2020 2020 6966 2064 6174 6173 6f75 7263      if datasourc
+0001ebb0: 655f 6578 6973 7473 2061 6e64 2064 735b  e_exists and ds[
+0001ebc0: 2270 6172 616d 7322 5d5b 2264 6573 6372  "params"]["descr
+0001ebd0: 6970 7469 6f6e 225d 2021 3d20 6578 6973  iption"] != exis
+0001ebe0: 7469 6e67 5f64 735b 2264 6573 6372 6970  ting_ds["descrip
+0001ebf0: 7469 6f6e 225d 3a0a 2020 2020 2020 2020  tion"]:.        
+0001ec00: 2020 2020 6e65 775f 6465 7363 7269 7074      new_descript
+0001ec10: 696f 6e20 3d20 6473 5b22 7061 7261 6d73  ion = ds["params
+0001ec20: 225d 5b22 6465 7363 7269 7074 696f 6e22  "]["description"
+0001ec30: 5d0a 0a20 2020 2020 2020 2069 6620 6461  ]..        if da
+0001ec40: 7461 736f 7572 6365 5f65 7869 7374 7320  tasource_exists 
+0001ec50: 616e 6420 6473 5b22 7061 7261 6d73 225d  and ds["params"]
+0001ec60: 2e67 6574 2822 656e 6769 6e65 5f74 746c  .get("engine_ttl
+0001ec70: 2229 2021 3d20 6578 6973 7469 6e67 5f64  ") != existing_d
+0001ec80: 735b 2265 6e67 696e 6522 5d2e 6765 7428  s["engine"].get(
+0001ec90: 2274 746c 2229 3a0a 2020 2020 2020 2020  "ttl"):.        
+0001eca0: 2020 2020 6e65 775f 7474 6c20 3d20 6473      new_ttl = ds
+0001ecb0: 5b22 7061 7261 6d73 225d 2e67 6574 2822  ["params"].get("
+0001ecc0: 656e 6769 6e65 5f74 746c 222c 2022 6661  engine_ttl", "fa
+0001ecd0: 6c73 6522 290a 0a20 2020 2020 2020 2023  lse")..        #
+0001ece0: 2053 6368 656d 6120 6669 7865 6420 6279   Schema fixed by
+0001ecf0: 2074 6865 206b 6166 6b61 2063 6f6e 6e65   the kafka conne
+0001ed00: 6374 6f72 0a20 2020 2020 2020 2069 6620  ctor.        if 
+0001ed10: 6461 7461 736f 7572 6365 5f65 7869 7374  datasource_exist
+0001ed20: 7320 616e 6420 280a 2020 2020 2020 2020  s and (.        
+0001ed30: 2020 2020 6473 5b22 7061 7261 6d73 225d      ds["params"]
+0001ed40: 5b22 7363 6865 6d61 225d 2e72 6570 6c61  ["schema"].repla
+0001ed50: 6365 2822 2022 2c20 2222 2920 213d 2065  ce(" ", "") != e
+0001ed60: 7869 7374 696e 675f 6473 5b22 7363 6865  xisting_ds["sche
+0001ed70: 6d61 225d 5b22 7371 6c5f 7363 6865 6d61  ma"]["sql_schema
+0001ed80: 225d 2e72 6570 6c61 6365 2822 2022 2c20  "].replace(" ", 
+0001ed90: 2222 290a 2020 2020 2020 2020 293a 0a20  "").        ):. 
+0001eda0: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
+0001edb0: 6368 656d 6120 3d20 6473 5b22 7061 7261  chema = ds["para
+0001edc0: 6d73 225d 5b22 7363 6865 6d61 225d 0a0a  ms"]["schema"]..
+0001edd0: 2020 2020 2020 2020 6966 2064 6174 6173          if datas
+0001ede0: 6f75 7263 655f 6578 6973 7473 3a0a 2020  ource_exists:.  
+0001edf0: 2020 2020 2020 2020 2020 6e65 7720 3d20            new = 
+0001ee00: 5b61 7364 6963 7428 696e 6465 7829 2066  [asdict(index) f
+0001ee10: 6f72 2069 6e64 6578 2069 6e20 6473 2e67  or index in ds.g
+0001ee20: 6574 2822 7061 7261 6d73 222c 207b 7d29  et("params", {})
+0001ee30: 2e67 6574 2822 696e 6465 7865 735f 6c69  .get("indexes_li
+0001ee40: 7374 222c 205b 5d29 5d0a 2020 2020 2020  st", [])].      
+0001ee50: 2020 2020 2020 6578 6973 7469 6e67 203d        existing =
+0001ee60: 2065 7869 7374 696e 675f 6473 2e67 6574   existing_ds.get
+0001ee70: 2822 696e 6465 7865 7322 2c20 5b5d 290a  ("indexes", []).
+0001ee80: 2020 2020 2020 2020 2020 2020 6e65 772e              new.
+0001ee90: 736f 7274 286b 6579 3d6c 616d 6264 6120  sort(key=lambda 
+0001eea0: 783a 2078 5b22 6e61 6d65 225d 290a 2020  x: x["name"]).  
+0001eeb0: 2020 2020 2020 2020 2020 6578 6973 7469            existi
+0001eec0: 6e67 2e73 6f72 7428 6b65 793d 6c61 6d62  ng.sort(key=lamb
+0001eed0: 6461 2078 3a20 785b 226e 616d 6522 5d29  da x: x["name"])
+0001eee0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001eef0: 6c65 6e28 6578 6973 7469 6e67 2920 213d  len(existing) !=
+0001ef00: 206c 656e 286e 6577 2920 6f72 2061 6e79   len(new) or any
+0001ef10: 285b 2864 2c20 6432 2920 666f 7220 642c  ([(d, d2) for d,
+0001ef20: 2064 3220 696e 207a 6970 286e 6577 2c20   d2 in zip(new, 
+0001ef30: 6578 6973 7469 6e67 2920 6966 2064 2021  existing) if d !
+0001ef40: 3d20 6432 5d29 3a0a 2020 2020 2020 2020  = d2]):.        
+0001ef50: 2020 2020 2020 2020 6e65 775f 696e 6469          new_indi
+0001ef60: 6365 7320 3d20 6473 2e67 6574 2822 7061  ces = ds.get("pa
+0001ef70: 7261 6d73 222c 207b 7d29 2e67 6574 2822  rams", {}).get("
+0001ef80: 696e 6465 7865 7322 2920 6f72 2022 3022  indexes") or "0"
+0001ef90: 0a20 2020 2020 2020 2069 6620 6e65 775f  .        if new_
+0001efa0: 6465 7363 7269 7074 696f 6e20 6f72 206e  description or n
+0001efb0: 6577 5f73 6368 656d 6120 6f72 206e 6577  ew_schema or new
+0001efc0: 5f74 746c 206f 7220 286e 6577 5f69 6e64  _ttl or (new_ind
+0001efd0: 6963 6573 2069 7320 6e6f 7420 4e6f 6e65  ices is not None
+0001efe0: 2920 616e 6420 286e 6f74 2066 6f72 6b5f  ) and (not fork_
+0001eff0: 646f 776e 7374 7265 616d 206f 7220 6e6f  downstream or no
+0001f000: 7420 666f 726b 293a 0a20 2020 2020 2020  t fork):.       
+0001f010: 2020 2020 2061 6c74 6572 5f72 6573 706f       alter_respo
+0001f020: 6e73 6520 3d20 6177 6169 7420 636c 6965  nse = await clie
+0001f030: 6e74 2e61 6c74 6572 5f64 6174 6173 6f75  nt.alter_datasou
+0001f040: 7263 6528 0a20 2020 2020 2020 2020 2020  rce(.           
+0001f050: 2020 2020 2064 735f 6e61 6d65 2c0a 2020       ds_name,.  
+0001f060: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0001f070: 775f 7363 6865 6d61 3d6e 6577 5f73 6368  w_schema=new_sch
+0001f080: 656d 612c 0a20 2020 2020 2020 2020 2020  ema,.           
+0001f090: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0001f0a0: 3d6e 6577 5f64 6573 6372 6970 7469 6f6e  =new_description
+0001f0b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001f0c0: 2020 7474 6c3d 6e65 775f 7474 6c2c 0a20    ttl=new_ttl,. 
+0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001f0e0: 7279 5f72 756e 3d54 7275 652c 0a20 2020  ry_run=True,.   
+0001f0f0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0001f100: 6578 6573 3d6e 6577 5f69 6e64 6963 6573  exes=new_indices
+0001f110: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0001f120: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0001f130: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+0001f140: 2020 2069 6620 2254 6865 7265 2077 6572     if "There wer
+0001f150: 6520 6e6f 206f 7065 7261 7469 6f6e 7320  e no operations 
+0001f160: 746f 2070 6572 666f 726d 2220 696e 2073  to perform" in s
+0001f170: 7472 2865 293a 0a20 2020 2020 2020 2020  tr(e):.         
+0001f180: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+0001f190: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001f1a0: 2020 616c 7465 725f 6572 726f 725f 6d65    alter_error_me
+0001f1b0: 7373 6167 6520 3d20 7374 7228 6529 0a0a  ssage = str(e)..
+0001f1c0: 2020 2020 6966 2061 6c74 6572 5f72 6573      if alter_res
+0001f1d0: 706f 6e73 653a 0a20 2020 2020 2020 2069  ponse:.        i
+0001f1e0: 6620 6769 745f 7265 6c65 6173 6520 616e  f git_release an
+0001f1f0: 6420 6e6f 7420 736b 6970 5f63 6f6e 6669  d not skip_confi
+0001f200: 726d 6174 696f 6e3a 0a20 2020 2020 2020  rmation:.       
+0001f210: 2020 2020 2063 6c69 636b 2e65 6368 6f28       click.echo(
+0001f220: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
+0001f230: 696e 666f 5f63 7573 746f 6d5f 6465 706c  info_custom_depl
+0001f240: 6f79 6d65 6e74 2829 290a 2020 2020 2020  oyment()).      
+0001f250: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
+0001f260: 2822 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ("**************
 0001f270: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0001f280: 2a22 290a 2020 2020 2020 2020 2020 2020  *").            
-0001f290: 636c 6963 6b2e 6563 686f 2822 2a2a 2a2a  click.echo("****
-0001f2a0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+0001f280: 2a2a 2a2a 2a2a 2a2a 2a22 290a 2020 2020  *********").    
+0001f290: 2020 2020 2020 2020 636c 6963 6b2e 6563          click.ec
+0001f2a0: 686f 2822 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ho("************
 0001f2b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-0001f2c0: 2a2a 2a22 290a 2020 2020 2020 2020 636c  ***").        cl
-0001f2d0: 6963 6b2e 6563 686f 2846 6565 6462 6163  ick.echo(Feedbac
-0001f2e0: 6b4d 616e 6167 6572 2e69 6e66 6f5f 6461  kManager.info_da
-0001f2f0: 7461 736f 7572 6365 5f64 6f65 736e 745f  tasource_doesnt_
-0001f300: 6d61 7463 6828 6461 7461 736f 7572 6365  match(datasource
-0001f310: 3d64 735f 6e61 6d65 2929 0a20 2020 2020  =ds_name)).     
-0001f320: 2020 2066 6f72 206f 7065 7261 7469 6f6e     for operation
-0001f330: 2069 6e20 616c 7465 725f 7265 7370 6f6e   in alter_respon
-0001f340: 7365 5b22 6f70 6572 6174 696f 6e73 225d  se["operations"]
-0001f350: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-0001f360: 6963 6b2e 6563 686f 2866 222a 2a20 2020  ick.echo(f"**   
-0001f370: 2d20 207b 6f70 6572 6174 696f 6e7d 2229  -  {operation}")
-0001f380: 0a0a 2020 2020 2020 2020 6966 2073 6b69  ..        if ski
-0001f390: 705f 636f 6e66 6972 6d61 7469 6f6e 3a0a  p_confirmation:.
-0001f3a0: 2020 2020 2020 2020 2020 2020 6d61 6b65              make
-0001f3b0: 5f63 6861 6e67 6573 203d 2054 7275 650a  _changes = True.
-0001f3c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001f3d0: 2020 2020 2020 2020 2020 6d61 6b65 5f63            make_c
-0001f3e0: 6861 6e67 6573 203d 2063 6c69 636b 2e70  hanges = click.p
-0001f3f0: 726f 6d70 7428 4665 6564 6261 636b 4d61  rompt(FeedbackMa
-0001f400: 6e61 6765 722e 696e 666f 5f61 736b 5f66  nager.info_ask_f
-0001f410: 6f72 5f61 6c74 6572 5f63 6f6e 6669 726d  or_alter_confirm
-0001f420: 6174 696f 6e28 2929 2e6c 6f77 6572 2829  ation()).lower()
-0001f430: 203d 3d20 2279 220a 0a20 2020 2020 2020   == "y"..       
-0001f440: 2069 6620 6d61 6b65 5f63 6861 6e67 6573   if make_changes
-0001f450: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-0001f460: 6169 7420 636c 6965 6e74 2e61 6c74 6572  ait client.alter
-0001f470: 5f64 6174 6173 6f75 7263 6528 0a20 2020  _datasource(.   
-0001f480: 2020 2020 2020 2020 2020 2020 2064 735f               ds_
-0001f490: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0001f4a0: 2020 2020 2020 6e65 775f 7363 6865 6d61        new_schema
-0001f4b0: 3d6e 6577 5f73 6368 656d 612c 0a20 2020  =new_schema,.   
-0001f4c0: 2020 2020 2020 2020 2020 2020 2064 6573               des
-0001f4d0: 6372 6970 7469 6f6e 3d6e 6577 5f64 6573  cription=new_des
-0001f4e0: 6372 6970 7469 6f6e 2c0a 2020 2020 2020  cription,.      
-0001f4f0: 2020 2020 2020 2020 2020 7474 6c3d 6e65            ttl=ne
-0001f500: 775f 7474 6c2c 0a20 2020 2020 2020 2020  w_ttl,.         
-0001f510: 2020 2020 2020 2064 7279 5f72 756e 3d46         dry_run=F
-0001f520: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0001f530: 2020 2020 2020 696e 6465 7865 733d 6e65        indexes=ne
-0001f540: 775f 696e 6469 6365 732c 0a20 2020 2020  w_indices,.     
-0001f550: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001f560: 2020 2020 2063 6c69 636b 2e65 6368 6f28       click.echo(
-0001f570: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
-0001f580: 7375 6363 6573 735f 6461 7461 736f 7572  success_datasour
-0001f590: 6365 5f61 6c74 6572 2829 290a 2020 2020  ce_alter()).    
-0001f5a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001f5b0: 2020 2020 2020 616c 7465 725f 6572 726f        alter_erro
-0001f5c0: 725f 6d65 7373 6167 6520 3d20 2241 6c74  r_message = "Alt
-0001f5d0: 6572 2064 6174 6173 6f75 7263 6520 6361  er datasource ca
-0001f5e0: 6e63 656c 6c65 6422 0a0a 2020 2020 6966  ncelled"..    if
-0001f5f0: 2064 6174 6173 6f75 7263 655f 6578 6973   datasource_exis
-0001f600: 7473 2061 6e64 2064 735b 2270 6172 616d  ts and ds["param
-0001f610: 7322 5d2e 6765 7428 2262 6163 6b66 696c  s"].get("backfil
-0001f620: 6c5f 636f 6c75 6d6e 2229 2021 3d20 6578  l_column") != ex
-0001f630: 6973 7469 6e67 5f64 735b 2274 6167 7322  isting_ds["tags"
-0001f640: 5d2e 6765 7428 2262 6163 6b66 696c 6c5f  ].get("backfill_
-0001f650: 636f 6c75 6d6e 2229 3a0a 2020 2020 2020  column"):.      
-0001f660: 2020 7061 7261 6d73 203d 207b 0a20 2020    params = {.   
-0001f670: 2020 2020 2020 2020 2022 6261 636b 6669           "backfi
-0001f680: 6c6c 5f63 6f6c 756d 6e22 3a20 6473 5b22  ll_column": ds["
-0001f690: 7061 7261 6d73 225d 2e67 6574 2822 6261  params"].get("ba
-0001f6a0: 636b 6669 6c6c 5f63 6f6c 756d 6e22 292c  ckfill_column"),
-0001f6b0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-0001f6c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0001f6d0: 2020 2020 2063 6c69 636b 2e65 6368 6f28       click.echo(
-0001f6e0: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
-0001f6f0: 696e 666f 5f75 7064 6174 655f 6461 7461  info_update_data
-0001f700: 736f 7572 6365 2864 6174 6173 6f75 7263  source(datasourc
-0001f710: 653d 6473 5f6e 616d 652c 2070 6172 616d  e=ds_name, param
-0001f720: 733d 7061 7261 6d73 2929 0a20 2020 2020  s=params)).     
-0001f730: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
-0001f740: 656e 742e 7570 6461 7465 5f64 6174 6173  ent.update_datas
-0001f750: 6f75 7263 6528 6473 5f6e 616d 652c 2070  ource(ds_name, p
-0001f760: 6172 616d 7329 0a20 2020 2020 2020 2020  arams).         
-0001f770: 2020 2063 6c69 636b 2e65 6368 6f28 4665     click.echo(Fe
-0001f780: 6564 6261 636b 4d61 6e61 6765 722e 7375  edbackManager.su
-0001f790: 6363 6573 735f 7570 6461 7465 5f64 6174  ccess_update_dat
-0001f7a0: 6173 6f75 7263 6528 6461 7461 736f 7572  asource(datasour
-0001f7b0: 6365 3d64 735f 6e61 6d65 2c20 7061 7261  ce=ds_name, para
-0001f7c0: 6d73 3d70 6172 616d 7329 290a 2020 2020  ms=params)).    
-0001f7d0: 2020 2020 2020 2020 6d61 6b65 5f63 6861          make_cha
-0001f7e0: 6e67 6573 203d 2054 7275 650a 2020 2020  nges = True.    
-0001f7f0: 2020 2020 2020 2020 616c 7465 725f 7265          alter_re
-0001f800: 7370 6f6e 7365 203d 2054 7275 650a 2020  sponse = True.  
-0001f810: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-0001f820: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-0001f830: 2020 2020 2020 2020 2072 6169 7365 2063           raise c
-0001f840: 6c69 636b 2e43 6c69 636b 4578 6365 7074  lick.ClickExcept
-0001f850: 696f 6e28 4665 6564 6261 636b 4d61 6e61  ion(FeedbackMana
-0001f860: 6765 722e 6572 726f 725f 7570 6461 7469  ger.error_updati
-0001f870: 6e67 5f64 6174 6173 6f75 7263 6528 6461  ng_datasource(da
-0001f880: 7461 736f 7572 6365 3d64 735f 6e61 6d65  tasource=ds_name
-0001f890: 2c20 6572 726f 723d 7374 7228 6529 2929  , error=str(e)))
-0001f8a0: 0a0a 2020 2020 636f 6e6e 6563 746f 725f  ..    connector_
-0001f8b0: 6461 7461 203d 204e 6f6e 650a 2020 2020  data = None.    
-0001f8c0: 7072 6f6d 6f74 655f 6572 726f 725f 6d65  promote_error_me
-0001f8d0: 7373 6167 6520 3d20 4e6f 6e65 0a0a 2020  ssage = None..  
-0001f8e0: 2020 6473 5f70 6172 616d 7320 3d20 6473    ds_params = ds
-0001f8f0: 5b22 7061 7261 6d73 225d 0a20 2020 2073  ["params"].    s
-0001f900: 6572 7669 6365 203d 2064 735f 7061 7261  ervice = ds_para
-0001f910: 6d73 2e67 6574 2822 7365 7276 6963 6522  ms.get("service"
-0001f920: 290a 2020 2020 4441 5441 534f 5552 4345  ).    DATASOURCE
-0001f930: 5f56 414c 4944 5f53 4552 5649 4345 535f  _VALID_SERVICES_
-0001f940: 544f 5f55 5044 4154 4520 3d20 5b22 6269  TO_UPDATE = ["bi
-0001f950: 6771 7565 7279 222c 2022 736e 6f77 666c  gquery", "snowfl
-0001f960: 616b 6522 5d0a 2020 2020 6966 2064 6174  ake"].    if dat
-0001f970: 6173 6f75 7263 655f 6578 6973 7473 2061  asource_exists a
-0001f980: 6e64 2073 6572 7669 6365 2061 6e64 2073  nd service and s
-0001f990: 6572 7669 6365 2069 6e20 5b2a 4441 5441  ervice in [*DATA
-0001f9a0: 534f 5552 4345 5f56 414c 4944 5f53 4552  SOURCE_VALID_SER
-0001f9b0: 5649 4345 535f 544f 5f55 5044 4154 452c  VICES_TO_UPDATE,
-0001f9c0: 202a 5052 4556 4945 575f 434f 4e4e 4543   *PREVIEW_CONNEC
-0001f9d0: 544f 525f 5345 5256 4943 4553 5d3a 0a20  TOR_SERVICES]:. 
-0001f9e0: 2020 2020 2020 2063 6f6e 6e65 6374 6f72         connector
-0001f9f0: 5f72 6571 7569 7265 645f 7061 7261 6d73  _required_params
-0001fa00: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0001fa10: 2022 6269 6771 7565 7279 223a 205b 2273   "bigquery": ["s
-0001fa20: 6572 7669 6365 222c 2022 6372 6f6e 222c  ervice", "cron",
-0001fa30: 2022 6578 7465 726e 616c 5f64 6174 615f   "external_data_
-0001fa40: 736f 7572 6365 225d 2c0a 2020 2020 2020  source"],.      
-0001fa50: 2020 2020 2020 2273 6e6f 7766 6c61 6b65        "snowflake
-0001fa60: 223a 205b 2263 6f6e 6e65 6374 6f72 222c  ": ["connector",
-0001fa70: 2022 7365 7276 6963 6522 2c20 2263 726f   "service", "cro
-0001fa80: 6e22 2c20 2265 7874 6572 6e61 6c5f 6461  n", "external_da
-0001fa90: 7461 5f73 6f75 7263 6522 5d2c 0a20 2020  ta_source"],.   
-0001faa0: 2020 2020 2020 2020 2022 7333 223a 205b           "s3": [
-0001fab0: 2263 6f6e 6e65 6374 6f72 222c 2022 7365  "connector", "se
-0001fac0: 7276 6963 6522 2c20 2263 726f 6e22 2c20  rvice", "cron", 
-0001fad0: 2262 7563 6b65 745f 7572 6922 5d2c 0a20  "bucket_uri"],. 
-0001fae0: 2020 2020 2020 2020 2020 2022 7333 5f69             "s3_i
-0001faf0: 616d 726f 6c65 223a 205b 2263 6f6e 6e65  amrole": ["conne
-0001fb00: 6374 6f72 222c 2022 7365 7276 6963 6522  ctor", "service"
-0001fb10: 2c20 2263 726f 6e22 2c20 2262 7563 6b65  , "cron", "bucke
-0001fb20: 745f 7572 6922 5d2c 0a20 2020 2020 2020  t_uri"],.       
-0001fb30: 2020 2020 2022 6763 7322 3a20 5b22 636f       "gcs": ["co
-0001fb40: 6e6e 6563 746f 7222 2c20 2273 6572 7669  nnector", "servi
-0001fb50: 6365 222c 2022 6372 6f6e 222c 2022 6275  ce", "cron", "bu
-0001fb60: 636b 6574 5f75 7269 225d 2c0a 2020 2020  cket_uri"],.    
-0001fb70: 2020 2020 7d2e 6765 7428 7365 7276 6963      }.get(servic
-0001fb80: 652c 205b 5d29 0a0a 2020 2020 2020 2020  e, [])..        
-0001fb90: 6966 206e 6f74 2061 6c6c 286b 6579 2069  if not all(key i
-0001fba0: 6e20 6473 5f70 6172 616d 7320 666f 7220  n ds_params for 
-0001fbb0: 6b65 7920 696e 2063 6f6e 6e65 6374 6f72  key in connector
-0001fbc0: 5f72 6571 7569 7265 645f 7061 7261 6d73  _required_params
-0001fbd0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0001fbe0: 6574 7572 6e0a 0a20 2020 2020 2020 2063  eturn..        c
-0001fbf0: 6f6e 6e65 6374 6f72 203d 2064 735f 7061  onnector = ds_pa
-0001fc00: 7261 6d73 2e67 6574 2822 636f 6e6e 6563  rams.get("connec
-0001fc10: 746f 7222 2c20 4e6f 6e65 290a 0a20 2020  tor", None)..   
-0001fc20: 2020 2020 2069 6620 7365 7276 6963 6520       if service 
-0001fc30: 696e 2050 5245 5649 4557 5f43 4f4e 4e45  in PREVIEW_CONNE
-0001fc40: 4354 4f52 5f53 4552 5649 4345 533a 0a20  CTOR_SERVICES:. 
-0001fc50: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-0001fc60: 6374 6f72 5f69 6420 3d20 6578 6973 7469  ctor_id = existi
-0001fc70: 6e67 5f64 732e 6765 7428 2263 6f6e 6e65  ng_ds.get("conne
-0001fc80: 6374 6f72 222c 2022 2229 0a20 2020 2020  ctor", "").     
-0001fc90: 2020 2020 2020 2069 6620 6e6f 7420 636f         if not co
-0001fca0: 6e6e 6563 746f 725f 6964 3a0a 2020 2020  nnector_id:.    
-0001fcb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001fcc0: 726e 0a0a 2020 2020 2020 2020 2020 2020  rn..            
-0001fcd0: 6375 7272 656e 745f 636f 6e6e 6563 746f  current_connecto
-0001fce0: 7220 3d20 6177 6169 7420 636c 6965 6e74  r = await client
-0001fcf0: 2e67 6574 5f63 6f6e 6e65 6374 6f72 5f62  .get_connector_b
-0001fd00: 795f 6964 2865 7869 7374 696e 675f 6473  y_id(existing_ds
-0001fd10: 2e67 6574 2822 636f 6e6e 6563 746f 7222  .get("connector"
-0001fd20: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
-0001fd30: 2020 2069 6620 6e6f 7420 6375 7272 656e     if not curren
-0001fd40: 745f 636f 6e6e 6563 746f 723a 0a20 2020  t_connector:.   
-0001fd50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001fd60: 7572 6e0a 0a20 2020 2020 2020 2020 2020  urn..           
-0001fd70: 2069 6620 6375 7272 656e 745f 636f 6e6e   if current_conn
-0001fd80: 6563 746f 725b 226e 616d 6522 5d20 213d  ector["name"] !=
-0001fd90: 2064 735f 7061 7261 6d73 5b22 636f 6e6e   ds_params["conn
-0001fda0: 6563 7469 6f6e 225d 3a0a 2020 2020 2020  ection"]:.      
-0001fdb0: 2020 2020 2020 2020 2020 7061 7261 6d20            param 
-0001fdc0: 3d20 2263 6f6e 6e65 6374 696f 6e22 0a20  = "connection". 
-0001fdd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001fde0: 6174 6166 696c 655f 7061 7261 6d20 3d20  atafile_param = 
-0001fdf0: 496d 706f 7274 5265 706c 6163 656d 656e  ImportReplacemen
-0001fe00: 7473 2e67 6574 5f64 6174 6166 696c 655f  ts.get_datafile_
-0001fe10: 7061 7261 6d5f 666f 725f 6c69 6e6b 6572  param_for_linker
-0001fe20: 5f70 6172 616d 2873 6572 7669 6365 2c20  _param(service, 
-0001fe30: 7061 7261 6d29 206f 7220 7061 7261 6d0a  param) or param.
-0001fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe50: 7261 6973 6520 636c 6963 6b2e 436c 6963  raise click.Clic
-0001fe60: 6b45 7863 6570 7469 6f6e 2846 6565 6462  kException(Feedb
-0001fe70: 6163 6b4d 616e 6167 6572 2e65 7272 6f72  ackManager.error
-0001fe80: 5f75 7064 6174 696e 675f 636f 6e6e 6563  _updating_connec
-0001fe90: 746f 725f 6e6f 745f 7375 7070 6f72 7465  tor_not_supporte
-0001fea0: 6428 7061 7261 6d3d 6461 7461 6669 6c65  d(param=datafile
-0001feb0: 5f70 6172 616d 2929 0a0a 2020 2020 2020  _param))..      
-0001fec0: 2020 2020 2020 6c69 6e6b 6572 7320 3d20        linkers = 
-0001fed0: 6375 7272 656e 745f 636f 6e6e 6563 746f  current_connecto
-0001fee0: 722e 6765 7428 226c 696e 6b65 7273 222c  r.get("linkers",
-0001fef0: 205b 5d29 0a20 2020 2020 2020 2020 2020   []).           
-0001ff00: 206c 696e 6b65 7220 3d20 6e65 7874 2828   linker = next((
-0001ff10: 6c69 6e6b 6572 2066 6f72 206c 696e 6b65  linker for linke
-0001ff20: 7220 696e 206c 696e 6b65 7273 2069 6620  r in linkers if 
-0001ff30: 6c69 6e6b 6572 5b22 6461 7461 736f 7572  linker["datasour
-0001ff40: 6365 5f69 6422 5d20 3d3d 2065 7869 7374  ce_id"] == exist
-0001ff50: 696e 675f 6473 5b22 6964 225d 292c 204e  ing_ds["id"]), N
-0001ff60: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
-0001ff70: 2069 6620 6e6f 7420 6c69 6e6b 6572 3a0a   if not linker:.
-0001ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff90: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-0001ffa0: 2020 2020 6c69 6e6b 6572 5f73 6574 7469      linker_setti
-0001ffb0: 6e67 7320 3d20 6c69 6e6b 6572 2e67 6574  ngs = linker.get
-0001ffc0: 2822 7365 7474 696e 6773 222c 207b 7d29  ("settings", {})
-0001ffd0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0001ffe0: 2070 6172 616d 2c20 7661 6c75 6520 696e   param, value in
-0001fff0: 206c 696e 6b65 725f 7365 7474 696e 6773   linker_settings
-00020000: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00020010: 2020 2020 2020 2020 2020 6473 5f70 6172            ds_par
-00020020: 616d 735f 7661 6c75 6520 3d20 6473 5f70  ams_value = ds_p
-00020030: 6172 616d 732e 6765 7428 7061 7261 6d2c  arams.get(param,
-00020040: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
-00020050: 2020 2020 2020 2069 6620 6473 5f70 6172         if ds_par
-00020060: 616d 735f 7661 6c75 6520 616e 6420 6473  ams_value and ds
-00020070: 5f70 6172 616d 735f 7661 6c75 6520 213d  _params_value !=
-00020080: 2076 616c 7565 3a0a 2020 2020 2020 2020   value:.        
-00020090: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000200a0: 6669 6c65 5f70 6172 616d 203d 2049 6d70  file_param = Imp
-000200b0: 6f72 7452 6570 6c61 6365 6d65 6e74 732e  ortReplacements.
-000200c0: 6765 745f 6461 7461 6669 6c65 5f70 6172  get_datafile_par
-000200d0: 616d 5f66 6f72 5f6c 696e 6b65 725f 7061  am_for_linker_pa
-000200e0: 7261 6d28 7365 7276 6963 652c 2070 6172  ram(service, par
-000200f0: 616d 2920 6f72 2070 6172 616d 0a20 2020  am) or param.   
-00020100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020110: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00020120: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00020130: 2020 2020 2020 2020 2020 4665 6564 6261            Feedba
-00020140: 636b 4d61 6e61 6765 722e 6572 726f 725f  ckManager.error_
-00020150: 7570 6461 7469 6e67 5f63 6f6e 6e65 6374  updating_connect
-00020160: 6f72 5f6e 6f74 5f73 7570 706f 7274 6564  or_not_supported
-00020170: 2870 6172 616d 3d64 6174 6166 696c 655f  (param=datafile_
-00020180: 7061 7261 6d2e 7570 7065 7228 2929 0a20  param.upper()). 
-00020190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000201a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000201b0: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-000201c0: 2063 6f6e 6e65 6374 6f72 5f64 6174 6120   connector_data 
-000201d0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-000201e0: 2263 6f6e 6e65 6374 6f72 223a 2063 6f6e  "connector": con
-000201f0: 6e65 6374 6f72 2c0a 2020 2020 2020 2020  nector,.        
-00020200: 2020 2020 2273 6572 7669 6365 223a 2073      "service": s
-00020210: 6572 7669 6365 2c0a 2020 2020 2020 2020  ervice,.        
-00020220: 2020 2020 2263 726f 6e22 3a20 6473 5f70      "cron": ds_p
-00020230: 6172 616d 732e 6765 7428 2263 726f 6e22  arams.get("cron"
-00020240: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
-00020250: 2020 2020 2022 6578 7465 726e 616c 5f64       "external_d
-00020260: 6174 615f 736f 7572 6365 223a 2064 735f  ata_source": ds_
-00020270: 7061 7261 6d73 2e67 6574 2822 6578 7465  params.get("exte
-00020280: 726e 616c 5f64 6174 615f 736f 7572 6365  rnal_data_source
-00020290: 222c 204e 6f6e 6529 2c0a 2020 2020 2020  ", None),.      
-000202a0: 2020 2020 2020 2262 7563 6b65 745f 7572        "bucket_ur
-000202b0: 6922 3a20 6473 5f70 6172 616d 732e 6765  i": ds_params.ge
-000202c0: 7428 2262 7563 6b65 745f 7572 6922 2c20  t("bucket_uri", 
-000202d0: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
-000202e0: 2020 2022 6d6f 6465 223a 2064 735f 7061     "mode": ds_pa
-000202f0: 7261 6d73 2e67 6574 2822 6d6f 6465 222c  rams.get("mode",
-00020300: 2022 7265 706c 6163 6522 292c 0a20 2020   "replace"),.   
-00020310: 2020 2020 2020 2020 2022 7175 6572 7922           "query"
-00020320: 3a20 6473 5f70 6172 616d 732e 6765 7428  : ds_params.get(
-00020330: 2271 7565 7279 222c 204e 6f6e 6529 2c0a  "query", None),.
-00020340: 2020 2020 2020 2020 2020 2020 2269 6e67              "ing
-00020350: 6573 745f 6e6f 7722 3a20 6473 5f70 6172  est_now": ds_par
-00020360: 616d 732e 6765 7428 2269 6e67 6573 745f  ams.get("ingest_
-00020370: 6e6f 7722 2c20 4661 6c73 6529 2c0a 2020  now", False),.  
-00020380: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00020390: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000203a0: 2020 6177 6169 7420 636c 6965 6e74 2e75    await client.u
-000203b0: 7064 6174 655f 6461 7461 736f 7572 6365  pdate_datasource
-000203c0: 2864 735f 6e61 6d65 2c20 636f 6e6e 6563  (ds_name, connec
-000203d0: 746f 725f 6461 7461 290a 2020 2020 2020  tor_data).      
-000203e0: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
-000203f0: 2846 6565 6462 6163 6b4d 616e 6167 6572  (FeedbackManager
-00020400: 2e73 7563 6365 7373 5f70 726f 6d6f 7469  .success_promoti
-00020410: 6e67 5f64 6174 6173 6f75 7263 6528 6461  ng_datasource(da
-00020420: 7461 736f 7572 6365 3d64 735f 6e61 6d65  tasource=ds_name
-00020430: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-00020440: 6574 7572 6e0a 2020 2020 2020 2020 6578  eturn.        ex
-00020450: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00020460: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00020470: 2070 726f 6d6f 7465 5f65 7272 6f72 5f6d   promote_error_m
-00020480: 6573 7361 6765 203d 2073 7472 2865 290a  essage = str(e).
-00020490: 0a20 2020 2069 6620 616c 7465 725f 7265  .    if alter_re
-000204a0: 7370 6f6e 7365 2061 6e64 206d 616b 655f  sponse and make_
-000204b0: 6368 616e 6765 733a 0a20 2020 2020 2020  changes:.       
-000204c0: 2023 2061 6c74 6572 206f 7065 7261 7469   # alter operati
-000204d0: 6f6e 2066 696e 6973 6865 640a 2020 2020  on finished.    
-000204e0: 2020 2020 7265 7475 726e 0a20 2020 2023      return.    #
-000204f0: 2072 656d 6f76 6564 2072 6570 6c61 6369   removed replaci
-00020500: 6e67 2062 7920 6465 6661 756c 742e 2057  ng by default. W
-00020510: 6865 6e20 6120 6461 7461 736f 7572 6365  hen a datasource
-00020520: 2069 7320 7265 6d6f 7665 6420 6461 7461   is removed data
-00020530: 2069 730a 2020 2020 2320 7265 6d6f 7665   is.    # remove
-00020540: 6420 616e 6420 616c 6c20 7468 6520 7265  d and all the re
-00020550: 6665 7265 6e63 6573 206e 6565 6473 2074  ferences needs t
-00020560: 6f20 6265 2075 7064 6174 6564 0a20 2020  o be updated.   
-00020570: 2069 6620 280a 2020 2020 2020 2020 6f73   if (.        os
-00020580: 2e67 6574 656e 7628 2254 425f 495f 4b4e  .getenv("TB_I_KN
-00020590: 4f57 5f57 4841 545f 495f 414d 5f44 4f49  OW_WHAT_I_AM_DOI
-000205a0: 4e47 2229 0a20 2020 2020 2020 2061 6e64  NG").        and
-000205b0: 2063 6c69 636b 2e70 726f 6d70 7428 4665   click.prompt(Fe
-000205c0: 6564 6261 636b 4d61 6e61 6765 722e 696e  edbackManager.in
-000205d0: 666f 5f61 736b 5f66 6f72 5f64 6174 6173  fo_ask_for_datas
-000205e0: 6f75 7263 655f 636f 6e66 6972 6d61 7469  ource_confirmati
-000205f0: 6f6e 2829 2920 3d3d 2064 735f 6e61 6d65  on()) == ds_name
-00020600: 0a20 2020 2029 3a20 2023 2054 4f44 4f20  .    ):  # TODO 
-00020610: 6d6f 7665 2074 6f20 434c 490a 2020 2020  move to CLI.    
-00020620: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00020630: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-00020640: 742e 6461 7461 736f 7572 6365 5f64 656c  t.datasource_del
-00020650: 6574 6528 6473 5f6e 616d 6529 0a20 2020  ete(ds_name).   
-00020660: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-00020670: 6368 6f28 4665 6564 6261 636b 4d61 6e61  cho(FeedbackMana
-00020680: 6765 722e 7375 6363 6573 735f 6465 6c65  ger.success_dele
-00020690: 7465 5f64 6174 6173 6f75 7263 6528 6461  te_datasource(da
-000206a0: 7461 736f 7572 6365 3d64 735f 6e61 6d65  tasource=ds_name
-000206b0: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
-000206c0: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
-000206d0: 2020 2020 2020 2020 2072 6169 7365 2063           raise c
-000206e0: 6c69 636b 2e43 6c69 636b 4578 6365 7074  lick.ClickExcept
-000206f0: 696f 6e28 4665 6564 6261 636b 4d61 6e61  ion(FeedbackMana
-00020700: 6765 722e 6572 726f 725f 7265 6d6f 7669  ger.error_removi
-00020710: 6e67 5f64 6174 6173 6f75 7263 6528 6461  ng_datasource(da
-00020720: 7461 736f 7572 6365 3d64 735f 6e61 6d65  tasource=ds_name
-00020730: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-00020740: 6e0a 2020 2020 656c 7365 3a0a 2020 2020  n.    else:.    
-00020750: 2020 2020 6966 2061 6c74 6572 5f65 7272      if alter_err
-00020760: 6f72 5f6d 6573 7361 6765 3a0a 2020 2020  or_message:.    
-00020770: 2020 2020 2020 2020 7261 6973 6520 636c          raise cl
-00020780: 6963 6b2e 436c 6963 6b45 7863 6570 7469  ick.ClickExcepti
-00020790: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-000207a0: 2020 2020 4665 6564 6261 636b 4d61 6e61      FeedbackMana
-000207b0: 6765 722e 6572 726f 725f 6461 7461 736f  ger.error_dataso
-000207c0: 7572 6365 5f61 6c72 6561 6479 5f65 7869  urce_already_exi
-000207d0: 7374 735f 616e 645f 616c 7465 725f 6661  sts_and_alter_fa
-000207e0: 696c 6564 280a 2020 2020 2020 2020 2020  iled(.          
-000207f0: 2020 2020 2020 2020 2020 6461 7461 736f            dataso
-00020800: 7572 6365 3d64 735f 6e61 6d65 2c20 616c  urce=ds_name, al
-00020810: 7465 725f 6572 726f 725f 6d65 7373 6167  ter_error_messag
-00020820: 653d 616c 7465 725f 6572 726f 725f 6d65  e=alter_error_me
-00020830: 7373 6167 650a 2020 2020 2020 2020 2020  ssage.          
-00020840: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00020850: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00020860: 2070 726f 6d6f 7465 5f65 7272 6f72 5f6d   promote_error_m
-00020870: 6573 7361 6765 3a0a 2020 2020 2020 2020  essage:.        
-00020880: 2020 2020 7261 6973 6520 636c 6963 6b2e      raise click.
-00020890: 436c 6963 6b45 7863 6570 7469 6f6e 280a  ClickException(.
-000208a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208b0: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
-000208c0: 6572 726f 725f 7072 6f6d 6f74 696e 675f  error_promoting_
-000208d0: 6461 7461 736f 7572 6365 2864 6174 6173  datasource(datas
-000208e0: 6f75 7263 653d 6473 5f6e 616d 652c 2065  ource=ds_name, e
-000208f0: 7272 6f72 3d70 726f 6d6f 7465 5f65 7272  rror=promote_err
-00020900: 6f72 5f6d 6573 7361 6765 290a 2020 2020  or_message).    
-00020910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00020920: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00020930: 2020 2020 636c 6963 6b2e 6563 686f 2846      click.echo(F
-00020940: 6565 6462 6163 6b4d 616e 6167 6572 2e77  eedbackManager.w
-00020950: 6172 6e69 6e67 5f64 6174 6173 6f75 7263  arning_datasourc
-00020960: 655f 616c 7265 6164 795f 6578 6973 7473  e_already_exists
-00020970: 2864 6174 6173 6f75 7263 653d 6473 5f6e  (datasource=ds_n
-00020980: 616d 6529 290a 0a0a 6173 796e 6320 6465  ame))...async de
-00020990: 6620 6e65 775f 746f 6b65 6e28 746f 6b65  f new_token(toke
-000209a0: 6e3a 2044 6963 745b 7374 722c 2041 6e79  n: Dict[str, Any
-000209b0: 5d2c 2063 6c69 656e 743a 2054 696e 7942  ], client: TinyB
-000209c0: 2c20 666f 7263 653a 2062 6f6f 6c20 3d20  , force: bool = 
-000209d0: 4661 6c73 6529 3a0a 2020 2020 6578 6973  False):.    exis
-000209e0: 7469 6e67 5f74 6f6b 656e 203d 204e 6f6e  ting_token = Non
-000209f0: 650a 2020 2020 7472 793a 0a20 2020 2020  e.    try:.     
-00020a00: 2020 2065 7869 7374 696e 675f 746f 6b65     existing_toke
-00020a10: 6e20 3d20 6177 6169 7420 636c 6965 6e74  n = await client
-00020a20: 2e74 6f6b 656e 5f67 6574 2874 6f6b 656e  .token_get(token
-00020a30: 5b22 6e61 6d65 225d 290a 2020 2020 6578  ["name"]).    ex
-00020a40: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
-00020a50: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00020a60: 2020 6966 206e 6f74 2065 7869 7374 696e    if not existin
-00020a70: 675f 746f 6b65 6e3a 0a20 2020 2020 2020  g_token:.       
-00020a80: 2061 7761 6974 2063 6c69 656e 742e 746f   await client.to
-00020a90: 6b65 6e5f 6372 6561 7465 2874 6f6b 656e  ken_create(token
-00020aa0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00020ab0: 0a0a 2020 2020 6966 2066 6f72 6365 3a0a  ..    if force:.
-00020ac0: 2020 2020 2020 2020 4144 4d49 4e5f 5343          ADMIN_SC
-00020ad0: 4f50 4553 203d 205b 2241 444d 494e 222c  OPES = ["ADMIN",
-00020ae0: 2022 4144 4d49 4e5f 5553 4552 225d 0a20   "ADMIN_USER"]. 
-00020af0: 2020 2020 2020 2069 6620 616e 7928 5b73         if any([s
-00020b00: 636f 7065 5b22 7479 7065 225d 2069 6e20  cope["type"] in 
-00020b10: 4144 4d49 4e5f 5343 4f50 4553 2066 6f72  ADMIN_SCOPES for
-00020b20: 2073 636f 7065 2069 6e20 6578 6973 7469   scope in existi
-00020b30: 6e67 5f74 6f6b 656e 5b22 7363 6f70 6573  ng_token["scopes
-00020b40: 225d 5d29 3a0a 2020 2020 2020 2020 2020  "]]):.          
-00020b50: 2020 7261 6973 6520 636c 6963 6b2e 436c    raise click.Cl
-00020b60: 6963 6b45 7863 6570 7469 6f6e 2846 6565  ickException(Fee
-00020b70: 6462 6163 6b4d 616e 6167 6572 2e65 7272  dbackManager.err
-00020b80: 6f72 5f74 6f6b 656e 5f63 616e 6e6f 745f  or_token_cannot_
-00020b90: 6265 5f6f 7665 7272 6964 656e 2874 6f6b  be_overriden(tok
-00020ba0: 656e 3d74 6f6b 656e 5b22 6e61 6d65 225d  en=token["name"]
-00020bb0: 2929 0a0a 2020 2020 2020 2020 6177 6169  ))..        awai
-00020bc0: 7420 636c 6965 6e74 2e74 6f6b 656e 5f75  t client.token_u
-00020bd0: 7064 6174 6528 746f 6b65 6e29 0a20 2020  pdate(token).   
-00020be0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00020bf0: 2072 6169 7365 2063 6c69 636b 2e43 6c69   raise click.Cli
-00020c00: 636b 4578 6365 7074 696f 6e28 4665 6564  ckException(Feed
-00020c10: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
-00020c20: 725f 746f 6b65 6e5f 616c 7265 6164 795f  r_token_already_
-00020c30: 6578 6973 7473 2874 6f6b 656e 3d74 6f6b  exists(token=tok
-00020c40: 656e 5b22 6e61 6d65 225d 2929 0a0a 0a61  en["name"]))...a
-00020c50: 7379 6e63 2064 6566 2065 7865 635f 6669  sync def exec_fi
-00020c60: 6c65 280a 2020 2020 636f 6e66 6967 3a20  le(.    config: 
-00020c70: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00020c80: 722c 2041 6e79 5d5d 2c0a 2020 2020 723a  r, Any]],.    r:
-00020c90: 2044 6963 745b 7374 722c 2041 6e79 5d2c   Dict[str, Any],
-00020ca0: 0a20 2020 2074 625f 636c 6965 6e74 3a20  .    tb_client: 
-00020cb0: 5469 6e79 422c 0a20 2020 2066 6f72 6365  TinyB,.    force
-00020cc0: 3a20 626f 6f6c 2c0a 2020 2020 6368 6563  : bool,.    chec
-00020cd0: 6b3a 2062 6f6f 6c2c 0a20 2020 2064 6562  k: bool,.    deb
-00020ce0: 7567 3a20 626f 6f6c 2c0a 2020 2020 706f  ug: bool,.    po
-00020cf0: 7075 6c61 7465 3a20 626f 6f6c 2c0a 2020  pulate: bool,.  
-00020d00: 2020 706f 7075 6c61 7465 5f73 7562 7365    populate_subse
-00020d10: 742c 0a20 2020 2070 6f70 756c 6174 655f  t,.    populate_
-00020d20: 636f 6e64 6974 696f 6e2c 0a20 2020 2075  condition,.    u
-00020d30: 6e6c 696e 6b5f 6f6e 5f70 6f70 756c 6174  nlink_on_populat
-00020d40: 655f 6572 726f 722c 0a20 2020 2077 6169  e_error,.    wai
-00020d50: 745f 706f 7075 6c61 7465 2c0a 2020 2020  t_populate,.    
-00020d60: 7573 6572 5f74 6f6b 656e 3a20 4f70 7469  user_token: Opti
-00020d70: 6f6e 616c 5b73 7472 5d2c 0a20 2020 206f  onal[str],.    o
-00020d80: 7665 7272 6964 655f 6461 7461 736f 7572  verride_datasour
-00020d90: 6365 3a20 626f 6f6c 203d 2046 616c 7365  ce: bool = False
-00020da0: 2c0a 2020 2020 6967 6e6f 7265 5f73 716c  ,.    ignore_sql
-00020db0: 5f65 7272 6f72 733a 2062 6f6f 6c20 3d20  _errors: bool = 
-00020dc0: 4661 6c73 652c 0a20 2020 2073 6b69 705f  False,.    skip_
-00020dd0: 636f 6e66 6972 6d61 7469 6f6e 3a20 626f  confirmation: bo
-00020de0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00020df0: 6f6e 6c79 5f72 6573 706f 6e73 655f 7469  only_response_ti
-00020e00: 6d65 733a 2062 6f6f 6c20 3d20 4661 6c73  mes: bool = Fals
-00020e10: 652c 0a20 2020 2074 696d 656f 7574 3d4e  e,.    timeout=N
-00020e20: 6f6e 652c 0a20 2020 2072 756e 5f74 6573  one,.    run_tes
-00020e30: 7473 3d46 616c 7365 2c0a 2020 2020 6173  ts=False,.    as
-00020e40: 5f73 7461 6e64 6172 643d 4661 6c73 652c  _standard=False,
-00020e50: 0a20 2020 2074 6573 7473 5f74 6f5f 7275  .    tests_to_ru
-00020e60: 6e3a 2069 6e74 203d 2030 2c0a 2020 2020  n: int = 0,.    
-00020e70: 7465 7374 735f 746f 5f73 616d 706c 655f  tests_to_sample_
-00020e80: 6279 5f70 6172 616d 733a 2069 6e74 203d  by_params: int =
-00020e90: 2030 2c0a 2020 2020 7465 7374 735f 6669   0,.    tests_fi
-00020ea0: 6c74 6572 5f62 793a 204f 7074 696f 6e61  lter_by: Optiona
-00020eb0: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
-00020ec0: 6f6e 652c 0a20 2020 2074 6573 7473 5f66  one,.    tests_f
-00020ed0: 6169 6c66 6173 743a 2062 6f6f 6c20 3d20  ailfast: bool = 
-00020ee0: 4661 6c73 652c 0a20 2020 2074 6573 7473  False,.    tests
-00020ef0: 5f69 676e 6f72 655f 6f72 6465 723a 2062  _ignore_order: b
-00020f00: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-00020f10: 2074 6573 7473 5f76 616c 6964 6174 655f   tests_validate_
-00020f20: 7072 6f63 6573 7365 645f 6279 7465 733a  processed_bytes:
-00020f30: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00020f40: 2020 2074 6573 7473 5f63 6865 636b 5f72     tests_check_r
-00020f50: 6571 7565 7374 735f 6672 6f6d 5f62 7261  equests_from_bra
-00020f60: 6e63 683a 2062 6f6f 6c20 3d20 4661 6c73  nch: bool = Fals
-00020f70: 652c 0a20 2020 2063 7572 7265 6e74 5f77  e,.    current_w
-00020f80: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
-00020f90: 5b73 7472 2c20 416e 795d 5d20 3d20 4e6f  [str, Any]] = No
-00020fa0: 6e65 2c0a 2020 2020 666f 726b 5f64 6f77  ne,.    fork_dow
-00020fb0: 6e73 7472 6561 6d3a 204f 7074 696f 6e61  nstream: Optiona
-00020fc0: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-00020fd0: 0a20 2020 2066 6f72 6b3a 204f 7074 696f  .    fork: Optio
-00020fe0: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
-00020ff0: 652c 0a20 2020 2067 6974 5f72 656c 6561  e,.    git_relea
-00021000: 7365 3a20 4f70 7469 6f6e 616c 5b62 6f6f  se: Optional[boo
-00021010: 6c5d 203d 2046 616c 7365 2c0a 293a 0a20  l] = False,.):. 
-00021020: 2020 2069 6620 6465 6275 673a 0a20 2020     if debug:.   
-00021030: 2020 2020 2063 6c69 636b 2e65 6368 6f28       click.echo(
-00021040: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
-00021050: 6465 6275 675f 7275 6e6e 696e 675f 6669  debug_running_fi
-00021060: 6c65 2866 696c 653d 7070 2e70 666f 726d  le(file=pp.pform
-00021070: 6174 2872 2929 290a 2020 2020 6966 2072  at(r))).    if r
-00021080: 5b22 7265 736f 7572 6365 225d 203d 3d20  ["resource"] == 
-00021090: 2270 6970 6573 223a 0a20 2020 2020 2020  "pipes":.       
-000210a0: 2061 7761 6974 206e 6577 5f70 6970 6528   await new_pipe(
-000210b0: 0a20 2020 2020 2020 2020 2020 2072 2c0a  .            r,.
-000210c0: 2020 2020 2020 2020 2020 2020 7462 5f63              tb_c
-000210d0: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
-000210e0: 2020 2066 6f72 6365 2c0a 2020 2020 2020     force,.      
-000210f0: 2020 2020 2020 6368 6563 6b2c 0a20 2020        check,.   
-00021100: 2020 2020 2020 2020 2070 6f70 756c 6174           populat
-00021110: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
-00021120: 6f70 756c 6174 655f 7375 6273 6574 2c0a  opulate_subset,.
-00021130: 2020 2020 2020 2020 2020 2020 706f 7075              popu
-00021140: 6c61 7465 5f63 6f6e 6469 7469 6f6e 2c0a  late_condition,.
-00021150: 2020 2020 2020 2020 2020 2020 756e 6c69              unli
-00021160: 6e6b 5f6f 6e5f 706f 7075 6c61 7465 5f65  nk_on_populate_e
-00021170: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
-00021180: 2020 7761 6974 5f70 6f70 756c 6174 652c    wait_populate,
-00021190: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-000211a0: 6f72 655f 7371 6c5f 6572 726f 7273 3d69  ore_sql_errors=i
-000211b0: 676e 6f72 655f 7371 6c5f 6572 726f 7273  gnore_sql_errors
-000211c0: 2c0a 2020 2020 2020 2020 2020 2020 6f6e  ,.            on
-000211d0: 6c79 5f72 6573 706f 6e73 655f 7469 6d65  ly_response_time
-000211e0: 733d 6f6e 6c79 5f72 6573 706f 6e73 655f  s=only_response_
-000211f0: 7469 6d65 732c 0a20 2020 2020 2020 2020  times,.         
-00021200: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
-00021210: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
-00021220: 7275 6e5f 7465 7374 733d 7275 6e5f 7465  run_tests=run_te
-00021230: 7374 732c 0a20 2020 2020 2020 2020 2020  sts,.           
-00021240: 2061 735f 7374 616e 6461 7264 3d61 735f   as_standard=as_
-00021250: 7374 616e 6461 7264 2c0a 2020 2020 2020  standard,.      
-00021260: 2020 2020 2020 7465 7374 735f 746f 5f72        tests_to_r
-00021270: 756e 3d74 6573 7473 5f74 6f5f 7275 6e2c  un=tests_to_run,
-00021280: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00021290: 7473 5f74 6f5f 7361 6d70 6c65 5f62 795f  ts_to_sample_by_
-000212a0: 7061 7261 6d73 3d74 6573 7473 5f74 6f5f  params=tests_to_
-000212b0: 7361 6d70 6c65 5f62 795f 7061 7261 6d73  sample_by_params
-000212c0: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
-000212d0: 7374 735f 6669 6c74 6572 5f62 793d 7465  sts_filter_by=te
-000212e0: 7374 735f 6669 6c74 6572 5f62 792c 0a20  sts_filter_by,. 
-000212f0: 2020 2020 2020 2020 2020 2074 6573 7473             tests
-00021300: 5f66 6169 6c66 6173 743d 7465 7374 735f  _failfast=tests_
-00021310: 6661 696c 6661 7374 2c0a 2020 2020 2020  failfast,.      
-00021320: 2020 2020 2020 7465 7374 735f 6967 6e6f        tests_igno
-00021330: 7265 5f6f 7264 6572 3d74 6573 7473 5f69  re_order=tests_i
-00021340: 676e 6f72 655f 6f72 6465 722c 0a20 2020  gnore_order,.   
-00021350: 2020 2020 2020 2020 2074 6573 7473 5f76           tests_v
-00021360: 616c 6964 6174 655f 7072 6f63 6573 7365  alidate_processe
-00021370: 645f 6279 7465 733d 7465 7374 735f 7661  d_bytes=tests_va
-00021380: 6c69 6461 7465 5f70 726f 6365 7373 6564  lidate_processed
-00021390: 5f62 7974 6573 2c0a 2020 2020 2020 2020  _bytes,.        
-000213a0: 2020 2020 6f76 6572 7269 6465 5f64 6174      override_dat
-000213b0: 6173 6f75 7263 653d 6f76 6572 7269 6465  asource=override
-000213c0: 5f64 6174 6173 6f75 7263 652c 0a20 2020  _datasource,.   
-000213d0: 2020 2020 2020 2020 2074 6573 7473 5f63           tests_c
-000213e0: 6865 636b 5f72 6571 7565 7374 735f 6672  heck_requests_fr
-000213f0: 6f6d 5f62 7261 6e63 683d 7465 7374 735f  om_branch=tests_
-00021400: 6368 6563 6b5f 7265 7175 6573 7473 5f66  check_requests_f
-00021410: 726f 6d5f 6272 616e 6368 2c0a 2020 2020  rom_branch,.    
-00021420: 2020 2020 2020 2020 666f 726b 5f64 6f77          fork_dow
-00021430: 6e73 7472 6561 6d3d 666f 726b 5f64 6f77  nstream=fork_dow
-00021440: 6e73 7472 6561 6d2c 0a20 2020 2020 2020  nstream,.       
-00021450: 2020 2020 2066 6f72 6b3d 666f 726b 2c0a       fork=fork,.
-00021460: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00021470: 6966 2072 5b22 7265 736f 7572 6365 225d  if r["resource"]
-00021480: 203d 3d20 2264 6174 6173 6f75 7263 6573   == "datasources
-00021490: 223a 0a20 2020 2020 2020 2061 7761 6974  ":.        await
-000214a0: 206e 6577 5f64 7328 0a20 2020 2020 2020   new_ds(.       
-000214b0: 2020 2020 2072 2c0a 2020 2020 2020 2020       r,.        
-000214c0: 2020 2020 7462 5f63 6c69 656e 742c 0a20      tb_client,. 
-000214d0: 2020 2020 2020 2020 2020 2075 7365 725f             user_
-000214e0: 746f 6b65 6e2c 0a20 2020 2020 2020 2020  token,.         
-000214f0: 2020 2066 6f72 6365 2c0a 2020 2020 2020     force,.      
-00021500: 2020 2020 2020 736b 6970 5f63 6f6e 6669        skip_confi
-00021510: 726d 6174 696f 6e3d 736b 6970 5f63 6f6e  rmation=skip_con
-00021520: 6669 726d 6174 696f 6e2c 0a20 2020 2020  firmation,.     
-00021530: 2020 2020 2020 2063 7572 7265 6e74 5f77         current_w
-00021540: 733d 6375 7272 656e 745f 7773 2c0a 2020  s=current_ws,.  
-00021550: 2020 2020 2020 2020 2020 666f 726b 5f64            fork_d
-00021560: 6f77 6e73 7472 6561 6d3d 666f 726b 5f64  ownstream=fork_d
-00021570: 6f77 6e73 7472 6561 6d2c 0a20 2020 2020  ownstream,.     
-00021580: 2020 2020 2020 2066 6f72 6b3d 666f 726b         fork=fork
-00021590: 2c0a 2020 2020 2020 2020 2020 2020 6769  ,.            gi
-000215a0: 745f 7265 6c65 6173 653d 6769 745f 7265  t_release=git_re
-000215b0: 6c65 6173 652c 0a20 2020 2020 2020 2029  lease,.        )
-000215c0: 0a20 2020 2065 6c69 6620 725b 2272 6573  .    elif r["res
-000215d0: 6f75 7263 6522 5d20 3d3d 2022 746f 6b65  ource"] == "toke
-000215e0: 6e73 223a 0a20 2020 2020 2020 2061 7761  ns":.        awa
-000215f0: 6974 206e 6577 5f74 6f6b 656e 2872 2c20  it new_token(r, 
-00021600: 7462 5f63 6c69 656e 742c 2066 6f72 6365  tb_client, force
-00021610: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00021620: 2020 2020 7261 6973 6520 636c 6963 6b2e      raise click.
-00021630: 436c 6963 6b45 7863 6570 7469 6f6e 2846  ClickException(F
-00021640: 6565 6462 6163 6b4d 616e 6167 6572 2e65  eedbackManager.e
-00021650: 7272 6f72 5f75 6e6b 6e6f 776e 5f72 6573  rror_unknown_res
-00021660: 6f75 7263 6528 7265 736f 7572 6365 3d72  ource(resource=r
-00021670: 5b22 7265 736f 7572 6365 225d 2929 0a0a  ["resource"]))..
-00021680: 0a64 6566 2067 6574 5f6e 616d 655f 7665  .def get_name_ve
-00021690: 7273 696f 6e28 6473 3a20 7374 7229 202d  rsion(ds: str) -
-000216a0: 3e20 4469 6374 5b73 7472 2c20 416e 795d  > Dict[str, Any]
-000216b0: 3a0a 2020 2020 2222 220a 2020 2020 4769  :.    """.    Gi
-000216c0: 7665 6e20 6120 6e61 6d65 206c 696b 6520  ven a name like 
-000216d0: 226e 616d 655f 5f64 6576 5f5f 7630 2220  "name__dev__v0" 
-000216e0: 7265 7475 726e 7320 5b27 6e61 6d65 272c  returns ['name',
-000216f0: 2027 6465 7627 2c20 2776 3027 5d0a 2020   'dev', 'v0'].  
-00021700: 2020 3e3e 3e20 6765 745f 6e61 6d65 5f76    >>> get_name_v
-00021710: 6572 7369 6f6e 2827 6465 765f 5f6e 616d  ersion('dev__nam
-00021720: 655f 5f76 3027 290a 2020 2020 7b27 6e61  e__v0').    {'na
-00021730: 6d65 273a 2027 6465 765f 5f6e 616d 6527  me': 'dev__name'
-00021740: 2c20 2776 6572 7369 6f6e 273a 2030 7d0a  , 'version': 0}.
-00021750: 2020 2020 3e3e 3e20 6765 745f 6e61 6d65      >>> get_name
-00021760: 5f76 6572 7369 6f6e 2827 6e61 6d65 5f5f  _version('name__
-00021770: 7630 2729 0a20 2020 207b 276e 616d 6527  v0').    {'name'
-00021780: 3a20 276e 616d 6527 2c20 2776 6572 7369  : 'name', 'versi
-00021790: 6f6e 273a 2030 7d0a 2020 2020 3e3e 3e20  on': 0}.    >>> 
-000217a0: 6765 745f 6e61 6d65 5f76 6572 7369 6f6e  get_name_version
-000217b0: 2827 6465 765f 5f6e 616d 6527 290a 2020  ('dev__name').  
-000217c0: 2020 7b27 6e61 6d65 273a 2027 6465 765f    {'name': 'dev_
-000217d0: 5f6e 616d 6527 2c20 2776 6572 7369 6f6e  _name', 'version
-000217e0: 273a 204e 6f6e 657d 0a20 2020 203e 3e3e  ': None}.    >>>
-000217f0: 2067 6574 5f6e 616d 655f 7665 7273 696f   get_name_versio
-00021800: 6e28 276e 616d 6527 290a 2020 2020 7b27  n('name').    {'
-00021810: 6e61 6d65 273a 2027 6e61 6d65 272c 2027  name': 'name', '
-00021820: 7665 7273 696f 6e27 3a20 4e6f 6e65 7d0a  version': None}.
-00021830: 2020 2020 3e3e 3e20 6765 745f 6e61 6d65      >>> get_name
-00021840: 5f76 6572 7369 6f6e 2827 686f 7261 7269  _version('horari
-00021850: 6f5f 5f33 5f5f 7069 7065 2729 0a20 2020  o__3__pipe').   
-00021860: 207b 276e 616d 6527 3a20 2768 6f72 6172   {'name': 'horar
-00021870: 696f 5f5f 335f 5f70 6970 6527 2c20 2776  io__3__pipe', 'v
-00021880: 6572 7369 6f6e 273a 204e 6f6e 657d 0a20  ersion': None}. 
-00021890: 2020 203e 3e3e 2067 6574 5f6e 616d 655f     >>> get_name_
-000218a0: 7665 7273 696f 6e28 2768 6f72 6172 696f  version('horario
-000218b0: 5f5f 6368 6563 6b65 7227 290a 2020 2020  __checker').    
-000218c0: 7b27 6e61 6d65 273a 2027 686f 7261 7269  {'name': 'horari
-000218d0: 6f5f 5f63 6865 636b 6572 272c 2027 7665  o__checker', 've
-000218e0: 7273 696f 6e27 3a20 4e6f 6e65 7d0a 2020  rsion': None}.  
-000218f0: 2020 3e3e 3e20 6765 745f 6e61 6d65 5f76    >>> get_name_v
-00021900: 6572 7369 6f6e 2827 6465 765f 5f68 6f72  ersion('dev__hor
-00021910: 6172 696f 5f5f 6368 6563 6b65 7227 290a  ario__checker').
-00021920: 2020 2020 7b27 6e61 6d65 273a 2027 6465      {'name': 'de
-00021930: 765f 5f68 6f72 6172 696f 5f5f 6368 6563  v__horario__chec
-00021940: 6b65 7227 2c20 2776 6572 7369 6f6e 273a  ker', 'version':
-00021950: 204e 6f6e 657d 0a20 2020 203e 3e3e 2067   None}.    >>> g
-00021960: 6574 5f6e 616d 655f 7665 7273 696f 6e28  et_name_version(
-00021970: 2774 675f 5f64 4163 7469 7669 6461 6465  'tg__dActividade
-00021980: 735f 5f76 305f 7069 7065 5f33 3930 3727  s__v0_pipe_3907'
-00021990: 290a 2020 2020 7b27 6e61 6d65 273a 2027  ).    {'name': '
-000219a0: 7467 5f5f 6441 6374 6976 6964 6164 6573  tg__dActividades
-000219b0: 272c 2027 7665 7273 696f 6e27 3a20 307d  ', 'version': 0}
-000219c0: 0a20 2020 203e 3e3e 2067 6574 5f6e 616d  .    >>> get_nam
-000219d0: 655f 7665 7273 696f 6e28 2774 675f 5f64  e_version('tg__d
-000219e0: 4163 7469 7669 6461 6465 735f 5f76 615f  Actividades__va_
-000219f0: 7069 7065 5f33 3930 3727 290a 2020 2020  pipe_3907').    
-00021a00: 7b27 6e61 6d65 273a 2027 7467 5f5f 6441  {'name': 'tg__dA
-00021a10: 6374 6976 6964 6164 6573 5f5f 7661 5f70  ctividades__va_p
-00021a20: 6970 655f 3339 3037 272c 2027 7665 7273  ipe_3907', 'vers
-00021a30: 696f 6e27 3a20 4e6f 6e65 7d0a 2020 2020  ion': None}.    
-00021a40: 3e3e 3e20 6765 745f 6e61 6d65 5f76 6572  >>> get_name_ver
-00021a50: 7369 6f6e 2827 7467 5f5f 6f72 6967 696e  sion('tg__origin
-00021a60: 5f77 6f72 6b73 7061 6365 2e73 6861 7265  _workspace.share
-00021a70: 645f 6473 5f5f 7633 3930 3727 290a 2020  d_ds__v3907').  
-00021a80: 2020 7b27 6e61 6d65 273a 2027 7467 5f5f    {'name': 'tg__
-00021a90: 6f72 6967 696e 5f77 6f72 6b73 7061 6365  origin_workspace
-00021aa0: 2e73 6861 7265 645f 6473 272c 2027 7665  .shared_ds', 've
-00021ab0: 7273 696f 6e27 3a20 3339 3037 7d0a 2020  rsion': 3907}.  
-00021ac0: 2020 3e3e 3e20 6765 745f 6e61 6d65 5f76    >>> get_name_v
-00021ad0: 6572 7369 6f6e 2827 746d 7068 3865 6774  ersion('tmph8egt
-00021ae0: 6c5f 5f27 290a 2020 2020 7b27 6e61 6d65  l__').    {'name
-00021af0: 273a 2027 746d 7068 3865 6774 6c5f 5f27  ': 'tmph8egtl__'
-00021b00: 2c20 2776 6572 7369 6f6e 273a 204e 6f6e  , 'version': Non
-00021b10: 657d 0a20 2020 203e 3e3e 2067 6574 5f6e  e}.    >>> get_n
-00021b20: 616d 655f 7665 7273 696f 6e28 2774 6d70  ame_version('tmp
-00021b30: 6838 6567 746c 5f5f 3132 335f 5f27 290a  h8egtl__123__').
-00021b40: 2020 2020 7b27 6e61 6d65 273a 2027 746d      {'name': 'tm
-00021b50: 7068 3865 6774 6c5f 5f31 3233 5f5f 272c  ph8egtl__123__',
-00021b60: 2027 7665 7273 696f 6e27 3a20 4e6f 6e65   'version': None
-00021b70: 7d0a 2020 2020 3e3e 3e20 6765 745f 6e61  }.    >>> get_na
-00021b80: 6d65 5f76 6572 7369 6f6e 2827 6465 765f  me_version('dev_
-00021b90: 5f6e 616d 655f 5f76 3027 290a 2020 2020  _name__v0').    
-00021ba0: 7b27 6e61 6d65 273a 2027 6465 765f 5f6e  {'name': 'dev__n
-00021bb0: 616d 6527 2c20 2776 6572 7369 6f6e 273a  ame', 'version':
-00021bc0: 2030 7d0a 2020 2020 3e3e 3e20 6765 745f   0}.    >>> get_
-00021bd0: 6e61 6d65 5f76 6572 7369 6f6e 2827 6e61  name_version('na
-00021be0: 6d65 5f5f 7630 2729 0a20 2020 207b 276e  me__v0').    {'n
-00021bf0: 616d 6527 3a20 276e 616d 6527 2c20 2776  ame': 'name', 'v
-00021c00: 6572 7369 6f6e 273a 2030 7d0a 2020 2020  ersion': 0}.    
-00021c10: 3e3e 3e20 6765 745f 6e61 6d65 5f76 6572  >>> get_name_ver
-00021c20: 7369 6f6e 2827 6465 765f 5f6e 616d 6527  sion('dev__name'
-00021c30: 290a 2020 2020 7b27 6e61 6d65 273a 2027  ).    {'name': '
-00021c40: 6465 765f 5f6e 616d 6527 2c20 2776 6572  dev__name', 'ver
-00021c50: 7369 6f6e 273a 204e 6f6e 657d 0a20 2020  sion': None}.   
-00021c60: 203e 3e3e 2067 6574 5f6e 616d 655f 7665   >>> get_name_ve
-00021c70: 7273 696f 6e28 276e 616d 6527 290a 2020  rsion('name').  
-00021c80: 2020 7b27 6e61 6d65 273a 2027 6e61 6d65    {'name': 'name
-00021c90: 272c 2027 7665 7273 696f 6e27 3a20 4e6f  ', 'version': No
-00021ca0: 6e65 7d0a 2020 2020 3e3e 3e20 6765 745f  ne}.    >>> get_
-00021cb0: 6e61 6d65 5f76 6572 7369 6f6e 2827 686f  name_version('ho
-00021cc0: 7261 7269 6f5f 5f33 5f5f 7069 7065 2729  rario__3__pipe')
-00021cd0: 0a20 2020 207b 276e 616d 6527 3a20 2768  .    {'name': 'h
-00021ce0: 6f72 6172 696f 5f5f 335f 5f70 6970 6527  orario__3__pipe'
-00021cf0: 2c20 2776 6572 7369 6f6e 273a 204e 6f6e  , 'version': Non
-00021d00: 657d 0a20 2020 203e 3e3e 2067 6574 5f6e  e}.    >>> get_n
-00021d10: 616d 655f 7665 7273 696f 6e28 2768 6f72  ame_version('hor
-00021d20: 6172 696f 5f5f 6368 6563 6b65 7227 290a  ario__checker').
-00021d30: 2020 2020 7b27 6e61 6d65 273a 2027 686f      {'name': 'ho
-00021d40: 7261 7269 6f5f 5f63 6865 636b 6572 272c  rario__checker',
-00021d50: 2027 7665 7273 696f 6e27 3a20 4e6f 6e65   'version': None
-00021d60: 7d0a 2020 2020 3e3e 3e20 6765 745f 6e61  }.    >>> get_na
-00021d70: 6d65 5f76 6572 7369 6f6e 2827 6465 765f  me_version('dev_
-00021d80: 5f68 6f72 6172 696f 5f5f 6368 6563 6b65  _horario__checke
-00021d90: 7227 290a 2020 2020 7b27 6e61 6d65 273a  r').    {'name':
-00021da0: 2027 6465 765f 5f68 6f72 6172 696f 5f5f   'dev__horario__
-00021db0: 6368 6563 6b65 7227 2c20 2776 6572 7369  checker', 'versi
-00021dc0: 6f6e 273a 204e 6f6e 657d 0a20 2020 203e  on': None}.    >
-00021dd0: 3e3e 2067 6574 5f6e 616d 655f 7665 7273  >> get_name_vers
-00021de0: 696f 6e28 2774 675f 5f64 4163 7469 7669  ion('tg__dActivi
-00021df0: 6461 6465 735f 5f76 305f 7069 7065 5f33  dades__v0_pipe_3
-00021e00: 3930 3727 290a 2020 2020 7b27 6e61 6d65  907').    {'name
-00021e10: 273a 2027 7467 5f5f 6441 6374 6976 6964  ': 'tg__dActivid
-00021e20: 6164 6573 272c 2027 7665 7273 696f 6e27  ades', 'version'
-00021e30: 3a20 307d 0a20 2020 203e 3e3e 2067 6574  : 0}.    >>> get
-00021e40: 5f6e 616d 655f 7665 7273 696f 6e28 2774  _name_version('t
-00021e50: 675f 5f6f 7269 6769 6e5f 776f 726b 7370  g__origin_worksp
-00021e60: 6163 652e 7368 6172 6564 5f64 735f 5f76  ace.shared_ds__v
-00021e70: 3339 3037 2729 0a20 2020 207b 276e 616d  3907').    {'nam
-00021e80: 6527 3a20 2774 675f 5f6f 7269 6769 6e5f  e': 'tg__origin_
-00021e90: 776f 726b 7370 6163 652e 7368 6172 6564  workspace.shared
-00021ea0: 5f64 7327 2c20 2776 6572 7369 6f6e 273a  _ds', 'version':
-00021eb0: 2033 3930 377d 0a20 2020 203e 3e3e 2067   3907}.    >>> g
-00021ec0: 6574 5f6e 616d 655f 7665 7273 696f 6e28  et_name_version(
-00021ed0: 2774 6d70 6838 6567 746c 5f5f 2729 0a20  'tmph8egtl__'). 
-00021ee0: 2020 207b 276e 616d 6527 3a20 2774 6d70     {'name': 'tmp
-00021ef0: 6838 6567 746c 5f5f 272c 2027 7665 7273  h8egtl__', 'vers
-00021f00: 696f 6e27 3a20 4e6f 6e65 7d0a 2020 2020  ion': None}.    
-00021f10: 3e3e 3e20 6765 745f 6e61 6d65 5f76 6572  >>> get_name_ver
-00021f20: 7369 6f6e 2827 746d 7068 3865 6774 6c5f  sion('tmph8egtl_
-00021f30: 5f31 3233 5f5f 2729 0a20 2020 207b 276e  _123__').    {'n
-00021f40: 616d 6527 3a20 2774 6d70 6838 6567 746c  ame': 'tmph8egtl
-00021f50: 5f5f 3132 335f 5f27 2c20 2776 6572 7369  __123__', 'versi
-00021f60: 6f6e 273a 204e 6f6e 657d 0a20 2020 2022  on': None}.    "
-00021f70: 2222 0a20 2020 2074 6b20 3d20 6473 2e72  "".    tk = ds.r
-00021f80: 7370 6c69 7428 225f 5f22 2c20 3229 0a20  split("__", 2). 
-00021f90: 2020 2069 6620 6c65 6e28 746b 2920 3d3d     if len(tk) ==
-00021fa0: 2031 3a0a 2020 2020 2020 2020 7265 7475   1:.        retu
-00021fb0: 726e 207b 226e 616d 6522 3a20 746b 5b30  rn {"name": tk[0
-00021fc0: 5d2c 2022 7665 7273 696f 6e22 3a20 4e6f  ], "version": No
-00021fd0: 6e65 7d0a 2020 2020 656c 6966 206c 656e  ne}.    elif len
-00021fe0: 2874 6b29 203d 3d20 323a 0a20 2020 2020  (tk) == 2:.     
-00021ff0: 2020 2069 6620 6c65 6e28 746b 5b31 5d29     if len(tk[1])
-00022000: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00022010: 2074 6b5b 315d 5b30 5d20 3d3d 2022 7622   tk[1][0] == "v"
-00022020: 2061 6e64 2072 652e 6d61 7463 6828 225b   and re.match("[
-00022030: 302d 395d 2b24 222c 2074 6b5b 315d 5b31  0-9]+$", tk[1][1
-00022040: 3a5d 293a 0a20 2020 2020 2020 2020 2020  :]):.           
-00022050: 2020 2020 2072 6574 7572 6e20 7b22 6e61       return {"na
-00022060: 6d65 223a 2074 6b5b 305d 2c20 2276 6572  me": tk[0], "ver
-00022070: 7369 6f6e 223a 2069 6e74 2874 6b5b 315d  sion": int(tk[1]
-00022080: 5b31 3a5d 297d 0a20 2020 2020 2020 2020  [1:])}.         
-00022090: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000220a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000220b0: 7b22 6e61 6d65 223a 2074 6b5b 305d 202b  {"name": tk[0] +
-000220c0: 2022 5f5f 2220 2b20 746b 5b31 5d2c 2022   "__" + tk[1], "
-000220d0: 7665 7273 696f 6e22 3a20 4e6f 6e65 7d0a  version": None}.
-000220e0: 2020 2020 656c 6966 206c 656e 2874 6b29      elif len(tk)
-000220f0: 203d 3d20 3320 616e 6420 6c65 6e28 746b   == 3 and len(tk
-00022100: 5b32 5d29 3a0a 2020 2020 2020 2020 6966  [2]):.        if
-00022110: 2074 6b5b 325d 203d 3d20 2263 6865 636b   tk[2] == "check
-00022120: 6572 223a 0a20 2020 2020 2020 2020 2020  er":.           
-00022130: 2072 6574 7572 6e20 7b22 6e61 6d65 223a   return {"name":
-00022140: 2074 6b5b 305d 202b 2022 5f5f 2220 2b20   tk[0] + "__" + 
-00022150: 746b 5b31 5d20 2b20 225f 5f22 202b 2074  tk[1] + "__" + t
-00022160: 6b5b 325d 2c20 2276 6572 7369 6f6e 223a  k[2], "version":
-00022170: 204e 6f6e 657d 0a20 2020 2020 2020 2069   None}.        i
-00022180: 6620 746b 5b32 5d5b 305d 203d 3d20 2276  f tk[2][0] == "v
-00022190: 223a 0a20 2020 2020 2020 2020 2020 2070  ":.            p
-000221a0: 6172 7473 203d 2074 6b5b 325d 2e73 706c  arts = tk[2].spl
-000221b0: 6974 2822 5f22 290a 2020 2020 2020 2020  it("_").        
-000221c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000221d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000221e0: 7b22 6e61 6d65 223a 2074 6b5b 305d 202b  {"name": tk[0] +
-000221f0: 2022 5f5f 2220 2b20 746b 5b31 5d2c 2022   "__" + tk[1], "
-00022200: 7665 7273 696f 6e22 3a20 696e 7428 7061  version": int(pa
-00022210: 7274 735b 305d 5b31 3a5d 297d 0a20 2020  rts[0][1:])}.   
-00022220: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00022230: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
-00022240: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00022250: 726e 207b 226e 616d 6522 3a20 746b 5b30  rn {"name": tk[0
-00022260: 5d20 2b20 225f 5f22 202b 2074 6b5b 315d  ] + "__" + tk[1]
-00022270: 202b 2022 5f5f 2220 2b20 746b 5b32 5d2c   + "__" + tk[2],
-00022280: 2022 7665 7273 696f 6e22 3a20 4e6f 6e65   "version": None
-00022290: 7d0a 2020 2020 2020 2020 656c 7365 3a0a  }.        else:.
-000222a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000222b0: 726e 207b 226e 616d 6522 3a20 225f 5f22  rn {"name": "__"
-000222c0: 2e6a 6f69 6e28 746b 5b30 3a5d 292c 2022  .join(tk[0:]), "
-000222d0: 7665 7273 696f 6e22 3a20 4e6f 6e65 7d0a  version": None}.
-000222e0: 0a20 2020 2072 6574 7572 6e20 7b22 6e61  .    return {"na
-000222f0: 6d65 223a 2064 732c 2022 7665 7273 696f  me": ds, "versio
-00022300: 6e22 3a20 4e6f 6e65 7d0a 0a0a 6465 6620  n": None}...def 
-00022310: 6765 745f 7265 736f 7572 6365 5f76 6572  get_resource_ver
-00022320: 7369 6f6e 7328 6461 7461 736f 7572 6365  sions(datasource
-00022330: 733a 204c 6973 745b 7374 725d 293a 0a20  s: List[str]):. 
-00022340: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
-00022350: 6e20 7468 6520 6c61 7465 7374 2076 6572  n the latest ver
-00022360: 7369 6f6e 2066 6f72 2061 6c6c 2074 6865  sion for all the
-00022370: 2064 6174 6173 6f75 7263 6573 0a20 2020   datasources.   
-00022380: 2022 2222 0a20 2020 2076 6572 7369 6f6e   """.    version
-00022390: 7320 3d20 7b7d 0a20 2020 2066 6f72 2078  s = {}.    for x
-000223a0: 2069 6e20 6461 7461 736f 7572 6365 733a   in datasources:
-000223b0: 0a20 2020 2020 2020 2074 203d 2067 6574  .        t = get
-000223c0: 5f6e 616d 655f 7665 7273 696f 6e28 7829  _name_version(x)
-000223d0: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
-000223e0: 745b 226e 616d 6522 5d0a 2020 2020 2020  t["name"].      
-000223f0: 2020 6966 2074 2e67 6574 2822 7665 7273    if t.get("vers
-00022400: 696f 6e22 2c20 4e6f 6e65 2920 6973 206e  ion", None) is n
-00022410: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00022420: 2020 2020 2076 6572 7369 6f6e 735b 6e61       versions[na
-00022430: 6d65 5d20 3d20 745b 2276 6572 7369 6f6e  me] = t["version
-00022440: 225d 0a20 2020 2072 6574 7572 6e20 7665  "].    return ve
-00022450: 7273 696f 6e73 0a0a 0a64 6566 2067 6574  rsions...def get
-00022460: 5f72 656d 6f74 655f 7265 736f 7572 6365  _remote_resource
-00022470: 5f6e 616d 655f 7769 7468 6f75 745f 7665  _name_without_ve
-00022480: 7273 696f 6e28 7265 6d6f 7465 5f72 6573  rsion(remote_res
-00022490: 6f75 7263 655f 6e61 6d65 3a20 7374 7229  ource_name: str)
-000224a0: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
-000224b0: 0a20 2020 203e 3e3e 2067 6574 5f72 656d  .    >>> get_rem
-000224c0: 6f74 655f 7265 736f 7572 6365 5f6e 616d  ote_resource_nam
-000224d0: 655f 7769 7468 6f75 745f 7665 7273 696f  e_without_versio
-000224e0: 6e28 2272 5f5f 6461 7461 736f 7572 6365  n("r__datasource
-000224f0: 2229 0a20 2020 2027 725f 5f64 6174 6173  ").    'r__datas
-00022500: 6f75 7263 6527 0a20 2020 203e 3e3e 2067  ource'.    >>> g
-00022510: 6574 5f72 656d 6f74 655f 7265 736f 7572  et_remote_resour
-00022520: 6365 5f6e 616d 655f 7769 7468 6f75 745f  ce_name_without_
-00022530: 7665 7273 696f 6e28 2272 5f5f 6461 7461  version("r__data
-00022540: 736f 7572 6365 5f5f 7630 2229 0a20 2020  source__v0").   
-00022550: 2027 725f 5f64 6174 6173 6f75 7263 6527   'r__datasource'
-00022560: 0a20 2020 203e 3e3e 2067 6574 5f72 656d  .    >>> get_rem
-00022570: 6f74 655f 7265 736f 7572 6365 5f6e 616d  ote_resource_nam
-00022580: 655f 7769 7468 6f75 745f 7665 7273 696f  e_without_versio
-00022590: 6e28 2264 6174 6173 6f75 7263 6522 290a  n("datasource").
-000225a0: 2020 2020 2764 6174 6173 6f75 7263 6527      'datasource'
-000225b0: 0a20 2020 2022 2222 0a20 2020 2070 6172  .    """.    par
-000225c0: 7473 203d 2067 6574 5f6e 616d 655f 7665  ts = get_name_ve
-000225d0: 7273 696f 6e28 7265 6d6f 7465 5f72 6573  rsion(remote_res
-000225e0: 6f75 7263 655f 6e61 6d65 290a 2020 2020  ource_name).    
-000225f0: 7265 7475 726e 2070 6172 7473 5b22 6e61  return parts["na
-00022600: 6d65 225d 0a0a 0a64 6566 2067 6574 5f64  me"]...def get_d
-00022610: 6570 5f66 726f 6d5f 7261 775f 7461 626c  ep_from_raw_tabl
-00022620: 6573 2878 3a20 7374 7229 202d 3e20 7374  es(x: str) -> st
-00022630: 723a 0a20 2020 2022 2222 0a20 2020 2064  r:.    """.    d
-00022640: 6174 6173 6f75 7263 6573 204b 4559 2063  atasources KEY c
-00022650: 6f6d 6d61 6e64 2067 656e 6572 6174 6573  ommand generates
-00022660: 2074 6162 6c65 732c 2074 6869 7320 7472   tables, this tr
-00022670: 616e 7366 6f72 6d20 7468 6520 7573 6564  ansform the used
-00022680: 2074 6162 6c65 2077 6974 6820 7468 6520   table with the 
-00022690: 736f 7572 6365 2066 696c 650a 2020 2020  source file.    
-000226a0: 3e3e 3e20 6765 745f 6465 705f 6672 6f6d  >>> get_dep_from
-000226b0: 5f72 6177 5f74 6162 6c65 7328 2774 6573  _raw_tables('tes
-000226c0: 7427 290a 2020 2020 2774 6573 7427 0a20  t').    'test'. 
-000226d0: 2020 203e 3e3e 2067 6574 5f64 6570 5f66     >>> get_dep_f
-000226e0: 726f 6d5f 7261 775f 7461 626c 6573 2827  rom_raw_tables('
-000226f0: 7465 7374 5f6a 6f69 6e5f 6279 5f63 6f6c  test_join_by_col
-00022700: 756d 6e27 290a 2020 2020 2774 6573 7427  umn').    'test'
-00022710: 0a20 2020 2022 2222 0a0a 2020 2020 7472  .    """..    tr
-00022720: 793a 0a20 2020 2020 2020 2072 6574 7572  y:.        retur
-00022730: 6e20 785b 3a20 782e 696e 6465 7828 225f  n x[: x.index("_
-00022740: 6a6f 696e 5f62 795f 2229 5d0a 2020 2020  join_by_")].    
-00022750: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00022760: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-00022770: 6e20 780a 0a0a 6465 6620 6372 6561 7465  n x...def create
-00022780: 5f64 6f77 6e73 7472 6561 6d5f 6465 7065  _downstream_depe
-00022790: 6e64 656e 6379 5f67 7261 7068 2864 6570  ndency_graph(dep
-000227a0: 656e 6465 6e63 795f 6772 6170 683a 2044  endency_graph: D
-000227b0: 6963 745b 7374 722c 2053 6574 5b73 7472  ict[str, Set[str
-000227c0: 5d5d 2c20 616c 6c5f 7265 736f 7572 6365  ]], all_resource
-000227d0: 733a 2044 6963 745b 7374 722c 2044 6963  s: Dict[str, Dic
-000227e0: 745b 7374 722c 2041 6e79 5d5d 293a 0a20  t[str, Any]]):. 
-000227f0: 2020 2022 2222 0a20 2020 2054 6869 7320     """.    This 
-00022800: 6675 6e63 7469 6f6e 2072 6576 6572 7365  function reverse
-00022810: 7320 7468 6520 6465 7065 6e64 656e 6379  s the dependency
-00022820: 2067 7261 7068 206f 6274 6169 6e65 6420   graph obtained 
-00022830: 6672 6f6d 2062 7569 6c64 5f67 7261 7068  from build_graph
-00022840: 2073 6f20 796f 7520 6861 7665 2064 6f77   so you have dow
-00022850: 6e73 7472 6561 6d20 6465 7065 6e64 656e  nstream dependen
-00022860: 6369 6573 2066 6f72 2065 6163 6820 6e6f  cies for each no
-00022870: 6465 2069 6e20 7468 6520 6772 6170 682e  de in the graph.
-00022880: 0a0a 2020 2020 4164 6469 7469 6f6e 616c  ..    Additional
-00022890: 6c79 2074 616b 6573 2069 6e74 6f20 6163  ly takes into ac
-000228a0: 636f 756e 7420 7461 7267 6574 5f64 6174  count target_dat
-000228b0: 6173 6f75 7263 6520 6f66 206d 6174 6572  asource of mater
-000228c0: 6961 6c69 7a65 6420 7669 6577 730a 2020  ialized views.  
-000228d0: 2020 2222 220a 2020 2020 646f 776e 7374    """.    downst
-000228e0: 7265 616d 5f64 6570 656e 6465 6e63 795f  ream_dependency_
-000228f0: 6772 6170 683a 2044 6963 745b 7374 722c  graph: Dict[str,
-00022900: 2053 6574 5b73 7472 5d5d 203d 207b 6e6f   Set[str]] = {no
-00022910: 6465 3a20 7365 7428 2920 666f 7220 6e6f  de: set() for no
-00022920: 6465 2069 6e20 6465 7065 6e64 656e 6379  de in dependency
-00022930: 5f67 7261 7068 7d0a 0a20 2020 2066 6f72  _graph}..    for
-00022940: 206e 6f64 652c 2064 6570 656e 6465 6e63   node, dependenc
-00022950: 6965 7320 696e 2064 6570 656e 6465 6e63  ies in dependenc
-00022960: 795f 6772 6170 682e 6974 656d 7328 293a  y_graph.items():
-00022970: 0a20 2020 2020 2020 2066 6f72 2064 6570  .        for dep
-00022980: 656e 6465 6e63 7920 696e 2064 6570 656e  endency in depen
-00022990: 6465 6e63 6965 733a 0a20 2020 2020 2020  dencies:.       
-000229a0: 2020 2020 2069 6620 6465 7065 6e64 656e       if dependen
-000229b0: 6379 206e 6f74 2069 6e20 646f 776e 7374  cy not in downst
-000229c0: 7265 616d 5f64 6570 656e 6465 6e63 795f  ream_dependency_
-000229d0: 6772 6170 683a 0a20 2020 2020 2020 2020  graph:.         
-000229e0: 2020 2020 2020 2023 2061 2073 6861 7265         # a share
-000229f0: 6420 6461 7461 2073 6f75 7263 652c 2077  d data source, w
-00022a00: 6520 6361 6e20 736b 6970 2069 740a 2020  e can skip it.  
-00022a10: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00022a20: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00022a30: 2020 2064 6f77 6e73 7472 6561 6d5f 6465     downstream_de
-00022a40: 7065 6e64 656e 6379 5f67 7261 7068 5b64  pendency_graph[d
-00022a50: 6570 656e 6465 6e63 795d 2e61 6464 286e  ependency].add(n
-00022a60: 6f64 6529 0a0a 2020 2020 666f 7220 6b65  ode)..    for ke
-00022a70: 7920 696e 2064 6963 7428 646f 776e 7374  y in dict(downst
-00022a80: 7265 616d 5f64 6570 656e 6465 6e63 795f  ream_dependency_
-00022a90: 6772 6170 6829 3a0a 2020 2020 2020 2020  graph):.        
-00022aa0: 7461 7267 6574 5f64 6174 6173 6f75 7263  target_datasourc
-00022ab0: 6520 3d20 6765 745f 7461 7267 6574 5f6d  e = get_target_m
-00022ac0: 6174 6572 6961 6c69 7a65 645f 6461 7461  aterialized_data
-00022ad0: 5f73 6f75 7263 655f 6e61 6d65 2861 6c6c  _source_name(all
-00022ae0: 5f72 6573 6f75 7263 6573 5b6b 6579 5d29  _resources[key])
-00022af0: 0a20 2020 2020 2020 2069 6620 7461 7267  .        if targ
-00022b00: 6574 5f64 6174 6173 6f75 7263 653a 0a20  et_datasource:. 
-00022b10: 2020 2020 2020 2020 2020 2064 6f77 6e73             downs
-00022b20: 7472 6561 6d5f 6465 7065 6e64 656e 6379  tream_dependency
-00022b30: 5f67 7261 7068 5b6b 6579 5d2e 7570 6461  _graph[key].upda
-00022b40: 7465 287b 7461 7267 6574 5f64 6174 6173  te({target_datas
-00022b50: 6f75 7263 657d 290a 2020 2020 2020 2020  ource}).        
-00022b60: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00022b70: 2020 2020 2020 2020 2064 6f77 6e73 7472           downstr
-00022b80: 6561 6d5f 6465 7065 6e64 656e 6379 5f67  eam_dependency_g
-00022b90: 7261 7068 5b74 6172 6765 745f 6461 7461  raph[target_data
-00022ba0: 736f 7572 6365 5d2e 7265 6d6f 7665 286b  source].remove(k
-00022bb0: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
-00022bc0: 6578 6365 7074 204b 6579 4572 726f 723a  except KeyError:
-00022bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022be0: 2070 6173 730a 0a20 2020 2072 6574 7572   pass..    retur
-00022bf0: 6e20 646f 776e 7374 7265 616d 5f64 6570  n downstream_dep
-00022c00: 656e 6465 6e63 795f 6772 6170 680a 0a0a  endency_graph...
-00022c10: 6465 6620 7570 6461 7465 5f64 6570 5f6d  def update_dep_m
-00022c20: 6170 5f72 6563 7572 7369 7665 6c79 280a  ap_recursively(.
-00022c30: 2020 2020 6465 705f 6d61 703a 2044 6963      dep_map: Dic
-00022c40: 745b 7374 722c 2053 6574 5b73 7472 5d5d  t[str, Set[str]]
-00022c50: 2c0a 2020 2020 646f 776e 7374 7265 616d  ,.    downstream
-00022c60: 5f64 6570 5f6d 6170 3a20 4469 6374 5b73  _dep_map: Dict[s
-00022c70: 7472 2c20 5365 745b 7374 725d 5d2c 0a20  tr, Set[str]],. 
-00022c80: 2020 2061 6c6c 5f72 6573 6f75 7263 6573     all_resources
-00022c90: 3a20 4469 6374 5b73 7472 2c20 4469 6374  : Dict[str, Dict
-00022ca0: 5b73 7472 2c20 416e 795d 5d2c 0a20 2020  [str, Any]],.   
-00022cb0: 2074 6f5f 7275 6e3a 2044 6963 745b 7374   to_run: Dict[st
-00022cc0: 722c 2044 6963 745b 7374 722c 2041 6e79  r, Dict[str, Any
-00022cd0: 5d5d 2c0a 2020 2020 6465 705f 6d61 705f  ]],.    dep_map_
-00022ce0: 6b65 7973 3a20 4c69 7374 5b73 7472 5d2c  keys: List[str],
-00022cf0: 0a20 2020 206b 6579 3a20 4f70 7469 6f6e  .    key: Option
-00022d00: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00022d10: 2020 2020 7669 7369 7465 643a 204f 7074      visited: Opt
-00022d20: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-00022d30: 203d 204e 6f6e 652c 0a29 3a0a 2020 2020   = None,.):.    
-00022d40: 2222 220a 2020 2020 4769 7665 6e20 6120  """.    Given a 
-00022d50: 646f 776e 7374 7265 616d 5f64 6570 5f6d  downstream_dep_m
-00022d60: 6170 206f 6274 6169 6e65 6420 6672 6f6d  ap obtained from
-00022d70: 2063 7265 6174 655f 646f 776e 7374 7265   create_downstre
-00022d80: 616d 5f64 6570 656e 6465 6e63 795f 6772  am_dependency_gr
-00022d90: 6170 6820 7468 6973 2066 756e 6374 696f  aph this functio
-00022da0: 6e20 7570 6461 7465 7320 6561 6368 206e  n updates each n
-00022db0: 6f64 6520 7265 6375 7273 6976 656c 7920  ode recursively 
-00022dc0: 746f 2063 6f6d 706c 6574 6520 7468 6520  to complete the 
-00022dd0: 646f 776e 7374 7265 616d 2064 6570 656e  downstream depen
-00022de0: 6465 6e63 7920 6772 6170 6820 666f 7220  dency graph for 
-00022df0: 6561 6368 206e 6f64 650a 2020 2020 2222  each node.    ""
-00022e00: 220a 2020 2020 6966 206e 6f74 2076 6973  ".    if not vis
-00022e10: 6974 6564 3a0a 2020 2020 2020 2020 7669  ited:.        vi
-00022e20: 7369 7465 6420 3d20 6c69 7374 2829 0a20  sited = list(). 
-00022e30: 2020 2069 6620 6e6f 7420 6b65 7920 616e     if not key an
-00022e40: 6420 6c65 6e28 6465 705f 6d61 705f 6b65  d len(dep_map_ke
-00022e50: 7973 2920 3d3d 2030 3a0a 2020 2020 2020  ys) == 0:.      
-00022e60: 2020 7265 7475 726e 0a20 2020 2069 6620    return.    if 
-00022e70: 6e6f 7420 6b65 793a 0a20 2020 2020 2020  not key:.       
-00022e80: 206b 6579 203d 2064 6570 5f6d 6170 5f6b   key = dep_map_k
-00022e90: 6579 732e 706f 7028 290a 2020 2020 6966  eys.pop().    if
-00022ea0: 206b 6579 206e 6f74 2069 6e20 6465 705f   key not in dep_
-00022eb0: 6d61 703a 0a20 2020 2020 2020 2064 6570  map:.        dep
-00022ec0: 5f6d 6170 5b6b 6579 5d20 3d20 7365 7428  _map[key] = set(
-00022ed0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00022ee0: 2020 2020 7669 7369 7465 642e 6170 7065      visited.appe
-00022ef0: 6e64 286b 6579 290a 2020 2020 2020 2020  nd(key).        
-00022f00: 7265 7475 726e 0a0a 2020 2020 666f 7220  return..    for 
-00022f10: 6465 7020 696e 2064 6f77 6e73 7472 6561  dep in downstrea
-00022f20: 6d5f 6465 705f 6d61 702e 6765 7428 6b65  m_dep_map.get(ke
-00022f30: 792c 207b 7d29 3a0a 2020 2020 2020 2020  y, {}):.        
-00022f40: 6966 2064 6570 206e 6f74 2069 6e20 646f  if dep not in do
-00022f50: 776e 7374 7265 616d 5f64 6570 5f6d 6170  wnstream_dep_map
-00022f60: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00022f70: 6e74 696e 7565 0a20 2020 2020 2020 2074  ntinue.        t
-00022f80: 6f5f 7275 6e5b 6465 705d 203d 2061 6c6c  o_run[dep] = all
-00022f90: 5f72 6573 6f75 7263 6573 2e67 6574 2864  _resources.get(d
-00022fa0: 6570 2c20 7b7d 290a 2020 2020 2020 2020  ep, {}).        
-00022fb0: 7570 6461 7465 5f64 6570 5f6d 6170 5f72  update_dep_map_r
-00022fc0: 6563 7572 7369 7665 6c79 280a 2020 2020  ecursively(.    
-00022fd0: 2020 2020 2020 2020 6465 705f 6d61 702c          dep_map,
-00022fe0: 2064 6f77 6e73 7472 6561 6d5f 6465 705f   downstream_dep_
-00022ff0: 6d61 702c 2061 6c6c 5f72 6573 6f75 7263  map, all_resourc
-00023000: 6573 2c20 746f 5f72 756e 2c20 6465 705f  es, to_run, dep_
-00023010: 6d61 705f 6b65 7973 2c20 6b65 793d 6465  map_keys, key=de
-00023020: 702c 2076 6973 6974 6564 3d76 6973 6974  p, visited=visit
-00023030: 6564 0a20 2020 2020 2020 2029 0a20 2020  ed.        ).   
-00023040: 2020 2020 2064 6570 5f6d 6170 5b6b 6579       dep_map[key
-00023050: 5d2e 7570 6461 7465 2864 6f77 6e73 7472  ].update(downstr
-00023060: 6561 6d5f 6465 705f 6d61 705b 6465 705d  eam_dep_map[dep]
-00023070: 290a 2020 2020 2020 2020 6465 705f 6d61  ).        dep_ma
-00023080: 705b 6b65 795d 2e75 7064 6174 6528 7b64  p[key].update({d
-00023090: 6570 7d29 0a20 2020 2020 2020 2074 7279  ep}).        try
-000230a0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000230b0: 705f 6d61 705b 6b65 795d 2e72 656d 6f76  p_map[key].remov
-000230c0: 6528 6b65 7929 0a20 2020 2020 2020 2065  e(key).        e
-000230d0: 7863 6570 7420 4b65 7945 7272 6f72 3a0a  xcept KeyError:.
-000230e0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-000230f0: 0a0a 2020 2020 746f 5f72 756e 5b6b 6579  ..    to_run[key
-00023100: 5d20 3d20 616c 6c5f 7265 736f 7572 6365  ] = all_resource
-00023110: 732e 6765 7428 6b65 792c 207b 7d29 0a20  s.get(key, {}). 
-00023120: 2020 2075 7064 6174 655f 6465 705f 6d61     update_dep_ma
-00023130: 705f 7265 6375 7273 6976 656c 7928 0a20  p_recursively(. 
-00023140: 2020 2020 2020 2064 6570 5f6d 6170 2c20         dep_map, 
-00023150: 646f 776e 7374 7265 616d 5f64 6570 5f6d  downstream_dep_m
-00023160: 6170 2c20 616c 6c5f 7265 736f 7572 6365  ap, all_resource
-00023170: 732c 2074 6f5f 7275 6e2c 2064 6570 5f6d  s, to_run, dep_m
-00023180: 6170 5f6b 6579 732c 206b 6579 3d4e 6f6e  ap_keys, key=Non
-00023190: 652c 2076 6973 6974 6564 3d76 6973 6974  e, visited=visit
-000231a0: 6564 0a20 2020 2029 0a0a 0a64 6566 2067  ed.    )...def g
-000231b0: 656e 6572 6174 655f 666f 726b 646f 776e  enerate_forkdown
-000231c0: 7374 7265 616d 5f67 7261 7068 280a 2020  stream_graph(.  
-000231d0: 2020 616c 6c5f 6465 705f 6d61 703a 2044    all_dep_map: D
-000231e0: 6963 745b 7374 722c 2053 6574 5b73 7472  ict[str, Set[str
-000231f0: 5d5d 2c0a 2020 2020 616c 6c5f 7265 736f  ]],.    all_reso
-00023200: 7572 6365 733a 2044 6963 745b 7374 722c  urces: Dict[str,
-00023210: 2044 6963 745b 7374 722c 2041 6e79 5d5d   Dict[str, Any]]
-00023220: 2c0a 2020 2020 746f 5f72 756e 3a20 4469  ,.    to_run: Di
-00023230: 6374 5b73 7472 2c20 4469 6374 5b73 7472  ct[str, Dict[str
-00023240: 2c20 416e 795d 5d2c 0a20 2020 2064 6570  , Any]],.    dep
-00023250: 5f6d 6170 5f6b 6579 733a 204c 6973 745b  _map_keys: List[
-00023260: 7374 725d 2c0a 2920 2d3e 2054 7570 6c65  str],.) -> Tuple
-00023270: 5b44 6963 745b 7374 722c 2053 6574 5b73  [Dict[str, Set[s
-00023280: 7472 5d5d 2c20 4469 6374 5b73 7472 2c20  tr]], Dict[str, 
-00023290: 4469 6374 5b73 7472 2c20 416e 795d 5d5d  Dict[str, Any]]]
-000232a0: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-000232b0: 6973 2066 756e 6374 696f 6e20 666f 7220  is function for 
-000232c0: 6120 6769 7665 6e20 6772 6170 6820 6f66  a given graph of
-000232d0: 2064 6570 656e 6465 6e63 6965 7320 6672   dependencies fr
-000232e0: 6f6d 206c 6566 7420 746f 2072 6967 6874  om left to right
-000232f0: 2e20 4974 2077 696c 6c20 6765 6e65 7261  . It will genera
-00023300: 7465 2061 206e 6577 2067 7261 7068 2077  te a new graph w
-00023310: 6974 6820 7468 6520 6465 7065 6e64 656e  ith the dependen
-00023320: 6369 6573 2066 726f 6d20 7269 6768 7420  cies from right 
-00023330: 746f 206c 6566 742c 2062 7574 2074 616b  to left, but tak
-00023340: 696e 6720 696e 746f 2061 6363 6f75 6e74  ing into account
-00023350: 2074 6861 7420 6576 656e 2069 6620 736f   that even if so
-00023360: 6d65 206e 6f64 6573 2061 7265 206e 6f74  me nodes are not
-00023370: 2069 6e73 6964 6520 746f 5f72 756e 2c20   inside to_run, 
-00023380: 7468 6579 2061 7265 2073 7469 6c6c 2064  they are still d
-00023390: 6570 656e 6465 6e63 6965 7320 7468 6174  ependencies that
-000233a0: 206e 6565 6420 746f 2062 6520 6465 706c   need to be depl
-000233b0: 6f79 6564 2e0a 0a20 2020 203e 3e3e 2064  oyed...    >>> d
-000233c0: 6570 732c 205f 203d 2067 656e 6572 6174  eps, _ = generat
-000233d0: 655f 666f 726b 646f 776e 7374 7265 616d  e_forkdownstream
-000233e0: 5f67 7261 7068 280a 2020 2020 2e2e 2e20  _graph(.    ... 
-000233f0: 2020 2020 7b0a 2020 2020 2e2e 2e20 2020      {.    ...   
-00023400: 2020 2020 2020 2761 273a 207b 2762 277d        'a': {'b'}
-00023410: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
-00023420: 2020 2762 273a 207b 2763 277d 2c0a 2020    'b': {'c'},.  
-00023430: 2020 2e2e 2e20 2020 2020 2020 2020 2763    ...         'c
-00023440: 273a 2073 6574 2829 2c0a 2020 2020 2e2e  ': set(),.    ..
-00023450: 2e20 2020 2020 7d2c 0a20 2020 202e 2e2e  .     },.    ...
-00023460: 2020 2020 207b 0a20 2020 202e 2e2e 2020       {.    ...  
-00023470: 2020 2020 2020 2027 6127 3a20 7b27 7265         'a': {'re
-00023480: 736f 7572 6365 5f6e 616d 6527 3a20 2761  source_name': 'a
-00023490: 277d 2c0a 2020 2020 2e2e 2e20 2020 2020  '},.    ...     
-000234a0: 2020 2020 2762 273a 207b 2772 6573 6f75      'b': {'resou
-000234b0: 7263 655f 6e61 6d65 273a 2027 6227 2c20  rce_name': 'b', 
-000234c0: 276e 6f64 6573 273a 205b 7b27 7061 7261  'nodes': [{'para
-000234d0: 6d73 273a 207b 2774 7970 6527 3a20 276d  ms': {'type': 'm
-000234e0: 6174 6572 6961 6c69 7a65 6427 2c20 2764  aterialized', 'd
-000234f0: 6174 6173 6f75 7263 6527 3a20 2763 277d  atasource': 'c'}
-00023500: 7d5d 207d 2c0a 2020 2020 2e2e 2e20 2020  }] },.    ...   
-00023510: 2020 2020 2020 2763 273a 207b 2772 6573        'c': {'res
-00023520: 6f75 7263 655f 6e61 6d65 273a 2027 6327  ource_name': 'c'
-00023530: 7d2c 0a20 2020 202e 2e2e 2020 2020 207d  },.    ...     }
-00023540: 2c0a 2020 2020 2e2e 2e20 2020 2020 7b0a  ,.    ...     {.
-00023550: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
-00023560: 2761 273a 207b 2772 6573 6f75 7263 655f  'a': {'resource_
-00023570: 6e61 6d65 273a 2027 6127 7d2c 0a20 2020  name': 'a'},.   
-00023580: 202e 2e2e 2020 2020 207d 2c0a 2020 2020   ...     },.    
-00023590: 2e2e 2e20 2020 2020 5b27 6127 2c20 2762  ...     ['a', 'b
-000235a0: 272c 2027 6327 5d2c 0a20 2020 202e 2e2e  ', 'c'],.    ...
-000235b0: 2029 0a20 2020 203e 3e3e 207b 6b3a 2073   ).    >>> {k: s
-000235c0: 6f72 7465 6428 7629 2066 6f72 206b 2c20  orted(v) for k, 
-000235d0: 7620 696e 2064 6570 732e 6974 656d 7328  v in deps.items(
-000235e0: 297d 0a20 2020 207b 2763 273a 205b 5d2c  )}.    {'c': [],
-000235f0: 2027 6227 3a20 5b27 6127 2c20 2763 275d   'b': ['a', 'c']
-00023600: 2c20 2761 273a 205b 5d7d 0a0a 2020 2020  , 'a': []}..    
-00023610: 3e3e 3e20 6465 7073 2c20 5f20 3d20 6765  >>> deps, _ = ge
-00023620: 6e65 7261 7465 5f66 6f72 6b64 6f77 6e73  nerate_forkdowns
-00023630: 7472 6561 6d5f 6772 6170 6828 0a20 2020  tream_graph(.   
-00023640: 202e 2e2e 2020 2020 207b 0a20 2020 202e   ...     {.    .
-00023650: 2e2e 2020 2020 2020 2020 2027 6127 3a20  ..         'a': 
-00023660: 7b27 6227 7d2c 0a20 2020 202e 2e2e 2020  {'b'},.    ...  
-00023670: 2020 2020 2020 2027 6227 3a20 7b27 6327         'b': {'c'
-00023680: 7d2c 0a20 2020 202e 2e2e 2020 2020 2020  },.    ...      
-00023690: 2020 2027 6327 3a20 7365 7428 292c 0a20     'c': set(),. 
-000236a0: 2020 202e 2e2e 2020 2020 207d 2c0a 2020     ...     },.  
-000236b0: 2020 2e2e 2e20 2020 2020 7b0a 2020 2020    ...     {.    
-000236c0: 2e2e 2e20 2020 2020 2020 2020 2761 273a  ...         'a':
-000236d0: 207b 2772 6573 6f75 7263 655f 6e61 6d65   {'resource_name
-000236e0: 273a 2027 6127 7d2c 0a20 2020 202e 2e2e  ': 'a'},.    ...
-000236f0: 2020 2020 2020 2020 2027 6227 3a20 7b27           'b': {'
-00023700: 7265 736f 7572 6365 5f6e 616d 6527 3a20  resource_name': 
-00023710: 2762 272c 2027 6e6f 6465 7327 3a20 5b7b  'b', 'nodes': [{
-00023720: 2770 6172 616d 7327 3a20 7b27 7479 7065  'params': {'type
-00023730: 273a 2027 6d61 7465 7269 616c 697a 6564  ': 'materialized
-00023740: 272c 2027 6461 7461 736f 7572 6365 273a  ', 'datasource':
-00023750: 2027 6327 7d7d 5d20 7d2c 0a20 2020 202e   'c'}}] },.    .
-00023760: 2e2e 2020 2020 2020 2020 2027 6327 3a20  ..         'c': 
-00023770: 7b27 7265 736f 7572 6365 5f6e 616d 6527  {'resource_name'
-00023780: 3a20 2763 277d 2c0a 2020 2020 2e2e 2e20  : 'c'},.    ... 
-00023790: 2020 2020 7d2c 0a20 2020 202e 2e2e 2020      },.    ...  
-000237a0: 2020 207b 0a20 2020 202e 2e2e 2020 2020     {.    ...    
-000237b0: 2020 2020 2027 6227 3a20 7b27 7265 736f       'b': {'reso
-000237c0: 7572 6365 5f6e 616d 6527 3a20 2762 277d  urce_name': 'b'}
-000237d0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7d2c  ,.    ...     },
-000237e0: 0a20 2020 202e 2e2e 2020 2020 205b 2761  .    ...     ['a
-000237f0: 272c 2027 6227 2c20 2763 275d 2c0a 2020  ', 'b', 'c'],.  
-00023800: 2020 2e2e 2e20 290a 2020 2020 3e3e 3e20    ... ).    >>> 
-00023810: 7b6b 3a20 736f 7274 6564 2876 2920 666f  {k: sorted(v) fo
-00023820: 7220 6b2c 2076 2069 6e20 6465 7073 2e69  r k, v in deps.i
-00023830: 7465 6d73 2829 7d0a 2020 2020 7b27 6327  tems()}.    {'c'
-00023840: 3a20 5b5d 2c20 2762 273a 205b 2761 272c  : [], 'b': ['a',
-00023850: 2027 6327 5d2c 2027 6127 3a20 5b5d 7d0a   'c'], 'a': []}.
-00023860: 0a20 2020 203e 3e3e 2064 6570 732c 205f  .    >>> deps, _
-00023870: 203d 2067 656e 6572 6174 655f 666f 726b   = generate_fork
-00023880: 646f 776e 7374 7265 616d 5f67 7261 7068  downstream_graph
-00023890: 280a 2020 2020 2e2e 2e20 2020 2020 7b0a  (.    ...     {.
-000238a0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
-000238b0: 276d 6967 7261 7465 645f 5f61 273a 207b  'migrated__a': {
-000238c0: 2761 277d 2c0a 2020 2020 2e2e 2e20 2020  'a'},.    ...   
-000238d0: 2020 2020 2020 2761 273a 207b 2762 277d        'a': {'b'}
-000238e0: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
-000238f0: 2020 2762 273a 207b 2763 277d 2c0a 2020    'b': {'c'},.  
-00023900: 2020 2e2e 2e20 2020 2020 2020 2020 2763    ...         'c
-00023910: 273a 2073 6574 2829 2c0a 2020 2020 2e2e  ': set(),.    ..
-00023920: 2e20 2020 2020 7d2c 0a20 2020 202e 2e2e  .     },.    ...
-00023930: 2020 2020 207b 0a20 2020 202e 2e2e 2020       {.    ...  
-00023940: 2020 2020 2020 2027 6d69 6772 6174 6564         'migrated
-00023950: 5f5f 6127 3a20 7b27 7265 736f 7572 6365  __a': {'resource
-00023960: 5f6e 616d 6527 3a20 276d 6967 7261 7465  _name': 'migrate
-00023970: 645f 5f61 272c 2027 6e6f 6465 7327 3a20  d__a', 'nodes': 
-00023980: 5b7b 2770 6172 616d 7327 3a20 7b27 7479  [{'params': {'ty
-00023990: 7065 273a 2027 6d61 7465 7269 616c 697a  pe': 'materializ
-000239a0: 6564 272c 2027 6461 7461 736f 7572 6365  ed', 'datasource
-000239b0: 273a 2027 6127 7d7d 5d7d 2c0a 2020 2020  ': 'a'}}]},.    
-000239c0: 2e2e 2e20 2020 2020 2020 2020 2761 273a  ...         'a':
-000239d0: 207b 2772 6573 6f75 7263 655f 6e61 6d65   {'resource_name
-000239e0: 273a 2027 6127 7d2c 0a20 2020 202e 2e2e  ': 'a'},.    ...
-000239f0: 2020 2020 2020 2020 2027 6227 3a20 7b27           'b': {'
-00023a00: 7265 736f 7572 6365 5f6e 616d 6527 3a20  resource_name': 
-00023a10: 2762 272c 2027 6e6f 6465 7327 3a20 5b7b  'b', 'nodes': [{
-00023a20: 2770 6172 616d 7327 3a20 7b27 7479 7065  'params': {'type
-00023a30: 273a 2027 6d61 7465 7269 616c 697a 6564  ': 'materialized
-00023a40: 272c 2027 6461 7461 736f 7572 6365 273a  ', 'datasource':
-00023a50: 2027 6327 7d7d 5d20 7d2c 0a20 2020 202e   'c'}}] },.    .
-00023a60: 2e2e 2020 2020 2020 2020 2027 6327 3a20  ..         'c': 
-00023a70: 7b27 7265 736f 7572 6365 5f6e 616d 6527  {'resource_name'
-00023a80: 3a20 2763 277d 2c0a 2020 2020 2e2e 2e20  : 'c'},.    ... 
-00023a90: 2020 2020 7d2c 0a20 2020 202e 2e2e 2020      },.    ...  
-00023aa0: 2020 207b 0a20 2020 202e 2e2e 2020 2020     {.    ...    
-00023ab0: 2020 2020 2027 6d69 6772 6174 6564 5f5f       'migrated__
-00023ac0: 6127 3a20 7b27 7265 736f 7572 6365 5f6e  a': {'resource_n
-00023ad0: 616d 6527 3a20 276d 6967 7261 7465 645f  ame': 'migrated_
-00023ae0: 5f61 277d 2c0a 2020 2020 2e2e 2e20 2020  _a'},.    ...   
-00023af0: 2020 2020 2020 2761 273a 207b 2772 6573        'a': {'res
-00023b00: 6f75 7263 655f 6e61 6d65 273a 2027 6127  ource_name': 'a'
-00023b10: 7d2c 0a20 2020 202e 2e2e 2020 2020 207d  },.    ...     }
-00023b20: 2c0a 2020 2020 2e2e 2e20 2020 2020 5b27  ,.    ...     ['
-00023b30: 6d69 6772 6174 6564 5f61 272c 2027 6127  migrated_a', 'a'
-00023b40: 2c20 2762 272c 2027 6327 5d2c 0a20 2020  , 'b', 'c'],.   
-00023b50: 202e 2e2e 2029 0a20 2020 203e 3e3e 207b   ... ).    >>> {
-00023b60: 6b3a 2073 6f72 7465 6428 7629 2066 6f72  k: sorted(v) for
-00023b70: 206b 2c20 7620 696e 2064 6570 732e 6974   k, v in deps.it
-00023b80: 656d 7328 297d 0a20 2020 207b 2763 273a  ems()}.    {'c':
-00023b90: 205b 5d2c 2027 6227 3a20 5b27 6127 2c20   [], 'b': ['a', 
-00023ba0: 2763 275d 2c20 2761 273a 205b 5d2c 2027  'c'], 'a': [], '
-00023bb0: 6d69 6772 6174 6564 5f61 273a 205b 5d7d  migrated_a': []}
-00023bc0: 0a20 2020 2022 2222 0a20 2020 2064 6f77  .    """.    dow
-00023bd0: 6e73 7472 6561 6d5f 6465 705f 6d61 7020  nstream_dep_map 
-00023be0: 3d20 6372 6561 7465 5f64 6f77 6e73 7472  = create_downstr
-00023bf0: 6561 6d5f 6465 7065 6e64 656e 6379 5f67  eam_dependency_g
-00023c00: 7261 7068 2861 6c6c 5f64 6570 5f6d 6170  raph(all_dep_map
-00023c10: 2c20 616c 6c5f 7265 736f 7572 6365 7329  , all_resources)
-00023c20: 0a20 2020 206e 6577 5f64 6570 5f6d 6170  .    new_dep_map
-00023c30: 3a20 4469 6374 5b73 7472 2c20 5365 745b  : Dict[str, Set[
-00023c40: 7374 725d 5d20 3d20 7b7d 0a20 2020 206e  str]] = {}.    n
-00023c50: 6577 5f74 6f5f 7275 6e20 3d20 6465 6570  ew_to_run = deep
-00023c60: 636f 7079 2874 6f5f 7275 6e29 0a20 2020  copy(to_run).   
-00023c70: 2075 7064 6174 655f 6465 705f 6d61 705f   update_dep_map_
-00023c80: 7265 6375 7273 6976 656c 7928 6e65 775f  recursively(new_
-00023c90: 6465 705f 6d61 702c 2064 6f77 6e73 7472  dep_map, downstr
-00023ca0: 6561 6d5f 6465 705f 6d61 702c 2061 6c6c  eam_dep_map, all
-00023cb0: 5f72 6573 6f75 7263 6573 2c20 6e65 775f  _resources, new_
-00023cc0: 746f 5f72 756e 2c20 6465 705f 6d61 705f  to_run, dep_map_
-00023cd0: 6b65 7973 290a 2020 2020 7265 7475 726e  keys).    return
-00023ce0: 206e 6577 5f64 6570 5f6d 6170 2c20 6e65   new_dep_map, ne
-00023cf0: 775f 746f 5f72 756e 0a0a 0a40 6461 7461  w_to_run...@data
-00023d00: 636c 6173 730a 636c 6173 7320 4772 6170  class.class Grap
-00023d10: 6844 6570 656e 6465 6e63 6965 733a 0a20  hDependencies:. 
-00023d20: 2020 2022 2222 0a20 2020 2054 6869 7320     """.    This 
-00023d30: 636c 6173 7320 6973 2075 7365 6420 746f  class is used to
-00023d40: 2073 746f 7265 2074 6865 2064 6570 656e   store the depen
-00023d50: 6465 6e63 6965 7320 6772 6170 6820 616e  dencies graph an
-00023d60: 6420 7468 6520 7265 736f 7572 6365 7320  d the resources 
-00023d70: 7468 6174 2061 7265 2067 6f69 6e67 2074  that are going t
-00023d80: 6f20 6265 2064 6570 6c6f 7965 640a 2020  o be deployed.  
-00023d90: 2020 2222 220a 0a20 2020 2064 6570 5f6d    """..    dep_m
-00023da0: 6170 3a20 4469 6374 5b73 7472 2c20 5365  ap: Dict[str, Se
-00023db0: 745b 7374 725d 5d0a 2020 2020 746f 5f72  t[str]].    to_r
-00023dc0: 756e 3a20 4469 6374 5b73 7472 2c20 4469  un: Dict[str, Di
-00023dd0: 6374 5b73 7472 2c20 416e 795d 5d0a 0a20  ct[str, Any]].. 
-00023de0: 2020 2023 2054 6865 2073 616d 6520 6173     # The same as
-00023df0: 2061 626f 7665 2062 7574 2066 6f72 2074   above but for t
-00023e00: 6865 2077 686f 6c65 2070 726f 6a65 6374  he whole project
-00023e10: 2c20 6e6f 7420 6a75 7374 2074 6865 2072  , not just the r
-00023e20: 6573 6f75 7263 6573 2061 6666 6563 7465  esources affecte
-00023e30: 6420 6279 2074 6865 2063 7572 7265 6e74  d by the current
-00023e40: 2064 6570 6c6f 796d 656e 740a 2020 2020   deployment.    
-00023e50: 616c 6c5f 6465 705f 6d61 703a 2044 6963  all_dep_map: Dic
-00023e60: 745b 7374 722c 2053 6574 5b73 7472 5d5d  t[str, Set[str]]
-00023e70: 0a20 2020 2061 6c6c 5f72 6573 6f75 7263  .    all_resourc
-00023e80: 6573 3a20 4469 6374 5b73 7472 2c20 4469  es: Dict[str, Di
-00023e90: 6374 5b73 7472 2c20 416e 795d 5d0a 0a0a  ct[str, Any]]...
-00023ea0: 6173 796e 6320 6465 6620 6275 696c 645f  async def build_
-00023eb0: 6772 6170 6828 0a20 2020 2066 696c 656e  graph(.    filen
-00023ec0: 616d 6573 3a20 4974 6572 6162 6c65 5b73  ames: Iterable[s
-00023ed0: 7472 5d2c 0a20 2020 2074 625f 636c 6965  tr],.    tb_clie
-00023ee0: 6e74 3a20 5469 6e79 422c 0a20 2020 2064  nt: TinyB,.    d
-00023ef0: 6972 5f70 6174 683a 204f 7074 696f 6e61  ir_path: Optiona
-00023f00: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00023f10: 2020 2072 6573 6f75 7263 655f 7665 7273     resource_vers
-00023f20: 696f 6e73 3d4e 6f6e 652c 0a20 2020 2077  ions=None,.    w
-00023f30: 6f72 6b73 7061 6365 5f6d 6170 3a20 4f70  orkspace_map: Op
-00023f40: 7469 6f6e 616c 5b44 6963 745d 203d 204e  tional[Dict] = N
-00023f50: 6f6e 652c 0a20 2020 2070 726f 6365 7373  one,.    process
-00023f60: 5f64 6570 656e 6465 6e63 6965 733a 2062  _dependencies: b
-00023f70: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-00023f80: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
-00023f90: 2046 616c 7365 2c0a 2020 2020 736b 6970   False,.    skip
-00023fa0: 5f63 6f6e 6e65 6374 6f72 733a 2062 6f6f  _connectors: boo
-00023fb0: 6c20 3d20 4661 6c73 652c 0a20 2020 2077  l = False,.    w
-00023fc0: 6f72 6b73 7061 6365 5f6c 6962 5f70 6174  orkspace_lib_pat
-00023fd0: 6873 3a20 4f70 7469 6f6e 616c 5b4c 6973  hs: Optional[Lis
-00023fe0: 745b 5475 706c 655b 7374 722c 2073 7472  t[Tuple[str, str
-00023ff0: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
-00024000: 6375 7272 656e 745f 7773 3a20 4f70 7469  current_ws: Opti
-00024010: 6f6e 616c 5b44 6963 745b 7374 722c 2041  onal[Dict[str, A
-00024020: 6e79 5d5d 203d 204e 6f6e 652c 0a20 2020  ny]] = None,.   
-00024030: 2063 6861 6e67 6564 3a20 4f70 7469 6f6e   changed: Option
-00024040: 616c 5b44 6963 745b 7374 722c 2041 6e79  al[Dict[str, Any
-00024050: 5d5d 203d 204e 6f6e 652c 0a20 2020 206f  ]] = None,.    o
-00024060: 6e6c 795f 6368 616e 6765 733a 2062 6f6f  nly_changes: boo
-00024070: 6c20 3d20 4661 6c73 652c 0a20 2020 2066  l = False,.    f
-00024080: 6f72 6b5f 646f 776e 7374 7265 616d 3a20  ork_downstream: 
-00024090: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-000240a0: 2046 616c 7365 2c0a 2020 2020 6973 5f69   False,.    is_i
-000240b0: 6e74 6572 6e61 6c3a 204f 7074 696f 6e61  nternal: Optiona
-000240c0: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-000240d0: 0a29 202d 3e20 4772 6170 6844 6570 656e  .) -> GraphDepen
-000240e0: 6465 6e63 6965 733a 0a20 2020 2022 2222  dencies:.    """
-000240f0: 0a20 2020 2054 6869 7320 6d65 7468 6f64  .    This method
-00024100: 2077 696c 6c20 6765 6e65 7261 7465 2061   will generate a
-00024110: 2064 6570 656e 6465 6e63 7920 6772 6170   dependency grap
-00024120: 6820 666f 7220 7468 6520 6769 7665 6e20  h for the given 
-00024130: 6669 6c65 732e 2049 7420 7769 6c6c 2061  files. It will a
-00024140: 6c73 6f20 7265 7475 726e 2061 206d 6170  lso return a map
-00024150: 206f 6620 616c 6c20 7468 6520 7265 736f   of all the reso
-00024160: 7572 6365 7320 7468 6174 2061 7265 2067  urces that are g
-00024170: 6f69 6e67 2074 6f20 6265 2064 6570 6c6f  oing to be deplo
-00024180: 7965 642e 0a20 2020 2042 7920 6465 6661  yed..    By defa
-00024190: 756c 7420 6974 2077 696c 6c20 6765 6e65  ult it will gene
-000241a0: 7261 7465 2074 6865 2067 7261 7068 2066  rate the graph f
-000241b0: 726f 6d20 6c65 6674 2074 6f20 7269 6768  rom left to righ
-000241c0: 742c 2062 7574 2069 6620 666f 726b 2d64  t, but if fork-d
-000241d0: 6f77 6e73 7472 6561 6d2c 2069 7420 7769  ownstream, it wi
-000241e0: 6c6c 2067 656e 6572 6174 6520 7468 6520  ll generate the 
-000241f0: 6772 6170 6820 6672 6f6d 2072 6967 6874  graph from right
-00024200: 2074 6f20 6c65 6674 2e0a 2020 2020 2222   to left..    ""
-00024210: 220a 2020 2020 746f 5f72 756e 3a20 4469  ".    to_run: Di
-00024220: 6374 5b73 7472 2c20 416e 795d 203d 207b  ct[str, Any] = {
-00024230: 7d0a 2020 2020 6465 7073 3a20 4c69 7374  }.    deps: List
-00024240: 5b73 7472 5d20 3d20 5b5d 0a20 2020 2064  [str] = [].    d
-00024250: 6570 5f6d 6170 3a20 4469 6374 5b73 7472  ep_map: Dict[str
-00024260: 2c20 416e 795d 203d 207b 7d0a 2020 2020  , Any] = {}.    
-00024270: 656d 6265 6464 6564 5f64 6174 6173 6f75  embedded_datasou
-00024280: 7263 6573 203d 207b 7d0a 2020 2020 6966  rces = {}.    if
-00024290: 206e 6f74 2077 6f72 6b73 7061 6365 5f6d   not workspace_m
-000242a0: 6170 3a0a 2020 2020 2020 2020 776f 726b  ap:.        work
-000242b0: 7370 6163 655f 6d61 7020 3d20 7b7d 0a0a  space_map = {}..
-000242c0: 2020 2020 2320 5468 6573 6520 6469 6374      # These dict
-000242d0: 696f 6e61 7269 6573 2061 7265 2075 7365  ionaries are use
-000242e0: 6420 746f 2073 746f 7265 2061 6c6c 2074  d to store all t
-000242f0: 6865 2072 6573 6f75 7263 6573 2061 6e64  he resources and
-00024300: 2074 6865 7265 2064 6570 656e 6465 6e63   there dependenc
-00024310: 6965 7320 666f 7220 7468 6520 7768 6f6c  ies for the whol
-00024320: 6520 7072 6f6a 6563 740a 2020 2020 2320  e project.    # 
-00024330: 5468 6973 2069 7320 7573 6564 2066 6f72  This is used for
-00024340: 2074 6865 2064 6f77 6e73 7472 6561 6d20   the downstream 
-00024350: 6465 7065 6e64 656e 6379 2067 7261 7068  dependency graph
-00024360: 0a20 2020 2061 6c6c 5f64 6570 5f6d 6170  .    all_dep_map
-00024370: 3a20 4469 6374 5b73 7472 2c20 5365 745b  : Dict[str, Set[
-00024380: 7374 725d 5d20 3d20 7b7d 0a20 2020 2061  str]] = {}.    a
-00024390: 6c6c 5f72 6573 6f75 7263 6573 3a20 4469  ll_resources: Di
-000243a0: 6374 5b73 7472 2c20 4469 6374 5b73 7472  ct[str, Dict[str
-000243b0: 2c20 416e 795d 5d20 3d20 7b7d 0a0a 2020  , Any]] = {}..  
-000243c0: 2020 6966 2064 6972 5f70 6174 6820 6973    if dir_path is
-000243d0: 204e 6f6e 653a 0a20 2020 2020 2020 2064   None:.        d
-000243e0: 6972 5f70 6174 6820 3d20 6f73 2e67 6574  ir_path = os.get
-000243f0: 6377 6428 290a 0a20 2020 2023 2057 6865  cwd()..    # Whe
-00024400: 6e20 7573 696e 6720 666f 726b 2d64 6f77  n using fork-dow
-00024410: 6e73 7472 6561 6d20 6f72 202d 2d6f 6e6c  nstream or --onl
-00024420: 792d 6368 616e 6765 732c 2077 6520 6e65  y-changes, we ne
-00024430: 6564 2074 6f20 6765 6e65 7261 7465 2061  ed to generate a
-00024440: 6c6c 2074 6865 2067 7261 7068 206f 6620  ll the graph of 
-00024450: 616c 6c20 7468 6520 7265 736f 7572 6365  all the resource
-00024460: 7320 616e 6420 7468 6569 7220 6465 7065  s and their depe
-00024470: 6e64 656e 6369 6573 0a20 2020 2023 2054  ndencies.    # T
-00024480: 6869 7320 7761 7920 7765 2063 616e 2061  his way we can a
-00024490: 6464 206d 6f72 6520 7265 736f 7572 6365  dd more resource
-000244a0: 7320 696e 746f 2074 6865 2074 6f5f 7275  s into the to_ru
-000244b0: 6e20 6469 6374 696f 6e61 7279 2069 6620  n dictionary if 
-000244c0: 6e65 6564 6564 2e0a 2020 2020 6966 2070  needed..    if p
-000244d0: 726f 6365 7373 5f64 6570 656e 6465 6e63  rocess_dependenc
-000244e0: 6965 7320 616e 6420 6f6e 6c79 5f63 6861  ies and only_cha
-000244f0: 6e67 6573 3a0a 2020 2020 2020 2020 616c  nges:.        al
-00024500: 6c5f 6465 7065 6e64 656e 6369 6573 5f67  l_dependencies_g
-00024510: 7261 7068 203d 2061 7761 6974 2062 7569  raph = await bui
-00024520: 6c64 5f67 7261 7068 280a 2020 2020 2020  ld_graph(.      
-00024530: 2020 2020 2020 6765 745f 7072 6f6a 6563        get_projec
-00024540: 745f 6669 6c65 6e61 6d65 7328 6469 725f  t_filenames(dir_
-00024550: 7061 7468 292c 0a20 2020 2020 2020 2020  path),.         
-00024560: 2020 2074 625f 636c 6965 6e74 2c0a 2020     tb_client,.  
-00024570: 2020 2020 2020 2020 2020 6469 725f 7061            dir_pa
-00024580: 7468 3d64 6972 5f70 6174 682c 0a20 2020  th=dir_path,.   
-00024590: 2020 2020 2020 2020 2070 726f 6365 7373           process
-000245a0: 5f64 6570 656e 6465 6e63 6965 733d 5472  _dependencies=Tr
-000245b0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-000245c0: 7265 736f 7572 6365 5f76 6572 7369 6f6e  resource_version
-000245d0: 733d 7265 736f 7572 6365 5f76 6572 7369  s=resource_versi
-000245e0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-000245f0: 2077 6f72 6b73 7061 6365 5f6d 6170 3d77   workspace_map=w
-00024600: 6f72 6b73 7061 6365 5f6d 6170 2c0a 2020  orkspace_map,.  
-00024610: 2020 2020 2020 2020 2020 736b 6970 5f63            skip_c
-00024620: 6f6e 6e65 6374 6f72 733d 5472 7565 2c0a  onnectors=True,.
-00024630: 2020 2020 2020 2020 2020 2020 776f 726b              work
-00024640: 7370 6163 655f 6c69 625f 7061 7468 733d  space_lib_paths=
-00024650: 776f 726b 7370 6163 655f 6c69 625f 7061  workspace_lib_pa
-00024660: 7468 732c 0a20 2020 2020 2020 2020 2020  ths,.           
-00024670: 2063 7572 7265 6e74 5f77 733d 6375 7272   current_ws=curr
-00024680: 656e 745f 7773 2c0a 2020 2020 2020 2020  ent_ws,.        
-00024690: 2020 2020 6368 616e 6765 643d 4e6f 6e65      changed=None
-000246a0: 2c0a 2020 2020 2020 2020 2020 2020 6f6e  ,.            on
-000246b0: 6c79 5f63 6861 6e67 6573 3d46 616c 7365  ly_changes=False
-000246c0: 2c0a 2020 2020 2020 2020 2020 2020 6973  ,.            is
-000246d0: 5f69 6e74 6572 6e61 6c3d 6973 5f69 6e74  _internal=is_int
-000246e0: 6572 6e61 6c2c 0a20 2020 2020 2020 2029  ernal,.        )
-000246f0: 0a20 2020 2020 2020 2061 6c6c 5f64 6570  .        all_dep
-00024700: 5f6d 6170 203d 2061 6c6c 5f64 6570 656e  _map = all_depen
-00024710: 6465 6e63 6965 735f 6772 6170 682e 6465  dencies_graph.de
-00024720: 705f 6d61 700a 2020 2020 2020 2020 616c  p_map.        al
-00024730: 6c5f 7265 736f 7572 6365 7320 3d20 616c  l_resources = al
-00024740: 6c5f 6465 7065 6e64 656e 6369 6573 5f67  l_dependencies_g
-00024750: 7261 7068 2e74 6f5f 7275 6e0a 0a20 2020  raph.to_run..   
-00024760: 2061 7379 6e63 2064 6566 2070 726f 6365   async def proce
-00024770: 7373 280a 2020 2020 2020 2020 6669 6c65  ss(.        file
-00024780: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-00024790: 2020 2064 6570 733a 204c 6973 745b 7374     deps: List[st
-000247a0: 725d 2c0a 2020 2020 2020 2020 6465 705f  r],.        dep_
-000247b0: 6d61 703a 2044 6963 745b 7374 722c 2041  map: Dict[str, A
-000247c0: 6e79 5d2c 0a20 2020 2020 2020 2074 6f5f  ny],.        to_
-000247d0: 7275 6e3a 2044 6963 745b 7374 722c 2041  run: Dict[str, A
-000247e0: 6e79 5d2c 0a20 2020 2020 2020 2077 6f72  ny],.        wor
-000247f0: 6b73 7061 6365 5f6c 6962 5f70 6174 6873  kspace_lib_paths
-00024800: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00024810: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
-00024820: 5d2c 0a20 2020 2029 3a0a 2020 2020 2020  ],.    ):.      
-00024830: 2020 6e61 6d65 2c20 6b69 6e64 203d 2066    name, kind = f
-00024840: 696c 656e 616d 652e 7273 706c 6974 2822  ilename.rsplit("
-00024850: 2e22 2c20 3129 0a0a 2020 2020 2020 2020  .", 1)..        
-00024860: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00024870: 2072 6573 203d 2061 7761 6974 2070 726f   res = await pro
-00024880: 6365 7373 5f66 696c 6528 0a20 2020 2020  cess_file(.     
-00024890: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-000248a0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-000248b0: 2020 2020 2074 625f 636c 6965 6e74 2c0a       tb_client,.
-000248c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000248d0: 7265 736f 7572 6365 5f76 6572 7369 6f6e  resource_version
-000248e0: 733d 7265 736f 7572 6365 5f76 6572 7369  s=resource_versi
-000248f0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-00024900: 2020 2020 2073 6b69 705f 636f 6e6e 6563       skip_connec
-00024910: 746f 7273 3d73 6b69 705f 636f 6e6e 6563  tors=skip_connec
-00024920: 746f 7273 2c0a 2020 2020 2020 2020 2020  tors,.          
-00024930: 2020 2020 2020 776f 726b 7370 6163 655f        workspace_
-00024940: 6d61 703d 776f 726b 7370 6163 655f 6d61  map=workspace_ma
-00024950: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
-00024960: 2020 2077 6f72 6b73 7061 6365 5f6c 6962     workspace_lib
-00024970: 5f70 6174 6873 3d77 6f72 6b73 7061 6365  _paths=workspace
-00024980: 5f6c 6962 5f70 6174 6873 2c0a 2020 2020  _lib_paths,.    
-00024990: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000249a0: 656e 745f 7773 3d63 7572 7265 6e74 5f77  ent_ws=current_w
-000249b0: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
-000249c0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000249d0: 636c 6963 6b2e 436c 6963 6b45 7863 6570  click.ClickExcep
-000249e0: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-000249f0: 2020 2020 2020 2072 6169 7365 2065 0a20         raise e. 
-00024a00: 2020 2020 2020 2065 7863 6570 7420 496e         except In
-00024a10: 636c 7564 6546 696c 654e 6f74 466f 756e  cludeFileNotFoun
-00024a20: 6445 7863 6570 7469 6f6e 2061 7320 653a  dException as e:
-00024a30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00024a40: 7365 2063 6c69 636b 2e43 6c69 636b 4578  se click.ClickEx
-00024a50: 6365 7074 696f 6e28 4665 6564 6261 636b  ception(Feedback
-00024a60: 4d61 6e61 6765 722e 6572 726f 725f 6465  Manager.error_de
-00024a70: 6c65 7465 645f 696e 636c 7564 6528 696e  leted_include(in
-00024a80: 636c 7564 655f 6669 6c65 3d73 7472 2865  clude_file=str(e
-00024a90: 292c 2066 696c 656e 616d 653d 6669 6c65  ), filename=file
-00024aa0: 6e61 6d65 2929 0a20 2020 2020 2020 2065  name)).        e
-00024ab0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00024ac0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00024ad0: 2020 7261 6973 6520 636c 6963 6b2e 436c    raise click.Cl
-00024ae0: 6963 6b45 7863 6570 7469 6f6e 2873 7472  ickException(str
-00024af0: 2865 2929 0a0a 2020 2020 2020 2020 666f  (e))..        fo
-00024b00: 7220 7220 696e 2072 6573 3a0a 2020 2020  r r in res:.    
-00024b10: 2020 2020 2020 2020 666e 203d 2072 5b22          fn = r["
-00024b20: 7265 736f 7572 6365 5f6e 616d 6522 5d0a  resource_name"].
-00024b30: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00024b40: 6861 6e67 6564 2061 6e64 2066 6e20 696e  hanged and fn in
-00024b50: 2063 6861 6e67 6564 2061 6e64 2028 6e6f   changed and (no
-00024b60: 7420 6368 616e 6765 645b 666e 5d20 6f72  t changed[fn] or
-00024b70: 2063 6861 6e67 6564 5b66 6e5d 2069 6e20   changed[fn] in 
-00024b80: 5b22 7368 6172 6564 222c 2022 7265 6d6f  ["shared", "remo
-00024b90: 7465 225d 293a 0a20 2020 2020 2020 2020  te"]):.         
-00024ba0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00024bb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00024bc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00024bd0: 2020 666f 726b 5f64 6f77 6e73 7472 6561    fork_downstrea
-00024be0: 6d0a 2020 2020 2020 2020 2020 2020 2020  m.              
-00024bf0: 2020 616e 6420 722e 6765 7428 2272 6573    and r.get("res
-00024c00: 6f75 7263 6522 2c20 2222 2920 3d3d 2022  ource", "") == "
-00024c10: 7069 7065 7322 0a20 2020 2020 2020 2020  pipes".         
-00024c20: 2020 2020 2020 2061 6e64 2061 6e79 285b         and any([
-00024c30: 2265 6e67 696e 6522 2069 6e20 782e 6765  "engine" in x.ge
-00024c40: 7428 2270 6172 616d 7322 2c20 7b7d 2920  t("params", {}) 
-00024c50: 666f 7220 7820 696e 2072 2e67 6574 2822  for x in r.get("
-00024c60: 6e6f 6465 7322 2c20 5b5d 295d 290a 2020  nodes", [])]).  
-00024c70: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00024c80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00024c90: 7365 2063 6c69 636b 2e43 6c69 636b 4578  se click.ClickEx
-00024ca0: 6365 7074 696f 6e28 4665 6564 6261 636b  ception(Feedback
-00024cb0: 4d61 6e61 6765 722e 6572 726f 725f 666f  Manager.error_fo
-00024cc0: 726b 646f 776e 7374 7265 616d 5f70 6970  rkdownstream_pip
-00024cd0: 6573 5f77 6974 685f 656e 6769 6e65 2870  es_with_engine(p
-00024ce0: 6970 653d 666e 2929 0a0a 2020 2020 2020  ipe=fn))..      
-00024cf0: 2020 2020 2020 746f 5f72 756e 5b66 6e5d        to_run[fn]
-00024d00: 203d 2072 0a20 2020 2020 2020 2020 2020   = r.           
-00024d10: 2066 696c 655f 6465 7073 203d 2072 2e67   file_deps = r.g
-00024d20: 6574 2822 6465 7073 222c 205b 5d29 0a20  et("deps", []). 
-00024d30: 2020 2020 2020 2020 2020 2064 6570 7320             deps 
-00024d40: 2b3d 2066 696c 655f 6465 7073 0a20 2020  += file_deps.   
-00024d50: 2020 2020 2020 2020 2023 2063 616c 6375           # calcu
-00024d60: 6c61 7465 2061 6e64 206c 6f6f 6b20 666f  late and look fo
-00024d70: 7220 6465 7073 0a20 2020 2020 2020 2020  r deps.         
-00024d80: 2020 2064 6570 5f6c 6973 7420 3d20 5b5d     dep_list = []
-00024d90: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00024da0: 2078 2069 6e20 6669 6c65 5f64 6570 733a   x in file_deps:
-00024db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024dc0: 2069 6620 7820 6e6f 7420 696e 2049 4e54   if x not in INT
-00024dd0: 4552 4e41 4c5f 5441 424c 4553 206f 7220  ERNAL_TABLES or 
-00024de0: 6973 5f69 6e74 6572 6e61 6c3a 0a20 2020  is_internal:.   
-00024df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e00: 2066 2c20 6473 203d 2066 696e 645f 6669   f, ds = find_fi
-00024e10: 6c65 5f62 795f 6e61 6d65 2864 6972 5f70  le_by_name(dir_p
-00024e20: 6174 682c 2078 2c20 7665 7262 6f73 652c  ath, x, verbose,
-00024e30: 2077 6f72 6b73 7061 6365 5f6c 6962 5f70   workspace_lib_p
-00024e40: 6174 6873 3d77 6f72 6b73 7061 6365 5f6c  aths=workspace_l
-00024e50: 6962 5f70 6174 6873 2c20 7265 736f 7572  ib_paths, resour
-00024e60: 6365 3d72 290a 2020 2020 2020 2020 2020  ce=r).          
-00024e70: 2020 2020 2020 2020 2020 6966 2066 3a0a            if f:.
-00024e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e90: 2020 2020 2020 2020 6465 705f 6c69 7374          dep_list
-00024ea0: 2e61 7070 656e 6428 662e 7273 706c 6974  .append(f.rsplit
-00024eb0: 2822 2e22 2c20 3129 5b30 5d29 0a20 2020  (".", 1)[0]).   
-00024ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ed0: 2069 6620 6473 3a0a 2020 2020 2020 2020   if ds:.        
+0001f2c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a22 290a 2020  ***********").  
+0001f2d0: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
+0001f2e0: 2846 6565 6462 6163 6b4d 616e 6167 6572  (FeedbackManager
+0001f2f0: 2e69 6e66 6f5f 6461 7461 736f 7572 6365  .info_datasource
+0001f300: 5f64 6f65 736e 745f 6d61 7463 6828 6461  _doesnt_match(da
+0001f310: 7461 736f 7572 6365 3d64 735f 6e61 6d65  tasource=ds_name
+0001f320: 2929 0a20 2020 2020 2020 2066 6f72 206f  )).        for o
+0001f330: 7065 7261 7469 6f6e 2069 6e20 616c 7465  peration in alte
+0001f340: 725f 7265 7370 6f6e 7365 5b22 6f70 6572  r_response["oper
+0001f350: 6174 696f 6e73 225d 3a0a 2020 2020 2020  ations"]:.      
+0001f360: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
+0001f370: 2866 222a 2a20 2020 2d20 207b 6f70 6572  (f"**   -  {oper
+0001f380: 6174 696f 6e7d 2229 0a0a 2020 2020 2020  ation}")..      
+0001f390: 2020 6966 2073 6b69 705f 636f 6e66 6972    if skip_confir
+0001f3a0: 6d61 7469 6f6e 3a0a 2020 2020 2020 2020  mation:.        
+0001f3b0: 2020 2020 6d61 6b65 5f63 6861 6e67 6573      make_changes
+0001f3c0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+0001f3d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001f3e0: 2020 6d61 6b65 5f63 6861 6e67 6573 203d    make_changes =
+0001f3f0: 2063 6c69 636b 2e70 726f 6d70 7428 4665   click.prompt(Fe
+0001f400: 6564 6261 636b 4d61 6e61 6765 722e 696e  edbackManager.in
+0001f410: 666f 5f61 736b 5f66 6f72 5f61 6c74 6572  fo_ask_for_alter
+0001f420: 5f63 6f6e 6669 726d 6174 696f 6e28 2929  _confirmation())
+0001f430: 2e6c 6f77 6572 2829 203d 3d20 2279 220a  .lower() == "y".
+0001f440: 0a20 2020 2020 2020 2069 6620 6d61 6b65  .        if make
+0001f450: 5f63 6861 6e67 6573 3a0a 2020 2020 2020  _changes:.      
+0001f460: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+0001f470: 6e74 2e61 6c74 6572 5f64 6174 6173 6f75  nt.alter_datasou
+0001f480: 7263 6528 0a20 2020 2020 2020 2020 2020  rce(.           
+0001f490: 2020 2020 2064 735f 6e61 6d65 2c0a 2020       ds_name,.  
+0001f4a0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0001f4b0: 775f 7363 6865 6d61 3d6e 6577 5f73 6368  w_schema=new_sch
+0001f4c0: 656d 612c 0a20 2020 2020 2020 2020 2020  ema,.           
+0001f4d0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0001f4e0: 3d6e 6577 5f64 6573 6372 6970 7469 6f6e  =new_description
+0001f4f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001f500: 2020 7474 6c3d 6e65 775f 7474 6c2c 0a20    ttl=new_ttl,. 
+0001f510: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001f520: 7279 5f72 756e 3d46 616c 7365 2c0a 2020  ry_run=False,.  
+0001f530: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0001f540: 6465 7865 733d 6e65 775f 696e 6469 6365  dexes=new_indice
+0001f550: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
+0001f560: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+0001f570: 636b 2e65 6368 6f28 4665 6564 6261 636b  ck.echo(Feedback
+0001f580: 4d61 6e61 6765 722e 7375 6363 6573 735f  Manager.success_
+0001f590: 6461 7461 736f 7572 6365 5f61 6c74 6572  datasource_alter
+0001f5a0: 2829 290a 2020 2020 2020 2020 656c 7365  ()).        else
+0001f5b0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+0001f5c0: 7465 725f 6572 726f 725f 6d65 7373 6167  ter_error_messag
+0001f5d0: 6520 3d20 2241 6c74 6572 2064 6174 6173  e = "Alter datas
+0001f5e0: 6f75 7263 6520 6361 6e63 656c 6c65 6422  ource cancelled"
+0001f5f0: 0a0a 2020 2020 6966 2064 6174 6173 6f75  ..    if datasou
+0001f600: 7263 655f 6578 6973 7473 2061 6e64 2064  rce_exists and d
+0001f610: 735b 2270 6172 616d 7322 5d2e 6765 7428  s["params"].get(
+0001f620: 2262 6163 6b66 696c 6c5f 636f 6c75 6d6e  "backfill_column
+0001f630: 2229 2021 3d20 6578 6973 7469 6e67 5f64  ") != existing_d
+0001f640: 735b 2274 6167 7322 5d2e 6765 7428 2262  s["tags"].get("b
+0001f650: 6163 6b66 696c 6c5f 636f 6c75 6d6e 2229  ackfill_column")
+0001f660: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
+0001f670: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0001f680: 2022 6261 636b 6669 6c6c 5f63 6f6c 756d   "backfill_colum
+0001f690: 6e22 3a20 6473 5b22 7061 7261 6d73 225d  n": ds["params"]
+0001f6a0: 2e67 6574 2822 6261 636b 6669 6c6c 5f63  .get("backfill_c
+0001f6b0: 6f6c 756d 6e22 292c 0a20 2020 2020 2020  olumn"),.       
+0001f6c0: 207d 0a0a 2020 2020 2020 2020 7472 793a   }..        try:
+0001f6d0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+0001f6e0: 636b 2e65 6368 6f28 4665 6564 6261 636b  ck.echo(Feedback
+0001f6f0: 4d61 6e61 6765 722e 696e 666f 5f75 7064  Manager.info_upd
+0001f700: 6174 655f 6461 7461 736f 7572 6365 2864  ate_datasource(d
+0001f710: 6174 6173 6f75 7263 653d 6473 5f6e 616d  atasource=ds_nam
+0001f720: 652c 2070 6172 616d 733d 7061 7261 6d73  e, params=params
+0001f730: 2929 0a20 2020 2020 2020 2020 2020 2061  )).            a
+0001f740: 7761 6974 2063 6c69 656e 742e 7570 6461  wait client.upda
+0001f750: 7465 5f64 6174 6173 6f75 7263 6528 6473  te_datasource(ds
+0001f760: 5f6e 616d 652c 2070 6172 616d 7329 0a20  _name, params). 
+0001f770: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+0001f780: 2e65 6368 6f28 4665 6564 6261 636b 4d61  .echo(FeedbackMa
+0001f790: 6e61 6765 722e 7375 6363 6573 735f 7570  nager.success_up
+0001f7a0: 6461 7465 5f64 6174 6173 6f75 7263 6528  date_datasource(
+0001f7b0: 6461 7461 736f 7572 6365 3d64 735f 6e61  datasource=ds_na
+0001f7c0: 6d65 2c20 7061 7261 6d73 3d70 6172 616d  me, params=param
+0001f7d0: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
+0001f7e0: 6d61 6b65 5f63 6861 6e67 6573 203d 2054  make_changes = T
+0001f7f0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0001f800: 616c 7465 725f 7265 7370 6f6e 7365 203d  alter_response =
+0001f810: 2054 7275 650a 2020 2020 2020 2020 6578   True.        ex
+0001f820: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0001f830: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+0001f840: 2072 6169 7365 2063 6c69 636b 2e43 6c69   raise click.Cli
+0001f850: 636b 4578 6365 7074 696f 6e28 4665 6564  ckException(Feed
+0001f860: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
+0001f870: 725f 7570 6461 7469 6e67 5f64 6174 6173  r_updating_datas
+0001f880: 6f75 7263 6528 6461 7461 736f 7572 6365  ource(datasource
+0001f890: 3d64 735f 6e61 6d65 2c20 6572 726f 723d  =ds_name, error=
+0001f8a0: 7374 7228 6529 2929 0a0a 2020 2020 636f  str(e)))..    co
+0001f8b0: 6e6e 6563 746f 725f 6461 7461 203d 204e  nnector_data = N
+0001f8c0: 6f6e 650a 2020 2020 7072 6f6d 6f74 655f  one.    promote_
+0001f8d0: 6572 726f 725f 6d65 7373 6167 6520 3d20  error_message = 
+0001f8e0: 4e6f 6e65 0a0a 2020 2020 6473 5f70 6172  None..    ds_par
+0001f8f0: 616d 7320 3d20 6473 5b22 7061 7261 6d73  ams = ds["params
+0001f900: 225d 0a20 2020 2073 6572 7669 6365 203d  "].    service =
+0001f910: 2064 735f 7061 7261 6d73 2e67 6574 2822   ds_params.get("
+0001f920: 7365 7276 6963 6522 290a 2020 2020 4441  service").    DA
+0001f930: 5441 534f 5552 4345 5f56 414c 4944 5f53  TASOURCE_VALID_S
+0001f940: 4552 5649 4345 535f 544f 5f55 5044 4154  ERVICES_TO_UPDAT
+0001f950: 4520 3d20 5b22 6269 6771 7565 7279 222c  E = ["bigquery",
+0001f960: 2022 736e 6f77 666c 616b 6522 5d0a 2020   "snowflake"].  
+0001f970: 2020 6966 2064 6174 6173 6f75 7263 655f    if datasource_
+0001f980: 6578 6973 7473 2061 6e64 2073 6572 7669  exists and servi
+0001f990: 6365 2061 6e64 2073 6572 7669 6365 2069  ce and service i
+0001f9a0: 6e20 5b2a 4441 5441 534f 5552 4345 5f56  n [*DATASOURCE_V
+0001f9b0: 414c 4944 5f53 4552 5649 4345 535f 544f  ALID_SERVICES_TO
+0001f9c0: 5f55 5044 4154 452c 202a 5052 4556 4945  _UPDATE, *PREVIE
+0001f9d0: 575f 434f 4e4e 4543 544f 525f 5345 5256  W_CONNECTOR_SERV
+0001f9e0: 4943 4553 5d3a 0a20 2020 2020 2020 2063  ICES]:.        c
+0001f9f0: 6f6e 6e65 6374 6f72 5f72 6571 7569 7265  onnector_require
+0001fa00: 645f 7061 7261 6d73 203d 207b 0a20 2020  d_params = {.   
+0001fa10: 2020 2020 2020 2020 2022 6269 6771 7565           "bigque
+0001fa20: 7279 223a 205b 2273 6572 7669 6365 222c  ry": ["service",
+0001fa30: 2022 6372 6f6e 222c 2022 6578 7465 726e   "cron", "extern
+0001fa40: 616c 5f64 6174 615f 736f 7572 6365 225d  al_data_source"]
+0001fa50: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+0001fa60: 6e6f 7766 6c61 6b65 223a 205b 2263 6f6e  nowflake": ["con
+0001fa70: 6e65 6374 6f72 222c 2022 7365 7276 6963  nector", "servic
+0001fa80: 6522 2c20 2263 726f 6e22 2c20 2265 7874  e", "cron", "ext
+0001fa90: 6572 6e61 6c5f 6461 7461 5f73 6f75 7263  ernal_data_sourc
+0001faa0: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
+0001fab0: 2022 7333 223a 205b 2263 6f6e 6e65 6374   "s3": ["connect
+0001fac0: 6f72 222c 2022 7365 7276 6963 6522 2c20  or", "service", 
+0001fad0: 2263 726f 6e22 2c20 2262 7563 6b65 745f  "cron", "bucket_
+0001fae0: 7572 6922 5d2c 0a20 2020 2020 2020 2020  uri"],.         
+0001faf0: 2020 2022 7333 5f69 616d 726f 6c65 223a     "s3_iamrole":
+0001fb00: 205b 2263 6f6e 6e65 6374 6f72 222c 2022   ["connector", "
+0001fb10: 7365 7276 6963 6522 2c20 2263 726f 6e22  service", "cron"
+0001fb20: 2c20 2262 7563 6b65 745f 7572 6922 5d2c  , "bucket_uri"],
+0001fb30: 0a20 2020 2020 2020 2020 2020 2022 6763  .            "gc
+0001fb40: 7322 3a20 5b22 636f 6e6e 6563 746f 7222  s": ["connector"
+0001fb50: 2c20 2273 6572 7669 6365 222c 2022 6372  , "service", "cr
+0001fb60: 6f6e 222c 2022 6275 636b 6574 5f75 7269  on", "bucket_uri
+0001fb70: 225d 2c0a 2020 2020 2020 2020 7d2e 6765  "],.        }.ge
+0001fb80: 7428 7365 7276 6963 652c 205b 5d29 0a0a  t(service, [])..
+0001fb90: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
+0001fba0: 6c6c 286b 6579 2069 6e20 6473 5f70 6172  ll(key in ds_par
+0001fbb0: 616d 7320 666f 7220 6b65 7920 696e 2063  ams for key in c
+0001fbc0: 6f6e 6e65 6374 6f72 5f72 6571 7569 7265  onnector_require
+0001fbd0: 645f 7061 7261 6d73 293a 0a20 2020 2020  d_params):.     
+0001fbe0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0001fbf0: 2020 2020 2020 2063 6f6e 6e65 6374 6f72         connector
+0001fc00: 203d 2064 735f 7061 7261 6d73 2e67 6574   = ds_params.get
+0001fc10: 2822 636f 6e6e 6563 746f 7222 2c20 4e6f  ("connector", No
+0001fc20: 6e65 290a 0a20 2020 2020 2020 2069 6620  ne)..        if 
+0001fc30: 7365 7276 6963 6520 696e 2050 5245 5649  service in PREVI
+0001fc40: 4557 5f43 4f4e 4e45 4354 4f52 5f53 4552  EW_CONNECTOR_SER
+0001fc50: 5649 4345 533a 0a20 2020 2020 2020 2020  VICES:.         
+0001fc60: 2020 2063 6f6e 6e65 6374 6f72 5f69 6420     connector_id 
+0001fc70: 3d20 6578 6973 7469 6e67 5f64 732e 6765  = existing_ds.ge
+0001fc80: 7428 2263 6f6e 6e65 6374 6f72 222c 2022  t("connector", "
+0001fc90: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+0001fca0: 6620 6e6f 7420 636f 6e6e 6563 746f 725f  f not connector_
+0001fcb0: 6964 3a0a 2020 2020 2020 2020 2020 2020  id:.            
+0001fcc0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0001fcd0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+0001fce0: 636f 6e6e 6563 746f 7220 3d20 6177 6169  connector = awai
+0001fcf0: 7420 636c 6965 6e74 2e67 6574 5f63 6f6e  t client.get_con
+0001fd00: 6e65 6374 6f72 5f62 795f 6964 2865 7869  nector_by_id(exi
+0001fd10: 7374 696e 675f 6473 2e67 6574 2822 636f  sting_ds.get("co
+0001fd20: 6e6e 6563 746f 7222 2c20 2222 2929 0a20  nnector", "")). 
+0001fd30: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001fd40: 7420 6375 7272 656e 745f 636f 6e6e 6563  t current_connec
+0001fd50: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+0001fd60: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0001fd70: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
+0001fd80: 656e 745f 636f 6e6e 6563 746f 725b 226e  ent_connector["n
+0001fd90: 616d 6522 5d20 213d 2064 735f 7061 7261  ame"] != ds_para
+0001fda0: 6d73 5b22 636f 6e6e 6563 7469 6f6e 225d  ms["connection"]
+0001fdb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001fdc0: 2020 7061 7261 6d20 3d20 2263 6f6e 6e65    param = "conne
+0001fdd0: 6374 696f 6e22 0a20 2020 2020 2020 2020  ction".         
+0001fde0: 2020 2020 2020 2064 6174 6166 696c 655f         datafile_
+0001fdf0: 7061 7261 6d20 3d20 496d 706f 7274 5265  param = ImportRe
+0001fe00: 706c 6163 656d 656e 7473 2e67 6574 5f64  placements.get_d
+0001fe10: 6174 6166 696c 655f 7061 7261 6d5f 666f  atafile_param_fo
+0001fe20: 725f 6c69 6e6b 6572 5f70 6172 616d 2873  r_linker_param(s
+0001fe30: 6572 7669 6365 2c20 7061 7261 6d29 206f  ervice, param) o
+0001fe40: 7220 7061 7261 6d0a 2020 2020 2020 2020  r param.        
+0001fe50: 2020 2020 2020 2020 7261 6973 6520 636c          raise cl
+0001fe60: 6963 6b2e 436c 6963 6b45 7863 6570 7469  ick.ClickExcepti
+0001fe70: 6f6e 2846 6565 6462 6163 6b4d 616e 6167  on(FeedbackManag
+0001fe80: 6572 2e65 7272 6f72 5f75 7064 6174 696e  er.error_updatin
+0001fe90: 675f 636f 6e6e 6563 746f 725f 6e6f 745f  g_connector_not_
+0001fea0: 7375 7070 6f72 7465 6428 7061 7261 6d3d  supported(param=
+0001feb0: 6461 7461 6669 6c65 5f70 6172 616d 2929  datafile_param))
+0001fec0: 0a0a 2020 2020 2020 2020 2020 2020 6c69  ..            li
+0001fed0: 6e6b 6572 7320 3d20 6375 7272 656e 745f  nkers = current_
+0001fee0: 636f 6e6e 6563 746f 722e 6765 7428 226c  connector.get("l
+0001fef0: 696e 6b65 7273 222c 205b 5d29 0a20 2020  inkers", []).   
+0001ff00: 2020 2020 2020 2020 206c 696e 6b65 7220           linker 
+0001ff10: 3d20 6e65 7874 2828 6c69 6e6b 6572 2066  = next((linker f
+0001ff20: 6f72 206c 696e 6b65 7220 696e 206c 696e  or linker in lin
+0001ff30: 6b65 7273 2069 6620 6c69 6e6b 6572 5b22  kers if linker["
+0001ff40: 6461 7461 736f 7572 6365 5f69 6422 5d20  datasource_id"] 
+0001ff50: 3d3d 2065 7869 7374 696e 675f 6473 5b22  == existing_ds["
+0001ff60: 6964 225d 292c 204e 6f6e 6529 0a20 2020  id"]), None).   
+0001ff70: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0001ff80: 6c69 6e6b 6572 3a0a 2020 2020 2020 2020  linker:.        
+0001ff90: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+0001ffa0: 2020 2020 2020 2020 2020 2020 6c69 6e6b              link
+0001ffb0: 6572 5f73 6574 7469 6e67 7320 3d20 6c69  er_settings = li
+0001ffc0: 6e6b 6572 2e67 6574 2822 7365 7474 696e  nker.get("settin
+0001ffd0: 6773 222c 207b 7d29 0a20 2020 2020 2020  gs", {}).       
+0001ffe0: 2020 2020 2066 6f72 2070 6172 616d 2c20       for param, 
+0001fff0: 7661 6c75 6520 696e 206c 696e 6b65 725f  value in linker_
+00020000: 7365 7474 696e 6773 2e69 7465 6d73 2829  settings.items()
+00020010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020020: 2020 6473 5f70 6172 616d 735f 7661 6c75    ds_params_valu
+00020030: 6520 3d20 6473 5f70 6172 616d 732e 6765  e = ds_params.ge
+00020040: 7428 7061 7261 6d2c 204e 6f6e 6529 0a20  t(param, None). 
+00020050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00020060: 6620 6473 5f70 6172 616d 735f 7661 6c75  f ds_params_valu
+00020070: 6520 616e 6420 6473 5f70 6172 616d 735f  e and ds_params_
+00020080: 7661 6c75 6520 213d 2076 616c 7565 3a0a  value != value:.
+00020090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200a0: 2020 2020 6461 7461 6669 6c65 5f70 6172      datafile_par
+000200b0: 616d 203d 2049 6d70 6f72 7452 6570 6c61  am = ImportRepla
+000200c0: 6365 6d65 6e74 732e 6765 745f 6461 7461  cements.get_data
+000200d0: 6669 6c65 5f70 6172 616d 5f66 6f72 5f6c  file_param_for_l
+000200e0: 696e 6b65 725f 7061 7261 6d28 7365 7276  inker_param(serv
+000200f0: 6963 652c 2070 6172 616d 2920 6f72 2070  ice, param) or p
+00020100: 6172 616d 0a20 2020 2020 2020 2020 2020  aram.           
+00020110: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+00020120: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+00020130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020140: 2020 4665 6564 6261 636b 4d61 6e61 6765    FeedbackManage
+00020150: 722e 6572 726f 725f 7570 6461 7469 6e67  r.error_updating
+00020160: 5f63 6f6e 6e65 6374 6f72 5f6e 6f74 5f73  _connector_not_s
+00020170: 7570 706f 7274 6564 2870 6172 616d 3d64  upported(param=d
+00020180: 6174 6166 696c 655f 7061 7261 6d2e 7570  atafile_param.up
+00020190: 7065 7228 2929 0a20 2020 2020 2020 2020  per()).         
+000201a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000201b0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000201c0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+000201d0: 6f72 5f64 6174 6120 3d20 7b0a 2020 2020  or_data = {.    
+000201e0: 2020 2020 2020 2020 2263 6f6e 6e65 6374          "connect
+000201f0: 6f72 223a 2063 6f6e 6e65 6374 6f72 2c0a  or": connector,.
+00020200: 2020 2020 2020 2020 2020 2020 2273 6572              "ser
+00020210: 7669 6365 223a 2073 6572 7669 6365 2c0a  vice": service,.
+00020220: 2020 2020 2020 2020 2020 2020 2263 726f              "cro
+00020230: 6e22 3a20 6473 5f70 6172 616d 732e 6765  n": ds_params.ge
+00020240: 7428 2263 726f 6e22 2c20 4e6f 6e65 292c  t("cron", None),
+00020250: 0a20 2020 2020 2020 2020 2020 2022 6578  .            "ex
+00020260: 7465 726e 616c 5f64 6174 615f 736f 7572  ternal_data_sour
+00020270: 6365 223a 2064 735f 7061 7261 6d73 2e67  ce": ds_params.g
+00020280: 6574 2822 6578 7465 726e 616c 5f64 6174  et("external_dat
+00020290: 615f 736f 7572 6365 222c 204e 6f6e 6529  a_source", None)
+000202a0: 2c0a 2020 2020 2020 2020 2020 2020 2262  ,.            "b
+000202b0: 7563 6b65 745f 7572 6922 3a20 6473 5f70  ucket_uri": ds_p
+000202c0: 6172 616d 732e 6765 7428 2262 7563 6b65  arams.get("bucke
+000202d0: 745f 7572 6922 2c20 4e6f 6e65 292c 0a20  t_uri", None),. 
+000202e0: 2020 2020 2020 2020 2020 2022 6d6f 6465             "mode
+000202f0: 223a 2064 735f 7061 7261 6d73 2e67 6574  ": ds_params.get
+00020300: 2822 6d6f 6465 222c 2022 7265 706c 6163  ("mode", "replac
+00020310: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
+00020320: 2022 7175 6572 7922 3a20 6473 5f70 6172   "query": ds_par
+00020330: 616d 732e 6765 7428 2271 7565 7279 222c  ams.get("query",
+00020340: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
+00020350: 2020 2020 2269 6e67 6573 745f 6e6f 7722      "ingest_now"
+00020360: 3a20 6473 5f70 6172 616d 732e 6765 7428  : ds_params.get(
+00020370: 2269 6e67 6573 745f 6e6f 7722 2c20 4661  "ingest_now", Fa
+00020380: 6c73 6529 2c0a 2020 2020 2020 2020 7d0a  lse),.        }.
+00020390: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+000203a0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+000203b0: 636c 6965 6e74 2e75 7064 6174 655f 6461  client.update_da
+000203c0: 7461 736f 7572 6365 2864 735f 6e61 6d65  tasource(ds_name
+000203d0: 2c20 636f 6e6e 6563 746f 725f 6461 7461  , connector_data
+000203e0: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
+000203f0: 6963 6b2e 6563 686f 2846 6565 6462 6163  ick.echo(Feedbac
+00020400: 6b4d 616e 6167 6572 2e73 7563 6365 7373  kManager.success
+00020410: 5f70 726f 6d6f 7469 6e67 5f64 6174 6173  _promoting_datas
+00020420: 6f75 7263 6528 6461 7461 736f 7572 6365  ource(datasource
+00020430: 3d64 735f 6e61 6d65 2929 0a20 2020 2020  =ds_name)).     
+00020440: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00020450: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00020460: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+00020470: 2020 2020 2020 2020 2070 726f 6d6f 7465           promote
+00020480: 5f65 7272 6f72 5f6d 6573 7361 6765 203d  _error_message =
+00020490: 2073 7472 2865 290a 0a20 2020 2069 6620   str(e)..    if 
+000204a0: 616c 7465 725f 7265 7370 6f6e 7365 2061  alter_response a
+000204b0: 6e64 206d 616b 655f 6368 616e 6765 733a  nd make_changes:
+000204c0: 0a20 2020 2020 2020 2023 2061 6c74 6572  .        # alter
+000204d0: 206f 7065 7261 7469 6f6e 2066 696e 6973   operation finis
+000204e0: 6865 640a 2020 2020 2020 2020 7265 7475  hed.        retu
+000204f0: 726e 0a20 2020 2023 2072 656d 6f76 6564  rn.    # removed
+00020500: 2072 6570 6c61 6369 6e67 2062 7920 6465   replacing by de
+00020510: 6661 756c 742e 2057 6865 6e20 6120 6461  fault. When a da
+00020520: 7461 736f 7572 6365 2069 7320 7265 6d6f  tasource is remo
+00020530: 7665 6420 6461 7461 2069 730a 2020 2020  ved data is.    
+00020540: 2320 7265 6d6f 7665 6420 616e 6420 616c  # removed and al
+00020550: 6c20 7468 6520 7265 6665 7265 6e63 6573  l the references
+00020560: 206e 6565 6473 2074 6f20 6265 2075 7064   needs to be upd
+00020570: 6174 6564 0a20 2020 2069 6620 280a 2020  ated.    if (.  
+00020580: 2020 2020 2020 6f73 2e67 6574 656e 7628        os.getenv(
+00020590: 2254 425f 495f 4b4e 4f57 5f57 4841 545f  "TB_I_KNOW_WHAT_
+000205a0: 495f 414d 5f44 4f49 4e47 2229 0a20 2020  I_AM_DOING").   
+000205b0: 2020 2020 2061 6e64 2063 6c69 636b 2e70       and click.p
+000205c0: 726f 6d70 7428 4665 6564 6261 636b 4d61  rompt(FeedbackMa
+000205d0: 6e61 6765 722e 696e 666f 5f61 736b 5f66  nager.info_ask_f
+000205e0: 6f72 5f64 6174 6173 6f75 7263 655f 636f  or_datasource_co
+000205f0: 6e66 6972 6d61 7469 6f6e 2829 2920 3d3d  nfirmation()) ==
+00020600: 2064 735f 6e61 6d65 0a20 2020 2029 3a20   ds_name.    ): 
+00020610: 2023 2054 4f44 4f20 6d6f 7665 2074 6f20   # TODO move to 
+00020620: 434c 490a 2020 2020 2020 2020 7472 793a  CLI.        try:
+00020630: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+00020640: 6974 2063 6c69 656e 742e 6461 7461 736f  it client.dataso
+00020650: 7572 6365 5f64 656c 6574 6528 6473 5f6e  urce_delete(ds_n
+00020660: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00020670: 2063 6c69 636b 2e65 6368 6f28 4665 6564   click.echo(Feed
+00020680: 6261 636b 4d61 6e61 6765 722e 7375 6363  backManager.succ
+00020690: 6573 735f 6465 6c65 7465 5f64 6174 6173  ess_delete_datas
+000206a0: 6f75 7263 6528 6461 7461 736f 7572 6365  ource(datasource
+000206b0: 3d64 735f 6e61 6d65 2929 0a20 2020 2020  =ds_name)).     
+000206c0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+000206d0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+000206e0: 2072 6169 7365 2063 6c69 636b 2e43 6c69   raise click.Cli
+000206f0: 636b 4578 6365 7074 696f 6e28 4665 6564  ckException(Feed
+00020700: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
+00020710: 725f 7265 6d6f 7669 6e67 5f64 6174 6173  r_removing_datas
+00020720: 6f75 7263 6528 6461 7461 736f 7572 6365  ource(datasource
+00020730: 3d64 735f 6e61 6d65 2929 0a20 2020 2020  =ds_name)).     
+00020740: 2020 2072 6574 7572 6e0a 2020 2020 656c     return.    el
+00020750: 7365 3a0a 2020 2020 2020 2020 6966 2061  se:.        if a
+00020760: 6c74 6572 5f65 7272 6f72 5f6d 6573 7361  lter_error_messa
+00020770: 6765 3a0a 2020 2020 2020 2020 2020 2020  ge:.            
+00020780: 7261 6973 6520 636c 6963 6b2e 436c 6963  raise click.Clic
+00020790: 6b45 7863 6570 7469 6f6e 280a 2020 2020  kException(.    
+000207a0: 2020 2020 2020 2020 2020 2020 4665 6564              Feed
+000207b0: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
+000207c0: 725f 6461 7461 736f 7572 6365 5f61 6c72  r_datasource_alr
+000207d0: 6561 6479 5f65 7869 7374 735f 616e 645f  eady_exists_and_
+000207e0: 616c 7465 725f 6661 696c 6564 280a 2020  alter_failed(.  
+000207f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020800: 2020 6461 7461 736f 7572 6365 3d64 735f    datasource=ds_
+00020810: 6e61 6d65 2c20 616c 7465 725f 6572 726f  name, alter_erro
+00020820: 725f 6d65 7373 6167 653d 616c 7465 725f  r_message=alter_
+00020830: 6572 726f 725f 6d65 7373 6167 650a 2020  error_message.  
+00020840: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00020850: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00020860: 2020 2020 2020 6966 2070 726f 6d6f 7465        if promote
+00020870: 5f65 7272 6f72 5f6d 6573 7361 6765 3a0a  _error_message:.
+00020880: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00020890: 6520 636c 6963 6b2e 436c 6963 6b45 7863  e click.ClickExc
+000208a0: 6570 7469 6f6e 280a 2020 2020 2020 2020  eption(.        
+000208b0: 2020 2020 2020 2020 4665 6564 6261 636b          Feedback
+000208c0: 4d61 6e61 6765 722e 6572 726f 725f 7072  Manager.error_pr
+000208d0: 6f6d 6f74 696e 675f 6461 7461 736f 7572  omoting_datasour
+000208e0: 6365 2864 6174 6173 6f75 7263 653d 6473  ce(datasource=ds
+000208f0: 5f6e 616d 652c 2065 7272 6f72 3d70 726f  _name, error=pro
+00020900: 6d6f 7465 5f65 7272 6f72 5f6d 6573 7361  mote_error_messa
+00020910: 6765 290a 2020 2020 2020 2020 2020 2020  ge).            
+00020920: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00020930: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+00020940: 6b2e 6563 686f 2846 6565 6462 6163 6b4d  k.echo(FeedbackM
+00020950: 616e 6167 6572 2e77 6172 6e69 6e67 5f64  anager.warning_d
+00020960: 6174 6173 6f75 7263 655f 616c 7265 6164  atasource_alread
+00020970: 795f 6578 6973 7473 2864 6174 6173 6f75  y_exists(datasou
+00020980: 7263 653d 6473 5f6e 616d 6529 290a 0a0a  rce=ds_name))...
+00020990: 6173 796e 6320 6465 6620 6e65 775f 746f  async def new_to
+000209a0: 6b65 6e28 746f 6b65 6e3a 2044 6963 745b  ken(token: Dict[
+000209b0: 7374 722c 2041 6e79 5d2c 2063 6c69 656e  str, Any], clien
+000209c0: 743a 2054 696e 7942 2c20 666f 7263 653a  t: TinyB, force:
+000209d0: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0a   bool = False):.
+000209e0: 2020 2020 6578 6973 7469 6e67 5f74 6f6b      existing_tok
+000209f0: 656e 203d 204e 6f6e 650a 2020 2020 7472  en = None.    tr
+00020a00: 793a 0a20 2020 2020 2020 2065 7869 7374  y:.        exist
+00020a10: 696e 675f 746f 6b65 6e20 3d20 6177 6169  ing_token = awai
+00020a20: 7420 636c 6965 6e74 2e74 6f6b 656e 5f67  t client.token_g
+00020a30: 6574 2874 6f6b 656e 5b22 6e61 6d65 225d  et(token["name"]
+00020a40: 290a 2020 2020 6578 6365 7074 2045 7863  ).    except Exc
+00020a50: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+00020a60: 7061 7373 0a0a 2020 2020 6966 206e 6f74  pass..    if not
+00020a70: 2065 7869 7374 696e 675f 746f 6b65 6e3a   existing_token:
+00020a80: 0a20 2020 2020 2020 2061 7761 6974 2063  .        await c
+00020a90: 6c69 656e 742e 746f 6b65 6e5f 6372 6561  lient.token_crea
+00020aa0: 7465 2874 6f6b 656e 290a 2020 2020 2020  te(token).      
+00020ab0: 2020 7265 7475 726e 0a0a 2020 2020 6966    return..    if
+00020ac0: 2066 6f72 6365 3a0a 2020 2020 2020 2020   force:.        
+00020ad0: 4144 4d49 4e5f 5343 4f50 4553 203d 205b  ADMIN_SCOPES = [
+00020ae0: 2241 444d 494e 222c 2022 4144 4d49 4e5f  "ADMIN", "ADMIN_
+00020af0: 5553 4552 225d 0a20 2020 2020 2020 2069  USER"].        i
+00020b00: 6620 616e 7928 5b73 636f 7065 5b22 7479  f any([scope["ty
+00020b10: 7065 225d 2069 6e20 4144 4d49 4e5f 5343  pe"] in ADMIN_SC
+00020b20: 4f50 4553 2066 6f72 2073 636f 7065 2069  OPES for scope i
+00020b30: 6e20 6578 6973 7469 6e67 5f74 6f6b 656e  n existing_token
+00020b40: 5b22 7363 6f70 6573 225d 5d29 3a0a 2020  ["scopes"]]):.  
+00020b50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00020b60: 636c 6963 6b2e 436c 6963 6b45 7863 6570  click.ClickExcep
+00020b70: 7469 6f6e 2846 6565 6462 6163 6b4d 616e  tion(FeedbackMan
+00020b80: 6167 6572 2e65 7272 6f72 5f74 6f6b 656e  ager.error_token
+00020b90: 5f63 616e 6e6f 745f 6265 5f6f 7665 7272  _cannot_be_overr
+00020ba0: 6964 656e 2874 6f6b 656e 3d74 6f6b 656e  iden(token=token
+00020bb0: 5b22 6e61 6d65 225d 2929 0a0a 2020 2020  ["name"]))..    
+00020bc0: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
+00020bd0: 2e74 6f6b 656e 5f75 7064 6174 6528 746f  .token_update(to
+00020be0: 6b65 6e29 0a20 2020 2020 2020 2072 6574  ken).        ret
+00020bf0: 7572 6e0a 0a20 2020 2072 6169 7365 2063  urn..    raise c
+00020c00: 6c69 636b 2e43 6c69 636b 4578 6365 7074  lick.ClickExcept
+00020c10: 696f 6e28 4665 6564 6261 636b 4d61 6e61  ion(FeedbackMana
+00020c20: 6765 722e 6572 726f 725f 746f 6b65 6e5f  ger.error_token_
+00020c30: 616c 7265 6164 795f 6578 6973 7473 2874  already_exists(t
+00020c40: 6f6b 656e 3d74 6f6b 656e 5b22 6e61 6d65  oken=token["name
+00020c50: 225d 2929 0a0a 0a61 7379 6e63 2064 6566  "]))...async def
+00020c60: 2065 7865 635f 6669 6c65 280a 2020 2020   exec_file(.    
+00020c70: 636f 6e66 6967 3a20 4f70 7469 6f6e 616c  config: Optional
+00020c80: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00020c90: 2c0a 2020 2020 723a 2044 6963 745b 7374  ,.    r: Dict[st
+00020ca0: 722c 2041 6e79 5d2c 0a20 2020 2074 625f  r, Any],.    tb_
+00020cb0: 636c 6965 6e74 3a20 5469 6e79 422c 0a20  client: TinyB,. 
+00020cc0: 2020 2066 6f72 6365 3a20 626f 6f6c 2c0a     force: bool,.
+00020cd0: 2020 2020 6368 6563 6b3a 2062 6f6f 6c2c      check: bool,
+00020ce0: 0a20 2020 2064 6562 7567 3a20 626f 6f6c  .    debug: bool
+00020cf0: 2c0a 2020 2020 706f 7075 6c61 7465 3a20  ,.    populate: 
+00020d00: 626f 6f6c 2c0a 2020 2020 706f 7075 6c61  bool,.    popula
+00020d10: 7465 5f73 7562 7365 742c 0a20 2020 2070  te_subset,.    p
+00020d20: 6f70 756c 6174 655f 636f 6e64 6974 696f  opulate_conditio
+00020d30: 6e2c 0a20 2020 2075 6e6c 696e 6b5f 6f6e  n,.    unlink_on
+00020d40: 5f70 6f70 756c 6174 655f 6572 726f 722c  _populate_error,
+00020d50: 0a20 2020 2077 6169 745f 706f 7075 6c61  .    wait_popula
+00020d60: 7465 2c0a 2020 2020 7573 6572 5f74 6f6b  te,.    user_tok
+00020d70: 656e 3a20 4f70 7469 6f6e 616c 5b73 7472  en: Optional[str
+00020d80: 5d2c 0a20 2020 206f 7665 7272 6964 655f  ],.    override_
+00020d90: 6461 7461 736f 7572 6365 3a20 626f 6f6c  datasource: bool
+00020da0: 203d 2046 616c 7365 2c0a 2020 2020 6967   = False,.    ig
+00020db0: 6e6f 7265 5f73 716c 5f65 7272 6f72 733a  nore_sql_errors:
+00020dc0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00020dd0: 2020 2073 6b69 705f 636f 6e66 6972 6d61     skip_confirma
+00020de0: 7469 6f6e 3a20 626f 6f6c 203d 2046 616c  tion: bool = Fal
+00020df0: 7365 2c0a 2020 2020 6f6e 6c79 5f72 6573  se,.    only_res
+00020e00: 706f 6e73 655f 7469 6d65 733a 2062 6f6f  ponse_times: boo
+00020e10: 6c20 3d20 4661 6c73 652c 0a20 2020 2074  l = False,.    t
+00020e20: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
+00020e30: 2072 756e 5f74 6573 7473 3d46 616c 7365   run_tests=False
+00020e40: 2c0a 2020 2020 6173 5f73 7461 6e64 6172  ,.    as_standar
+00020e50: 643d 4661 6c73 652c 0a20 2020 2074 6573  d=False,.    tes
+00020e60: 7473 5f74 6f5f 7275 6e3a 2069 6e74 203d  ts_to_run: int =
+00020e70: 2030 2c0a 2020 2020 7465 7374 735f 746f   0,.    tests_to
+00020e80: 5f73 616d 706c 655f 6279 5f70 6172 616d  _sample_by_param
+00020e90: 733a 2069 6e74 203d 2030 2c0a 2020 2020  s: int = 0,.    
+00020ea0: 7465 7374 735f 6669 6c74 6572 5f62 793a  tests_filter_by:
+00020eb0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00020ec0: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+00020ed0: 2074 6573 7473 5f66 6169 6c66 6173 743a   tests_failfast:
+00020ee0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00020ef0: 2020 2074 6573 7473 5f69 676e 6f72 655f     tests_ignore_
+00020f00: 6f72 6465 723a 2062 6f6f 6c20 3d20 4661  order: bool = Fa
+00020f10: 6c73 652c 0a20 2020 2074 6573 7473 5f76  lse,.    tests_v
+00020f20: 616c 6964 6174 655f 7072 6f63 6573 7365  alidate_processe
+00020f30: 645f 6279 7465 733a 2062 6f6f 6c20 3d20  d_bytes: bool = 
+00020f40: 4661 6c73 652c 0a20 2020 2074 6573 7473  False,.    tests
+00020f50: 5f63 6865 636b 5f72 6571 7565 7374 735f  _check_requests_
+00020f60: 6672 6f6d 5f62 7261 6e63 683a 2062 6f6f  from_branch: boo
+00020f70: 6c20 3d20 4661 6c73 652c 0a20 2020 2063  l = False,.    c
+00020f80: 7572 7265 6e74 5f77 733a 204f 7074 696f  urrent_ws: Optio
+00020f90: 6e61 6c5b 4469 6374 5b73 7472 2c20 416e  nal[Dict[str, An
+00020fa0: 795d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  y]] = None,.    
+00020fb0: 666f 726b 5f64 6f77 6e73 7472 6561 6d3a  fork_downstream:
+00020fc0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00020fd0: 3d20 4661 6c73 652c 0a20 2020 2066 6f72  = False,.    for
+00020fe0: 6b3a 204f 7074 696f 6e61 6c5b 626f 6f6c  k: Optional[bool
+00020ff0: 5d20 3d20 4661 6c73 652c 0a20 2020 2067  ] = False,.    g
+00021000: 6974 5f72 656c 6561 7365 3a20 4f70 7469  it_release: Opti
+00021010: 6f6e 616c 5b62 6f6f 6c5d 203d 2046 616c  onal[bool] = Fal
+00021020: 7365 2c0a 293a 0a20 2020 2069 6620 6465  se,.):.    if de
+00021030: 6275 673a 0a20 2020 2020 2020 2063 6c69  bug:.        cli
+00021040: 636b 2e65 6368 6f28 4665 6564 6261 636b  ck.echo(Feedback
+00021050: 4d61 6e61 6765 722e 6465 6275 675f 7275  Manager.debug_ru
+00021060: 6e6e 696e 675f 6669 6c65 2866 696c 653d  nning_file(file=
+00021070: 7070 2e70 666f 726d 6174 2872 2929 290a  pp.pformat(r))).
+00021080: 2020 2020 6966 2072 5b22 7265 736f 7572      if r["resour
+00021090: 6365 225d 203d 3d20 2270 6970 6573 223a  ce"] == "pipes":
+000210a0: 0a20 2020 2020 2020 2061 7761 6974 206e  .        await n
+000210b0: 6577 5f70 6970 6528 0a20 2020 2020 2020  ew_pipe(.       
+000210c0: 2020 2020 2072 2c0a 2020 2020 2020 2020       r,.        
+000210d0: 2020 2020 7462 5f63 6c69 656e 742c 0a20      tb_client,. 
+000210e0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+000210f0: 2c0a 2020 2020 2020 2020 2020 2020 6368  ,.            ch
+00021100: 6563 6b2c 0a20 2020 2020 2020 2020 2020  eck,.           
+00021110: 2070 6f70 756c 6174 652c 0a20 2020 2020   populate,.     
+00021120: 2020 2020 2020 2070 6f70 756c 6174 655f         populate_
+00021130: 7375 6273 6574 2c0a 2020 2020 2020 2020  subset,.        
+00021140: 2020 2020 706f 7075 6c61 7465 5f63 6f6e      populate_con
+00021150: 6469 7469 6f6e 2c0a 2020 2020 2020 2020  dition,.        
+00021160: 2020 2020 756e 6c69 6e6b 5f6f 6e5f 706f      unlink_on_po
+00021170: 7075 6c61 7465 5f65 7272 6f72 2c0a 2020  pulate_error,.  
+00021180: 2020 2020 2020 2020 2020 7761 6974 5f70            wait_p
+00021190: 6f70 756c 6174 652c 0a20 2020 2020 2020  opulate,.       
+000211a0: 2020 2020 2069 676e 6f72 655f 7371 6c5f       ignore_sql_
+000211b0: 6572 726f 7273 3d69 676e 6f72 655f 7371  errors=ignore_sq
+000211c0: 6c5f 6572 726f 7273 2c0a 2020 2020 2020  l_errors,.      
+000211d0: 2020 2020 2020 6f6e 6c79 5f72 6573 706f        only_respo
+000211e0: 6e73 655f 7469 6d65 733d 6f6e 6c79 5f72  nse_times=only_r
+000211f0: 6573 706f 6e73 655f 7469 6d65 732c 0a20  esponse_times,. 
+00021200: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+00021210: 7574 3d74 696d 656f 7574 2c0a 2020 2020  ut=timeout,.    
+00021220: 2020 2020 2020 2020 7275 6e5f 7465 7374          run_test
+00021230: 733d 7275 6e5f 7465 7374 732c 0a20 2020  s=run_tests,.   
+00021240: 2020 2020 2020 2020 2061 735f 7374 616e           as_stan
+00021250: 6461 7264 3d61 735f 7374 616e 6461 7264  dard=as_standard
+00021260: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
+00021270: 7374 735f 746f 5f72 756e 3d74 6573 7473  sts_to_run=tests
+00021280: 5f74 6f5f 7275 6e2c 0a20 2020 2020 2020  _to_run,.       
+00021290: 2020 2020 2074 6573 7473 5f74 6f5f 7361       tests_to_sa
+000212a0: 6d70 6c65 5f62 795f 7061 7261 6d73 3d74  mple_by_params=t
+000212b0: 6573 7473 5f74 6f5f 7361 6d70 6c65 5f62  ests_to_sample_b
+000212c0: 795f 7061 7261 6d73 2c0a 2020 2020 2020  y_params,.      
+000212d0: 2020 2020 2020 7465 7374 735f 6669 6c74        tests_filt
+000212e0: 6572 5f62 793d 7465 7374 735f 6669 6c74  er_by=tests_filt
+000212f0: 6572 5f62 792c 0a20 2020 2020 2020 2020  er_by,.         
+00021300: 2020 2074 6573 7473 5f66 6169 6c66 6173     tests_failfas
+00021310: 743d 7465 7374 735f 6661 696c 6661 7374  t=tests_failfast
+00021320: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
+00021330: 7374 735f 6967 6e6f 7265 5f6f 7264 6572  sts_ignore_order
+00021340: 3d74 6573 7473 5f69 676e 6f72 655f 6f72  =tests_ignore_or
+00021350: 6465 722c 0a20 2020 2020 2020 2020 2020  der,.           
+00021360: 2074 6573 7473 5f76 616c 6964 6174 655f   tests_validate_
+00021370: 7072 6f63 6573 7365 645f 6279 7465 733d  processed_bytes=
+00021380: 7465 7374 735f 7661 6c69 6461 7465 5f70  tests_validate_p
+00021390: 726f 6365 7373 6564 5f62 7974 6573 2c0a  rocessed_bytes,.
+000213a0: 2020 2020 2020 2020 2020 2020 6f76 6572              over
+000213b0: 7269 6465 5f64 6174 6173 6f75 7263 653d  ride_datasource=
+000213c0: 6f76 6572 7269 6465 5f64 6174 6173 6f75  override_datasou
+000213d0: 7263 652c 0a20 2020 2020 2020 2020 2020  rce,.           
+000213e0: 2074 6573 7473 5f63 6865 636b 5f72 6571   tests_check_req
+000213f0: 7565 7374 735f 6672 6f6d 5f62 7261 6e63  uests_from_branc
+00021400: 683d 7465 7374 735f 6368 6563 6b5f 7265  h=tests_check_re
+00021410: 7175 6573 7473 5f66 726f 6d5f 6272 616e  quests_from_bran
+00021420: 6368 2c0a 2020 2020 2020 2020 2020 2020  ch,.            
+00021430: 666f 726b 5f64 6f77 6e73 7472 6561 6d3d  fork_downstream=
+00021440: 666f 726b 5f64 6f77 6e73 7472 6561 6d2c  fork_downstream,
+00021450: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00021460: 6b3d 666f 726b 2c0a 2020 2020 2020 2020  k=fork,.        
+00021470: 290a 2020 2020 656c 6966 2072 5b22 7265  ).    elif r["re
+00021480: 736f 7572 6365 225d 203d 3d20 2264 6174  source"] == "dat
+00021490: 6173 6f75 7263 6573 223a 0a20 2020 2020  asources":.     
+000214a0: 2020 2061 7761 6974 206e 6577 5f64 7328     await new_ds(
+000214b0: 0a20 2020 2020 2020 2020 2020 2072 2c0a  .            r,.
+000214c0: 2020 2020 2020 2020 2020 2020 7462 5f63              tb_c
+000214d0: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
+000214e0: 2020 2075 7365 725f 746f 6b65 6e2c 0a20     user_token,. 
+000214f0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+00021500: 2c0a 2020 2020 2020 2020 2020 2020 736b  ,.            sk
+00021510: 6970 5f63 6f6e 6669 726d 6174 696f 6e3d  ip_confirmation=
+00021520: 736b 6970 5f63 6f6e 6669 726d 6174 696f  skip_confirmatio
+00021530: 6e2c 0a20 2020 2020 2020 2020 2020 2063  n,.            c
+00021540: 7572 7265 6e74 5f77 733d 6375 7272 656e  urrent_ws=curren
+00021550: 745f 7773 2c0a 2020 2020 2020 2020 2020  t_ws,.          
+00021560: 2020 666f 726b 5f64 6f77 6e73 7472 6561    fork_downstrea
+00021570: 6d3d 666f 726b 5f64 6f77 6e73 7472 6561  m=fork_downstrea
+00021580: 6d2c 0a20 2020 2020 2020 2020 2020 2066  m,.            f
+00021590: 6f72 6b3d 666f 726b 2c0a 2020 2020 2020  ork=fork,.      
+000215a0: 2020 2020 2020 6769 745f 7265 6c65 6173        git_releas
+000215b0: 653d 6769 745f 7265 6c65 6173 652c 0a20  e=git_release,. 
+000215c0: 2020 2020 2020 2029 0a20 2020 2065 6c69         ).    eli
+000215d0: 6620 725b 2272 6573 6f75 7263 6522 5d20  f r["resource"] 
+000215e0: 3d3d 2022 746f 6b65 6e73 223a 0a20 2020  == "tokens":.   
+000215f0: 2020 2020 2061 7761 6974 206e 6577 5f74       await new_t
+00021600: 6f6b 656e 2872 2c20 7462 5f63 6c69 656e  oken(r, tb_clien
+00021610: 742c 2066 6f72 6365 290a 2020 2020 656c  t, force).    el
+00021620: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
+00021630: 6520 636c 6963 6b2e 436c 6963 6b45 7863  e click.ClickExc
+00021640: 6570 7469 6f6e 2846 6565 6462 6163 6b4d  eption(FeedbackM
+00021650: 616e 6167 6572 2e65 7272 6f72 5f75 6e6b  anager.error_unk
+00021660: 6e6f 776e 5f72 6573 6f75 7263 6528 7265  nown_resource(re
+00021670: 736f 7572 6365 3d72 5b22 7265 736f 7572  source=r["resour
+00021680: 6365 225d 2929 0a0a 0a64 6566 2067 6574  ce"]))...def get
+00021690: 5f6e 616d 655f 7665 7273 696f 6e28 6473  _name_version(ds
+000216a0: 3a20 7374 7229 202d 3e20 4469 6374 5b73  : str) -> Dict[s
+000216b0: 7472 2c20 416e 795d 3a0a 2020 2020 2222  tr, Any]:.    ""
+000216c0: 220a 2020 2020 4769 7665 6e20 6120 6e61  ".    Given a na
+000216d0: 6d65 206c 696b 6520 226e 616d 655f 5f64  me like "name__d
+000216e0: 6576 5f5f 7630 2220 7265 7475 726e 7320  ev__v0" returns 
+000216f0: 5b27 6e61 6d65 272c 2027 6465 7627 2c20  ['name', 'dev', 
+00021700: 2776 3027 5d0a 2020 2020 3e3e 3e20 6765  'v0'].    >>> ge
+00021710: 745f 6e61 6d65 5f76 6572 7369 6f6e 2827  t_name_version('
+00021720: 6465 765f 5f6e 616d 655f 5f76 3027 290a  dev__name__v0').
+00021730: 2020 2020 7b27 6e61 6d65 273a 2027 6465      {'name': 'de
+00021740: 765f 5f6e 616d 6527 2c20 2776 6572 7369  v__name', 'versi
+00021750: 6f6e 273a 2030 7d0a 2020 2020 3e3e 3e20  on': 0}.    >>> 
+00021760: 6765 745f 6e61 6d65 5f76 6572 7369 6f6e  get_name_version
+00021770: 2827 6e61 6d65 5f5f 7630 2729 0a20 2020  ('name__v0').   
+00021780: 207b 276e 616d 6527 3a20 276e 616d 6527   {'name': 'name'
+00021790: 2c20 2776 6572 7369 6f6e 273a 2030 7d0a  , 'version': 0}.
+000217a0: 2020 2020 3e3e 3e20 6765 745f 6e61 6d65      >>> get_name
+000217b0: 5f76 6572 7369 6f6e 2827 6465 765f 5f6e  _version('dev__n
+000217c0: 616d 6527 290a 2020 2020 7b27 6e61 6d65  ame').    {'name
+000217d0: 273a 2027 6465 765f 5f6e 616d 6527 2c20  ': 'dev__name', 
+000217e0: 2776 6572 7369 6f6e 273a 204e 6f6e 657d  'version': None}
+000217f0: 0a20 2020 203e 3e3e 2067 6574 5f6e 616d  .    >>> get_nam
+00021800: 655f 7665 7273 696f 6e28 276e 616d 6527  e_version('name'
+00021810: 290a 2020 2020 7b27 6e61 6d65 273a 2027  ).    {'name': '
+00021820: 6e61 6d65 272c 2027 7665 7273 696f 6e27  name', 'version'
+00021830: 3a20 4e6f 6e65 7d0a 2020 2020 3e3e 3e20  : None}.    >>> 
+00021840: 6765 745f 6e61 6d65 5f76 6572 7369 6f6e  get_name_version
+00021850: 2827 686f 7261 7269 6f5f 5f33 5f5f 7069  ('horario__3__pi
+00021860: 7065 2729 0a20 2020 207b 276e 616d 6527  pe').    {'name'
+00021870: 3a20 2768 6f72 6172 696f 5f5f 335f 5f70  : 'horario__3__p
+00021880: 6970 6527 2c20 2776 6572 7369 6f6e 273a  ipe', 'version':
+00021890: 204e 6f6e 657d 0a20 2020 203e 3e3e 2067   None}.    >>> g
+000218a0: 6574 5f6e 616d 655f 7665 7273 696f 6e28  et_name_version(
+000218b0: 2768 6f72 6172 696f 5f5f 6368 6563 6b65  'horario__checke
+000218c0: 7227 290a 2020 2020 7b27 6e61 6d65 273a  r').    {'name':
+000218d0: 2027 686f 7261 7269 6f5f 5f63 6865 636b   'horario__check
+000218e0: 6572 272c 2027 7665 7273 696f 6e27 3a20  er', 'version': 
+000218f0: 4e6f 6e65 7d0a 2020 2020 3e3e 3e20 6765  None}.    >>> ge
+00021900: 745f 6e61 6d65 5f76 6572 7369 6f6e 2827  t_name_version('
+00021910: 6465 765f 5f68 6f72 6172 696f 5f5f 6368  dev__horario__ch
+00021920: 6563 6b65 7227 290a 2020 2020 7b27 6e61  ecker').    {'na
+00021930: 6d65 273a 2027 6465 765f 5f68 6f72 6172  me': 'dev__horar
+00021940: 696f 5f5f 6368 6563 6b65 7227 2c20 2776  io__checker', 'v
+00021950: 6572 7369 6f6e 273a 204e 6f6e 657d 0a20  ersion': None}. 
+00021960: 2020 203e 3e3e 2067 6574 5f6e 616d 655f     >>> get_name_
+00021970: 7665 7273 696f 6e28 2774 675f 5f64 4163  version('tg__dAc
+00021980: 7469 7669 6461 6465 735f 5f76 305f 7069  tividades__v0_pi
+00021990: 7065 5f33 3930 3727 290a 2020 2020 7b27  pe_3907').    {'
+000219a0: 6e61 6d65 273a 2027 7467 5f5f 6441 6374  name': 'tg__dAct
+000219b0: 6976 6964 6164 6573 272c 2027 7665 7273  ividades', 'vers
+000219c0: 696f 6e27 3a20 307d 0a20 2020 203e 3e3e  ion': 0}.    >>>
+000219d0: 2067 6574 5f6e 616d 655f 7665 7273 696f   get_name_versio
+000219e0: 6e28 2774 675f 5f64 4163 7469 7669 6461  n('tg__dActivida
+000219f0: 6465 735f 5f76 615f 7069 7065 5f33 3930  des__va_pipe_390
+00021a00: 3727 290a 2020 2020 7b27 6e61 6d65 273a  7').    {'name':
+00021a10: 2027 7467 5f5f 6441 6374 6976 6964 6164   'tg__dActividad
+00021a20: 6573 5f5f 7661 5f70 6970 655f 3339 3037  es__va_pipe_3907
+00021a30: 272c 2027 7665 7273 696f 6e27 3a20 4e6f  ', 'version': No
+00021a40: 6e65 7d0a 2020 2020 3e3e 3e20 6765 745f  ne}.    >>> get_
+00021a50: 6e61 6d65 5f76 6572 7369 6f6e 2827 7467  name_version('tg
+00021a60: 5f5f 6f72 6967 696e 5f77 6f72 6b73 7061  __origin_workspa
+00021a70: 6365 2e73 6861 7265 645f 6473 5f5f 7633  ce.shared_ds__v3
+00021a80: 3930 3727 290a 2020 2020 7b27 6e61 6d65  907').    {'name
+00021a90: 273a 2027 7467 5f5f 6f72 6967 696e 5f77  ': 'tg__origin_w
+00021aa0: 6f72 6b73 7061 6365 2e73 6861 7265 645f  orkspace.shared_
+00021ab0: 6473 272c 2027 7665 7273 696f 6e27 3a20  ds', 'version': 
+00021ac0: 3339 3037 7d0a 2020 2020 3e3e 3e20 6765  3907}.    >>> ge
+00021ad0: 745f 6e61 6d65 5f76 6572 7369 6f6e 2827  t_name_version('
+00021ae0: 746d 7068 3865 6774 6c5f 5f27 290a 2020  tmph8egtl__').  
+00021af0: 2020 7b27 6e61 6d65 273a 2027 746d 7068    {'name': 'tmph
+00021b00: 3865 6774 6c5f 5f27 2c20 2776 6572 7369  8egtl__', 'versi
+00021b10: 6f6e 273a 204e 6f6e 657d 0a20 2020 203e  on': None}.    >
+00021b20: 3e3e 2067 6574 5f6e 616d 655f 7665 7273  >> get_name_vers
+00021b30: 696f 6e28 2774 6d70 6838 6567 746c 5f5f  ion('tmph8egtl__
+00021b40: 3132 335f 5f27 290a 2020 2020 7b27 6e61  123__').    {'na
+00021b50: 6d65 273a 2027 746d 7068 3865 6774 6c5f  me': 'tmph8egtl_
+00021b60: 5f31 3233 5f5f 272c 2027 7665 7273 696f  _123__', 'versio
+00021b70: 6e27 3a20 4e6f 6e65 7d0a 2020 2020 3e3e  n': None}.    >>
+00021b80: 3e20 6765 745f 6e61 6d65 5f76 6572 7369  > get_name_versi
+00021b90: 6f6e 2827 6465 765f 5f6e 616d 655f 5f76  on('dev__name__v
+00021ba0: 3027 290a 2020 2020 7b27 6e61 6d65 273a  0').    {'name':
+00021bb0: 2027 6465 765f 5f6e 616d 6527 2c20 2776   'dev__name', 'v
+00021bc0: 6572 7369 6f6e 273a 2030 7d0a 2020 2020  ersion': 0}.    
+00021bd0: 3e3e 3e20 6765 745f 6e61 6d65 5f76 6572  >>> get_name_ver
+00021be0: 7369 6f6e 2827 6e61 6d65 5f5f 7630 2729  sion('name__v0')
+00021bf0: 0a20 2020 207b 276e 616d 6527 3a20 276e  .    {'name': 'n
+00021c00: 616d 6527 2c20 2776 6572 7369 6f6e 273a  ame', 'version':
+00021c10: 2030 7d0a 2020 2020 3e3e 3e20 6765 745f   0}.    >>> get_
+00021c20: 6e61 6d65 5f76 6572 7369 6f6e 2827 6465  name_version('de
+00021c30: 765f 5f6e 616d 6527 290a 2020 2020 7b27  v__name').    {'
+00021c40: 6e61 6d65 273a 2027 6465 765f 5f6e 616d  name': 'dev__nam
+00021c50: 6527 2c20 2776 6572 7369 6f6e 273a 204e  e', 'version': N
+00021c60: 6f6e 657d 0a20 2020 203e 3e3e 2067 6574  one}.    >>> get
+00021c70: 5f6e 616d 655f 7665 7273 696f 6e28 276e  _name_version('n
+00021c80: 616d 6527 290a 2020 2020 7b27 6e61 6d65  ame').    {'name
+00021c90: 273a 2027 6e61 6d65 272c 2027 7665 7273  ': 'name', 'vers
+00021ca0: 696f 6e27 3a20 4e6f 6e65 7d0a 2020 2020  ion': None}.    
+00021cb0: 3e3e 3e20 6765 745f 6e61 6d65 5f76 6572  >>> get_name_ver
+00021cc0: 7369 6f6e 2827 686f 7261 7269 6f5f 5f33  sion('horario__3
+00021cd0: 5f5f 7069 7065 2729 0a20 2020 207b 276e  __pipe').    {'n
+00021ce0: 616d 6527 3a20 2768 6f72 6172 696f 5f5f  ame': 'horario__
+00021cf0: 335f 5f70 6970 6527 2c20 2776 6572 7369  3__pipe', 'versi
+00021d00: 6f6e 273a 204e 6f6e 657d 0a20 2020 203e  on': None}.    >
+00021d10: 3e3e 2067 6574 5f6e 616d 655f 7665 7273  >> get_name_vers
+00021d20: 696f 6e28 2768 6f72 6172 696f 5f5f 6368  ion('horario__ch
+00021d30: 6563 6b65 7227 290a 2020 2020 7b27 6e61  ecker').    {'na
+00021d40: 6d65 273a 2027 686f 7261 7269 6f5f 5f63  me': 'horario__c
+00021d50: 6865 636b 6572 272c 2027 7665 7273 696f  hecker', 'versio
+00021d60: 6e27 3a20 4e6f 6e65 7d0a 2020 2020 3e3e  n': None}.    >>
+00021d70: 3e20 6765 745f 6e61 6d65 5f76 6572 7369  > get_name_versi
+00021d80: 6f6e 2827 6465 765f 5f68 6f72 6172 696f  on('dev__horario
+00021d90: 5f5f 6368 6563 6b65 7227 290a 2020 2020  __checker').    
+00021da0: 7b27 6e61 6d65 273a 2027 6465 765f 5f68  {'name': 'dev__h
+00021db0: 6f72 6172 696f 5f5f 6368 6563 6b65 7227  orario__checker'
+00021dc0: 2c20 2776 6572 7369 6f6e 273a 204e 6f6e  , 'version': Non
+00021dd0: 657d 0a20 2020 203e 3e3e 2067 6574 5f6e  e}.    >>> get_n
+00021de0: 616d 655f 7665 7273 696f 6e28 2774 675f  ame_version('tg_
+00021df0: 5f64 4163 7469 7669 6461 6465 735f 5f76  _dActividades__v
+00021e00: 305f 7069 7065 5f33 3930 3727 290a 2020  0_pipe_3907').  
+00021e10: 2020 7b27 6e61 6d65 273a 2027 7467 5f5f    {'name': 'tg__
+00021e20: 6441 6374 6976 6964 6164 6573 272c 2027  dActividades', '
+00021e30: 7665 7273 696f 6e27 3a20 307d 0a20 2020  version': 0}.   
+00021e40: 203e 3e3e 2067 6574 5f6e 616d 655f 7665   >>> get_name_ve
+00021e50: 7273 696f 6e28 2774 675f 5f6f 7269 6769  rsion('tg__origi
+00021e60: 6e5f 776f 726b 7370 6163 652e 7368 6172  n_workspace.shar
+00021e70: 6564 5f64 735f 5f76 3339 3037 2729 0a20  ed_ds__v3907'). 
+00021e80: 2020 207b 276e 616d 6527 3a20 2774 675f     {'name': 'tg_
+00021e90: 5f6f 7269 6769 6e5f 776f 726b 7370 6163  _origin_workspac
+00021ea0: 652e 7368 6172 6564 5f64 7327 2c20 2776  e.shared_ds', 'v
+00021eb0: 6572 7369 6f6e 273a 2033 3930 377d 0a20  ersion': 3907}. 
+00021ec0: 2020 203e 3e3e 2067 6574 5f6e 616d 655f     >>> get_name_
+00021ed0: 7665 7273 696f 6e28 2774 6d70 6838 6567  version('tmph8eg
+00021ee0: 746c 5f5f 2729 0a20 2020 207b 276e 616d  tl__').    {'nam
+00021ef0: 6527 3a20 2774 6d70 6838 6567 746c 5f5f  e': 'tmph8egtl__
+00021f00: 272c 2027 7665 7273 696f 6e27 3a20 4e6f  ', 'version': No
+00021f10: 6e65 7d0a 2020 2020 3e3e 3e20 6765 745f  ne}.    >>> get_
+00021f20: 6e61 6d65 5f76 6572 7369 6f6e 2827 746d  name_version('tm
+00021f30: 7068 3865 6774 6c5f 5f31 3233 5f5f 2729  ph8egtl__123__')
+00021f40: 0a20 2020 207b 276e 616d 6527 3a20 2774  .    {'name': 't
+00021f50: 6d70 6838 6567 746c 5f5f 3132 335f 5f27  mph8egtl__123__'
+00021f60: 2c20 2776 6572 7369 6f6e 273a 204e 6f6e  , 'version': Non
+00021f70: 657d 0a20 2020 2022 2222 0a20 2020 2074  e}.    """.    t
+00021f80: 6b20 3d20 6473 2e72 7370 6c69 7428 225f  k = ds.rsplit("_
+00021f90: 5f22 2c20 3229 0a20 2020 2069 6620 6c65  _", 2).    if le
+00021fa0: 6e28 746b 2920 3d3d 2031 3a0a 2020 2020  n(tk) == 1:.    
+00021fb0: 2020 2020 7265 7475 726e 207b 226e 616d      return {"nam
+00021fc0: 6522 3a20 746b 5b30 5d2c 2022 7665 7273  e": tk[0], "vers
+00021fd0: 696f 6e22 3a20 4e6f 6e65 7d0a 2020 2020  ion": None}.    
+00021fe0: 656c 6966 206c 656e 2874 6b29 203d 3d20  elif len(tk) == 
+00021ff0: 323a 0a20 2020 2020 2020 2069 6620 6c65  2:.        if le
+00022000: 6e28 746b 5b31 5d29 3a0a 2020 2020 2020  n(tk[1]):.      
+00022010: 2020 2020 2020 6966 2074 6b5b 315d 5b30        if tk[1][0
+00022020: 5d20 3d3d 2022 7622 2061 6e64 2072 652e  ] == "v" and re.
+00022030: 6d61 7463 6828 225b 302d 395d 2b24 222c  match("[0-9]+$",
+00022040: 2074 6b5b 315d 5b31 3a5d 293a 0a20 2020   tk[1][1:]):.   
+00022050: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00022060: 7572 6e20 7b22 6e61 6d65 223a 2074 6b5b  urn {"name": tk[
+00022070: 305d 2c20 2276 6572 7369 6f6e 223a 2069  0], "version": i
+00022080: 6e74 2874 6b5b 315d 5b31 3a5d 297d 0a20  nt(tk[1][1:])}. 
+00022090: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000220a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000220b0: 2072 6574 7572 6e20 7b22 6e61 6d65 223a   return {"name":
+000220c0: 2074 6b5b 305d 202b 2022 5f5f 2220 2b20   tk[0] + "__" + 
+000220d0: 746b 5b31 5d2c 2022 7665 7273 696f 6e22  tk[1], "version"
+000220e0: 3a20 4e6f 6e65 7d0a 2020 2020 656c 6966  : None}.    elif
+000220f0: 206c 656e 2874 6b29 203d 3d20 3320 616e   len(tk) == 3 an
+00022100: 6420 6c65 6e28 746b 5b32 5d29 3a0a 2020  d len(tk[2]):.  
+00022110: 2020 2020 2020 6966 2074 6b5b 325d 203d        if tk[2] =
+00022120: 3d20 2263 6865 636b 6572 223a 0a20 2020  = "checker":.   
+00022130: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00022140: 7b22 6e61 6d65 223a 2074 6b5b 305d 202b  {"name": tk[0] +
+00022150: 2022 5f5f 2220 2b20 746b 5b31 5d20 2b20   "__" + tk[1] + 
+00022160: 225f 5f22 202b 2074 6b5b 325d 2c20 2276  "__" + tk[2], "v
+00022170: 6572 7369 6f6e 223a 204e 6f6e 657d 0a20  ersion": None}. 
+00022180: 2020 2020 2020 2069 6620 746b 5b32 5d5b         if tk[2][
+00022190: 305d 203d 3d20 2276 223a 0a20 2020 2020  0] == "v":.     
+000221a0: 2020 2020 2020 2070 6172 7473 203d 2074         parts = t
+000221b0: 6b5b 325d 2e73 706c 6974 2822 5f22 290a  k[2].split("_").
+000221c0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000221d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000221e0: 2072 6574 7572 6e20 7b22 6e61 6d65 223a   return {"name":
+000221f0: 2074 6b5b 305d 202b 2022 5f5f 2220 2b20   tk[0] + "__" + 
+00022200: 746b 5b31 5d2c 2022 7665 7273 696f 6e22  tk[1], "version"
+00022210: 3a20 696e 7428 7061 7274 735b 305d 5b31  : int(parts[0][1
+00022220: 3a5d 297d 0a20 2020 2020 2020 2020 2020  :])}.           
+00022230: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00022240: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00022250: 2020 2020 7265 7475 726e 207b 226e 616d      return {"nam
+00022260: 6522 3a20 746b 5b30 5d20 2b20 225f 5f22  e": tk[0] + "__"
+00022270: 202b 2074 6b5b 315d 202b 2022 5f5f 2220   + tk[1] + "__" 
+00022280: 2b20 746b 5b32 5d2c 2022 7665 7273 696f  + tk[2], "versio
+00022290: 6e22 3a20 4e6f 6e65 7d0a 2020 2020 2020  n": None}.      
+000222a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000222b0: 2020 2020 7265 7475 726e 207b 226e 616d      return {"nam
+000222c0: 6522 3a20 225f 5f22 2e6a 6f69 6e28 746b  e": "__".join(tk
+000222d0: 5b30 3a5d 292c 2022 7665 7273 696f 6e22  [0:]), "version"
+000222e0: 3a20 4e6f 6e65 7d0a 0a20 2020 2072 6574  : None}..    ret
+000222f0: 7572 6e20 7b22 6e61 6d65 223a 2064 732c  urn {"name": ds,
+00022300: 2022 7665 7273 696f 6e22 3a20 4e6f 6e65   "version": None
+00022310: 7d0a 0a0a 6465 6620 6765 745f 7265 736f  }...def get_reso
+00022320: 7572 6365 5f76 6572 7369 6f6e 7328 6461  urce_versions(da
+00022330: 7461 736f 7572 6365 733a 204c 6973 745b  tasources: List[
+00022340: 7374 725d 293a 0a20 2020 2022 2222 0a20  str]):.    """. 
+00022350: 2020 2072 6574 7572 6e20 7468 6520 6c61     return the la
+00022360: 7465 7374 2076 6572 7369 6f6e 2066 6f72  test version for
+00022370: 2061 6c6c 2074 6865 2064 6174 6173 6f75   all the datasou
+00022380: 7263 6573 0a20 2020 2022 2222 0a20 2020  rces.    """.   
+00022390: 2076 6572 7369 6f6e 7320 3d20 7b7d 0a20   versions = {}. 
+000223a0: 2020 2066 6f72 2078 2069 6e20 6461 7461     for x in data
+000223b0: 736f 7572 6365 733a 0a20 2020 2020 2020  sources:.       
+000223c0: 2074 203d 2067 6574 5f6e 616d 655f 7665   t = get_name_ve
+000223d0: 7273 696f 6e28 7829 0a20 2020 2020 2020  rsion(x).       
+000223e0: 206e 616d 6520 3d20 745b 226e 616d 6522   name = t["name"
+000223f0: 5d0a 2020 2020 2020 2020 6966 2074 2e67  ].        if t.g
+00022400: 6574 2822 7665 7273 696f 6e22 2c20 4e6f  et("version", No
+00022410: 6e65 2920 6973 206e 6f74 204e 6f6e 653a  ne) is not None:
+00022420: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
+00022430: 7369 6f6e 735b 6e61 6d65 5d20 3d20 745b  sions[name] = t[
+00022440: 2276 6572 7369 6f6e 225d 0a20 2020 2072  "version"].    r
+00022450: 6574 7572 6e20 7665 7273 696f 6e73 0a0a  eturn versions..
+00022460: 0a64 6566 2067 6574 5f72 656d 6f74 655f  .def get_remote_
+00022470: 7265 736f 7572 6365 5f6e 616d 655f 7769  resource_name_wi
+00022480: 7468 6f75 745f 7665 7273 696f 6e28 7265  thout_version(re
+00022490: 6d6f 7465 5f72 6573 6f75 7263 655f 6e61  mote_resource_na
+000224a0: 6d65 3a20 7374 7229 202d 3e20 7374 723a  me: str) -> str:
+000224b0: 0a20 2020 2022 2222 0a20 2020 203e 3e3e  .    """.    >>>
+000224c0: 2067 6574 5f72 656d 6f74 655f 7265 736f   get_remote_reso
+000224d0: 7572 6365 5f6e 616d 655f 7769 7468 6f75  urce_name_withou
+000224e0: 745f 7665 7273 696f 6e28 2272 5f5f 6461  t_version("r__da
+000224f0: 7461 736f 7572 6365 2229 0a20 2020 2027  tasource").    '
+00022500: 725f 5f64 6174 6173 6f75 7263 6527 0a20  r__datasource'. 
+00022510: 2020 203e 3e3e 2067 6574 5f72 656d 6f74     >>> get_remot
+00022520: 655f 7265 736f 7572 6365 5f6e 616d 655f  e_resource_name_
+00022530: 7769 7468 6f75 745f 7665 7273 696f 6e28  without_version(
+00022540: 2272 5f5f 6461 7461 736f 7572 6365 5f5f  "r__datasource__
+00022550: 7630 2229 0a20 2020 2027 725f 5f64 6174  v0").    'r__dat
+00022560: 6173 6f75 7263 6527 0a20 2020 203e 3e3e  asource'.    >>>
+00022570: 2067 6574 5f72 656d 6f74 655f 7265 736f   get_remote_reso
+00022580: 7572 6365 5f6e 616d 655f 7769 7468 6f75  urce_name_withou
+00022590: 745f 7665 7273 696f 6e28 2264 6174 6173  t_version("datas
+000225a0: 6f75 7263 6522 290a 2020 2020 2764 6174  ource").    'dat
+000225b0: 6173 6f75 7263 6527 0a20 2020 2022 2222  asource'.    """
+000225c0: 0a20 2020 2070 6172 7473 203d 2067 6574  .    parts = get
+000225d0: 5f6e 616d 655f 7665 7273 696f 6e28 7265  _name_version(re
+000225e0: 6d6f 7465 5f72 6573 6f75 7263 655f 6e61  mote_resource_na
+000225f0: 6d65 290a 2020 2020 7265 7475 726e 2070  me).    return p
+00022600: 6172 7473 5b22 6e61 6d65 225d 0a0a 0a64  arts["name"]...d
+00022610: 6566 2067 6574 5f64 6570 5f66 726f 6d5f  ef get_dep_from_
+00022620: 7261 775f 7461 626c 6573 2878 3a20 7374  raw_tables(x: st
+00022630: 7229 202d 3e20 7374 723a 0a20 2020 2022  r) -> str:.    "
+00022640: 2222 0a20 2020 2064 6174 6173 6f75 7263  "".    datasourc
+00022650: 6573 204b 4559 2063 6f6d 6d61 6e64 2067  es KEY command g
+00022660: 656e 6572 6174 6573 2074 6162 6c65 732c  enerates tables,
+00022670: 2074 6869 7320 7472 616e 7366 6f72 6d20   this transform 
+00022680: 7468 6520 7573 6564 2074 6162 6c65 2077  the used table w
+00022690: 6974 6820 7468 6520 736f 7572 6365 2066  ith the source f
+000226a0: 696c 650a 2020 2020 3e3e 3e20 6765 745f  ile.    >>> get_
+000226b0: 6465 705f 6672 6f6d 5f72 6177 5f74 6162  dep_from_raw_tab
+000226c0: 6c65 7328 2774 6573 7427 290a 2020 2020  les('test').    
+000226d0: 2774 6573 7427 0a20 2020 203e 3e3e 2067  'test'.    >>> g
+000226e0: 6574 5f64 6570 5f66 726f 6d5f 7261 775f  et_dep_from_raw_
+000226f0: 7461 626c 6573 2827 7465 7374 5f6a 6f69  tables('test_joi
+00022700: 6e5f 6279 5f63 6f6c 756d 6e27 290a 2020  n_by_column').  
+00022710: 2020 2774 6573 7427 0a20 2020 2022 2222    'test'.    """
+00022720: 0a0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
+00022730: 2020 2072 6574 7572 6e20 785b 3a20 782e     return x[: x.
+00022740: 696e 6465 7828 225f 6a6f 696e 5f62 795f  index("_join_by_
+00022750: 2229 5d0a 2020 2020 6578 6365 7074 2056  ")].    except V
+00022760: 616c 7565 4572 726f 723a 0a20 2020 2020  alueError:.     
+00022770: 2020 2072 6574 7572 6e20 780a 0a0a 6465     return x...de
+00022780: 6620 6372 6561 7465 5f64 6f77 6e73 7472  f create_downstr
+00022790: 6561 6d5f 6465 7065 6e64 656e 6379 5f67  eam_dependency_g
+000227a0: 7261 7068 2864 6570 656e 6465 6e63 795f  raph(dependency_
+000227b0: 6772 6170 683a 2044 6963 745b 7374 722c  graph: Dict[str,
+000227c0: 2053 6574 5b73 7472 5d5d 2c20 616c 6c5f   Set[str]], all_
+000227d0: 7265 736f 7572 6365 733a 2044 6963 745b  resources: Dict[
+000227e0: 7374 722c 2044 6963 745b 7374 722c 2041  str, Dict[str, A
+000227f0: 6e79 5d5d 293a 0a20 2020 2022 2222 0a20  ny]]):.    """. 
+00022800: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+00022810: 2072 6576 6572 7365 7320 7468 6520 6465   reverses the de
+00022820: 7065 6e64 656e 6379 2067 7261 7068 206f  pendency graph o
+00022830: 6274 6169 6e65 6420 6672 6f6d 2062 7569  btained from bui
+00022840: 6c64 5f67 7261 7068 2073 6f20 796f 7520  ld_graph so you 
+00022850: 6861 7665 2064 6f77 6e73 7472 6561 6d20  have downstream 
+00022860: 6465 7065 6e64 656e 6369 6573 2066 6f72  dependencies for
+00022870: 2065 6163 6820 6e6f 6465 2069 6e20 7468   each node in th
+00022880: 6520 6772 6170 682e 0a0a 2020 2020 4164  e graph...    Ad
+00022890: 6469 7469 6f6e 616c 6c79 2074 616b 6573  ditionally takes
+000228a0: 2069 6e74 6f20 6163 636f 756e 7420 7461   into account ta
+000228b0: 7267 6574 5f64 6174 6173 6f75 7263 6520  rget_datasource 
+000228c0: 6f66 206d 6174 6572 6961 6c69 7a65 6420  of materialized 
+000228d0: 7669 6577 730a 2020 2020 2222 220a 2020  views.    """.  
+000228e0: 2020 646f 776e 7374 7265 616d 5f64 6570    downstream_dep
+000228f0: 656e 6465 6e63 795f 6772 6170 683a 2044  endency_graph: D
+00022900: 6963 745b 7374 722c 2053 6574 5b73 7472  ict[str, Set[str
+00022910: 5d5d 203d 207b 6e6f 6465 3a20 7365 7428  ]] = {node: set(
+00022920: 2920 666f 7220 6e6f 6465 2069 6e20 6465  ) for node in de
+00022930: 7065 6e64 656e 6379 5f67 7261 7068 7d0a  pendency_graph}.
+00022940: 0a20 2020 2066 6f72 206e 6f64 652c 2064  .    for node, d
+00022950: 6570 656e 6465 6e63 6965 7320 696e 2064  ependencies in d
+00022960: 6570 656e 6465 6e63 795f 6772 6170 682e  ependency_graph.
+00022970: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00022980: 2066 6f72 2064 6570 656e 6465 6e63 7920   for dependency 
+00022990: 696e 2064 6570 656e 6465 6e63 6965 733a  in dependencies:
+000229a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000229b0: 6465 7065 6e64 656e 6379 206e 6f74 2069  dependency not i
+000229c0: 6e20 646f 776e 7374 7265 616d 5f64 6570  n downstream_dep
+000229d0: 656e 6465 6e63 795f 6772 6170 683a 0a20  endency_graph:. 
+000229e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000229f0: 2061 2073 6861 7265 6420 6461 7461 2073   a shared data s
+00022a00: 6f75 7263 652c 2077 6520 6361 6e20 736b  ource, we can sk
+00022a10: 6970 2069 740a 2020 2020 2020 2020 2020  ip it.          
+00022a20: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00022a30: 2020 2020 2020 2020 2020 2064 6f77 6e73             downs
+00022a40: 7472 6561 6d5f 6465 7065 6e64 656e 6379  tream_dependency
+00022a50: 5f67 7261 7068 5b64 6570 656e 6465 6e63  _graph[dependenc
+00022a60: 795d 2e61 6464 286e 6f64 6529 0a0a 2020  y].add(node)..  
+00022a70: 2020 666f 7220 6b65 7920 696e 2064 6963    for key in dic
+00022a80: 7428 646f 776e 7374 7265 616d 5f64 6570  t(downstream_dep
+00022a90: 656e 6465 6e63 795f 6772 6170 6829 3a0a  endency_graph):.
+00022aa0: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
+00022ab0: 6174 6173 6f75 7263 6520 3d20 6765 745f  atasource = get_
+00022ac0: 7461 7267 6574 5f6d 6174 6572 6961 6c69  target_materiali
+00022ad0: 7a65 645f 6461 7461 5f73 6f75 7263 655f  zed_data_source_
+00022ae0: 6e61 6d65 2861 6c6c 5f72 6573 6f75 7263  name(all_resourc
+00022af0: 6573 5b6b 6579 5d29 0a20 2020 2020 2020  es[key]).       
+00022b00: 2069 6620 7461 7267 6574 5f64 6174 6173   if target_datas
+00022b10: 6f75 7263 653a 0a20 2020 2020 2020 2020  ource:.         
+00022b20: 2020 2064 6f77 6e73 7472 6561 6d5f 6465     downstream_de
+00022b30: 7065 6e64 656e 6379 5f67 7261 7068 5b6b  pendency_graph[k
+00022b40: 6579 5d2e 7570 6461 7465 287b 7461 7267  ey].update({targ
+00022b50: 6574 5f64 6174 6173 6f75 7263 657d 290a  et_datasource}).
+00022b60: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00022b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022b80: 2064 6f77 6e73 7472 6561 6d5f 6465 7065   downstream_depe
+00022b90: 6e64 656e 6379 5f67 7261 7068 5b74 6172  ndency_graph[tar
+00022ba0: 6765 745f 6461 7461 736f 7572 6365 5d2e  get_datasource].
+00022bb0: 7265 6d6f 7665 286b 6579 290a 2020 2020  remove(key).    
+00022bc0: 2020 2020 2020 2020 6578 6365 7074 204b          except K
+00022bd0: 6579 4572 726f 723a 0a20 2020 2020 2020  eyError:.       
+00022be0: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
+00022bf0: 2020 2072 6574 7572 6e20 646f 776e 7374     return downst
+00022c00: 7265 616d 5f64 6570 656e 6465 6e63 795f  ream_dependency_
+00022c10: 6772 6170 680a 0a0a 6465 6620 7570 6461  graph...def upda
+00022c20: 7465 5f64 6570 5f6d 6170 5f72 6563 7572  te_dep_map_recur
+00022c30: 7369 7665 6c79 280a 2020 2020 6465 705f  sively(.    dep_
+00022c40: 6d61 703a 2044 6963 745b 7374 722c 2053  map: Dict[str, S
+00022c50: 6574 5b73 7472 5d5d 2c0a 2020 2020 646f  et[str]],.    do
+00022c60: 776e 7374 7265 616d 5f64 6570 5f6d 6170  wnstream_dep_map
+00022c70: 3a20 4469 6374 5b73 7472 2c20 5365 745b  : Dict[str, Set[
+00022c80: 7374 725d 5d2c 0a20 2020 2061 6c6c 5f72  str]],.    all_r
+00022c90: 6573 6f75 7263 6573 3a20 4469 6374 5b73  esources: Dict[s
+00022ca0: 7472 2c20 4469 6374 5b73 7472 2c20 416e  tr, Dict[str, An
+00022cb0: 795d 5d2c 0a20 2020 2074 6f5f 7275 6e3a  y]],.    to_run:
+00022cc0: 2044 6963 745b 7374 722c 2044 6963 745b   Dict[str, Dict[
+00022cd0: 7374 722c 2041 6e79 5d5d 2c0a 2020 2020  str, Any]],.    
+00022ce0: 6465 705f 6d61 705f 6b65 7973 3a20 4c69  dep_map_keys: Li
+00022cf0: 7374 5b73 7472 5d2c 0a20 2020 206b 6579  st[str],.    key
+00022d00: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00022d10: 3d20 4e6f 6e65 2c0a 2020 2020 7669 7369  = None,.    visi
+00022d20: 7465 643a 204f 7074 696f 6e61 6c5b 4c69  ted: Optional[Li
+00022d30: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+00022d40: 0a29 3a0a 2020 2020 2222 220a 2020 2020  .):.    """.    
+00022d50: 4769 7665 6e20 6120 646f 776e 7374 7265  Given a downstre
+00022d60: 616d 5f64 6570 5f6d 6170 206f 6274 6169  am_dep_map obtai
+00022d70: 6e65 6420 6672 6f6d 2063 7265 6174 655f  ned from create_
+00022d80: 646f 776e 7374 7265 616d 5f64 6570 656e  downstream_depen
+00022d90: 6465 6e63 795f 6772 6170 6820 7468 6973  dency_graph this
+00022da0: 2066 756e 6374 696f 6e20 7570 6461 7465   function update
+00022db0: 7320 6561 6368 206e 6f64 6520 7265 6375  s each node recu
+00022dc0: 7273 6976 656c 7920 746f 2063 6f6d 706c  rsively to compl
+00022dd0: 6574 6520 7468 6520 646f 776e 7374 7265  ete the downstre
+00022de0: 616d 2064 6570 656e 6465 6e63 7920 6772  am dependency gr
+00022df0: 6170 6820 666f 7220 6561 6368 206e 6f64  aph for each nod
+00022e00: 650a 2020 2020 2222 220a 2020 2020 6966  e.    """.    if
+00022e10: 206e 6f74 2076 6973 6974 6564 3a0a 2020   not visited:.  
+00022e20: 2020 2020 2020 7669 7369 7465 6420 3d20        visited = 
+00022e30: 6c69 7374 2829 0a20 2020 2069 6620 6e6f  list().    if no
+00022e40: 7420 6b65 7920 616e 6420 6c65 6e28 6465  t key and len(de
+00022e50: 705f 6d61 705f 6b65 7973 2920 3d3d 2030  p_map_keys) == 0
+00022e60: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00022e70: 0a20 2020 2069 6620 6e6f 7420 6b65 793a  .    if not key:
+00022e80: 0a20 2020 2020 2020 206b 6579 203d 2064  .        key = d
+00022e90: 6570 5f6d 6170 5f6b 6579 732e 706f 7028  ep_map_keys.pop(
+00022ea0: 290a 2020 2020 6966 206b 6579 206e 6f74  ).    if key not
+00022eb0: 2069 6e20 6465 705f 6d61 703a 0a20 2020   in dep_map:.   
+00022ec0: 2020 2020 2064 6570 5f6d 6170 5b6b 6579       dep_map[key
+00022ed0: 5d20 3d20 7365 7428 290a 2020 2020 656c  ] = set().    el
+00022ee0: 7365 3a0a 2020 2020 2020 2020 7669 7369  se:.        visi
+00022ef0: 7465 642e 6170 7065 6e64 286b 6579 290a  ted.append(key).
+00022f00: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00022f10: 2020 2020 666f 7220 6465 7020 696e 2064      for dep in d
+00022f20: 6f77 6e73 7472 6561 6d5f 6465 705f 6d61  ownstream_dep_ma
+00022f30: 702e 6765 7428 6b65 792c 207b 7d29 3a0a  p.get(key, {}):.
+00022f40: 2020 2020 2020 2020 6966 2064 6570 206e          if dep n
+00022f50: 6f74 2069 6e20 646f 776e 7374 7265 616d  ot in downstream
+00022f60: 5f64 6570 5f6d 6170 3a0a 2020 2020 2020  _dep_map:.      
+00022f70: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00022f80: 2020 2020 2020 2074 6f5f 7275 6e5b 6465         to_run[de
+00022f90: 705d 203d 2061 6c6c 5f72 6573 6f75 7263  p] = all_resourc
+00022fa0: 6573 2e67 6574 2864 6570 2c20 7b7d 290a  es.get(dep, {}).
+00022fb0: 2020 2020 2020 2020 7570 6461 7465 5f64          update_d
+00022fc0: 6570 5f6d 6170 5f72 6563 7572 7369 7665  ep_map_recursive
+00022fd0: 6c79 280a 2020 2020 2020 2020 2020 2020  ly(.            
+00022fe0: 6465 705f 6d61 702c 2064 6f77 6e73 7472  dep_map, downstr
+00022ff0: 6561 6d5f 6465 705f 6d61 702c 2061 6c6c  eam_dep_map, all
+00023000: 5f72 6573 6f75 7263 6573 2c20 746f 5f72  _resources, to_r
+00023010: 756e 2c20 6465 705f 6d61 705f 6b65 7973  un, dep_map_keys
+00023020: 2c20 6b65 793d 6465 702c 2076 6973 6974  , key=dep, visit
+00023030: 6564 3d76 6973 6974 6564 0a20 2020 2020  ed=visited.     
+00023040: 2020 2029 0a20 2020 2020 2020 2064 6570     ).        dep
+00023050: 5f6d 6170 5b6b 6579 5d2e 7570 6461 7465  _map[key].update
+00023060: 2864 6f77 6e73 7472 6561 6d5f 6465 705f  (downstream_dep_
+00023070: 6d61 705b 6465 705d 290a 2020 2020 2020  map[dep]).      
+00023080: 2020 6465 705f 6d61 705b 6b65 795d 2e75    dep_map[key].u
+00023090: 7064 6174 6528 7b64 6570 7d29 0a20 2020  pdate({dep}).   
+000230a0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000230b0: 2020 2020 2020 6465 705f 6d61 705b 6b65        dep_map[ke
+000230c0: 795d 2e72 656d 6f76 6528 6b65 7929 0a20  y].remove(key). 
+000230d0: 2020 2020 2020 2065 7863 6570 7420 4b65         except Ke
+000230e0: 7945 7272 6f72 3a0a 2020 2020 2020 2020  yError:.        
+000230f0: 2020 2020 7061 7373 0a0a 2020 2020 746f      pass..    to
+00023100: 5f72 756e 5b6b 6579 5d20 3d20 616c 6c5f  _run[key] = all_
+00023110: 7265 736f 7572 6365 732e 6765 7428 6b65  resources.get(ke
+00023120: 792c 207b 7d29 0a20 2020 2075 7064 6174  y, {}).    updat
+00023130: 655f 6465 705f 6d61 705f 7265 6375 7273  e_dep_map_recurs
+00023140: 6976 656c 7928 0a20 2020 2020 2020 2064  ively(.        d
+00023150: 6570 5f6d 6170 2c20 646f 776e 7374 7265  ep_map, downstre
+00023160: 616d 5f64 6570 5f6d 6170 2c20 616c 6c5f  am_dep_map, all_
+00023170: 7265 736f 7572 6365 732c 2074 6f5f 7275  resources, to_ru
+00023180: 6e2c 2064 6570 5f6d 6170 5f6b 6579 732c  n, dep_map_keys,
+00023190: 206b 6579 3d4e 6f6e 652c 2076 6973 6974   key=None, visit
+000231a0: 6564 3d76 6973 6974 6564 0a20 2020 2029  ed=visited.    )
+000231b0: 0a0a 0a64 6566 2067 656e 6572 6174 655f  ...def generate_
+000231c0: 666f 726b 646f 776e 7374 7265 616d 5f67  forkdownstream_g
+000231d0: 7261 7068 280a 2020 2020 616c 6c5f 6465  raph(.    all_de
+000231e0: 705f 6d61 703a 2044 6963 745b 7374 722c  p_map: Dict[str,
+000231f0: 2053 6574 5b73 7472 5d5d 2c0a 2020 2020   Set[str]],.    
+00023200: 616c 6c5f 7265 736f 7572 6365 733a 2044  all_resources: D
+00023210: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
+00023220: 722c 2041 6e79 5d5d 2c0a 2020 2020 746f  r, Any]],.    to
+00023230: 5f72 756e 3a20 4469 6374 5b73 7472 2c20  _run: Dict[str, 
+00023240: 4469 6374 5b73 7472 2c20 416e 795d 5d2c  Dict[str, Any]],
+00023250: 0a20 2020 2064 6570 5f6d 6170 5f6b 6579  .    dep_map_key
+00023260: 733a 204c 6973 745b 7374 725d 2c0a 2920  s: List[str],.) 
+00023270: 2d3e 2054 7570 6c65 5b44 6963 745b 7374  -> Tuple[Dict[st
+00023280: 722c 2053 6574 5b73 7472 5d5d 2c20 4469  r, Set[str]], Di
+00023290: 6374 5b73 7472 2c20 4469 6374 5b73 7472  ct[str, Dict[str
+000232a0: 2c20 416e 795d 5d5d 3a0a 2020 2020 2222  , Any]]]:.    ""
+000232b0: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
+000232c0: 696f 6e20 666f 7220 6120 6769 7665 6e20  ion for a given 
+000232d0: 6772 6170 6820 6f66 2064 6570 656e 6465  graph of depende
+000232e0: 6e63 6965 7320 6672 6f6d 206c 6566 7420  ncies from left 
+000232f0: 746f 2072 6967 6874 2e20 4974 2077 696c  to right. It wil
+00023300: 6c20 6765 6e65 7261 7465 2061 206e 6577  l generate a new
+00023310: 2067 7261 7068 2077 6974 6820 7468 6520   graph with the 
+00023320: 6465 7065 6e64 656e 6369 6573 2066 726f  dependencies fro
+00023330: 6d20 7269 6768 7420 746f 206c 6566 742c  m right to left,
+00023340: 2062 7574 2074 616b 696e 6720 696e 746f   but taking into
+00023350: 2061 6363 6f75 6e74 2074 6861 7420 6576   account that ev
+00023360: 656e 2069 6620 736f 6d65 206e 6f64 6573  en if some nodes
+00023370: 2061 7265 206e 6f74 2069 6e73 6964 6520   are not inside 
+00023380: 746f 5f72 756e 2c20 7468 6579 2061 7265  to_run, they are
+00023390: 2073 7469 6c6c 2064 6570 656e 6465 6e63   still dependenc
+000233a0: 6965 7320 7468 6174 206e 6565 6420 746f  ies that need to
+000233b0: 2062 6520 6465 706c 6f79 6564 2e0a 0a20   be deployed... 
+000233c0: 2020 203e 3e3e 2064 6570 732c 205f 203d     >>> deps, _ =
+000233d0: 2067 656e 6572 6174 655f 666f 726b 646f   generate_forkdo
+000233e0: 776e 7374 7265 616d 5f67 7261 7068 280a  wnstream_graph(.
+000233f0: 2020 2020 2e2e 2e20 2020 2020 7b0a 2020      ...     {.  
+00023400: 2020 2e2e 2e20 2020 2020 2020 2020 2761    ...         'a
+00023410: 273a 207b 2762 277d 2c0a 2020 2020 2e2e  ': {'b'},.    ..
+00023420: 2e20 2020 2020 2020 2020 2762 273a 207b  .         'b': {
+00023430: 2763 277d 2c0a 2020 2020 2e2e 2e20 2020  'c'},.    ...   
+00023440: 2020 2020 2020 2763 273a 2073 6574 2829        'c': set()
+00023450: 2c0a 2020 2020 2e2e 2e20 2020 2020 7d2c  ,.    ...     },
+00023460: 0a20 2020 202e 2e2e 2020 2020 207b 0a20  .    ...     {. 
+00023470: 2020 202e 2e2e 2020 2020 2020 2020 2027     ...         '
+00023480: 6127 3a20 7b27 7265 736f 7572 6365 5f6e  a': {'resource_n
+00023490: 616d 6527 3a20 2761 277d 2c0a 2020 2020  ame': 'a'},.    
+000234a0: 2e2e 2e20 2020 2020 2020 2020 2762 273a  ...         'b':
+000234b0: 207b 2772 6573 6f75 7263 655f 6e61 6d65   {'resource_name
+000234c0: 273a 2027 6227 2c20 276e 6f64 6573 273a  ': 'b', 'nodes':
+000234d0: 205b 7b27 7061 7261 6d73 273a 207b 2774   [{'params': {'t
+000234e0: 7970 6527 3a20 276d 6174 6572 6961 6c69  ype': 'materiali
+000234f0: 7a65 6427 2c20 2764 6174 6173 6f75 7263  zed', 'datasourc
+00023500: 6527 3a20 2763 277d 7d5d 207d 2c0a 2020  e': 'c'}}] },.  
+00023510: 2020 2e2e 2e20 2020 2020 2020 2020 2763    ...         'c
+00023520: 273a 207b 2772 6573 6f75 7263 655f 6e61  ': {'resource_na
+00023530: 6d65 273a 2027 6327 7d2c 0a20 2020 202e  me': 'c'},.    .
+00023540: 2e2e 2020 2020 207d 2c0a 2020 2020 2e2e  ..     },.    ..
+00023550: 2e20 2020 2020 7b0a 2020 2020 2e2e 2e20  .     {.    ... 
+00023560: 2020 2020 2020 2020 2761 273a 207b 2772          'a': {'r
+00023570: 6573 6f75 7263 655f 6e61 6d65 273a 2027  esource_name': '
+00023580: 6127 7d2c 0a20 2020 202e 2e2e 2020 2020  a'},.    ...    
+00023590: 207d 2c0a 2020 2020 2e2e 2e20 2020 2020   },.    ...     
+000235a0: 5b27 6127 2c20 2762 272c 2027 6327 5d2c  ['a', 'b', 'c'],
+000235b0: 0a20 2020 202e 2e2e 2029 0a20 2020 203e  .    ... ).    >
+000235c0: 3e3e 207b 6b3a 2073 6f72 7465 6428 7629  >> {k: sorted(v)
+000235d0: 2066 6f72 206b 2c20 7620 696e 2064 6570   for k, v in dep
+000235e0: 732e 6974 656d 7328 297d 0a20 2020 207b  s.items()}.    {
+000235f0: 2763 273a 205b 5d2c 2027 6227 3a20 5b27  'c': [], 'b': ['
+00023600: 6127 2c20 2763 275d 2c20 2761 273a 205b  a', 'c'], 'a': [
+00023610: 5d7d 0a0a 2020 2020 3e3e 3e20 6465 7073  ]}..    >>> deps
+00023620: 2c20 5f20 3d20 6765 6e65 7261 7465 5f66  , _ = generate_f
+00023630: 6f72 6b64 6f77 6e73 7472 6561 6d5f 6772  orkdownstream_gr
+00023640: 6170 6828 0a20 2020 202e 2e2e 2020 2020  aph(.    ...    
+00023650: 207b 0a20 2020 202e 2e2e 2020 2020 2020   {.    ...      
+00023660: 2020 2027 6127 3a20 7b27 6227 7d2c 0a20     'a': {'b'},. 
+00023670: 2020 202e 2e2e 2020 2020 2020 2020 2027     ...         '
+00023680: 6227 3a20 7b27 6327 7d2c 0a20 2020 202e  b': {'c'},.    .
+00023690: 2e2e 2020 2020 2020 2020 2027 6327 3a20  ..         'c': 
+000236a0: 7365 7428 292c 0a20 2020 202e 2e2e 2020  set(),.    ...  
+000236b0: 2020 207d 2c0a 2020 2020 2e2e 2e20 2020     },.    ...   
+000236c0: 2020 7b0a 2020 2020 2e2e 2e20 2020 2020    {.    ...     
+000236d0: 2020 2020 2761 273a 207b 2772 6573 6f75      'a': {'resou
+000236e0: 7263 655f 6e61 6d65 273a 2027 6127 7d2c  rce_name': 'a'},
+000236f0: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00023700: 2027 6227 3a20 7b27 7265 736f 7572 6365   'b': {'resource
+00023710: 5f6e 616d 6527 3a20 2762 272c 2027 6e6f  _name': 'b', 'no
+00023720: 6465 7327 3a20 5b7b 2770 6172 616d 7327  des': [{'params'
+00023730: 3a20 7b27 7479 7065 273a 2027 6d61 7465  : {'type': 'mate
+00023740: 7269 616c 697a 6564 272c 2027 6461 7461  rialized', 'data
+00023750: 736f 7572 6365 273a 2027 6327 7d7d 5d20  source': 'c'}}] 
+00023760: 7d2c 0a20 2020 202e 2e2e 2020 2020 2020  },.    ...      
+00023770: 2020 2027 6327 3a20 7b27 7265 736f 7572     'c': {'resour
+00023780: 6365 5f6e 616d 6527 3a20 2763 277d 2c0a  ce_name': 'c'},.
+00023790: 2020 2020 2e2e 2e20 2020 2020 7d2c 0a20      ...     },. 
+000237a0: 2020 202e 2e2e 2020 2020 207b 0a20 2020     ...     {.   
+000237b0: 202e 2e2e 2020 2020 2020 2020 2027 6227   ...         'b'
+000237c0: 3a20 7b27 7265 736f 7572 6365 5f6e 616d  : {'resource_nam
+000237d0: 6527 3a20 2762 277d 2c0a 2020 2020 2e2e  e': 'b'},.    ..
+000237e0: 2e20 2020 2020 7d2c 0a20 2020 202e 2e2e  .     },.    ...
+000237f0: 2020 2020 205b 2761 272c 2027 6227 2c20       ['a', 'b', 
+00023800: 2763 275d 2c0a 2020 2020 2e2e 2e20 290a  'c'],.    ... ).
+00023810: 2020 2020 3e3e 3e20 7b6b 3a20 736f 7274      >>> {k: sort
+00023820: 6564 2876 2920 666f 7220 6b2c 2076 2069  ed(v) for k, v i
+00023830: 6e20 6465 7073 2e69 7465 6d73 2829 7d0a  n deps.items()}.
+00023840: 2020 2020 7b27 6327 3a20 5b5d 2c20 2762      {'c': [], 'b
+00023850: 273a 205b 2761 272c 2027 6327 5d2c 2027  ': ['a', 'c'], '
+00023860: 6127 3a20 5b5d 7d0a 0a20 2020 203e 3e3e  a': []}..    >>>
+00023870: 2064 6570 732c 205f 203d 2067 656e 6572   deps, _ = gener
+00023880: 6174 655f 666f 726b 646f 776e 7374 7265  ate_forkdownstre
+00023890: 616d 5f67 7261 7068 280a 2020 2020 2e2e  am_graph(.    ..
+000238a0: 2e20 2020 2020 7b0a 2020 2020 2e2e 2e20  .     {.    ... 
+000238b0: 2020 2020 2020 2020 276d 6967 7261 7465          'migrate
+000238c0: 645f 5f61 273a 207b 2761 277d 2c0a 2020  d__a': {'a'},.  
+000238d0: 2020 2e2e 2e20 2020 2020 2020 2020 2761    ...         'a
+000238e0: 273a 207b 2762 277d 2c0a 2020 2020 2e2e  ': {'b'},.    ..
+000238f0: 2e20 2020 2020 2020 2020 2762 273a 207b  .         'b': {
+00023900: 2763 277d 2c0a 2020 2020 2e2e 2e20 2020  'c'},.    ...   
+00023910: 2020 2020 2020 2763 273a 2073 6574 2829        'c': set()
+00023920: 2c0a 2020 2020 2e2e 2e20 2020 2020 7d2c  ,.    ...     },
+00023930: 0a20 2020 202e 2e2e 2020 2020 207b 0a20  .    ...     {. 
+00023940: 2020 202e 2e2e 2020 2020 2020 2020 2027     ...         '
+00023950: 6d69 6772 6174 6564 5f5f 6127 3a20 7b27  migrated__a': {'
+00023960: 7265 736f 7572 6365 5f6e 616d 6527 3a20  resource_name': 
+00023970: 276d 6967 7261 7465 645f 5f61 272c 2027  'migrated__a', '
+00023980: 6e6f 6465 7327 3a20 5b7b 2770 6172 616d  nodes': [{'param
+00023990: 7327 3a20 7b27 7479 7065 273a 2027 6d61  s': {'type': 'ma
+000239a0: 7465 7269 616c 697a 6564 272c 2027 6461  terialized', 'da
+000239b0: 7461 736f 7572 6365 273a 2027 6127 7d7d  tasource': 'a'}}
+000239c0: 5d7d 2c0a 2020 2020 2e2e 2e20 2020 2020  ]},.    ...     
+000239d0: 2020 2020 2761 273a 207b 2772 6573 6f75      'a': {'resou
+000239e0: 7263 655f 6e61 6d65 273a 2027 6127 7d2c  rce_name': 'a'},
+000239f0: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00023a00: 2027 6227 3a20 7b27 7265 736f 7572 6365   'b': {'resource
+00023a10: 5f6e 616d 6527 3a20 2762 272c 2027 6e6f  _name': 'b', 'no
+00023a20: 6465 7327 3a20 5b7b 2770 6172 616d 7327  des': [{'params'
+00023a30: 3a20 7b27 7479 7065 273a 2027 6d61 7465  : {'type': 'mate
+00023a40: 7269 616c 697a 6564 272c 2027 6461 7461  rialized', 'data
+00023a50: 736f 7572 6365 273a 2027 6327 7d7d 5d20  source': 'c'}}] 
+00023a60: 7d2c 0a20 2020 202e 2e2e 2020 2020 2020  },.    ...      
+00023a70: 2020 2027 6327 3a20 7b27 7265 736f 7572     'c': {'resour
+00023a80: 6365 5f6e 616d 6527 3a20 2763 277d 2c0a  ce_name': 'c'},.
+00023a90: 2020 2020 2e2e 2e20 2020 2020 7d2c 0a20      ...     },. 
+00023aa0: 2020 202e 2e2e 2020 2020 207b 0a20 2020     ...     {.   
+00023ab0: 202e 2e2e 2020 2020 2020 2020 2027 6d69   ...         'mi
+00023ac0: 6772 6174 6564 5f5f 6127 3a20 7b27 7265  grated__a': {'re
+00023ad0: 736f 7572 6365 5f6e 616d 6527 3a20 276d  source_name': 'm
+00023ae0: 6967 7261 7465 645f 5f61 277d 2c0a 2020  igrated__a'},.  
+00023af0: 2020 2e2e 2e20 2020 2020 2020 2020 2761    ...         'a
+00023b00: 273a 207b 2772 6573 6f75 7263 655f 6e61  ': {'resource_na
+00023b10: 6d65 273a 2027 6127 7d2c 0a20 2020 202e  me': 'a'},.    .
+00023b20: 2e2e 2020 2020 207d 2c0a 2020 2020 2e2e  ..     },.    ..
+00023b30: 2e20 2020 2020 5b27 6d69 6772 6174 6564  .     ['migrated
+00023b40: 5f61 272c 2027 6127 2c20 2762 272c 2027  _a', 'a', 'b', '
+00023b50: 6327 5d2c 0a20 2020 202e 2e2e 2029 0a20  c'],.    ... ). 
+00023b60: 2020 203e 3e3e 207b 6b3a 2073 6f72 7465     >>> {k: sorte
+00023b70: 6428 7629 2066 6f72 206b 2c20 7620 696e  d(v) for k, v in
+00023b80: 2064 6570 732e 6974 656d 7328 297d 0a20   deps.items()}. 
+00023b90: 2020 207b 2763 273a 205b 5d2c 2027 6227     {'c': [], 'b'
+00023ba0: 3a20 5b27 6127 2c20 2763 275d 2c20 2761  : ['a', 'c'], 'a
+00023bb0: 273a 205b 5d2c 2027 6d69 6772 6174 6564  ': [], 'migrated
+00023bc0: 5f61 273a 205b 5d7d 0a20 2020 2022 2222  _a': []}.    """
+00023bd0: 0a20 2020 2064 6f77 6e73 7472 6561 6d5f  .    downstream_
+00023be0: 6465 705f 6d61 7020 3d20 6372 6561 7465  dep_map = create
+00023bf0: 5f64 6f77 6e73 7472 6561 6d5f 6465 7065  _downstream_depe
+00023c00: 6e64 656e 6379 5f67 7261 7068 2861 6c6c  ndency_graph(all
+00023c10: 5f64 6570 5f6d 6170 2c20 616c 6c5f 7265  _dep_map, all_re
+00023c20: 736f 7572 6365 7329 0a20 2020 206e 6577  sources).    new
+00023c30: 5f64 6570 5f6d 6170 3a20 4469 6374 5b73  _dep_map: Dict[s
+00023c40: 7472 2c20 5365 745b 7374 725d 5d20 3d20  tr, Set[str]] = 
+00023c50: 7b7d 0a20 2020 206e 6577 5f74 6f5f 7275  {}.    new_to_ru
+00023c60: 6e20 3d20 6465 6570 636f 7079 2874 6f5f  n = deepcopy(to_
+00023c70: 7275 6e29 0a20 2020 2075 7064 6174 655f  run).    update_
+00023c80: 6465 705f 6d61 705f 7265 6375 7273 6976  dep_map_recursiv
+00023c90: 656c 7928 6e65 775f 6465 705f 6d61 702c  ely(new_dep_map,
+00023ca0: 2064 6f77 6e73 7472 6561 6d5f 6465 705f   downstream_dep_
+00023cb0: 6d61 702c 2061 6c6c 5f72 6573 6f75 7263  map, all_resourc
+00023cc0: 6573 2c20 6e65 775f 746f 5f72 756e 2c20  es, new_to_run, 
+00023cd0: 6465 705f 6d61 705f 6b65 7973 290a 2020  dep_map_keys).  
+00023ce0: 2020 7265 7475 726e 206e 6577 5f64 6570    return new_dep
+00023cf0: 5f6d 6170 2c20 6e65 775f 746f 5f72 756e  _map, new_to_run
+00023d00: 0a0a 0a40 6461 7461 636c 6173 730a 636c  ...@dataclass.cl
+00023d10: 6173 7320 4772 6170 6844 6570 656e 6465  ass GraphDepende
+00023d20: 6e63 6965 733a 0a20 2020 2022 2222 0a20  ncies:.    """. 
+00023d30: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
+00023d40: 2075 7365 6420 746f 2073 746f 7265 2074   used to store t
+00023d50: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
+00023d60: 6772 6170 6820 616e 6420 7468 6520 7265  graph and the re
+00023d70: 736f 7572 6365 7320 7468 6174 2061 7265  sources that are
+00023d80: 2067 6f69 6e67 2074 6f20 6265 2064 6570   going to be dep
+00023d90: 6c6f 7965 640a 2020 2020 2222 220a 0a20  loyed.    """.. 
+00023da0: 2020 2064 6570 5f6d 6170 3a20 4469 6374     dep_map: Dict
+00023db0: 5b73 7472 2c20 5365 745b 7374 725d 5d0a  [str, Set[str]].
+00023dc0: 2020 2020 746f 5f72 756e 3a20 4469 6374      to_run: Dict
+00023dd0: 5b73 7472 2c20 4469 6374 5b73 7472 2c20  [str, Dict[str, 
+00023de0: 416e 795d 5d0a 0a20 2020 2023 2054 6865  Any]]..    # The
+00023df0: 2073 616d 6520 6173 2061 626f 7665 2062   same as above b
+00023e00: 7574 2066 6f72 2074 6865 2077 686f 6c65  ut for the whole
+00023e10: 2070 726f 6a65 6374 2c20 6e6f 7420 6a75   project, not ju
+00023e20: 7374 2074 6865 2072 6573 6f75 7263 6573  st the resources
+00023e30: 2061 6666 6563 7465 6420 6279 2074 6865   affected by the
+00023e40: 2063 7572 7265 6e74 2064 6570 6c6f 796d   current deploym
+00023e50: 656e 740a 2020 2020 616c 6c5f 6465 705f  ent.    all_dep_
+00023e60: 6d61 703a 2044 6963 745b 7374 722c 2053  map: Dict[str, S
+00023e70: 6574 5b73 7472 5d5d 0a20 2020 2061 6c6c  et[str]].    all
+00023e80: 5f72 6573 6f75 7263 6573 3a20 4469 6374  _resources: Dict
+00023e90: 5b73 7472 2c20 4469 6374 5b73 7472 2c20  [str, Dict[str, 
+00023ea0: 416e 795d 5d0a 0a0a 6173 796e 6320 6465  Any]]...async de
+00023eb0: 6620 6275 696c 645f 6772 6170 6828 0a20  f build_graph(. 
+00023ec0: 2020 2066 696c 656e 616d 6573 3a20 4974     filenames: It
+00023ed0: 6572 6162 6c65 5b73 7472 5d2c 0a20 2020  erable[str],.   
+00023ee0: 2074 625f 636c 6965 6e74 3a20 5469 6e79   tb_client: Tiny
+00023ef0: 422c 0a20 2020 2064 6972 5f70 6174 683a  B,.    dir_path:
+00023f00: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00023f10: 204e 6f6e 652c 0a20 2020 2072 6573 6f75   None,.    resou
+00023f20: 7263 655f 7665 7273 696f 6e73 3d4e 6f6e  rce_versions=Non
+00023f30: 652c 0a20 2020 2077 6f72 6b73 7061 6365  e,.    workspace
+00023f40: 5f6d 6170 3a20 4f70 7469 6f6e 616c 5b44  _map: Optional[D
+00023f50: 6963 745d 203d 204e 6f6e 652c 0a20 2020  ict] = None,.   
+00023f60: 2070 726f 6365 7373 5f64 6570 656e 6465   process_depende
+00023f70: 6e63 6965 733a 2062 6f6f 6c20 3d20 4661  ncies: bool = Fa
+00023f80: 6c73 652c 0a20 2020 2076 6572 626f 7365  lse,.    verbose
+00023f90: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00023fa0: 2020 2020 736b 6970 5f63 6f6e 6e65 6374      skip_connect
+00023fb0: 6f72 733a 2062 6f6f 6c20 3d20 4661 6c73  ors: bool = Fals
+00023fc0: 652c 0a20 2020 2077 6f72 6b73 7061 6365  e,.    workspace
+00023fd0: 5f6c 6962 5f70 6174 6873 3a20 4f70 7469  _lib_paths: Opti
+00023fe0: 6f6e 616c 5b4c 6973 745b 5475 706c 655b  onal[List[Tuple[
+00023ff0: 7374 722c 2073 7472 5d5d 5d20 3d20 4e6f  str, str]]] = No
+00024000: 6e65 2c0a 2020 2020 6375 7272 656e 745f  ne,.    current_
+00024010: 7773 3a20 4f70 7469 6f6e 616c 5b44 6963  ws: Optional[Dic
+00024020: 745b 7374 722c 2041 6e79 5d5d 203d 204e  t[str, Any]] = N
+00024030: 6f6e 652c 0a20 2020 2063 6861 6e67 6564  one,.    changed
+00024040: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00024050: 7374 722c 2041 6e79 5d5d 203d 204e 6f6e  str, Any]] = Non
+00024060: 652c 0a20 2020 206f 6e6c 795f 6368 616e  e,.    only_chan
+00024070: 6765 733a 2062 6f6f 6c20 3d20 4661 6c73  ges: bool = Fals
+00024080: 652c 0a20 2020 2066 6f72 6b5f 646f 776e  e,.    fork_down
+00024090: 7374 7265 616d 3a20 4f70 7469 6f6e 616c  stream: Optional
+000240a0: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
+000240b0: 2020 2020 6973 5f69 6e74 6572 6e61 6c3a      is_internal:
+000240c0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+000240d0: 3d20 4661 6c73 652c 0a29 202d 3e20 4772  = False,.) -> Gr
+000240e0: 6170 6844 6570 656e 6465 6e63 6965 733a  aphDependencies:
+000240f0: 0a20 2020 2022 2222 0a20 2020 2054 6869  .    """.    Thi
+00024100: 7320 6d65 7468 6f64 2077 696c 6c20 6765  s method will ge
+00024110: 6e65 7261 7465 2061 2064 6570 656e 6465  nerate a depende
+00024120: 6e63 7920 6772 6170 6820 666f 7220 7468  ncy graph for th
+00024130: 6520 6769 7665 6e20 6669 6c65 732e 2049  e given files. I
+00024140: 7420 7769 6c6c 2061 6c73 6f20 7265 7475  t will also retu
+00024150: 726e 2061 206d 6170 206f 6620 616c 6c20  rn a map of all 
+00024160: 7468 6520 7265 736f 7572 6365 7320 7468  the resources th
+00024170: 6174 2061 7265 2067 6f69 6e67 2074 6f20  at are going to 
+00024180: 6265 2064 6570 6c6f 7965 642e 0a20 2020  be deployed..   
+00024190: 2042 7920 6465 6661 756c 7420 6974 2077   By default it w
+000241a0: 696c 6c20 6765 6e65 7261 7465 2074 6865  ill generate the
+000241b0: 2067 7261 7068 2066 726f 6d20 6c65 6674   graph from left
+000241c0: 2074 6f20 7269 6768 742c 2062 7574 2069   to right, but i
+000241d0: 6620 666f 726b 2d64 6f77 6e73 7472 6561  f fork-downstrea
+000241e0: 6d2c 2069 7420 7769 6c6c 2067 656e 6572  m, it will gener
+000241f0: 6174 6520 7468 6520 6772 6170 6820 6672  ate the graph fr
+00024200: 6f6d 2072 6967 6874 2074 6f20 6c65 6674  om right to left
+00024210: 2e0a 2020 2020 2222 220a 2020 2020 746f  ..    """.    to
+00024220: 5f72 756e 3a20 4469 6374 5b73 7472 2c20  _run: Dict[str, 
+00024230: 416e 795d 203d 207b 7d0a 2020 2020 6465  Any] = {}.    de
+00024240: 7073 3a20 4c69 7374 5b73 7472 5d20 3d20  ps: List[str] = 
+00024250: 5b5d 0a20 2020 2064 6570 5f6d 6170 3a20  [].    dep_map: 
+00024260: 4469 6374 5b73 7472 2c20 416e 795d 203d  Dict[str, Any] =
+00024270: 207b 7d0a 2020 2020 656d 6265 6464 6564   {}.    embedded
+00024280: 5f64 6174 6173 6f75 7263 6573 203d 207b  _datasources = {
+00024290: 7d0a 2020 2020 6966 206e 6f74 2077 6f72  }.    if not wor
+000242a0: 6b73 7061 6365 5f6d 6170 3a0a 2020 2020  kspace_map:.    
+000242b0: 2020 2020 776f 726b 7370 6163 655f 6d61      workspace_ma
+000242c0: 7020 3d20 7b7d 0a0a 2020 2020 2320 5468  p = {}..    # Th
+000242d0: 6573 6520 6469 6374 696f 6e61 7269 6573  ese dictionaries
+000242e0: 2061 7265 2075 7365 6420 746f 2073 746f   are used to sto
+000242f0: 7265 2061 6c6c 2074 6865 2072 6573 6f75  re all the resou
+00024300: 7263 6573 2061 6e64 2074 6865 7265 2064  rces and there d
+00024310: 6570 656e 6465 6e63 6965 7320 666f 7220  ependencies for 
+00024320: 7468 6520 7768 6f6c 6520 7072 6f6a 6563  the whole projec
+00024330: 740a 2020 2020 2320 5468 6973 2069 7320  t.    # This is 
+00024340: 7573 6564 2066 6f72 2074 6865 2064 6f77  used for the dow
+00024350: 6e73 7472 6561 6d20 6465 7065 6e64 656e  nstream dependen
+00024360: 6379 2067 7261 7068 0a20 2020 2061 6c6c  cy graph.    all
+00024370: 5f64 6570 5f6d 6170 3a20 4469 6374 5b73  _dep_map: Dict[s
+00024380: 7472 2c20 5365 745b 7374 725d 5d20 3d20  tr, Set[str]] = 
+00024390: 7b7d 0a20 2020 2061 6c6c 5f72 6573 6f75  {}.    all_resou
+000243a0: 7263 6573 3a20 4469 6374 5b73 7472 2c20  rces: Dict[str, 
+000243b0: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
+000243c0: 3d20 7b7d 0a0a 2020 2020 6966 2064 6972  = {}..    if dir
+000243d0: 5f70 6174 6820 6973 204e 6f6e 653a 0a20  _path is None:. 
+000243e0: 2020 2020 2020 2064 6972 5f70 6174 6820         dir_path 
+000243f0: 3d20 6f73 2e67 6574 6377 6428 290a 0a20  = os.getcwd().. 
+00024400: 2020 2023 2057 6865 6e20 7573 696e 6720     # When using 
+00024410: 666f 726b 2d64 6f77 6e73 7472 6561 6d20  fork-downstream 
+00024420: 6f72 202d 2d6f 6e6c 792d 6368 616e 6765  or --only-change
+00024430: 732c 2077 6520 6e65 6564 2074 6f20 6765  s, we need to ge
+00024440: 6e65 7261 7465 2061 6c6c 2074 6865 2067  nerate all the g
+00024450: 7261 7068 206f 6620 616c 6c20 7468 6520  raph of all the 
+00024460: 7265 736f 7572 6365 7320 616e 6420 7468  resources and th
+00024470: 6569 7220 6465 7065 6e64 656e 6369 6573  eir dependencies
+00024480: 0a20 2020 2023 2054 6869 7320 7761 7920  .    # This way 
+00024490: 7765 2063 616e 2061 6464 206d 6f72 6520  we can add more 
+000244a0: 7265 736f 7572 6365 7320 696e 746f 2074  resources into t
+000244b0: 6865 2074 6f5f 7275 6e20 6469 6374 696f  he to_run dictio
+000244c0: 6e61 7279 2069 6620 6e65 6564 6564 2e0a  nary if needed..
+000244d0: 2020 2020 6966 2070 726f 6365 7373 5f64      if process_d
+000244e0: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
+000244f0: 6f6e 6c79 5f63 6861 6e67 6573 3a0a 2020  only_changes:.  
+00024500: 2020 2020 2020 616c 6c5f 6465 7065 6e64        all_depend
+00024510: 656e 6369 6573 5f67 7261 7068 203d 2061  encies_graph = a
+00024520: 7761 6974 2062 7569 6c64 5f67 7261 7068  wait build_graph
+00024530: 280a 2020 2020 2020 2020 2020 2020 6765  (.            ge
+00024540: 745f 7072 6f6a 6563 745f 6669 6c65 6e61  t_project_filena
+00024550: 6d65 7328 6469 725f 7061 7468 292c 0a20  mes(dir_path),. 
+00024560: 2020 2020 2020 2020 2020 2074 625f 636c             tb_cl
+00024570: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
+00024580: 2020 6469 725f 7061 7468 3d64 6972 5f70    dir_path=dir_p
+00024590: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+000245a0: 2070 726f 6365 7373 5f64 6570 656e 6465   process_depende
+000245b0: 6e63 6965 733d 5472 7565 2c0a 2020 2020  ncies=True,.    
+000245c0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+000245d0: 5f76 6572 7369 6f6e 733d 7265 736f 7572  _versions=resour
+000245e0: 6365 5f76 6572 7369 6f6e 732c 0a20 2020  ce_versions,.   
+000245f0: 2020 2020 2020 2020 2077 6f72 6b73 7061           workspa
+00024600: 6365 5f6d 6170 3d77 6f72 6b73 7061 6365  ce_map=workspace
+00024610: 5f6d 6170 2c0a 2020 2020 2020 2020 2020  _map,.          
+00024620: 2020 736b 6970 5f63 6f6e 6e65 6374 6f72    skip_connector
+00024630: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
+00024640: 2020 2020 776f 726b 7370 6163 655f 6c69      workspace_li
+00024650: 625f 7061 7468 733d 776f 726b 7370 6163  b_paths=workspac
+00024660: 655f 6c69 625f 7061 7468 732c 0a20 2020  e_lib_paths,.   
+00024670: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00024680: 5f77 733d 6375 7272 656e 745f 7773 2c0a  _ws=current_ws,.
+00024690: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+000246a0: 6765 643d 4e6f 6e65 2c0a 2020 2020 2020  ged=None,.      
+000246b0: 2020 2020 2020 6f6e 6c79 5f63 6861 6e67        only_chang
+000246c0: 6573 3d46 616c 7365 2c0a 2020 2020 2020  es=False,.      
+000246d0: 2020 2020 2020 6973 5f69 6e74 6572 6e61        is_interna
+000246e0: 6c3d 6973 5f69 6e74 6572 6e61 6c2c 0a20  l=is_internal,. 
+000246f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00024700: 2061 6c6c 5f64 6570 5f6d 6170 203d 2061   all_dep_map = a
+00024710: 6c6c 5f64 6570 656e 6465 6e63 6965 735f  ll_dependencies_
+00024720: 6772 6170 682e 6465 705f 6d61 700a 2020  graph.dep_map.  
+00024730: 2020 2020 2020 616c 6c5f 7265 736f 7572        all_resour
+00024740: 6365 7320 3d20 616c 6c5f 6465 7065 6e64  ces = all_depend
+00024750: 656e 6369 6573 5f67 7261 7068 2e74 6f5f  encies_graph.to_
+00024760: 7275 6e0a 0a20 2020 2061 7379 6e63 2064  run..    async d
+00024770: 6566 2070 726f 6365 7373 280a 2020 2020  ef process(.    
+00024780: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
+00024790: 722c 0a20 2020 2020 2020 2064 6570 733a  r,.        deps:
+000247a0: 204c 6973 745b 7374 725d 2c0a 2020 2020   List[str],.    
+000247b0: 2020 2020 6465 705f 6d61 703a 2044 6963      dep_map: Dic
+000247c0: 745b 7374 722c 2041 6e79 5d2c 0a20 2020  t[str, Any],.   
+000247d0: 2020 2020 2074 6f5f 7275 6e3a 2044 6963       to_run: Dic
+000247e0: 745b 7374 722c 2041 6e79 5d2c 0a20 2020  t[str, Any],.   
+000247f0: 2020 2020 2077 6f72 6b73 7061 6365 5f6c       workspace_l
+00024800: 6962 5f70 6174 6873 3a20 4f70 7469 6f6e  ib_paths: Option
+00024810: 616c 5b4c 6973 745b 5475 706c 655b 7374  al[List[Tuple[st
+00024820: 722c 2073 7472 5d5d 5d2c 0a20 2020 2029  r, str]]],.    )
+00024830: 3a0a 2020 2020 2020 2020 6e61 6d65 2c20  :.        name, 
+00024840: 6b69 6e64 203d 2066 696c 656e 616d 652e  kind = filename.
+00024850: 7273 706c 6974 2822 2e22 2c20 3129 0a0a  rsplit(".", 1)..
+00024860: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00024870: 2020 2020 2020 2020 2072 6573 203d 2061           res = a
+00024880: 7761 6974 2070 726f 6365 7373 5f66 696c  wait process_fil
+00024890: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+000248a0: 2020 2066 696c 656e 616d 652c 0a20 2020     filename,.   
+000248b0: 2020 2020 2020 2020 2020 2020 2074 625f               tb_
+000248c0: 636c 6965 6e74 2c0a 2020 2020 2020 2020  client,.        
+000248d0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+000248e0: 5f76 6572 7369 6f6e 733d 7265 736f 7572  _versions=resour
+000248f0: 6365 5f76 6572 7369 6f6e 732c 0a20 2020  ce_versions,.   
+00024900: 2020 2020 2020 2020 2020 2020 2073 6b69               ski
+00024910: 705f 636f 6e6e 6563 746f 7273 3d73 6b69  p_connectors=ski
+00024920: 705f 636f 6e6e 6563 746f 7273 2c0a 2020  p_connectors,.  
+00024930: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+00024940: 726b 7370 6163 655f 6d61 703d 776f 726b  rkspace_map=work
+00024950: 7370 6163 655f 6d61 702c 0a20 2020 2020  space_map,.     
+00024960: 2020 2020 2020 2020 2020 2077 6f72 6b73             works
+00024970: 7061 6365 5f6c 6962 5f70 6174 6873 3d77  pace_lib_paths=w
+00024980: 6f72 6b73 7061 6365 5f6c 6962 5f70 6174  orkspace_lib_pat
+00024990: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
+000249a0: 2020 2020 6375 7272 656e 745f 7773 3d63      current_ws=c
+000249b0: 7572 7265 6e74 5f77 732c 0a20 2020 2020  urrent_ws,.     
+000249c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000249d0: 2065 7863 6570 7420 636c 6963 6b2e 436c   except click.Cl
+000249e0: 6963 6b45 7863 6570 7469 6f6e 2061 7320  ickException as 
+000249f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00024a00: 6169 7365 2065 0a20 2020 2020 2020 2065  aise e.        e
+00024a10: 7863 6570 7420 496e 636c 7564 6546 696c  xcept IncludeFil
+00024a20: 654e 6f74 466f 756e 6445 7863 6570 7469  eNotFoundExcepti
+00024a30: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00024a40: 2020 2020 2072 6169 7365 2063 6c69 636b       raise click
+00024a50: 2e43 6c69 636b 4578 6365 7074 696f 6e28  .ClickException(
+00024a60: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
+00024a70: 6572 726f 725f 6465 6c65 7465 645f 696e  error_deleted_in
+00024a80: 636c 7564 6528 696e 636c 7564 655f 6669  clude(include_fi
+00024a90: 6c65 3d73 7472 2865 292c 2066 696c 656e  le=str(e), filen
+00024aa0: 616d 653d 6669 6c65 6e61 6d65 2929 0a20  ame=filename)). 
+00024ab0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00024ac0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00024ad0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00024ae0: 636c 6963 6b2e 436c 6963 6b45 7863 6570  click.ClickExcep
+00024af0: 7469 6f6e 2873 7472 2865 2929 0a0a 2020  tion(str(e))..  
+00024b00: 2020 2020 2020 666f 7220 7220 696e 2072        for r in r
+00024b10: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00024b20: 666e 203d 2072 5b22 7265 736f 7572 6365  fn = r["resource
+00024b30: 5f6e 616d 6522 5d0a 2020 2020 2020 2020  _name"].        
+00024b40: 2020 2020 6966 2063 6861 6e67 6564 2061      if changed a
+00024b50: 6e64 2066 6e20 696e 2063 6861 6e67 6564  nd fn in changed
+00024b60: 2061 6e64 2028 6e6f 7420 6368 616e 6765   and (not change
+00024b70: 645b 666e 5d20 6f72 2063 6861 6e67 6564  d[fn] or changed
+00024b80: 5b66 6e5d 2069 6e20 5b22 7368 6172 6564  [fn] in ["shared
+00024b90: 222c 2022 7265 6d6f 7465 225d 293a 0a20  ", "remote"]):. 
+00024ba0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00024bb0: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+00024bc0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00024bd0: 2020 2020 2020 2020 2020 666f 726b 5f64            fork_d
+00024be0: 6f77 6e73 7472 6561 6d0a 2020 2020 2020  ownstream.      
+00024bf0: 2020 2020 2020 2020 2020 616e 6420 722e            and r.
+00024c00: 6765 7428 2272 6573 6f75 7263 6522 2c20  get("resource", 
+00024c10: 2222 2920 3d3d 2022 7069 7065 7322 0a20  "") == "pipes". 
+00024c20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00024c30: 6e64 2061 6e79 285b 2265 6e67 696e 6522  nd any(["engine"
+00024c40: 2069 6e20 782e 6765 7428 2270 6172 616d   in x.get("param
+00024c50: 7322 2c20 7b7d 2920 666f 7220 7820 696e  s", {}) for x in
+00024c60: 2072 2e67 6574 2822 6e6f 6465 7322 2c20   r.get("nodes", 
+00024c70: 5b5d 295d 290a 2020 2020 2020 2020 2020  [])]).          
+00024c80: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+00024c90: 2020 2020 2072 6169 7365 2063 6c69 636b       raise click
+00024ca0: 2e43 6c69 636b 4578 6365 7074 696f 6e28  .ClickException(
+00024cb0: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
+00024cc0: 6572 726f 725f 666f 726b 646f 776e 7374  error_forkdownst
+00024cd0: 7265 616d 5f70 6970 6573 5f77 6974 685f  ream_pipes_with_
+00024ce0: 656e 6769 6e65 2870 6970 653d 666e 2929  engine(pipe=fn))
+00024cf0: 0a0a 2020 2020 2020 2020 2020 2020 746f  ..            to
+00024d00: 5f72 756e 5b66 6e5d 203d 2072 0a20 2020  _run[fn] = r.   
+00024d10: 2020 2020 2020 2020 2066 696c 655f 6465           file_de
+00024d20: 7073 203d 2072 2e67 6574 2822 6465 7073  ps = r.get("deps
+00024d30: 222c 205b 5d29 0a20 2020 2020 2020 2020  ", []).         
+00024d40: 2020 2064 6570 7320 2b3d 2066 696c 655f     deps += file_
+00024d50: 6465 7073 0a20 2020 2020 2020 2020 2020  deps.           
+00024d60: 2023 2063 616c 6375 6c61 7465 2061 6e64   # calculate and
+00024d70: 206c 6f6f 6b20 666f 7220 6465 7073 0a20   look for deps. 
+00024d80: 2020 2020 2020 2020 2020 2064 6570 5f6c             dep_l
+00024d90: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
+00024da0: 2020 2020 2066 6f72 2078 2069 6e20 6669       for x in fi
+00024db0: 6c65 5f64 6570 733a 0a20 2020 2020 2020  le_deps:.       
+00024dc0: 2020 2020 2020 2020 2069 6620 7820 6e6f           if x no
+00024dd0: 7420 696e 2049 4e54 4552 4e41 4c5f 5441  t in INTERNAL_TA
+00024de0: 424c 4553 206f 7220 6973 5f69 6e74 6572  BLES or is_inter
+00024df0: 6e61 6c3a 0a20 2020 2020 2020 2020 2020  nal:.           
+00024e00: 2020 2020 2020 2020 2066 2c20 6473 203d           f, ds =
+00024e10: 2066 696e 645f 6669 6c65 5f62 795f 6e61   find_file_by_na
+00024e20: 6d65 2864 6972 5f70 6174 682c 2078 2c20  me(dir_path, x, 
+00024e30: 7665 7262 6f73 652c 2077 6f72 6b73 7061  verbose, workspa
+00024e40: 6365 5f6c 6962 5f70 6174 6873 3d77 6f72  ce_lib_paths=wor
+00024e50: 6b73 7061 6365 5f6c 6962 5f70 6174 6873  kspace_lib_paths
+00024e60: 2c20 7265 736f 7572 6365 3d72 290a 2020  , resource=r).  
+00024e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e80: 2020 6966 2066 3a0a 2020 2020 2020 2020    if f:.        
+00024e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024ea0: 6465 705f 6c69 7374 2e61 7070 656e 6428  dep_list.append(
+00024eb0: 662e 7273 706c 6974 2822 2e22 2c20 3129  f.rsplit(".", 1)
+00024ec0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+00024ed0: 2020 2020 2020 2020 2069 6620 6473 3a0a           if ds:.
 00024ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ef0: 6473 5f66 6e20 3d20 6473 5b22 7265 736f  ds_fn = ds["reso
-00024f00: 7572 6365 5f6e 616d 6522 5d0a 2020 2020  urce_name"].    
-00024f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f20: 2020 2020 7072 6576 203d 2074 6f5f 7275      prev = to_ru
-00024f30: 6e2e 6765 7428 6473 5f66 6e2c 207b 7d29  n.get(ds_fn, {})
-00024f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024f50: 2020 2020 2020 2020 2074 6f5f 7275 6e5b           to_run[
-00024f60: 6473 5f66 6e5d 203d 2064 6565 7063 6f70  ds_fn] = deepcop
-00024f70: 7928 7229 0a20 2020 2020 2020 2020 2020  y(r).           
-00024f80: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00024f90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024fa0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00024fb0: 5f72 756e 5b64 735f 666e 5d5b 2264 6570  _run[ds_fn]["dep
-00024fc0: 7322 5d20 3d20 6c69 7374 280a 2020 2020  s"] = list(.    
-00024fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fe0: 2020 2020 2020 2020 2020 2020 7365 7428              set(
-00024ff0: 746f 5f72 756e 5b64 735f 666e 5d2e 6765  to_run[ds_fn].ge
-00025000: 7428 2264 6570 7322 2c20 5b5d 2920 2b20  t("deps", []) + 
-00025010: 7072 6576 2e67 6574 2822 6465 7073 222c  prev.get("deps",
-00025020: 205b 5d29 202b 205b 666e 5d29 0a20 2020   []) + [fn]).   
-00025030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025040: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00025050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025060: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
-00025070: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00024ef0: 2020 2020 2020 2020 6473 5f66 6e20 3d20          ds_fn = 
+00024f00: 6473 5b22 7265 736f 7572 6365 5f6e 616d  ds["resource_nam
+00024f10: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+00024f20: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00024f30: 203d 2074 6f5f 7275 6e2e 6765 7428 6473   = to_run.get(ds
+00024f40: 5f66 6e2c 207b 7d29 0a20 2020 2020 2020  _fn, {}).       
+00024f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024f60: 2074 6f5f 7275 6e5b 6473 5f66 6e5d 203d   to_run[ds_fn] =
+00024f70: 2064 6565 7063 6f70 7928 7229 0a20 2020   deepcopy(r).   
+00024f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024f90: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00024fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024fb0: 2020 2020 2020 746f 5f72 756e 5b64 735f        to_run[ds_
+00024fc0: 666e 5d5b 2264 6570 7322 5d20 3d20 6c69  fn]["deps"] = li
+00024fd0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+00024fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024ff0: 2020 2020 7365 7428 746f 5f72 756e 5b64      set(to_run[d
+00025000: 735f 666e 5d2e 6765 7428 2264 6570 7322  s_fn].get("deps"
+00025010: 2c20 5b5d 2920 2b20 7072 6576 2e67 6574  , []) + prev.get
+00025020: 2822 6465 7073 222c 205b 5d29 202b 205b  ("deps", []) + [
+00025030: 666e 5d29 0a20 2020 2020 2020 2020 2020  fn]).           
+00025040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025050: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00025060: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00025070: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
 00025080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025090: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
-000250a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000250b0: 6d62 6564 6465 645f 6461 7461 736f 7572  mbedded_datasour
-000250c0: 6365 735b 785d 203d 2074 6f5f 7275 6e5b  ces[x] = to_run[
-000250d0: 6473 5f66 6e5d 0a20 2020 2020 2020 2020  ds_fn].         
-000250e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000250f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025100: 2020 2020 2020 2020 2065 5f64 7320 3d20           e_ds = 
-00025110: 656d 6265 6464 6564 5f64 6174 6173 6f75  embedded_datasou
-00025120: 7263 6573 2e67 6574 2878 2c20 4e6f 6e65  rces.get(x, None
-00025130: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00025140: 2020 2020 2020 2020 2020 6966 2065 5f64            if e_d
-00025150: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00025160: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00025170: 6570 5f6c 6973 742e 6170 7065 6e64 2865  ep_list.append(e
-00025180: 5f64 735b 2272 6573 6f75 7263 655f 6e61  _ds["resource_na
-00025190: 6d65 225d 290a 0a20 2020 2020 2020 2020  me"])..         
-000251a0: 2020 2023 2049 6e20 6361 7365 2074 6865     # In case the
-000251b0: 2064 6174 6173 6f75 7263 6520 6973 2074   datasource is t
-000251c0: 6f20 6265 2073 6861 7265 6420 616e 6420  o be shared and 
-000251d0: 7765 2068 6176 6520 6d61 7070 696e 672c  we have mapping,
-000251e0: 206c 6574 2773 2072 6570 6c61 6365 2074   let's replace t
-000251f0: 6865 206e 616d 650a 2020 2020 2020 2020  he name.        
-00025200: 2020 2020 6966 2022 7368 6172 6564 5f77      if "shared_w
-00025210: 6974 6822 2069 6e20 7220 616e 6420 776f  ith" in r and wo
-00025220: 726b 7370 6163 655f 6d61 703a 0a20 2020  rkspace_map:.   
-00025230: 2020 2020 2020 2020 2020 2020 206d 6170               map
-00025240: 7065 645f 776f 726b 7370 6163 6573 3a20  ped_workspaces: 
-00025250: 4c69 7374 5b73 7472 5d20 3d20 5b5d 0a20  List[str] = []. 
-00025260: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00025270: 6f72 2073 6861 7265 645f 7769 7468 2069  or shared_with i
-00025280: 6e20 725b 2273 6861 7265 645f 7769 7468  n r["shared_with
-00025290: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-000252a0: 2020 2020 2020 2020 6d61 7070 6564 5f77          mapped_w
-000252b0: 6f72 6b73 7061 6365 732e 6170 7065 6e64  orkspaces.append
-000252c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000252d0: 2020 2020 2020 2020 2020 776f 726b 7370            worksp
-000252e0: 6163 655f 6d61 702e 6765 7428 7368 6172  ace_map.get(shar
-000252f0: 6564 5f77 6974 6829 0a20 2020 2020 2020  ed_with).       
-00025300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025310: 2069 6620 776f 726b 7370 6163 655f 6d61   if workspace_ma
-00025320: 702e 6765 7428 7368 6172 6564 5f77 6974  p.get(shared_wit
-00025330: 682c 204e 6f6e 6529 2069 7320 6e6f 7420  h, None) is not 
-00025340: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00025350: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00025360: 6520 7368 6172 6564 5f77 6974 680a 2020  e shared_with.  
-00025370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025380: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00025390: 2020 2020 725b 2273 6861 7265 645f 7769      r["shared_wi
-000253a0: 7468 225d 203d 206d 6170 7065 645f 776f  th"] = mapped_wo
-000253b0: 726b 7370 6163 6573 0a0a 2020 2020 2020  rkspaces..      
-000253c0: 2020 2020 2020 6465 705f 6d61 705b 666e        dep_map[fn
-000253d0: 5d20 3d20 7365 7428 6465 705f 6c69 7374  ] = set(dep_list
-000253e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000253f0: 206f 732e 7061 7468 2e62 6173 656e 616d   os.path.basenam
-00025400: 6528 6e61 6d65 290a 0a20 2020 2070 726f  e(name)..    pro
-00025410: 6365 7373 6564 203d 2073 6574 2829 0a0a  cessed = set()..
-00025420: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
-00025430: 745f 7072 6f63 6573 7365 6428 6669 6c65  t_processed(file
-00025440: 6e61 6d65 733a 2049 7465 7261 626c 655b  names: Iterable[
-00025450: 7374 725d 293a 0a20 2020 2020 2020 2066  str]):.        f
-00025460: 6f72 2066 696c 656e 616d 6520 696e 2066  or filename in f
-00025470: 696c 656e 616d 6573 3a0a 2020 2020 2020  ilenames:.      
-00025480: 2020 2020 2020 2320 6a75 7374 2070 726f        # just pro
-00025490: 6365 7373 2063 6861 6e67 6564 2066 696c  cess changed fil
-000254a0: 656e 616d 6573 2028 7462 2064 6570 6c6f  enames (tb deplo
-000254b0: 7920 616e 6420 2d2d 6f6e 6c79 2d63 6861  y and --only-cha
-000254c0: 6e67 6573 290a 2020 2020 2020 2020 2020  nges).          
-000254d0: 2020 6966 2063 6861 6e67 6564 3a0a 2020    if changed:.  
-000254e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000254f0: 736f 7572 6365 203d 2050 6174 6828 6669  source = Path(fi
-00025500: 6c65 6e61 6d65 292e 7265 736f 6c76 6528  lename).resolve(
-00025510: 292e 7374 656d 0a20 2020 2020 2020 2020  ).stem.         
-00025520: 2020 2020 2020 2069 6620 7265 736f 7572         if resour
-00025530: 6365 2069 6e20 6368 616e 6765 6420 616e  ce in changed an
-00025540: 6420 286e 6f74 2063 6861 6e67 6564 5b72  d (not changed[r
-00025550: 6573 6f75 7263 655d 206f 7220 6368 616e  esource] or chan
-00025560: 6765 645b 7265 736f 7572 6365 5d20 696e  ged[resource] in
-00025570: 205b 2273 6861 7265 6422 2c20 2272 656d   ["shared", "rem
-00025580: 6f74 6522 5d29 3a0a 2020 2020 2020 2020  ote"]):.        
-00025590: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000255a0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-000255b0: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
-000255c0: 7228 6669 6c65 6e61 6d65 293a 0a20 2020  r(filename):.   
-000255d0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-000255e0: 6974 2067 6574 5f70 726f 6365 7373 6564  it get_processed
-000255f0: 2866 696c 656e 616d 6573 3d67 6574 5f70  (filenames=get_p
-00025600: 726f 6a65 6374 5f66 696c 656e 616d 6573  roject_filenames
-00025610: 2866 696c 656e 616d 6529 290a 2020 2020  (filename)).    
-00025620: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00025630: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00025640: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00025650: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00025660: 6963 6b2e 6563 686f 2846 6565 6462 6163  ick.echo(Feedbac
-00025670: 6b4d 616e 6167 6572 2e69 6e66 6f5f 7072  kManager.info_pr
-00025680: 6f63 6573 7369 6e67 5f66 696c 6528 6669  ocessing_file(fi
-00025690: 6c65 6e61 6d65 3d66 696c 656e 616d 6529  lename=filename)
-000256a0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-000256b0: 2020 2069 6620 222e 696e 636c 2220 696e     if ".incl" in
-000256c0: 2066 696c 656e 616d 653a 0a20 2020 2020   filename:.     
-000256d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000256e0: 6c69 636b 2e65 6368 6f28 4665 6564 6261  lick.echo(Feedba
-000256f0: 636b 4d61 6e61 6765 722e 7761 726e 696e  ckManager.warnin
-00025700: 675f 736b 6970 7069 6e67 5f69 6e63 6c75  g_skipping_inclu
-00025710: 6465 5f66 696c 6528 6669 6c65 3d66 696c  de_file(file=fil
-00025720: 656e 616d 6529 290a 0a20 2020 2020 2020  ename))..       
-00025730: 2020 2020 2020 2020 206e 616d 6520 3d20           name = 
-00025740: 6177 6169 7420 7072 6f63 6573 7328 6669  await process(fi
-00025750: 6c65 6e61 6d65 2c20 6465 7073 2c20 6465  lename, deps, de
-00025760: 705f 6d61 702c 2074 6f5f 7275 6e2c 2077  p_map, to_run, w
-00025770: 6f72 6b73 7061 6365 5f6c 6962 5f70 6174  orkspace_lib_pat
-00025780: 6873 290a 2020 2020 2020 2020 2020 2020  hs).            
-00025790: 2020 2020 7072 6f63 6573 7365 642e 6164      processed.ad
-000257a0: 6428 6e61 6d65 290a 0a20 2020 2061 7761  d(name)..    awa
-000257b0: 6974 2067 6574 5f70 726f 6365 7373 6564  it get_processed
-000257c0: 2866 696c 656e 616d 6573 3d66 696c 656e  (filenames=filen
-000257d0: 616d 6573 290a 0a20 2020 2069 6620 7072  ames)..    if pr
-000257e0: 6f63 6573 735f 6465 7065 6e64 656e 6369  ocess_dependenci
-000257f0: 6573 3a0a 2020 2020 2020 2020 6966 206f  es:.        if o
-00025800: 6e6c 795f 6368 616e 6765 733a 0a20 2020  nly_changes:.   
-00025810: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
-00025820: 2069 6e20 6469 6374 2874 6f5f 7275 6e29   in dict(to_run)
-00025830: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00025840: 2020 2320 6c6f 6f6b 2066 6f72 2064 6570    # look for dep
-00025850: 7320 7468 6174 2061 7265 2074 6865 2074  s that are the t
-00025860: 6172 6765 7420 6461 7461 2073 6f75 7263  arget data sourc
-00025870: 6520 6f66 2061 206d 6174 6572 6961 6c69  e of a materiali
-00025880: 7a65 6420 6e6f 6465 0a20 2020 2020 2020  zed node.       
-00025890: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-000258a0: 6461 7461 736f 7572 6365 203d 2067 6574  datasource = get
-000258b0: 5f74 6172 6765 745f 6d61 7465 7269 616c  _target_material
-000258c0: 697a 6564 5f64 6174 615f 736f 7572 6365  ized_data_source
-000258d0: 5f6e 616d 6528 746f 5f72 756e 5b6b 6579  _name(to_run[key
-000258e0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-000258f0: 2020 2069 6620 7461 7267 6574 5f64 6174     if target_dat
-00025900: 6173 6f75 7263 653a 0a20 2020 2020 2020  asource:.       
-00025910: 2020 2020 2020 2020 2020 2020 2023 206c               # l
-00025920: 6f6f 6b20 696e 2061 6c6c 5f64 6570 5f6d  ook in all_dep_m
-00025930: 6170 2069 7465 6d73 2074 6861 7420 6861  ap items that ha
-00025940: 7665 2061 7320 6120 6465 7065 6e64 656e  ve as a dependen
-00025950: 6379 2074 6865 2074 6172 6765 7420 6461  cy the target da
-00025960: 7461 2073 6f75 7263 6520 616e 6420 6172  ta source and ar
-00025970: 6520 616e 2065 6e64 706f 696e 740a 2020  e an endpoint.  
-00025980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025990: 2020 666f 7220 5f6b 6579 2c20 5f64 6570    for _key, _dep
-000259a0: 7320 696e 2061 6c6c 5f64 6570 5f6d 6170  s in all_dep_map
-000259b0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-000259c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259d0: 2020 666f 7220 6465 7020 696e 205f 6465    for dep in _de
-000259e0: 7073 3a0a 2020 2020 2020 2020 2020 2020  ps:.            
+00025090: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+000250a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250b0: 2020 2020 2020 2065 6d62 6564 6465 645f         embedded_
+000250c0: 6461 7461 736f 7572 6365 735b 785d 203d  datasources[x] =
+000250d0: 2074 6f5f 7275 6e5b 6473 5f66 6e5d 0a20   to_run[ds_fn]. 
+000250e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00025100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025110: 2065 5f64 7320 3d20 656d 6265 6464 6564   e_ds = embedded
+00025120: 5f64 6174 6173 6f75 7263 6573 2e67 6574  _datasources.get
+00025130: 2878 2c20 4e6f 6e65 290a 2020 2020 2020  (x, None).      
+00025140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025150: 2020 6966 2065 5f64 733a 0a20 2020 2020    if e_ds:.     
+00025160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025170: 2020 2020 2020 2064 6570 5f6c 6973 742e         dep_list.
+00025180: 6170 7065 6e64 2865 5f64 735b 2272 6573  append(e_ds["res
+00025190: 6f75 7263 655f 6e61 6d65 225d 290a 0a20  ource_name"]).. 
+000251a0: 2020 2020 2020 2020 2020 2023 2049 6e20             # In 
+000251b0: 6361 7365 2074 6865 2064 6174 6173 6f75  case the datasou
+000251c0: 7263 6520 6973 2074 6f20 6265 2073 6861  rce is to be sha
+000251d0: 7265 6420 616e 6420 7765 2068 6176 6520  red and we have 
+000251e0: 6d61 7070 696e 672c 206c 6574 2773 2072  mapping, let's r
+000251f0: 6570 6c61 6365 2074 6865 206e 616d 650a  eplace the name.
+00025200: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00025210: 7368 6172 6564 5f77 6974 6822 2069 6e20  shared_with" in 
+00025220: 7220 616e 6420 776f 726b 7370 6163 655f  r and workspace_
+00025230: 6d61 703a 0a20 2020 2020 2020 2020 2020  map:.           
+00025240: 2020 2020 206d 6170 7065 645f 776f 726b       mapped_work
+00025250: 7370 6163 6573 3a20 4c69 7374 5b73 7472  spaces: List[str
+00025260: 5d20 3d20 5b5d 0a20 2020 2020 2020 2020  ] = [].         
+00025270: 2020 2020 2020 2066 6f72 2073 6861 7265         for share
+00025280: 645f 7769 7468 2069 6e20 725b 2273 6861  d_with in r["sha
+00025290: 7265 645f 7769 7468 225d 3a0a 2020 2020  red_with"]:.    
+000252a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000252b0: 6d61 7070 6564 5f77 6f72 6b73 7061 6365  mapped_workspace
+000252c0: 732e 6170 7065 6e64 280a 2020 2020 2020  s.append(.      
+000252d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000252e0: 2020 776f 726b 7370 6163 655f 6d61 702e    workspace_map.
+000252f0: 6765 7428 7368 6172 6564 5f77 6974 6829  get(shared_with)
+00025300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025310: 2020 2020 2020 2020 2069 6620 776f 726b           if work
+00025320: 7370 6163 655f 6d61 702e 6765 7428 7368  space_map.get(sh
+00025330: 6172 6564 5f77 6974 682c 204e 6f6e 6529  ared_with, None)
+00025340: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+00025350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025360: 2020 2020 2065 6c73 6520 7368 6172 6564       else shared
+00025370: 5f77 6974 680a 2020 2020 2020 2020 2020  _with.          
+00025380: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00025390: 2020 2020 2020 2020 2020 2020 725b 2273              r["s
+000253a0: 6861 7265 645f 7769 7468 225d 203d 206d  hared_with"] = m
+000253b0: 6170 7065 645f 776f 726b 7370 6163 6573  apped_workspaces
+000253c0: 0a0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+000253d0: 705f 6d61 705b 666e 5d20 3d20 7365 7428  p_map[fn] = set(
+000253e0: 6465 705f 6c69 7374 290a 2020 2020 2020  dep_list).      
+000253f0: 2020 7265 7475 726e 206f 732e 7061 7468    return os.path
+00025400: 2e62 6173 656e 616d 6528 6e61 6d65 290a  .basename(name).
+00025410: 0a20 2020 2070 726f 6365 7373 6564 203d  .    processed =
+00025420: 2073 6574 2829 0a0a 2020 2020 6173 796e   set()..    asyn
+00025430: 6320 6465 6620 6765 745f 7072 6f63 6573  c def get_proces
+00025440: 7365 6428 6669 6c65 6e61 6d65 733a 2049  sed(filenames: I
+00025450: 7465 7261 626c 655b 7374 725d 293a 0a20  terable[str]):. 
+00025460: 2020 2020 2020 2066 6f72 2066 696c 656e         for filen
+00025470: 616d 6520 696e 2066 696c 656e 616d 6573  ame in filenames
+00025480: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00025490: 6a75 7374 2070 726f 6365 7373 2063 6861  just process cha
+000254a0: 6e67 6564 2066 696c 656e 616d 6573 2028  nged filenames (
+000254b0: 7462 2064 6570 6c6f 7920 616e 6420 2d2d  tb deploy and --
+000254c0: 6f6e 6c79 2d63 6861 6e67 6573 290a 2020  only-changes).  
+000254d0: 2020 2020 2020 2020 2020 6966 2063 6861            if cha
+000254e0: 6e67 6564 3a0a 2020 2020 2020 2020 2020  nged:.          
+000254f0: 2020 2020 2020 7265 736f 7572 6365 203d        resource =
+00025500: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
+00025510: 7265 736f 6c76 6528 292e 7374 656d 0a20  resolve().stem. 
+00025520: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00025530: 6620 7265 736f 7572 6365 2069 6e20 6368  f resource in ch
+00025540: 616e 6765 6420 616e 6420 286e 6f74 2063  anged and (not c
+00025550: 6861 6e67 6564 5b72 6573 6f75 7263 655d  hanged[resource]
+00025560: 206f 7220 6368 616e 6765 645b 7265 736f   or changed[reso
+00025570: 7572 6365 5d20 696e 205b 2273 6861 7265  urce] in ["share
+00025580: 6422 2c20 2272 656d 6f74 6522 5d29 3a0a  d", "remote"]):.
+00025590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000255a0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+000255b0: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+000255c0: 6174 682e 6973 6469 7228 6669 6c65 6e61  ath.isdir(filena
+000255d0: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
+000255e0: 2020 2020 2061 7761 6974 2067 6574 5f70       await get_p
+000255f0: 726f 6365 7373 6564 2866 696c 656e 616d  rocessed(filenam
+00025600: 6573 3d67 6574 5f70 726f 6a65 6374 5f66  es=get_project_f
+00025610: 696c 656e 616d 6573 2866 696c 656e 616d  ilenames(filenam
+00025620: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+00025630: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00025640: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00025650: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025660: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
+00025670: 2846 6565 6462 6163 6b4d 616e 6167 6572  (FeedbackManager
+00025680: 2e69 6e66 6f5f 7072 6f63 6573 7369 6e67  .info_processing
+00025690: 5f66 696c 6528 6669 6c65 6e61 6d65 3d66  _file(filename=f
+000256a0: 696c 656e 616d 6529 290a 0a20 2020 2020  ilename))..     
+000256b0: 2020 2020 2020 2020 2020 2069 6620 222e             if ".
+000256c0: 696e 636c 2220 696e 2066 696c 656e 616d  incl" in filenam
+000256d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000256e0: 2020 2020 2020 2063 6c69 636b 2e65 6368         click.ech
+000256f0: 6f28 4665 6564 6261 636b 4d61 6e61 6765  o(FeedbackManage
+00025700: 722e 7761 726e 696e 675f 736b 6970 7069  r.warning_skippi
+00025710: 6e67 5f69 6e63 6c75 6465 5f66 696c 6528  ng_include_file(
+00025720: 6669 6c65 3d66 696c 656e 616d 6529 290a  file=filename)).
+00025730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025740: 206e 616d 6520 3d20 6177 6169 7420 7072   name = await pr
+00025750: 6f63 6573 7328 6669 6c65 6e61 6d65 2c20  ocess(filename, 
+00025760: 6465 7073 2c20 6465 705f 6d61 702c 2074  deps, dep_map, t
+00025770: 6f5f 7275 6e2c 2077 6f72 6b73 7061 6365  o_run, workspace
+00025780: 5f6c 6962 5f70 6174 6873 290a 2020 2020  _lib_paths).    
+00025790: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+000257a0: 6573 7365 642e 6164 6428 6e61 6d65 290a  essed.add(name).
+000257b0: 0a20 2020 2061 7761 6974 2067 6574 5f70  .    await get_p
+000257c0: 726f 6365 7373 6564 2866 696c 656e 616d  rocessed(filenam
+000257d0: 6573 3d66 696c 656e 616d 6573 290a 0a20  es=filenames).. 
+000257e0: 2020 2069 6620 7072 6f63 6573 735f 6465     if process_de
+000257f0: 7065 6e64 656e 6369 6573 3a0a 2020 2020  pendencies:.    
+00025800: 2020 2020 6966 206f 6e6c 795f 6368 616e      if only_chan
+00025810: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
+00025820: 2066 6f72 206b 6579 2069 6e20 6469 6374   for key in dict
+00025830: 2874 6f5f 7275 6e29 3a0a 2020 2020 2020  (to_run):.      
+00025840: 2020 2020 2020 2020 2020 2320 6c6f 6f6b            # look
+00025850: 2066 6f72 2064 6570 7320 7468 6174 2061   for deps that a
+00025860: 7265 2074 6865 2074 6172 6765 7420 6461  re the target da
+00025870: 7461 2073 6f75 7263 6520 6f66 2061 206d  ta source of a m
+00025880: 6174 6572 6961 6c69 7a65 6420 6e6f 6465  aterialized node
+00025890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000258a0: 2074 6172 6765 745f 6461 7461 736f 7572   target_datasour
+000258b0: 6365 203d 2067 6574 5f74 6172 6765 745f  ce = get_target_
+000258c0: 6d61 7465 7269 616c 697a 6564 5f64 6174  materialized_dat
+000258d0: 615f 736f 7572 6365 5f6e 616d 6528 746f  a_source_name(to
+000258e0: 5f72 756e 5b6b 6579 5d29 0a20 2020 2020  _run[key]).     
+000258f0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00025900: 7267 6574 5f64 6174 6173 6f75 7263 653a  rget_datasource:
+00025910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025920: 2020 2020 2023 206c 6f6f 6b20 696e 2061       # look in a
+00025930: 6c6c 5f64 6570 5f6d 6170 2069 7465 6d73  ll_dep_map items
+00025940: 2074 6861 7420 6861 7665 2061 7320 6120   that have as a 
+00025950: 6465 7065 6e64 656e 6379 2074 6865 2074  dependency the t
+00025960: 6172 6765 7420 6461 7461 2073 6f75 7263  arget data sourc
+00025970: 6520 616e 6420 6172 6520 616e 2065 6e64  e and are an end
+00025980: 706f 696e 740a 2020 2020 2020 2020 2020  point.          
+00025990: 2020 2020 2020 2020 2020 666f 7220 5f6b            for _k
+000259a0: 6579 2c20 5f64 6570 7320 696e 2061 6c6c  ey, _deps in all
+000259b0: 5f64 6570 5f6d 6170 2e69 7465 6d73 2829  _dep_map.items()
+000259c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000259d0: 2020 2020 2020 2020 2020 666f 7220 6465            for de
+000259e0: 7020 696e 205f 6465 7073 3a0a 2020 2020  p in _deps:.    
 000259f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a00: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00025a00: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
 00025a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a20: 2020 2020 2064 6570 203d 3d20 7461 7267       dep == targ
-00025a30: 6574 5f64 6174 6173 6f75 7263 650a 2020  et_datasource.  
-00025a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a50: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00025a60: 2028 6465 7020 3d3d 206b 6579 2061 6e64   (dep == key and
-00025a70: 2074 6172 6765 745f 6461 7461 736f 7572   target_datasour
-00025a80: 6365 206e 6f74 2069 6e20 616c 6c5f 6465  ce not in all_de
-00025a90: 705f 6d61 702e 6765 7428 6b65 792c 205b  p_map.get(key, [
-00025aa0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00025a20: 2020 2020 2020 2020 2020 2020 2064 6570               dep
+00025a30: 203d 3d20 7461 7267 6574 5f64 6174 6173   == target_datas
+00025a40: 6f75 7263 650a 2020 2020 2020 2020 2020  ource.          
+00025a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a60: 2020 2020 2020 6f72 2028 6465 7020 3d3d        or (dep ==
+00025a70: 206b 6579 2061 6e64 2074 6172 6765 745f   key and target_
+00025a80: 6461 7461 736f 7572 6365 206e 6f74 2069  datasource not i
+00025a90: 6e20 616c 6c5f 6465 705f 6d61 702e 6765  n all_dep_map.ge
+00025aa0: 7428 6b65 792c 205b 5d29 290a 2020 2020  t(key, [])).    
 00025ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ac0: 2920 616e 6420 6973 5f65 6e64 706f 696e  ) and is_endpoin
-00025ad0: 745f 7769 7468 5f6e 6f5f 6465 7065 6e64  t_with_no_depend
-00025ae0: 656e 6369 6573 280a 2020 2020 2020 2020  encies(.        
+00025ac0: 2020 2020 2020 2020 2920 616e 6420 6973          ) and is
+00025ad0: 5f65 6e64 706f 696e 745f 7769 7468 5f6e  _endpoint_with_n
+00025ae0: 6f5f 6465 7065 6e64 656e 6369 6573 280a  o_dependencies(.
 00025af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b00: 2020 2020 2020 2020 616c 6c5f 7265 736f          all_reso
-00025b10: 7572 6365 732e 6765 7428 5f6b 6579 2c20  urces.get(_key, 
-00025b20: 7b7d 292c 2061 6c6c 5f64 6570 5f6d 6170  {}), all_dep_map
-00025b30: 2c20 616c 6c5f 7265 736f 7572 6365 730a  , all_resources.
-00025b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b50: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-00025b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b70: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00025b80: 6570 5f6d 6170 5b5f 6b65 795d 203d 205f  ep_map[_key] = _
-00025b90: 6465 7073 0a20 2020 2020 2020 2020 2020  deps.           
+00025b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b10: 616c 6c5f 7265 736f 7572 6365 732e 6765  all_resources.ge
+00025b20: 7428 5f6b 6579 2c20 7b7d 292c 2061 6c6c  t(_key, {}), all
+00025b30: 5f64 6570 5f6d 6170 2c20 616c 6c5f 7265  _dep_map, all_re
+00025b40: 736f 7572 6365 730a 2020 2020 2020 2020  sources.        
+00025b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b60: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00025b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b80: 2020 2020 2020 2064 6570 5f6d 6170 5b5f         dep_map[_
+00025b90: 6b65 795d 203d 205f 6465 7073 0a20 2020  key] = _deps.   
 00025ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025bb0: 2020 2020 2074 6f5f 7275 6e5b 5f6b 6579       to_run[_key
-00025bc0: 5d20 3d20 616c 6c5f 7265 736f 7572 6365  ] = all_resource
-00025bd0: 732e 6765 7428 5f6b 6579 290a 2020 2020  s.get(_key).    
-00025be0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00025bf0: 2020 2020 2020 7768 696c 6520 6c65 6e28        while len(
-00025c00: 6465 7073 2920 3e20 303a 0a20 2020 2020  deps) > 0:.     
-00025c10: 2020 2020 2020 2020 2020 2064 6570 203d             dep =
-00025c20: 2064 6570 732e 706f 7028 290a 2020 2020   deps.pop().    
-00025c30: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00025c40: 6570 206e 6f74 2069 6e20 7072 6f63 6573  ep not in proces
-00025c50: 7365 643a 0a20 2020 2020 2020 2020 2020  sed:.           
-00025c60: 2020 2020 2020 2020 2070 726f 6365 7373           process
-00025c70: 6564 2e61 6464 2864 6570 290a 2020 2020  ed.add(dep).    
-00025c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025c90: 6620 3d20 6675 6c6c 5f70 6174 685f 6279  f = full_path_by
-00025ca0: 5f6e 616d 6528 6469 725f 7061 7468 2c20  _name(dir_path, 
-00025cb0: 6465 702c 2077 6f72 6b73 7061 6365 5f6c  dep, workspace_l
-00025cc0: 6962 5f70 6174 6873 290a 2020 2020 2020  ib_paths).      
-00025cd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00025ce0: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-00025cf0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00025d00: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+00025bb0: 2020 2020 2020 2020 2020 2020 2074 6f5f               to_
+00025bc0: 7275 6e5b 5f6b 6579 5d20 3d20 616c 6c5f  run[_key] = all_
+00025bd0: 7265 736f 7572 6365 732e 6765 7428 5f6b  resources.get(_k
+00025be0: 6579 290a 2020 2020 2020 2020 656c 7365  ey).        else
+00025bf0: 3a0a 2020 2020 2020 2020 2020 2020 7768  :.            wh
+00025c00: 696c 6520 6c65 6e28 6465 7073 2920 3e20  ile len(deps) > 
+00025c10: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00025c20: 2020 2064 6570 203d 2064 6570 732e 706f     dep = deps.po
+00025c30: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00025c40: 2020 2020 6966 2064 6570 206e 6f74 2069      if dep not i
+00025c50: 6e20 7072 6f63 6573 7365 643a 0a20 2020  n processed:.   
+00025c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c70: 2070 726f 6365 7373 6564 2e61 6464 2864   processed.add(d
+00025c80: 6570 290a 2020 2020 2020 2020 2020 2020  ep).            
+00025c90: 2020 2020 2020 2020 6620 3d20 6675 6c6c          f = full
+00025ca0: 5f70 6174 685f 6279 5f6e 616d 6528 6469  _path_by_name(di
+00025cb0: 725f 7061 7468 2c20 6465 702c 2077 6f72  r_path, dep, wor
+00025cc0: 6b73 7061 6365 5f6c 6962 5f70 6174 6873  kspace_lib_paths
+00025cd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00025ce0: 2020 2020 2020 6966 2066 3a0a 2020 2020        if f:.    
+00025cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d00: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
 00025d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d20: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00025d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d40: 2020 2020 2020 2020 2070 726f 6365 7373           process
-00025d50: 6564 5f66 696c 656e 616d 6520 3d20 662e  ed_filename = f.
-00025d60: 7265 6c61 7469 7665 5f74 6f28 6f73 2e67  relative_to(os.g
-00025d70: 6574 6377 6428 2929 0a20 2020 2020 2020  etcwd()).       
-00025d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d90: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-00025da0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00025d20: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00025d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d50: 2070 726f 6365 7373 6564 5f66 696c 656e   processed_filen
+00025d60: 616d 6520 3d20 662e 7265 6c61 7469 7665  ame = f.relative
+00025d70: 5f74 6f28 6f73 2e67 6574 6377 6428 2929  _to(os.getcwd())
+00025d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025d90: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00025da0: 6570 7420 5661 6c75 6545 7272 6f72 3a0a  ept ValueError:.
 00025db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025dc0: 2020 2020 2020 2020 7072 6f63 6573 7365          processe
-00025dd0: 645f 6669 6c65 6e61 6d65 203d 2066 0a20  d_filename = f. 
-00025de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025df0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-00025e00: 2e65 6368 6f28 4665 6564 6261 636b 4d61  .echo(FeedbackMa
-00025e10: 6e61 6765 722e 696e 666f 5f70 726f 6365  nager.info_proce
-00025e20: 7373 696e 675f 6669 6c65 2866 696c 656e  ssing_file(filen
-00025e30: 616d 653d 7072 6f63 6573 7365 645f 6669  ame=processed_fi
-00025e40: 6c65 6e61 6d65 2929 0a20 2020 2020 2020  lename)).       
-00025e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e60: 2061 7761 6974 2070 726f 6365 7373 2873   await process(s
-00025e70: 7472 2866 292c 2064 6570 732c 2064 6570  tr(f), deps, dep
-00025e80: 5f6d 6170 2c20 746f 5f72 756e 2c20 776f  _map, to_run, wo
-00025e90: 726b 7370 6163 655f 6c69 625f 7061 7468  rkspace_lib_path
-00025ea0: 7329 0a0a 2020 2020 7265 7475 726e 2047  s)..    return G
-00025eb0: 7261 7068 4465 7065 6e64 656e 6369 6573  raphDependencies
-00025ec0: 2864 6570 5f6d 6170 2c20 746f 5f72 756e  (dep_map, to_run
-00025ed0: 2c20 616c 6c5f 6465 705f 6d61 702c 2061  , all_dep_map, a
-00025ee0: 6c6c 5f72 6573 6f75 7263 6573 290a 0a0a  ll_resources)...
-00025ef0: 6173 796e 6320 6465 6620 6765 745f 6368  async def get_ch
-00025f00: 616e 6765 735f 6672 6f6d 5f6d 6169 6e28  anges_from_main(
-00025f10: 0a20 2020 206f 6e6c 795f 6368 616e 6765  .    only_change
-00025f20: 733a 2062 6f6f 6c2c 0a20 2020 2063 6c69  s: bool,.    cli
-00025f30: 656e 743a 2054 696e 7942 2c0a 2020 2020  ent: TinyB,.    
-00025f40: 636f 6e66 6967 3a20 4f70 7469 6f6e 616c  config: Optional
-00025f50: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
-00025f60: 203d 204e 6f6e 652c 0a20 2020 2063 7572   = None,.    cur
-00025f70: 7265 6e74 5f77 733a 204f 7074 696f 6e61  rent_ws: Optiona
-00025f80: 6c5b 4469 6374 5b73 7472 2c20 416e 795d  l[Dict[str, Any]
-00025f90: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6669  ] = None,.    fi
-00025fa0: 6c65 6e61 6d65 733a 204f 7074 696f 6e61  lenames: Optiona
-00025fb0: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
-00025fc0: 6f6e 652c 0a29 3a0a 2020 2020 6368 616e  one,.):.    chan
-00025fd0: 6765 6420 3d20 4e6f 6e65 0a20 2020 2069  ged = None.    i
-00025fe0: 6620 6e6f 7420 6f6e 6c79 5f63 6861 6e67  f not only_chang
-00025ff0: 6573 3a0a 2020 2020 2020 2020 7265 7475  es:.        retu
-00026000: 726e 2063 6861 6e67 6564 0a0a 2020 2020  rn changed..    
-00026010: 6966 2063 7572 7265 6e74 5f77 7320 616e  if current_ws an
-00026020: 6420 6e6f 7420 6375 7272 656e 745f 7773  d not current_ws
-00026030: 2e67 6574 2822 6973 5f62 7261 6e63 6822  .get("is_branch"
-00026040: 293a 0a20 2020 2020 2020 2063 6861 6e67  ):.        chang
-00026050: 6564 203d 2061 7761 6974 2064 6966 665f  ed = await diff_
-00026060: 636f 6d6d 616e 6428 6669 6c65 6e61 6d65  command(filename
-00026070: 732c 2054 7275 652c 2063 6c69 656e 742c  s, True, client,
-00026080: 206e 6f5f 636f 6c6f 723d 5472 7565 2c20   no_color=True, 
-00026090: 7769 7468 5f70 7269 6e74 3d46 616c 7365  with_print=False
-000260a0: 290a 2020 2020 656c 6966 2063 6f6e 6669  ).    elif confi
-000260b0: 6720 616e 6420 636f 6e66 6967 2e67 6574  g and config.get
-000260c0: 2822 686f 7374 2229 3a0a 2020 2020 2020  ("host"):.      
-000260d0: 2020 776f 726b 7370 6163 6520 3d20 6177    workspace = aw
-000260e0: 6169 7420 6765 745f 6375 7272 656e 745f  ait get_current_
-000260f0: 6d61 696e 5f77 6f72 6b73 7061 6365 2863  main_workspace(c
-00026100: 6c69 656e 742c 2063 6f6e 6669 6729 0a0a  lient, config)..
-00026110: 2020 2020 2020 2020 6966 2077 6f72 6b73          if works
-00026120: 7061 6365 3a0a 2020 2020 2020 2020 2020  pace:.          
-00026130: 2020 7773 5f63 6c69 656e 7420 3d20 5f67    ws_client = _g
-00026140: 6574 5f74 625f 636c 6965 6e74 2877 6f72  et_tb_client(wor
-00026150: 6b73 7061 6365 5b22 746f 6b65 6e22 5d2c  kspace["token"],
-00026160: 2063 6f6e 6669 675b 2268 6f73 7422 5d29   config["host"])
-00026170: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-00026180: 6e67 6564 203d 2061 7761 6974 2064 6966  nged = await dif
-00026190: 665f 636f 6d6d 616e 6428 6669 6c65 6e61  f_command(filena
-000261a0: 6d65 732c 2054 7275 652c 2077 735f 636c  mes, True, ws_cl
-000261b0: 6965 6e74 2c20 6e6f 5f63 6f6c 6f72 3d54  ient, no_color=T
-000261c0: 7275 652c 2077 6974 685f 7072 696e 743d  rue, with_print=
-000261d0: 4661 6c73 6529 0a20 2020 2072 6574 7572  False).    retur
-000261e0: 6e20 6368 616e 6765 640a 0a0a 6465 6620  n changed...def 
-000261f0: 6765 745f 7072 6f6a 6563 745f 6669 6c65  get_project_file
-00026200: 6e61 6d65 7328 666f 6c64 6572 3a20 7374  names(folder: st
-00026210: 722c 2077 6974 685f 7665 6e64 6f72 3d46  r, with_vendor=F
-00026220: 616c 7365 2920 2d3e 204c 6973 745b 7374  alse) -> List[st
-00026230: 725d 3a0a 2020 2020 666f 6c64 6572 733a  r]:.    folders:
-00026240: 204c 6973 745b 7374 725d 203d 205b 0a20   List[str] = [. 
-00026250: 2020 2020 2020 2066 227b 666f 6c64 6572         f"{folder
-00026260: 7d2f 2a2e 6461 7461 736f 7572 6365 222c  }/*.datasource",
-00026270: 0a20 2020 2020 2020 2066 227b 666f 6c64  .        f"{fold
-00026280: 6572 7d2f 6461 7461 736f 7572 6365 732f  er}/datasources/
-00026290: 2a2e 6461 7461 736f 7572 6365 222c 0a20  *.datasource",. 
-000262a0: 2020 2020 2020 2066 227b 666f 6c64 6572         f"{folder
-000262b0: 7d2f 2a2e 7069 7065 222c 0a20 2020 2020  }/*.pipe",.     
-000262c0: 2020 2066 227b 666f 6c64 6572 7d2f 7069     f"{folder}/pi
-000262d0: 7065 732f 2a2e 7069 7065 222c 0a20 2020  pes/*.pipe",.   
-000262e0: 2020 2020 2066 227b 666f 6c64 6572 7d2f       f"{folder}/
-000262f0: 656e 6470 6f69 6e74 732f 2a2e 7069 7065  endpoints/*.pipe
-00026300: 222c 0a20 2020 2020 2020 2066 227b 666f  ",.        f"{fo
-00026310: 6c64 6572 7d2f 2a2e 746f 6b65 6e22 2c0a  lder}/*.token",.
-00026320: 2020 2020 2020 2020 6622 7b66 6f6c 6465          f"{folde
-00026330: 727d 2f74 6f6b 656e 732f 2a2e 746f 6b65  r}/tokens/*.toke
-00026340: 6e22 2c0a 2020 2020 5d0a 2020 2020 6966  n",.    ].    if
-00026350: 2077 6974 685f 7665 6e64 6f72 3a0a 2020   with_vendor:.  
-00026360: 2020 2020 2020 666f 6c64 6572 732e 6170        folders.ap
-00026370: 7065 6e64 2866 227b 666f 6c64 6572 7d2f  pend(f"{folder}/
-00026380: 7665 6e64 6f72 2f2a 2a2f 2a2a 2f2a 2e64  vendor/**/**/*.d
-00026390: 6174 6173 6f75 7263 6522 290a 2020 2020  atasource").    
-000263a0: 6669 6c65 6e61 6d65 733a 204c 6973 745b  filenames: List[
-000263b0: 7374 725d 203d 205b 5d0a 2020 2020 666f  str] = [].    fo
-000263c0: 7220 7820 696e 2066 6f6c 6465 7273 3a0a  r x in folders:.
-000263d0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-000263e0: 7320 2b3d 2067 6c6f 622e 676c 6f62 2878  s += glob.glob(x
-000263f0: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
-00026400: 656e 616d 6573 0a0a 0a64 6566 2069 735f  enames...def is_
-00026410: 6e65 7728 0a20 2020 206e 616d 653a 2073  new(.    name: s
-00026420: 7472 2c0a 2020 2020 6368 616e 6765 643a  tr,.    changed:
-00026430: 2044 6963 745b 7374 722c 2073 7472 5d2c   Dict[str, str],
-00026440: 0a20 2020 206e 6f72 6d61 6c5f 6465 7065  .    normal_depe
-00026450: 6e64 656e 6379 3a20 4469 6374 5b73 7472  ndency: Dict[str
-00026460: 2c20 5365 745b 7374 725d 5d2c 0a20 2020  , Set[str]],.   
-00026470: 2066 6f72 6b5f 646f 776e 7374 7265 616d   fork_downstream
-00026480: 5f64 6570 656e 6465 6e63 793a 2044 6963  _dependency: Dic
-00026490: 745b 7374 722c 2053 6574 5b73 7472 5d5d  t[str, Set[str]]
-000264a0: 2c0a 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ,.) -> bool:.   
-000264b0: 2064 6566 2069 735f 6769 745f 6e65 7728   def is_git_new(
-000264c0: 6e61 6d65 3a20 7374 7229 3a0a 2020 2020  name: str):.    
-000264d0: 2020 2020 7265 7475 726e 2063 6861 6e67      return chang
-000264e0: 6564 2061 6e64 2063 6861 6e67 6564 2e67  ed and changed.g
-000264f0: 6574 286e 616d 6529 203d 3d20 2241 220a  et(name) == "A".
-00026500: 0a20 2020 2069 6620 6e6f 7420 6973 5f67  .    if not is_g
-00026510: 6974 5f6e 6577 286e 616d 6529 3a0a 2020  it_new(name):.  
-00026520: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00026530: 7365 0a0a 2020 2020 2320 6966 2073 686f  se..    # if sho
-00026540: 756c 6420 6e6f 7420 6465 7065 6e64 206f  uld not depend o
-00026550: 6e20 6120 6368 616e 6765 6420 7265 736f  n a changed reso
-00026560: 7572 6365 0a20 2020 2069 6620 6261 636b  urce.    if back
-00026570: 5f64 6570 7320 3a3d 206e 6f72 6d61 6c5f  _deps := normal_
-00026580: 6465 7065 6e64 656e 6379 2e67 6574 286e  dependency.get(n
-00026590: 616d 6529 3a0a 2020 2020 2020 2020 666f  ame):.        fo
-000265a0: 7220 6465 7020 696e 2062 6163 6b5f 6465  r dep in back_de
-000265b0: 7073 3a0a 2020 2020 2020 2020 2020 2020  ps:.            
-000265c0: 6966 2064 6570 2069 6e20 666f 726b 5f64  if dep in fork_d
-000265d0: 6f77 6e73 7472 6561 6d5f 6465 7065 6e64  ownstream_depend
-000265e0: 656e 6379 2061 6e64 206e 6f74 2069 735f  ency and not is_
-000265f0: 6769 745f 6e65 7728 6465 7029 3a0a 2020  git_new(dep):.  
-00026600: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00026610: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-00026620: 7265 7475 726e 2054 7275 650a 0a0a 6173  return True...as
-00026630: 796e 6320 6465 6620 666f 6c64 6572 5f70  ync def folder_p
-00026640: 7573 6828 0a20 2020 2074 625f 636c 6965  ush(.    tb_clie
-00026650: 6e74 3a20 5469 6e79 422c 0a20 2020 2066  nt: TinyB,.    f
-00026660: 696c 656e 616d 6573 3a20 4f70 7469 6f6e  ilenames: Option
-00026670: 616c 5b4c 6973 745b 7374 725d 5d20 3d20  al[List[str]] = 
-00026680: 4e6f 6e65 2c0a 2020 2020 6472 795f 7275  None,.    dry_ru
-00026690: 6e3a 2062 6f6f 6c20 3d20 4661 6c73 652c  n: bool = False,
-000266a0: 0a20 2020 2063 6865 636b 3a20 626f 6f6c  .    check: bool
-000266b0: 203d 2046 616c 7365 2c0a 2020 2020 7075   = False,.    pu
-000266c0: 7368 5f64 6570 733a 2062 6f6f 6c20 3d20  sh_deps: bool = 
-000266d0: 4661 6c73 652c 0a20 2020 206f 6e6c 795f  False,.    only_
-000266e0: 6368 616e 6765 733a 2062 6f6f 6c20 3d20  changes: bool = 
-000266f0: 4661 6c73 652c 0a20 2020 2067 6974 5f72  False,.    git_r
-00026700: 656c 6561 7365 3a20 626f 6f6c 203d 2046  elease: bool = F
-00026710: 616c 7365 2c0a 2020 2020 6465 6275 673a  alse,.    debug:
-00026720: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00026730: 2020 2066 6f72 6365 3a20 626f 6f6c 203d     force: bool =
-00026740: 2046 616c 7365 2c0a 2020 2020 6f76 6572   False,.    over
-00026750: 7269 6465 5f64 6174 6173 6f75 7263 653a  ride_datasource:
-00026760: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00026770: 2020 2066 6f6c 6465 723a 2073 7472 203d     folder: str =
-00026780: 2022 2e22 2c0a 2020 2020 706f 7075 6c61   ".",.    popula
-00026790: 7465 3a20 626f 6f6c 203d 2046 616c 7365  te: bool = False
-000267a0: 2c0a 2020 2020 706f 7075 6c61 7465 5f73  ,.    populate_s
-000267b0: 7562 7365 743d 4e6f 6e65 2c0a 2020 2020  ubset=None,.    
-000267c0: 706f 7075 6c61 7465 5f63 6f6e 6469 7469  populate_conditi
-000267d0: 6f6e 3a20 4f70 7469 6f6e 616c 5b73 7472  on: Optional[str
-000267e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 756e  ] = None,.    un
-000267f0: 6c69 6e6b 5f6f 6e5f 706f 7075 6c61 7465  link_on_populate
-00026800: 5f65 7272 6f72 3a20 626f 6f6c 203d 2046  _error: bool = F
-00026810: 616c 7365 2c0a 2020 2020 7570 6c6f 6164  alse,.    upload
-00026820: 5f66 6978 7475 7265 733a 2062 6f6f 6c20  _fixtures: bool 
-00026830: 3d20 4661 6c73 652c 0a20 2020 2077 6169  = False,.    wai
-00026840: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-00026850: 0a20 2020 2069 676e 6f72 655f 7371 6c5f  .    ignore_sql_
-00026860: 6572 726f 7273 3a20 626f 6f6c 203d 2046  errors: bool = F
-00026870: 616c 7365 2c0a 2020 2020 736b 6970 5f63  alse,.    skip_c
-00026880: 6f6e 6669 726d 6174 696f 6e3a 2062 6f6f  onfirmation: boo
-00026890: 6c20 3d20 4661 6c73 652c 0a20 2020 206f  l = False,.    o
-000268a0: 6e6c 795f 7265 7370 6f6e 7365 5f74 696d  nly_response_tim
-000268b0: 6573 3a20 626f 6f6c 203d 2046 616c 7365  es: bool = False
-000268c0: 2c0a 2020 2020 776f 726b 7370 6163 655f  ,.    workspace_
-000268d0: 6d61 703d 4e6f 6e65 2c0a 2020 2020 776f  map=None,.    wo
-000268e0: 726b 7370 6163 655f 6c69 625f 7061 7468  rkspace_lib_path
-000268f0: 733d 4e6f 6e65 2c0a 2020 2020 6e6f 5f76  s=None,.    no_v
-00026900: 6572 7369 6f6e 733a 2062 6f6f 6c20 3d20  ersions: bool = 
-00026910: 4661 6c73 652c 0a20 2020 2074 696d 656f  False,.    timeo
-00026920: 7574 3d4e 6f6e 652c 0a20 2020 2072 756e  ut=None,.    run
-00026930: 5f74 6573 7473 3a20 626f 6f6c 203d 2046  _tests: bool = F
-00026940: 616c 7365 2c0a 2020 2020 6173 5f73 7461  alse,.    as_sta
-00026950: 6e64 6172 643a 2062 6f6f 6c20 3d20 4661  ndard: bool = Fa
-00026960: 6c73 652c 0a20 2020 2072 6169 7365 5f6f  lse,.    raise_o
-00026970: 6e5f 6578 6973 7473 3a20 626f 6f6c 203d  n_exists: bool =
-00026980: 2046 616c 7365 2c0a 2020 2020 7665 7262   False,.    verb
-00026990: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
-000269a0: 2c0a 2020 2020 7465 7374 735f 746f 5f72  ,.    tests_to_r
-000269b0: 756e 3a20 696e 7420 3d20 302c 0a20 2020  un: int = 0,.   
-000269c0: 2074 6573 7473 5f73 616d 706c 655f 6279   tests_sample_by
-000269d0: 5f70 6172 616d 733a 2069 6e74 203d 2030  _params: int = 0
-000269e0: 2c0a 2020 2020 7465 7374 735f 6669 6c74  ,.    tests_filt
-000269f0: 6572 5f62 793a 204f 7074 696f 6e61 6c5b  er_by: Optional[
-00026a00: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
-00026a10: 652c 0a20 2020 2074 6573 7473 5f66 6169  e,.    tests_fai
-00026a20: 6c66 6173 743a 2062 6f6f 6c20 3d20 4661  lfast: bool = Fa
-00026a30: 6c73 652c 0a20 2020 2074 6573 7473 5f69  lse,.    tests_i
-00026a40: 676e 6f72 655f 6f72 6465 723a 2062 6f6f  gnore_order: boo
-00026a50: 6c20 3d20 4661 6c73 652c 0a20 2020 2074  l = False,.    t
-00026a60: 6573 7473 5f76 616c 6964 6174 655f 7072  ests_validate_pr
-00026a70: 6f63 6573 7365 645f 6279 7465 733a 2062  ocessed_bytes: b
-00026a80: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-00026a90: 2074 6573 7473 5f63 6865 636b 5f72 6571   tests_check_req
-00026aa0: 7565 7374 735f 6672 6f6d 5f62 7261 6e63  uests_from_branc
-00026ab0: 683a 2062 6f6f 6c20 3d20 4661 6c73 652c  h: bool = False,
-00026ac0: 0a20 2020 2063 6f6e 6669 673a 204f 7074  .    config: Opt
-00026ad0: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-00026ae0: 416e 795d 5d20 3d20 4e6f 6e65 2c0a 2020  Any]] = None,.  
-00026af0: 2020 7573 6572 5f74 6f6b 656e 3a20 4f70    user_token: Op
-00026b00: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00026b10: 6e65 2c0a 2020 2020 666f 726b 5f64 6f77  ne,.    fork_dow
-00026b20: 6e73 7472 6561 6d3a 204f 7074 696f 6e61  nstream: Optiona
-00026b30: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-00026b40: 0a20 2020 2066 6f72 6b3a 204f 7074 696f  .    fork: Optio
-00026b50: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
-00026b60: 652c 0a20 2020 2069 735f 696e 7465 726e  e,.    is_intern
-00026b70: 616c 3a20 4f70 7469 6f6e 616c 5b62 6f6f  al: Optional[boo
-00026b80: 6c5d 203d 2046 616c 7365 2c0a 2020 2020  l] = False,.    
-00026b90: 7265 6c65 6173 655f 6372 6561 7465 643a  release_created:
-00026ba0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-00026bb0: 3d20 4661 6c73 652c 0a20 2020 2061 7574  = False,.    aut
-00026bc0: 6f5f 7072 6f6d 6f74 653a 204f 7074 696f  o_promote: Optio
-00026bd0: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
-00026be0: 652c 0a20 2020 2063 6865 636b 5f62 6163  e,.    check_bac
-00026bf0: 6b66 696c 6c5f 7265 7175 6972 6564 3a20  kfill_required: 
-00026c00: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00026c10: 2020 7573 655f 6d61 696e 3a20 626f 6f6c    use_main: bool
-00026c20: 203d 2046 616c 7365 2c0a 293a 2020 2320   = False,.):  # 
-00026c30: 6e6f 7161 3a20 4339 3031 0a20 2020 2077  noqa: C901.    w
-00026c40: 6f72 6b73 7061 6365 733a 204c 6973 745b  orkspaces: List[
-00026c50: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-00026c60: 3d20 2861 7761 6974 2074 625f 636c 6965  = (await tb_clie
-00026c70: 6e74 2e75 7365 725f 776f 726b 7370 6163  nt.user_workspac
-00026c80: 6573 5f61 6e64 5f62 7261 6e63 6865 7328  es_and_branches(
-00026c90: 2929 2e67 6574 2822 776f 726b 7370 6163  )).get("workspac
-00026ca0: 6573 222c 205b 5d29 0a20 2020 2063 7572  es", []).    cur
-00026cb0: 7265 6e74 5f77 733a 2044 6963 745b 7374  rent_ws: Dict[st
-00026cc0: 722c 2041 6e79 5d20 3d20 6e65 7874 280a  r, Any] = next(.
-00026cd0: 2020 2020 2020 2020 2877 6f72 6b73 7061          (workspa
-00026ce0: 6365 2066 6f72 2077 6f72 6b73 7061 6365  ce for workspace
-00026cf0: 2069 6e20 776f 726b 7370 6163 6573 2069   in workspaces i
-00026d00: 6620 636f 6e66 6967 2061 6e64 2077 6f72  f config and wor
-00026d10: 6b73 7061 6365 2e67 6574 2822 6964 222c  kspace.get("id",
-00026d20: 2022 2e22 2920 3d3d 2063 6f6e 6669 672e   ".") == config.
-00026d30: 6765 7428 2269 6422 2c20 222e 2e22 2929  get("id", ".."))
-00026d40: 2c20 7b7d 0a20 2020 2029 0a20 2020 2069  , {}.    ).    i
-00026d50: 735f 6272 616e 6368 203d 2063 7572 7265  s_branch = curre
-00026d60: 6e74 5f77 732e 6765 7428 2269 735f 6272  nt_ws.get("is_br
-00026d70: 616e 6368 222c 2046 616c 7365 290a 2020  anch", False).  
-00026d80: 2020 6861 735f 7365 6d76 6572 3a20 626f    has_semver: bo
-00026d90: 6f6c 203d 2072 656c 6561 7365 5f63 7265  ol = release_cre
-00026da0: 6174 6564 206f 7220 4661 6c73 650a 0a20  ated or False.. 
-00026db0: 2020 2064 6570 6c6f 796d 656e 7420 3d20     deployment = 
-00026dc0: 4465 706c 6f79 6d65 6e74 2863 7572 7265  Deployment(curre
-00026dd0: 6e74 5f77 732c 2067 6974 5f72 656c 6561  nt_ws, git_relea
-00026de0: 7365 2c20 7462 5f63 6c69 656e 742c 2064  se, tb_client, d
-00026df0: 7279 5f72 756e 2c20 6f6e 6c79 5f63 6861  ry_run, only_cha
-00026e00: 6e67 6573 290a 0a20 2020 2069 6620 6e6f  nges)..    if no
-00026e10: 7420 776f 726b 7370 6163 655f 6d61 703a  t workspace_map:
-00026e20: 0a20 2020 2020 2020 2077 6f72 6b73 7061  .        workspa
-00026e30: 6365 5f6d 6170 203d 207b 7d0a 2020 2020  ce_map = {}.    
-00026e40: 6966 206e 6f74 2077 6f72 6b73 7061 6365  if not workspace
-00026e50: 5f6c 6962 5f70 6174 6873 3a0a 2020 2020  _lib_paths:.    
-00026e60: 2020 2020 776f 726b 7370 6163 655f 6c69      workspace_li
-00026e70: 625f 7061 7468 7320 3d20 5b5d 0a0a 2020  b_paths = []..  
-00026e80: 2020 776f 726b 7370 6163 655f 6c69 625f    workspace_lib_
-00026e90: 7061 7468 7320 3d20 6c69 7374 2877 6f72  paths = list(wor
-00026ea0: 6b73 7061 6365 5f6c 6962 5f70 6174 6873  kspace_lib_paths
-00026eb0: 290a 2020 2020 2320 696e 636c 7564 6520  ).    # include 
-00026ec0: 7665 6e64 6f72 206c 6962 7320 7769 7468  vendor libs with
-00026ed0: 6f75 7420 6f76 6572 7269 6469 6e67 2075  out overriding u
-00026ee0: 7365 7220 6f6e 6573 0a20 2020 2065 7869  ser ones.    exi
-00026ef0: 7374 696e 675f 776f 726b 7370 6163 6573  sting_workspaces
-00026f00: 203d 2073 6574 2878 5b31 5d20 666f 7220   = set(x[1] for 
-00026f10: 7820 696e 2077 6f72 6b73 7061 6365 5f6c  x in workspace_l
-00026f20: 6962 5f70 6174 6873 290a 2020 2020 7665  ib_paths).    ve
-00026f30: 6e64 6f72 5f70 6174 6820 3d20 5061 7468  ndor_path = Path
-00026f40: 2822 7665 6e64 6f72 2229 0a20 2020 2069  ("vendor").    i
-00026f50: 6620 7665 6e64 6f72 5f70 6174 682e 6578  f vendor_path.ex
-00026f60: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
-00026f70: 666f 7220 7820 696e 2076 656e 646f 725f  for x in vendor_
-00026f80: 7061 7468 2e69 7465 7264 6972 2829 3a0a  path.iterdir():.
-00026f90: 2020 2020 2020 2020 2020 2020 6966 2078              if x
-00026fa0: 2e69 735f 6469 7228 2920 616e 6420 782e  .is_dir() and x.
-00026fb0: 6e61 6d65 206e 6f74 2069 6e20 6578 6973  name not in exis
-00026fc0: 7469 6e67 5f77 6f72 6b73 7061 6365 733a  ting_workspaces:
-00026fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026fe0: 2077 6f72 6b73 7061 6365 5f6c 6962 5f70   workspace_lib_p
-00026ff0: 6174 6873 2e61 7070 656e 6428 2878 2e6e  aths.append((x.n
-00027000: 616d 652c 2078 2929 0a0a 2020 2020 6461  ame, x))..    da
-00027010: 7461 736f 7572 6365 733a 204c 6973 745b  tasources: List[
-00027020: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-00027030: 3d20 6177 6169 7420 7462 5f63 6c69 656e  = await tb_clien
-00027040: 742e 6461 7461 736f 7572 6365 7328 290a  t.datasources().
-00027050: 2020 2020 7069 7065 733a 204c 6973 745b      pipes: List[
-00027060: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-00027070: 3d20 6177 6169 7420 7462 5f63 6c69 656e  = await tb_clien
-00027080: 742e 7069 7065 7328 6465 7065 6e64 656e  t.pipes(dependen
-00027090: 6369 6573 3d54 7275 6529 0a0a 2020 2020  cies=True)..    
-000270a0: 6578 6973 7469 6e67 5f72 6573 6f75 7263  existing_resourc
-000270b0: 6573 3a20 4c69 7374 5b73 7472 5d20 3d20  es: List[str] = 
-000270c0: 5b78 5b22 6e61 6d65 225d 2066 6f72 2078  [x["name"] for x
-000270d0: 2069 6e20 6461 7461 736f 7572 6365 735d   in datasources]
-000270e0: 202b 205b 785b 226e 616d 6522 5d20 666f   + [x["name"] fo
-000270f0: 7220 7820 696e 2070 6970 6573 5d0a 2020  r x in pipes].  
-00027100: 2020 2320 7265 706c 6163 6520 776f 726b    # replace work
-00027110: 7370 6163 6520 6d61 7070 696e 6720 6e61  space mapping na
-00027120: 6d65 730a 2020 2020 666f 7220 6f6c 645f  mes.    for old_
-00027130: 7773 2c20 6e65 775f 7773 2069 6e20 776f  ws, new_ws in wo
-00027140: 726b 7370 6163 655f 6d61 702e 6974 656d  rkspace_map.item
-00027150: 7328 293a 0a20 2020 2020 2020 2065 7869  s():.        exi
-00027160: 7374 696e 675f 7265 736f 7572 6365 7320  sting_resources 
-00027170: 3d20 5b72 652e 7375 6228 6622 5e7b 6f6c  = [re.sub(f"^{ol
-00027180: 645f 7773 7d5c 2e22 2c20 6622 7b6e 6577  d_ws}\.", f"{new
-00027190: 5f77 737d 2e22 2c20 7829 2066 6f72 2078  _ws}.", x) for x
-000271a0: 2069 6e20 6578 6973 7469 6e67 5f72 6573   in existing_res
-000271b0: 6f75 7263 6573 5d0a 0a20 2020 2072 656d  ources]..    rem
-000271c0: 6f74 655f 7265 736f 7572 6365 5f6e 616d  ote_resource_nam
-000271d0: 6573 203d 205b 6765 745f 7265 6d6f 7465  es = [get_remote
-000271e0: 5f72 6573 6f75 7263 655f 6e61 6d65 5f77  _resource_name_w
-000271f0: 6974 686f 7574 5f76 6572 7369 6f6e 2878  ithout_version(x
-00027200: 2920 666f 7220 7820 696e 2065 7869 7374  ) for x in exist
-00027210: 696e 675f 7265 736f 7572 6365 735d 0a0a  ing_resources]..
-00027220: 2020 2020 2320 7265 706c 6163 6520 776f      # replace wo
-00027230: 726b 7370 6163 6520 6d61 7070 696e 6720  rkspace mapping 
-00027240: 6e61 6d65 730a 2020 2020 666f 7220 6f6c  names.    for ol
-00027250: 645f 7773 2c20 6e65 775f 7773 2069 6e20  d_ws, new_ws in 
-00027260: 776f 726b 7370 6163 655f 6d61 702e 6974  workspace_map.it
-00027270: 656d 7328 293a 0a20 2020 2020 2020 2072  ems():.        r
-00027280: 656d 6f74 655f 7265 736f 7572 6365 5f6e  emote_resource_n
-00027290: 616d 6573 203d 205b 7265 2e73 7562 2866  ames = [re.sub(f
-000272a0: 225e 7b6f 6c64 5f77 737d 5c2e 222c 2066  "^{old_ws}\.", f
-000272b0: 227b 6e65 775f 7773 7d2e 222c 2078 2920  "{new_ws}.", x) 
-000272c0: 666f 7220 7820 696e 2072 656d 6f74 655f  for x in remote_
-000272d0: 7265 736f 7572 6365 5f6e 616d 6573 5d0a  resource_names].
-000272e0: 0a20 2020 2069 6620 6e6f 7420 6669 6c65  .    if not file
-000272f0: 6e61 6d65 733a 0a20 2020 2020 2020 2066  names:.        f
-00027300: 696c 656e 616d 6573 203d 2067 6574 5f70  ilenames = get_p
-00027310: 726f 6a65 6374 5f66 696c 656e 616d 6573  roject_filenames
-00027320: 2866 6f6c 6465 7229 0a0a 2020 2020 2320  (folder)..    # 
-00027330: 6765 7420 7468 6520 6c69 7374 206f 6620  get the list of 
-00027340: 6368 616e 6765 730a 2020 2020 6368 616e  changes.    chan
-00027350: 6765 642c 2064 656c 6574 6564 203d 2061  ged, deleted = a
-00027360: 7761 6974 2064 6570 6c6f 796d 656e 742e  wait deployment.
-00027370: 6465 7465 6374 5f63 6861 6e67 6573 2866  detect_changes(f
-00027380: 696c 656e 616d 6573 2c20 6f6e 6c79 5f63  ilenames, only_c
-00027390: 6861 6e67 6573 2c20 636f 6e66 6967 2c20  hanges, config, 
-000273a0: 7573 655f 6d61 696e 290a 0a20 2020 2064  use_main)..    d
-000273b0: 6570 6c6f 796d 656e 742e 6368 6563 6b5f  eployment.check_
-000273c0: 6368 616e 6765 7328 6368 616e 6765 642c  changes(changed,
-000273d0: 2070 6970 6573 2c20 7265 6c65 6173 655f   pipes, release_
-000273e0: 6372 6561 7465 6429 0a0a 2020 2020 6465  created)..    de
-000273f0: 706c 6f79 6d65 6e74 2e70 7265 7061 7269  ployment.prepari
-00027400: 6e67 5f72 656c 6561 7365 2829 0a0a 2020  ng_release()..  
-00027410: 2020 2320 6275 696c 6420 6772 6170 6820    # build graph 
-00027420: 746f 2067 6574 206e 6577 2076 6572 7369  to get new versi
-00027430: 6f6e 7320 666f 7220 616c 6c20 7468 6520  ons for all the 
-00027440: 6669 6c65 7320 696e 766f 6c76 6564 2069  files involved i
-00027450: 6e20 7468 6520 7175 6572 790a 2020 2020  n the query.    
-00027460: 2320 6465 7065 6e64 656e 6369 6573 206e  # dependencies n
-00027470: 6565 6420 746f 2062 6520 7072 6f63 6573  eed to be proces
-00027480: 7365 6420 616c 7761 7973 2074 6f20 6765  sed always to ge
-00027490: 7420 7468 6520 7665 7273 696f 6e73 0a20  t the versions. 
-000274a0: 2020 2064 6570 656e 6465 6e63 6965 735f     dependencies_
-000274b0: 6772 6170 6820 3d20 6177 6169 7420 6275  graph = await bu
-000274c0: 696c 645f 6772 6170 6828 0a20 2020 2020  ild_graph(.     
-000274d0: 2020 2066 696c 656e 616d 6573 2c0a 2020     filenames,.  
-000274e0: 2020 2020 2020 7462 5f63 6c69 656e 742c        tb_client,
-000274f0: 0a20 2020 2020 2020 2064 6972 5f70 6174  .        dir_pat
-00027500: 683d 666f 6c64 6572 2c0a 2020 2020 2020  h=folder,.      
-00027510: 2020 7072 6f63 6573 735f 6465 7065 6e64    process_depend
-00027520: 656e 6369 6573 3d54 7275 652c 0a20 2020  encies=True,.   
-00027530: 2020 2020 2077 6f72 6b73 7061 6365 5f6d       workspace_m
-00027540: 6170 3d77 6f72 6b73 7061 6365 5f6d 6170  ap=workspace_map
-00027550: 2c0a 2020 2020 2020 2020 736b 6970 5f63  ,.        skip_c
-00027560: 6f6e 6e65 6374 6f72 733d 5472 7565 2c0a  onnectors=True,.
-00027570: 2020 2020 2020 2020 776f 726b 7370 6163          workspac
-00027580: 655f 6c69 625f 7061 7468 733d 776f 726b  e_lib_paths=work
-00027590: 7370 6163 655f 6c69 625f 7061 7468 732c  space_lib_paths,
-000275a0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-000275b0: 5f77 733d 6375 7272 656e 745f 7773 2c0a  _ws=current_ws,.
-000275c0: 2020 2020 2020 2020 6368 616e 6765 643d          changed=
-000275d0: 6368 616e 6765 642c 0a20 2020 2020 2020  changed,.       
-000275e0: 206f 6e6c 795f 6368 616e 6765 733d 6f6e   only_changes=on
-000275f0: 6c79 5f63 6861 6e67 6573 206f 7220 2864  ly_changes or (d
-00027600: 6570 6c6f 796d 656e 742e 6973 5f67 6974  eployment.is_git
-00027610: 5f72 656c 6561 7365 2061 6e64 2068 6173  _release and has
-00027620: 5f73 656d 7665 7229 2c0a 2020 2020 2020  _semver),.      
-00027630: 2020 666f 726b 5f64 6f77 6e73 7472 6561    fork_downstrea
-00027640: 6d3d 666f 726b 5f64 6f77 6e73 7472 6561  m=fork_downstrea
-00027650: 6d2c 0a20 2020 2020 2020 2069 735f 696e  m,.        is_in
-00027660: 7465 726e 616c 3d69 735f 696e 7465 726e  ternal=is_intern
-00027670: 616c 2c0a 2020 2020 290a 0a20 2020 2023  al,.    )..    #
-00027680: 2075 7064 6174 6520 6578 6973 7469 6e67   update existing
-00027690: 2076 6572 7369 6f6e 730a 2020 2020 6966   versions.    if
-000276a0: 206e 6f74 206e 6f5f 7665 7273 696f 6e73   not no_versions
-000276b0: 3a0a 2020 2020 2020 2020 7265 736f 7572  :.        resour
-000276c0: 6365 5f76 6572 7369 6f6e 7320 3d20 6765  ce_versions = ge
-000276d0: 745f 7265 736f 7572 6365 5f76 6572 7369  t_resource_versi
-000276e0: 6f6e 7328 6578 6973 7469 6e67 5f72 6573  ons(existing_res
-000276f0: 6f75 7263 6573 290a 2020 2020 2020 2020  ources).        
-00027700: 6c61 7465 7374 5f64 6174 6173 6f75 7263  latest_datasourc
-00027710: 655f 7665 7273 696f 6e73 203d 2072 6573  e_versions = res
-00027720: 6f75 7263 655f 7665 7273 696f 6e73 2e63  ource_versions.c
-00027730: 6f70 7928 290a 0a20 2020 2020 2020 2066  opy()..        f
-00027740: 6f72 2064 6570 2069 6e20 6465 7065 6e64  or dep in depend
-00027750: 656e 6369 6573 5f67 7261 7068 2e74 6f5f  encies_graph.to_
-00027760: 7275 6e2e 7661 6c75 6573 2829 3a0a 2020  run.values():.  
-00027770: 2020 2020 2020 2020 2020 6473 203d 2064            ds = d
-00027780: 6570 5b22 7265 736f 7572 6365 5f6e 616d  ep["resource_nam
-00027790: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
-000277a0: 6966 2064 6570 5b22 7665 7273 696f 6e22  if dep["version"
-000277b0: 5d20 6973 206e 6f74 204e 6f6e 653a 0a20  ] is not None:. 
-000277c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000277d0: 6174 6573 745f 6461 7461 736f 7572 6365  atest_datasource
-000277e0: 5f76 6572 7369 6f6e 735b 6473 5d20 3d20  _versions[ds] = 
-000277f0: 6465 705b 2276 6572 7369 6f6e 225d 0a20  dep["version"]. 
-00027800: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00027810: 2072 6573 6f75 7263 655f 7665 7273 696f   resource_versio
-00027820: 6e73 203d 207b 7d0a 2020 2020 2020 2020  ns = {}.        
-00027830: 6c61 7465 7374 5f64 6174 6173 6f75 7263  latest_datasourc
-00027840: 655f 7665 7273 696f 6e73 203d 207b 7d0a  e_versions = {}.
-00027850: 0a20 2020 2023 2049 6620 7765 2068 6176  .    # If we hav
-00027860: 6520 6461 7461 736f 7572 6365 7320 7573  e datasources us
-00027870: 696e 6720 5645 5253 494f 4e2c 206c 6574  ing VERSION, let
-00027880: 2773 2074 7279 2074 6f20 6765 7420 7468  's try to get th
-00027890: 6520 6c61 7465 7374 2076 6572 7369 6f6e  e latest version
-000278a0: 0a20 2020 2064 6570 656e 6465 6e63 6965  .    dependencie
-000278b0: 735f 6772 6170 6820 3d20 6177 6169 7420  s_graph = await 
-000278c0: 6275 696c 645f 6772 6170 6828 0a20 2020  build_graph(.   
-000278d0: 2020 2020 2066 696c 656e 616d 6573 2c0a       filenames,.
-000278e0: 2020 2020 2020 2020 7462 5f63 6c69 656e          tb_clien
-000278f0: 742c 0a20 2020 2020 2020 2064 6972 5f70  t,.        dir_p
-00027900: 6174 683d 666f 6c64 6572 2c0a 2020 2020  ath=folder,.    
-00027910: 2020 2020 7265 736f 7572 6365 5f76 6572      resource_ver
-00027920: 7369 6f6e 733d 6c61 7465 7374 5f64 6174  sions=latest_dat
-00027930: 6173 6f75 7263 655f 7665 7273 696f 6e73  asource_versions
-00027940: 2c0a 2020 2020 2020 2020 776f 726b 7370  ,.        worksp
-00027950: 6163 655f 6d61 703d 776f 726b 7370 6163  ace_map=workspac
-00027960: 655f 6d61 702c 0a20 2020 2020 2020 2070  e_map,.        p
-00027970: 726f 6365 7373 5f64 6570 656e 6465 6e63  rocess_dependenc
-00027980: 6965 733d 7075 7368 5f64 6570 732c 0a20  ies=push_deps,. 
-00027990: 2020 2020 2020 2076 6572 626f 7365 3d76         verbose=v
-000279a0: 6572 626f 7365 2c0a 2020 2020 2020 2020  erbose,.        
-000279b0: 776f 726b 7370 6163 655f 6c69 625f 7061  workspace_lib_pa
-000279c0: 7468 733d 776f 726b 7370 6163 655f 6c69  ths=workspace_li
-000279d0: 625f 7061 7468 732c 0a20 2020 2020 2020  b_paths,.       
-000279e0: 2063 7572 7265 6e74 5f77 733d 6375 7272   current_ws=curr
-000279f0: 656e 745f 7773 2c0a 2020 2020 2020 2020  ent_ws,.        
-00027a00: 6368 616e 6765 643d 6368 616e 6765 642c  changed=changed,
-00027a10: 0a20 2020 2020 2020 206f 6e6c 795f 6368  .        only_ch
-00027a20: 616e 6765 733d 6f6e 6c79 5f63 6861 6e67  anges=only_chang
-00027a30: 6573 206f 7220 2864 6570 6c6f 796d 656e  es or (deploymen
-00027a40: 742e 6973 5f67 6974 5f72 656c 6561 7365  t.is_git_release
-00027a50: 2061 6e64 2068 6173 5f73 656d 7665 7229   and has_semver)
-00027a60: 2c0a 2020 2020 2020 2020 666f 726b 5f64  ,.        fork_d
-00027a70: 6f77 6e73 7472 6561 6d3d 666f 726b 5f64  ownstream=fork_d
-00027a80: 6f77 6e73 7472 6561 6d2c 0a20 2020 2020  ownstream,.     
-00027a90: 2020 2069 735f 696e 7465 726e 616c 3d69     is_internal=i
-00027aa0: 735f 696e 7465 726e 616c 2c0a 2020 2020  s_internal,.    
-00027ab0: 290a 0a20 2020 2069 6620 6465 6275 673a  )..    if debug:
-00027ac0: 0a20 2020 2020 2020 2070 702e 7070 7269  .        pp.ppri
-00027ad0: 6e74 2864 6570 656e 6465 6e63 6965 735f  nt(dependencies_
-00027ae0: 6772 6170 682e 746f 5f72 756e 290a 0a20  graph.to_run).. 
-00027af0: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
-00027b00: 2020 2020 2020 2063 6c69 636b 2e65 6368         click.ech
-00027b10: 6f28 4665 6564 6261 636b 4d61 6e61 6765  o(FeedbackManage
-00027b20: 722e 696e 666f 5f62 7569 6c64 696e 675f  r.info_building_
-00027b30: 6465 7065 6e64 656e 6369 6573 2829 290a  dependencies()).
-00027b40: 0a20 2020 2064 6570 6c6f 796d 656e 742e  .    deployment.
-00027b50: 7072 6570 6172 696e 675f 6465 7065 6e64  preparing_depend
-00027b60: 656e 6369 6573 2863 6861 6e67 6564 2c20  encies(changed, 
-00027b70: 6465 7065 6e64 656e 6369 6573 5f67 7261  dependencies_gra
-00027b80: 7068 2e64 6570 5f6d 6170 2c20 6c61 7465  ph.dep_map, late
-00027b90: 7374 5f64 6174 6173 6f75 7263 655f 7665  st_datasource_ve
-00027ba0: 7273 696f 6e73 290a 0a20 2020 2064 6566  rsions)..    def
-00027bb0: 2073 686f 756c 645f 7075 7368 5f66 696c   should_push_fil
-00027bc0: 6528 0a20 2020 2020 2020 206e 616d 653a  e(.        name:
-00027bd0: 2073 7472 2c0a 2020 2020 2020 2020 7265   str,.        re
-00027be0: 6d6f 7465 5f72 6573 6f75 7263 655f 6e61  mote_resource_na
-00027bf0: 6d65 733a 204c 6973 745b 7374 725d 2c0a  mes: List[str],.
-00027c00: 2020 2020 2020 2020 6c61 7465 7374 5f64          latest_d
-00027c10: 6174 6173 6f75 7263 655f 7665 7273 696f  atasource_versio
-00027c20: 6e73 3a20 4469 6374 5b73 7472 2c20 416e  ns: Dict[str, An
-00027c30: 795d 2c0a 2020 2020 2020 2020 666f 7263  y],.        forc
-00027c40: 653a 2062 6f6f 6c2c 0a20 2020 2020 2020  e: bool,.       
-00027c50: 2072 756e 5f74 6573 7473 3a20 626f 6f6c   run_tests: bool
-00027c60: 2c0a 2020 2020 2920 2d3e 2062 6f6f 6c3a  ,.    ) -> bool:
-00027c70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00027c80: 2020 2020 2046 756e 6374 696f 6e20 746f       Function to
-00027c90: 206b 6e6f 7720 6966 2077 6520 6e65 6564   know if we need
-00027ca0: 2074 6f20 7275 6e20 6120 6669 6c65 206f   to run a file o
-00027cb0: 7220 6e6f 740a 2020 2020 2020 2020 2222  r not.        ""
-00027cc0: 220a 2020 2020 2020 2020 6966 206e 616d  ".        if nam
-00027cd0: 6520 6e6f 7420 696e 2072 656d 6f74 655f  e not in remote_
-00027ce0: 7265 736f 7572 6365 5f6e 616d 6573 3a0a  resource_names:.
-00027cf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00027d00: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00027d10: 2320 5768 656e 2077 6520 6e65 6564 2074  # When we need t
-00027d20: 6f20 7472 7920 746f 2070 7573 6820 6120  o try to push a 
-00027d30: 6669 6c65 2077 6865 6e20 6974 2064 6f65  file when it doe
-00027d40: 736e 2774 2065 7869 7374 2061 6e64 2074  sn't exist and t
-00027d50: 6865 2076 6572 7369 6f6e 2069 7320 6469  he version is di
-00027d60: 6666 6572 656e 7420 7468 6174 2074 6865  fferent that the
-00027d70: 2065 7869 7374 696e 6720 6f6e 650a 2020   existing one.  
-00027d80: 2020 2020 2020 7265 736f 7572 6365 5f66        resource_f
-00027d90: 756c 6c5f 6e61 6d65 203d 2028 0a20 2020  ull_name = (.   
-00027da0: 2020 2020 2020 2020 2066 227b 6e61 6d65           f"{name
-00027db0: 7d5f 5f76 7b6c 6174 6573 745f 6461 7461  }__v{latest_data
-00027dc0: 736f 7572 6365 5f76 6572 7369 6f6e 732e  source_versions.
-00027dd0: 6765 7428 6e61 6d65 297d 2220 6966 206e  get(name)}" if n
-00027de0: 616d 6520 696e 206c 6174 6573 745f 6461  ame in latest_da
-00027df0: 7461 736f 7572 6365 5f76 6572 7369 6f6e  tasource_version
-00027e00: 7320 656c 7365 206e 616d 650a 2020 2020  s else name.    
-00027e10: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00027e20: 2072 6573 6f75 7263 655f 6675 6c6c 5f6e   resource_full_n
-00027e30: 616d 6520 6e6f 7420 696e 2065 7869 7374  ame not in exist
-00027e40: 696e 675f 7265 736f 7572 6365 733a 0a20  ing_resources:. 
-00027e50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00027e60: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
-00027e70: 6620 666f 7263 6520 6f72 2072 756e 5f74  f force or run_t
-00027e80: 6573 7473 3a0a 2020 2020 2020 2020 2020  ests:.          
-00027e90: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-00027ea0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00027eb0: 7365 0a0a 2020 2020 6173 796e 6320 6465  se..    async de
-00027ec0: 6620 7075 7368 280a 2020 2020 2020 2020  f push(.        
-00027ed0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-00027ee0: 2020 2074 6f5f 7275 6e3a 2044 6963 745b     to_run: Dict[
-00027ef0: 7374 722c 2044 6963 745b 7374 722c 2041  str, Dict[str, A
-00027f00: 6e79 5d5d 2c0a 2020 2020 2020 2020 7265  ny]],.        re
-00027f10: 736f 7572 6365 5f76 6572 7369 6f6e 733a  source_versions:
-00027f20: 2044 6963 745b 7374 722c 2041 6e79 5d2c   Dict[str, Any],
-00027f30: 0a20 2020 2020 2020 206c 6174 6573 745f  .        latest_
-00027f40: 6461 7461 736f 7572 6365 5f76 6572 7369  datasource_versi
-00027f50: 6f6e 733a 2044 6963 745b 7374 722c 2041  ons: Dict[str, A
-00027f60: 6e79 5d2c 0a20 2020 2020 2020 2064 7279  ny],.        dry
-00027f70: 5f72 756e 3a20 626f 6f6c 2c0a 2020 2020  _run: bool,.    
-00027f80: 2020 2020 666f 726b 5f64 6f77 6e73 7472      fork_downstr
-00027f90: 6561 6d3a 204f 7074 696f 6e61 6c5b 626f  eam: Optional[bo
-00027fa0: 6f6c 5d20 3d20 4661 6c73 652c 0a20 2020  ol] = False,.   
-00027fb0: 2020 2020 2066 6f72 6b3a 204f 7074 696f       fork: Optio
-00027fc0: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
-00027fd0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00027fe0: 2020 6966 206e 616d 6520 696e 2074 6f5f    if name in to_
-00027ff0: 7275 6e3a 0a20 2020 2020 2020 2020 2020  run:.           
-00028000: 2069 6620 6e6f 7420 6472 795f 7275 6e3a   if not dry_run:
-00028010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028020: 2069 6620 7368 6f75 6c64 5f70 7573 685f   if should_push_
-00028030: 6669 6c65 286e 616d 652c 2072 656d 6f74  file(name, remot
-00028040: 655f 7265 736f 7572 6365 5f6e 616d 6573  e_resource_names
-00028050: 2c20 6c61 7465 7374 5f64 6174 6173 6f75  , latest_datasou
-00028060: 7263 655f 7665 7273 696f 6e73 2c20 666f  rce_versions, fo
-00028070: 7263 652c 2072 756e 5f74 6573 7473 293a  rce, run_tests):
-00028080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028090: 2020 2020 2069 6620 6e61 6d65 206e 6f74       if name not
-000280a0: 2069 6e20 7265 736f 7572 6365 5f76 6572   in resource_ver
-000280b0: 7369 6f6e 733a 0a20 2020 2020 2020 2020  sions:.         
-000280c0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000280d0: 6572 7369 6f6e 203d 2022 220a 2020 2020  ersion = "".    
-000280e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000280f0: 2020 2020 6966 206e 616d 6520 696e 206c      if name in l
-00028100: 6174 6573 745f 6461 7461 736f 7572 6365  atest_datasource
-00028110: 5f76 6572 7369 6f6e 733a 0a20 2020 2020  _versions:.     
-00028120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028130: 2020 2020 2020 2076 6572 7369 6f6e 203d         version =
-00028140: 2066 2228 767b 6c61 7465 7374 5f64 6174   f"(v{latest_dat
-00028150: 6173 6f75 7263 655f 7665 7273 696f 6e73  asource_versions
-00028160: 5b6e 616d 655d 7d29 220a 2020 2020 2020  [name]})".      
-00028170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028180: 2020 636c 6963 6b2e 6563 686f 2846 6565    click.echo(Fee
-00028190: 6462 6163 6b4d 616e 6167 6572 2e69 6e66  dbackManager.inf
-000281a0: 6f5f 7072 6f63 6573 7369 6e67 5f6e 6577  o_processing_new
-000281b0: 5f72 6573 6f75 7263 6528 6e61 6d65 3d6e  _resource(name=n
-000281c0: 616d 652c 2076 6572 7369 6f6e 3d76 6572  ame, version=ver
-000281d0: 7369 6f6e 2929 0a20 2020 2020 2020 2020  sion)).         
-000281e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000281f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028200: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-00028210: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+00025dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025dd0: 7072 6f63 6573 7365 645f 6669 6c65 6e61  processed_filena
+00025de0: 6d65 203d 2066 0a20 2020 2020 2020 2020  me = f.         
+00025df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e00: 2020 2063 6c69 636b 2e65 6368 6f28 4665     click.echo(Fe
+00025e10: 6564 6261 636b 4d61 6e61 6765 722e 696e  edbackManager.in
+00025e20: 666f 5f70 726f 6365 7373 696e 675f 6669  fo_processing_fi
+00025e30: 6c65 2866 696c 656e 616d 653d 7072 6f63  le(filename=proc
+00025e40: 6573 7365 645f 6669 6c65 6e61 6d65 2929  essed_filename))
+00025e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025e60: 2020 2020 2020 2020 2061 7761 6974 2070           await p
+00025e70: 726f 6365 7373 2873 7472 2866 292c 2064  rocess(str(f), d
+00025e80: 6570 732c 2064 6570 5f6d 6170 2c20 746f  eps, dep_map, to
+00025e90: 5f72 756e 2c20 776f 726b 7370 6163 655f  _run, workspace_
+00025ea0: 6c69 625f 7061 7468 7329 0a0a 2020 2020  lib_paths)..    
+00025eb0: 7265 7475 726e 2047 7261 7068 4465 7065  return GraphDepe
+00025ec0: 6e64 656e 6369 6573 2864 6570 5f6d 6170  ndencies(dep_map
+00025ed0: 2c20 746f 5f72 756e 2c20 616c 6c5f 6465  , to_run, all_de
+00025ee0: 705f 6d61 702c 2061 6c6c 5f72 6573 6f75  p_map, all_resou
+00025ef0: 7263 6573 290a 0a0a 6173 796e 6320 6465  rces)...async de
+00025f00: 6620 6765 745f 6368 616e 6765 735f 6672  f get_changes_fr
+00025f10: 6f6d 5f6d 6169 6e28 0a20 2020 206f 6e6c  om_main(.    onl
+00025f20: 795f 6368 616e 6765 733a 2062 6f6f 6c2c  y_changes: bool,
+00025f30: 0a20 2020 2063 6c69 656e 743a 2054 696e  .    client: Tin
+00025f40: 7942 2c0a 2020 2020 636f 6e66 6967 3a20  yB,.    config: 
+00025f50: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00025f60: 722c 2041 6e79 5d5d 203d 204e 6f6e 652c  r, Any]] = None,
+00025f70: 0a20 2020 2063 7572 7265 6e74 5f77 733a  .    current_ws:
+00025f80: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00025f90: 7472 2c20 416e 795d 5d20 3d20 4e6f 6e65  tr, Any]] = None
+00025fa0: 2c0a 2020 2020 6669 6c65 6e61 6d65 733a  ,.    filenames:
+00025fb0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00025fc0: 7472 5d5d 203d 204e 6f6e 652c 0a29 3a0a  tr]] = None,.):.
+00025fd0: 2020 2020 6368 616e 6765 6420 3d20 4e6f      changed = No
+00025fe0: 6e65 0a20 2020 2069 6620 6e6f 7420 6f6e  ne.    if not on
+00025ff0: 6c79 5f63 6861 6e67 6573 3a0a 2020 2020  ly_changes:.    
+00026000: 2020 2020 7265 7475 726e 2063 6861 6e67      return chang
+00026010: 6564 0a0a 2020 2020 6966 2063 7572 7265  ed..    if curre
+00026020: 6e74 5f77 7320 616e 6420 6e6f 7420 6375  nt_ws and not cu
+00026030: 7272 656e 745f 7773 2e67 6574 2822 6973  rrent_ws.get("is
+00026040: 5f62 7261 6e63 6822 293a 0a20 2020 2020  _branch"):.     
+00026050: 2020 2063 6861 6e67 6564 203d 2061 7761     changed = awa
+00026060: 6974 2064 6966 665f 636f 6d6d 616e 6428  it diff_command(
+00026070: 6669 6c65 6e61 6d65 732c 2054 7275 652c  filenames, True,
+00026080: 2063 6c69 656e 742c 206e 6f5f 636f 6c6f   client, no_colo
+00026090: 723d 5472 7565 2c20 7769 7468 5f70 7269  r=True, with_pri
+000260a0: 6e74 3d46 616c 7365 290a 2020 2020 656c  nt=False).    el
+000260b0: 6966 2063 6f6e 6669 6720 616e 6420 636f  if config and co
+000260c0: 6e66 6967 2e67 6574 2822 686f 7374 2229  nfig.get("host")
+000260d0: 3a0a 2020 2020 2020 2020 776f 726b 7370  :.        worksp
+000260e0: 6163 6520 3d20 6177 6169 7420 6765 745f  ace = await get_
+000260f0: 6375 7272 656e 745f 6d61 696e 5f77 6f72  current_main_wor
+00026100: 6b73 7061 6365 2863 6c69 656e 742c 2063  kspace(client, c
+00026110: 6f6e 6669 6729 0a0a 2020 2020 2020 2020  onfig)..        
+00026120: 6966 2077 6f72 6b73 7061 6365 3a0a 2020  if workspace:.  
+00026130: 2020 2020 2020 2020 2020 7773 5f63 6c69            ws_cli
+00026140: 656e 7420 3d20 5f67 6574 5f74 625f 636c  ent = _get_tb_cl
+00026150: 6965 6e74 2877 6f72 6b73 7061 6365 5b22  ient(workspace["
+00026160: 746f 6b65 6e22 5d2c 2063 6f6e 6669 675b  token"], config[
+00026170: 2268 6f73 7422 5d29 0a20 2020 2020 2020  "host"]).       
+00026180: 2020 2020 2063 6861 6e67 6564 203d 2061       changed = a
+00026190: 7761 6974 2064 6966 665f 636f 6d6d 616e  wait diff_comman
+000261a0: 6428 6669 6c65 6e61 6d65 732c 2054 7275  d(filenames, Tru
+000261b0: 652c 2077 735f 636c 6965 6e74 2c20 6e6f  e, ws_client, no
+000261c0: 5f63 6f6c 6f72 3d54 7275 652c 2077 6974  _color=True, wit
+000261d0: 685f 7072 696e 743d 4661 6c73 6529 0a20  h_print=False). 
+000261e0: 2020 2072 6574 7572 6e20 6368 616e 6765     return change
+000261f0: 640a 0a0a 6465 6620 6765 745f 7072 6f6a  d...def get_proj
+00026200: 6563 745f 6669 6c65 6e61 6d65 7328 666f  ect_filenames(fo
+00026210: 6c64 6572 3a20 7374 722c 2077 6974 685f  lder: str, with_
+00026220: 7665 6e64 6f72 3d46 616c 7365 2920 2d3e  vendor=False) ->
+00026230: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+00026240: 666f 6c64 6572 733a 204c 6973 745b 7374  folders: List[st
+00026250: 725d 203d 205b 0a20 2020 2020 2020 2066  r] = [.        f
+00026260: 227b 666f 6c64 6572 7d2f 2a2e 6461 7461  "{folder}/*.data
+00026270: 736f 7572 6365 222c 0a20 2020 2020 2020  source",.       
+00026280: 2066 227b 666f 6c64 6572 7d2f 6461 7461   f"{folder}/data
+00026290: 736f 7572 6365 732f 2a2e 6461 7461 736f  sources/*.dataso
+000262a0: 7572 6365 222c 0a20 2020 2020 2020 2066  urce",.        f
+000262b0: 227b 666f 6c64 6572 7d2f 2a2e 7069 7065  "{folder}/*.pipe
+000262c0: 222c 0a20 2020 2020 2020 2066 227b 666f  ",.        f"{fo
+000262d0: 6c64 6572 7d2f 7069 7065 732f 2a2e 7069  lder}/pipes/*.pi
+000262e0: 7065 222c 0a20 2020 2020 2020 2066 227b  pe",.        f"{
+000262f0: 666f 6c64 6572 7d2f 656e 6470 6f69 6e74  folder}/endpoint
+00026300: 732f 2a2e 7069 7065 222c 0a20 2020 2020  s/*.pipe",.     
+00026310: 2020 2066 227b 666f 6c64 6572 7d2f 2a2e     f"{folder}/*.
+00026320: 746f 6b65 6e22 2c0a 2020 2020 2020 2020  token",.        
+00026330: 6622 7b66 6f6c 6465 727d 2f74 6f6b 656e  f"{folder}/token
+00026340: 732f 2a2e 746f 6b65 6e22 2c0a 2020 2020  s/*.token",.    
+00026350: 5d0a 2020 2020 6966 2077 6974 685f 7665  ].    if with_ve
+00026360: 6e64 6f72 3a0a 2020 2020 2020 2020 666f  ndor:.        fo
+00026370: 6c64 6572 732e 6170 7065 6e64 2866 227b  lders.append(f"{
+00026380: 666f 6c64 6572 7d2f 7665 6e64 6f72 2f2a  folder}/vendor/*
+00026390: 2a2f 2a2a 2f2a 2e64 6174 6173 6f75 7263  */**/*.datasourc
+000263a0: 6522 290a 2020 2020 6669 6c65 6e61 6d65  e").    filename
+000263b0: 733a 204c 6973 745b 7374 725d 203d 205b  s: List[str] = [
+000263c0: 5d0a 2020 2020 666f 7220 7820 696e 2066  ].    for x in f
+000263d0: 6f6c 6465 7273 3a0a 2020 2020 2020 2020  olders:.        
+000263e0: 6669 6c65 6e61 6d65 7320 2b3d 2067 6c6f  filenames += glo
+000263f0: 622e 676c 6f62 2878 290a 2020 2020 7265  b.glob(x).    re
+00026400: 7475 726e 2066 696c 656e 616d 6573 0a0a  turn filenames..
+00026410: 0a64 6566 2069 735f 6e65 7728 0a20 2020  .def is_new(.   
+00026420: 206e 616d 653a 2073 7472 2c0a 2020 2020   name: str,.    
+00026430: 6368 616e 6765 643a 2044 6963 745b 7374  changed: Dict[st
+00026440: 722c 2073 7472 5d2c 0a20 2020 206e 6f72  r, str],.    nor
+00026450: 6d61 6c5f 6465 7065 6e64 656e 6379 3a20  mal_dependency: 
+00026460: 4469 6374 5b73 7472 2c20 5365 745b 7374  Dict[str, Set[st
+00026470: 725d 5d2c 0a20 2020 2066 6f72 6b5f 646f  r]],.    fork_do
+00026480: 776e 7374 7265 616d 5f64 6570 656e 6465  wnstream_depende
+00026490: 6e63 793a 2044 6963 745b 7374 722c 2053  ncy: Dict[str, S
+000264a0: 6574 5b73 7472 5d5d 2c0a 2920 2d3e 2062  et[str]],.) -> b
+000264b0: 6f6f 6c3a 0a20 2020 2064 6566 2069 735f  ool:.    def is_
+000264c0: 6769 745f 6e65 7728 6e61 6d65 3a20 7374  git_new(name: st
+000264d0: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
+000264e0: 726e 2063 6861 6e67 6564 2061 6e64 2063  rn changed and c
+000264f0: 6861 6e67 6564 2e67 6574 286e 616d 6529  hanged.get(name)
+00026500: 203d 3d20 2241 220a 0a20 2020 2069 6620   == "A"..    if 
+00026510: 6e6f 7420 6973 5f67 6974 5f6e 6577 286e  not is_git_new(n
+00026520: 616d 6529 3a0a 2020 2020 2020 2020 7265  ame):.        re
+00026530: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00026540: 2320 6966 2073 686f 756c 6420 6e6f 7420  # if should not 
+00026550: 6465 7065 6e64 206f 6e20 6120 6368 616e  depend on a chan
+00026560: 6765 6420 7265 736f 7572 6365 0a20 2020  ged resource.   
+00026570: 2069 6620 6261 636b 5f64 6570 7320 3a3d   if back_deps :=
+00026580: 206e 6f72 6d61 6c5f 6465 7065 6e64 656e   normal_dependen
+00026590: 6379 2e67 6574 286e 616d 6529 3a0a 2020  cy.get(name):.  
+000265a0: 2020 2020 2020 666f 7220 6465 7020 696e        for dep in
+000265b0: 2062 6163 6b5f 6465 7073 3a0a 2020 2020   back_deps:.    
+000265c0: 2020 2020 2020 2020 6966 2064 6570 2069          if dep i
+000265d0: 6e20 666f 726b 5f64 6f77 6e73 7472 6561  n fork_downstrea
+000265e0: 6d5f 6465 7065 6e64 656e 6379 2061 6e64  m_dependency and
+000265f0: 206e 6f74 2069 735f 6769 745f 6e65 7728   not is_git_new(
+00026600: 6465 7029 3a0a 2020 2020 2020 2020 2020  dep):.          
+00026610: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00026620: 7365 0a0a 2020 2020 7265 7475 726e 2054  se..    return T
+00026630: 7275 650a 0a0a 6173 796e 6320 6465 6620  rue...async def 
+00026640: 666f 6c64 6572 5f70 7573 6828 0a20 2020  folder_push(.   
+00026650: 2074 625f 636c 6965 6e74 3a20 5469 6e79   tb_client: Tiny
+00026660: 422c 0a20 2020 2066 696c 656e 616d 6573  B,.    filenames
+00026670: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00026680: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00026690: 2020 6472 795f 7275 6e3a 2062 6f6f 6c20    dry_run: bool 
+000266a0: 3d20 4661 6c73 652c 0a20 2020 2063 6865  = False,.    che
+000266b0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+000266c0: 2c0a 2020 2020 7075 7368 5f64 6570 733a  ,.    push_deps:
+000266d0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+000266e0: 2020 206f 6e6c 795f 6368 616e 6765 733a     only_changes:
+000266f0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00026700: 2020 2067 6974 5f72 656c 6561 7365 3a20     git_release: 
+00026710: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00026720: 2020 6465 6275 673a 2062 6f6f 6c20 3d20    debug: bool = 
+00026730: 4661 6c73 652c 0a20 2020 2066 6f72 6365  False,.    force
+00026740: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00026750: 2020 2020 6f76 6572 7269 6465 5f64 6174      override_dat
+00026760: 6173 6f75 7263 653a 2062 6f6f 6c20 3d20  asource: bool = 
+00026770: 4661 6c73 652c 0a20 2020 2066 6f6c 6465  False,.    folde
+00026780: 723a 2073 7472 203d 2022 2e22 2c0a 2020  r: str = ".",.  
+00026790: 2020 706f 7075 6c61 7465 3a20 626f 6f6c    populate: bool
+000267a0: 203d 2046 616c 7365 2c0a 2020 2020 706f   = False,.    po
+000267b0: 7075 6c61 7465 5f73 7562 7365 743d 4e6f  pulate_subset=No
+000267c0: 6e65 2c0a 2020 2020 706f 7075 6c61 7465  ne,.    populate
+000267d0: 5f63 6f6e 6469 7469 6f6e 3a20 4f70 7469  _condition: Opti
+000267e0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000267f0: 2c0a 2020 2020 756e 6c69 6e6b 5f6f 6e5f  ,.    unlink_on_
+00026800: 706f 7075 6c61 7465 5f65 7272 6f72 3a20  populate_error: 
+00026810: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00026820: 2020 7570 6c6f 6164 5f66 6978 7475 7265    upload_fixture
+00026830: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
+00026840: 0a20 2020 2077 6169 743a 2062 6f6f 6c20  .    wait: bool 
+00026850: 3d20 4661 6c73 652c 0a20 2020 2069 676e  = False,.    ign
+00026860: 6f72 655f 7371 6c5f 6572 726f 7273 3a20  ore_sql_errors: 
+00026870: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00026880: 2020 736b 6970 5f63 6f6e 6669 726d 6174    skip_confirmat
+00026890: 696f 6e3a 2062 6f6f 6c20 3d20 4661 6c73  ion: bool = Fals
+000268a0: 652c 0a20 2020 206f 6e6c 795f 7265 7370  e,.    only_resp
+000268b0: 6f6e 7365 5f74 696d 6573 3a20 626f 6f6c  onse_times: bool
+000268c0: 203d 2046 616c 7365 2c0a 2020 2020 776f   = False,.    wo
+000268d0: 726b 7370 6163 655f 6d61 703d 4e6f 6e65  rkspace_map=None
+000268e0: 2c0a 2020 2020 776f 726b 7370 6163 655f  ,.    workspace_
+000268f0: 6c69 625f 7061 7468 733d 4e6f 6e65 2c0a  lib_paths=None,.
+00026900: 2020 2020 6e6f 5f76 6572 7369 6f6e 733a      no_versions:
+00026910: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00026920: 2020 2074 696d 656f 7574 3d4e 6f6e 652c     timeout=None,
+00026930: 0a20 2020 2072 756e 5f74 6573 7473 3a20  .    run_tests: 
+00026940: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00026950: 2020 6173 5f73 7461 6e64 6172 643a 2062    as_standard: b
+00026960: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00026970: 2072 6169 7365 5f6f 6e5f 6578 6973 7473   raise_on_exists
+00026980: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00026990: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+000269a0: 6c20 3d20 5472 7565 2c0a 2020 2020 7465  l = True,.    te
+000269b0: 7374 735f 746f 5f72 756e 3a20 696e 7420  sts_to_run: int 
+000269c0: 3d20 302c 0a20 2020 2074 6573 7473 5f73  = 0,.    tests_s
+000269d0: 616d 706c 655f 6279 5f70 6172 616d 733a  ample_by_params:
+000269e0: 2069 6e74 203d 2030 2c0a 2020 2020 7465   int = 0,.    te
+000269f0: 7374 735f 6669 6c74 6572 5f62 793a 204f  sts_filter_by: O
+00026a00: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
+00026a10: 5d5d 203d 204e 6f6e 652c 0a20 2020 2074  ]] = None,.    t
+00026a20: 6573 7473 5f66 6169 6c66 6173 743a 2062  ests_failfast: b
+00026a30: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00026a40: 2074 6573 7473 5f69 676e 6f72 655f 6f72   tests_ignore_or
+00026a50: 6465 723a 2062 6f6f 6c20 3d20 4661 6c73  der: bool = Fals
+00026a60: 652c 0a20 2020 2074 6573 7473 5f76 616c  e,.    tests_val
+00026a70: 6964 6174 655f 7072 6f63 6573 7365 645f  idate_processed_
+00026a80: 6279 7465 733a 2062 6f6f 6c20 3d20 4661  bytes: bool = Fa
+00026a90: 6c73 652c 0a20 2020 2074 6573 7473 5f63  lse,.    tests_c
+00026aa0: 6865 636b 5f72 6571 7565 7374 735f 6672  heck_requests_fr
+00026ab0: 6f6d 5f62 7261 6e63 683a 2062 6f6f 6c20  om_branch: bool 
+00026ac0: 3d20 4661 6c73 652c 0a20 2020 2063 6f6e  = False,.    con
+00026ad0: 6669 673a 204f 7074 696f 6e61 6c5b 4469  fig: Optional[Di
+00026ae0: 6374 5b73 7472 2c20 416e 795d 5d20 3d20  ct[str, Any]] = 
+00026af0: 4e6f 6e65 2c0a 2020 2020 7573 6572 5f74  None,.    user_t
+00026b00: 6f6b 656e 3a20 4f70 7469 6f6e 616c 5b73  oken: Optional[s
+00026b10: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00026b20: 666f 726b 5f64 6f77 6e73 7472 6561 6d3a  fork_downstream:
+00026b30: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00026b40: 3d20 4661 6c73 652c 0a20 2020 2066 6f72  = False,.    for
+00026b50: 6b3a 204f 7074 696f 6e61 6c5b 626f 6f6c  k: Optional[bool
+00026b60: 5d20 3d20 4661 6c73 652c 0a20 2020 2069  ] = False,.    i
+00026b70: 735f 696e 7465 726e 616c 3a20 4f70 7469  s_internal: Opti
+00026b80: 6f6e 616c 5b62 6f6f 6c5d 203d 2046 616c  onal[bool] = Fal
+00026b90: 7365 2c0a 2020 2020 7265 6c65 6173 655f  se,.    release_
+00026ba0: 6372 6561 7465 643a 204f 7074 696f 6e61  created: Optiona
+00026bb0: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
+00026bc0: 0a20 2020 2061 7574 6f5f 7072 6f6d 6f74  .    auto_promot
+00026bd0: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+00026be0: 5d20 3d20 4661 6c73 652c 0a20 2020 2063  ] = False,.    c
+00026bf0: 6865 636b 5f62 6163 6b66 696c 6c5f 7265  heck_backfill_re
+00026c00: 7175 6972 6564 3a20 626f 6f6c 203d 2046  quired: bool = F
+00026c10: 616c 7365 2c0a 2020 2020 7573 655f 6d61  alse,.    use_ma
+00026c20: 696e 3a20 626f 6f6c 203d 2046 616c 7365  in: bool = False
+00026c30: 2c0a 293a 2020 2320 6e6f 7161 3a20 4339  ,.):  # noqa: C9
+00026c40: 3031 0a20 2020 2077 6f72 6b73 7061 6365  01.    workspace
+00026c50: 733a 204c 6973 745b 4469 6374 5b73 7472  s: List[Dict[str
+00026c60: 2c20 416e 795d 5d20 3d20 2861 7761 6974  , Any]] = (await
+00026c70: 2074 625f 636c 6965 6e74 2e75 7365 725f   tb_client.user_
+00026c80: 776f 726b 7370 6163 6573 5f61 6e64 5f62  workspaces_and_b
+00026c90: 7261 6e63 6865 7328 2929 2e67 6574 2822  ranches()).get("
+00026ca0: 776f 726b 7370 6163 6573 222c 205b 5d29  workspaces", [])
+00026cb0: 0a20 2020 2063 7572 7265 6e74 5f77 733a  .    current_ws:
+00026cc0: 2044 6963 745b 7374 722c 2041 6e79 5d20   Dict[str, Any] 
+00026cd0: 3d20 6e65 7874 280a 2020 2020 2020 2020  = next(.        
+00026ce0: 2877 6f72 6b73 7061 6365 2066 6f72 2077  (workspace for w
+00026cf0: 6f72 6b73 7061 6365 2069 6e20 776f 726b  orkspace in work
+00026d00: 7370 6163 6573 2069 6620 636f 6e66 6967  spaces if config
+00026d10: 2061 6e64 2077 6f72 6b73 7061 6365 2e67   and workspace.g
+00026d20: 6574 2822 6964 222c 2022 2e22 2920 3d3d  et("id", ".") ==
+00026d30: 2063 6f6e 6669 672e 6765 7428 2269 6422   config.get("id"
+00026d40: 2c20 222e 2e22 2929 2c20 7b7d 0a20 2020  , "..")), {}.   
+00026d50: 2029 0a20 2020 2069 735f 6272 616e 6368   ).    is_branch
+00026d60: 203d 2063 7572 7265 6e74 5f77 732e 6765   = current_ws.ge
+00026d70: 7428 2269 735f 6272 616e 6368 222c 2046  t("is_branch", F
+00026d80: 616c 7365 290a 2020 2020 6861 735f 7365  alse).    has_se
+00026d90: 6d76 6572 3a20 626f 6f6c 203d 2072 656c  mver: bool = rel
+00026da0: 6561 7365 5f63 7265 6174 6564 206f 7220  ease_created or 
+00026db0: 4661 6c73 650a 0a20 2020 2064 6570 6c6f  False..    deplo
+00026dc0: 796d 656e 7420 3d20 4465 706c 6f79 6d65  yment = Deployme
+00026dd0: 6e74 2863 7572 7265 6e74 5f77 732c 2067  nt(current_ws, g
+00026de0: 6974 5f72 656c 6561 7365 2c20 7462 5f63  it_release, tb_c
+00026df0: 6c69 656e 742c 2064 7279 5f72 756e 2c20  lient, dry_run, 
+00026e00: 6f6e 6c79 5f63 6861 6e67 6573 290a 0a20  only_changes).. 
+00026e10: 2020 2069 6620 6e6f 7420 776f 726b 7370     if not worksp
+00026e20: 6163 655f 6d61 703a 0a20 2020 2020 2020  ace_map:.       
+00026e30: 2077 6f72 6b73 7061 6365 5f6d 6170 203d   workspace_map =
+00026e40: 207b 7d0a 2020 2020 6966 206e 6f74 2077   {}.    if not w
+00026e50: 6f72 6b73 7061 6365 5f6c 6962 5f70 6174  orkspace_lib_pat
+00026e60: 6873 3a0a 2020 2020 2020 2020 776f 726b  hs:.        work
+00026e70: 7370 6163 655f 6c69 625f 7061 7468 7320  space_lib_paths 
+00026e80: 3d20 5b5d 0a0a 2020 2020 776f 726b 7370  = []..    worksp
+00026e90: 6163 655f 6c69 625f 7061 7468 7320 3d20  ace_lib_paths = 
+00026ea0: 6c69 7374 2877 6f72 6b73 7061 6365 5f6c  list(workspace_l
+00026eb0: 6962 5f70 6174 6873 290a 2020 2020 2320  ib_paths).    # 
+00026ec0: 696e 636c 7564 6520 7665 6e64 6f72 206c  include vendor l
+00026ed0: 6962 7320 7769 7468 6f75 7420 6f76 6572  ibs without over
+00026ee0: 7269 6469 6e67 2075 7365 7220 6f6e 6573  riding user ones
+00026ef0: 0a20 2020 2065 7869 7374 696e 675f 776f  .    existing_wo
+00026f00: 726b 7370 6163 6573 203d 2073 6574 2878  rkspaces = set(x
+00026f10: 5b31 5d20 666f 7220 7820 696e 2077 6f72  [1] for x in wor
+00026f20: 6b73 7061 6365 5f6c 6962 5f70 6174 6873  kspace_lib_paths
+00026f30: 290a 2020 2020 7665 6e64 6f72 5f70 6174  ).    vendor_pat
+00026f40: 6820 3d20 5061 7468 2822 7665 6e64 6f72  h = Path("vendor
+00026f50: 2229 0a20 2020 2069 6620 7665 6e64 6f72  ").    if vendor
+00026f60: 5f70 6174 682e 6578 6973 7473 2829 3a0a  _path.exists():.
+00026f70: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
+00026f80: 2076 656e 646f 725f 7061 7468 2e69 7465   vendor_path.ite
+00026f90: 7264 6972 2829 3a0a 2020 2020 2020 2020  rdir():.        
+00026fa0: 2020 2020 6966 2078 2e69 735f 6469 7228      if x.is_dir(
+00026fb0: 2920 616e 6420 782e 6e61 6d65 206e 6f74  ) and x.name not
+00026fc0: 2069 6e20 6578 6973 7469 6e67 5f77 6f72   in existing_wor
+00026fd0: 6b73 7061 6365 733a 0a20 2020 2020 2020  kspaces:.       
+00026fe0: 2020 2020 2020 2020 2077 6f72 6b73 7061           workspa
+00026ff0: 6365 5f6c 6962 5f70 6174 6873 2e61 7070  ce_lib_paths.app
+00027000: 656e 6428 2878 2e6e 616d 652c 2078 2929  end((x.name, x))
+00027010: 0a0a 2020 2020 6461 7461 736f 7572 6365  ..    datasource
+00027020: 733a 204c 6973 745b 4469 6374 5b73 7472  s: List[Dict[str
+00027030: 2c20 416e 795d 5d20 3d20 6177 6169 7420  , Any]] = await 
+00027040: 7462 5f63 6c69 656e 742e 6461 7461 736f  tb_client.dataso
+00027050: 7572 6365 7328 290a 2020 2020 7069 7065  urces().    pipe
+00027060: 733a 204c 6973 745b 4469 6374 5b73 7472  s: List[Dict[str
+00027070: 2c20 416e 795d 5d20 3d20 6177 6169 7420  , Any]] = await 
+00027080: 7462 5f63 6c69 656e 742e 7069 7065 7328  tb_client.pipes(
+00027090: 6465 7065 6e64 656e 6369 6573 3d54 7275  dependencies=Tru
+000270a0: 6529 0a0a 2020 2020 6578 6973 7469 6e67  e)..    existing
+000270b0: 5f72 6573 6f75 7263 6573 3a20 4c69 7374  _resources: List
+000270c0: 5b73 7472 5d20 3d20 5b78 5b22 6e61 6d65  [str] = [x["name
+000270d0: 225d 2066 6f72 2078 2069 6e20 6461 7461  "] for x in data
+000270e0: 736f 7572 6365 735d 202b 205b 785b 226e  sources] + [x["n
+000270f0: 616d 6522 5d20 666f 7220 7820 696e 2070  ame"] for x in p
+00027100: 6970 6573 5d0a 2020 2020 2320 7265 706c  ipes].    # repl
+00027110: 6163 6520 776f 726b 7370 6163 6520 6d61  ace workspace ma
+00027120: 7070 696e 6720 6e61 6d65 730a 2020 2020  pping names.    
+00027130: 666f 7220 6f6c 645f 7773 2c20 6e65 775f  for old_ws, new_
+00027140: 7773 2069 6e20 776f 726b 7370 6163 655f  ws in workspace_
+00027150: 6d61 702e 6974 656d 7328 293a 0a20 2020  map.items():.   
+00027160: 2020 2020 2065 7869 7374 696e 675f 7265       existing_re
+00027170: 736f 7572 6365 7320 3d20 5b72 652e 7375  sources = [re.su
+00027180: 6228 6622 5e7b 6f6c 645f 7773 7d5c 2e22  b(f"^{old_ws}\."
+00027190: 2c20 6622 7b6e 6577 5f77 737d 2e22 2c20  , f"{new_ws}.", 
+000271a0: 7829 2066 6f72 2078 2069 6e20 6578 6973  x) for x in exis
+000271b0: 7469 6e67 5f72 6573 6f75 7263 6573 5d0a  ting_resources].
+000271c0: 0a20 2020 2072 656d 6f74 655f 7265 736f  .    remote_reso
+000271d0: 7572 6365 5f6e 616d 6573 203d 205b 6765  urce_names = [ge
+000271e0: 745f 7265 6d6f 7465 5f72 6573 6f75 7263  t_remote_resourc
+000271f0: 655f 6e61 6d65 5f77 6974 686f 7574 5f76  e_name_without_v
+00027200: 6572 7369 6f6e 2878 2920 666f 7220 7820  ersion(x) for x 
+00027210: 696e 2065 7869 7374 696e 675f 7265 736f  in existing_reso
+00027220: 7572 6365 735d 0a0a 2020 2020 2320 7265  urces]..    # re
+00027230: 706c 6163 6520 776f 726b 7370 6163 6520  place workspace 
+00027240: 6d61 7070 696e 6720 6e61 6d65 730a 2020  mapping names.  
+00027250: 2020 666f 7220 6f6c 645f 7773 2c20 6e65    for old_ws, ne
+00027260: 775f 7773 2069 6e20 776f 726b 7370 6163  w_ws in workspac
+00027270: 655f 6d61 702e 6974 656d 7328 293a 0a20  e_map.items():. 
+00027280: 2020 2020 2020 2072 656d 6f74 655f 7265         remote_re
+00027290: 736f 7572 6365 5f6e 616d 6573 203d 205b  source_names = [
+000272a0: 7265 2e73 7562 2866 225e 7b6f 6c64 5f77  re.sub(f"^{old_w
+000272b0: 737d 5c2e 222c 2066 227b 6e65 775f 7773  s}\.", f"{new_ws
+000272c0: 7d2e 222c 2078 2920 666f 7220 7820 696e  }.", x) for x in
+000272d0: 2072 656d 6f74 655f 7265 736f 7572 6365   remote_resource
+000272e0: 5f6e 616d 6573 5d0a 0a20 2020 2069 6620  _names]..    if 
+000272f0: 6e6f 7420 6669 6c65 6e61 6d65 733a 0a20  not filenames:. 
+00027300: 2020 2020 2020 2066 696c 656e 616d 6573         filenames
+00027310: 203d 2067 6574 5f70 726f 6a65 6374 5f66   = get_project_f
+00027320: 696c 656e 616d 6573 2866 6f6c 6465 7229  ilenames(folder)
+00027330: 0a0a 2020 2020 2320 6765 7420 7468 6520  ..    # get the 
+00027340: 6c69 7374 206f 6620 6368 616e 6765 730a  list of changes.
+00027350: 2020 2020 6368 616e 6765 642c 2064 656c      changed, del
+00027360: 6574 6564 203d 2061 7761 6974 2064 6570  eted = await dep
+00027370: 6c6f 796d 656e 742e 6465 7465 6374 5f63  loyment.detect_c
+00027380: 6861 6e67 6573 2866 696c 656e 616d 6573  hanges(filenames
+00027390: 2c20 6f6e 6c79 5f63 6861 6e67 6573 2c20  , only_changes, 
+000273a0: 636f 6e66 6967 2c20 7573 655f 6d61 696e  config, use_main
+000273b0: 290a 0a20 2020 2064 6570 6c6f 796d 656e  )..    deploymen
+000273c0: 742e 6368 6563 6b5f 6368 616e 6765 7328  t.check_changes(
+000273d0: 6368 616e 6765 642c 2070 6970 6573 2c20  changed, pipes, 
+000273e0: 7265 6c65 6173 655f 6372 6561 7465 6429  release_created)
+000273f0: 0a0a 2020 2020 6465 706c 6f79 6d65 6e74  ..    deployment
+00027400: 2e70 7265 7061 7269 6e67 5f72 656c 6561  .preparing_relea
+00027410: 7365 2829 0a0a 2020 2020 2320 6275 696c  se()..    # buil
+00027420: 6420 6772 6170 6820 746f 2067 6574 206e  d graph to get n
+00027430: 6577 2076 6572 7369 6f6e 7320 666f 7220  ew versions for 
+00027440: 616c 6c20 7468 6520 6669 6c65 7320 696e  all the files in
+00027450: 766f 6c76 6564 2069 6e20 7468 6520 7175  volved in the qu
+00027460: 6572 790a 2020 2020 2320 6465 7065 6e64  ery.    # depend
+00027470: 656e 6369 6573 206e 6565 6420 746f 2062  encies need to b
+00027480: 6520 7072 6f63 6573 7365 6420 616c 7761  e processed alwa
+00027490: 7973 2074 6f20 6765 7420 7468 6520 7665  ys to get the ve
+000274a0: 7273 696f 6e73 0a20 2020 2064 6570 656e  rsions.    depen
+000274b0: 6465 6e63 6965 735f 6772 6170 6820 3d20  dencies_graph = 
+000274c0: 6177 6169 7420 6275 696c 645f 6772 6170  await build_grap
+000274d0: 6828 0a20 2020 2020 2020 2066 696c 656e  h(.        filen
+000274e0: 616d 6573 2c0a 2020 2020 2020 2020 7462  ames,.        tb
+000274f0: 5f63 6c69 656e 742c 0a20 2020 2020 2020  _client,.       
+00027500: 2064 6972 5f70 6174 683d 666f 6c64 6572   dir_path=folder
+00027510: 2c0a 2020 2020 2020 2020 7072 6f63 6573  ,.        proces
+00027520: 735f 6465 7065 6e64 656e 6369 6573 3d54  s_dependencies=T
+00027530: 7275 652c 0a20 2020 2020 2020 2077 6f72  rue,.        wor
+00027540: 6b73 7061 6365 5f6d 6170 3d77 6f72 6b73  kspace_map=works
+00027550: 7061 6365 5f6d 6170 2c0a 2020 2020 2020  pace_map,.      
+00027560: 2020 736b 6970 5f63 6f6e 6e65 6374 6f72    skip_connector
+00027570: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
+00027580: 776f 726b 7370 6163 655f 6c69 625f 7061  workspace_lib_pa
+00027590: 7468 733d 776f 726b 7370 6163 655f 6c69  ths=workspace_li
+000275a0: 625f 7061 7468 732c 0a20 2020 2020 2020  b_paths,.       
+000275b0: 2063 7572 7265 6e74 5f77 733d 6375 7272   current_ws=curr
+000275c0: 656e 745f 7773 2c0a 2020 2020 2020 2020  ent_ws,.        
+000275d0: 6368 616e 6765 643d 6368 616e 6765 642c  changed=changed,
+000275e0: 0a20 2020 2020 2020 206f 6e6c 795f 6368  .        only_ch
+000275f0: 616e 6765 733d 6f6e 6c79 5f63 6861 6e67  anges=only_chang
+00027600: 6573 206f 7220 2864 6570 6c6f 796d 656e  es or (deploymen
+00027610: 742e 6973 5f67 6974 5f72 656c 6561 7365  t.is_git_release
+00027620: 2061 6e64 2068 6173 5f73 656d 7665 7229   and has_semver)
+00027630: 2c0a 2020 2020 2020 2020 666f 726b 5f64  ,.        fork_d
+00027640: 6f77 6e73 7472 6561 6d3d 666f 726b 5f64  ownstream=fork_d
+00027650: 6f77 6e73 7472 6561 6d2c 0a20 2020 2020  ownstream,.     
+00027660: 2020 2069 735f 696e 7465 726e 616c 3d69     is_internal=i
+00027670: 735f 696e 7465 726e 616c 2c0a 2020 2020  s_internal,.    
+00027680: 290a 0a20 2020 2023 2075 7064 6174 6520  )..    # update 
+00027690: 6578 6973 7469 6e67 2076 6572 7369 6f6e  existing version
+000276a0: 730a 2020 2020 6966 206e 6f74 206e 6f5f  s.    if not no_
+000276b0: 7665 7273 696f 6e73 3a0a 2020 2020 2020  versions:.      
+000276c0: 2020 7265 736f 7572 6365 5f76 6572 7369    resource_versi
+000276d0: 6f6e 7320 3d20 6765 745f 7265 736f 7572  ons = get_resour
+000276e0: 6365 5f76 6572 7369 6f6e 7328 6578 6973  ce_versions(exis
+000276f0: 7469 6e67 5f72 6573 6f75 7263 6573 290a  ting_resources).
+00027700: 2020 2020 2020 2020 6c61 7465 7374 5f64          latest_d
+00027710: 6174 6173 6f75 7263 655f 7665 7273 696f  atasource_versio
+00027720: 6e73 203d 2072 6573 6f75 7263 655f 7665  ns = resource_ve
+00027730: 7273 696f 6e73 2e63 6f70 7928 290a 0a20  rsions.copy().. 
+00027740: 2020 2020 2020 2066 6f72 2064 6570 2069         for dep i
+00027750: 6e20 6465 7065 6e64 656e 6369 6573 5f67  n dependencies_g
+00027760: 7261 7068 2e74 6f5f 7275 6e2e 7661 6c75  raph.to_run.valu
+00027770: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
+00027780: 2020 6473 203d 2064 6570 5b22 7265 736f    ds = dep["reso
+00027790: 7572 6365 5f6e 616d 6522 5d0a 2020 2020  urce_name"].    
+000277a0: 2020 2020 2020 2020 6966 2064 6570 5b22          if dep["
+000277b0: 7665 7273 696f 6e22 5d20 6973 206e 6f74  version"] is not
+000277c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000277d0: 2020 2020 2020 206c 6174 6573 745f 6461         latest_da
+000277e0: 7461 736f 7572 6365 5f76 6572 7369 6f6e  tasource_version
+000277f0: 735b 6473 5d20 3d20 6465 705b 2276 6572  s[ds] = dep["ver
+00027800: 7369 6f6e 225d 0a20 2020 2065 6c73 653a  sion"].    else:
+00027810: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
+00027820: 655f 7665 7273 696f 6e73 203d 207b 7d0a  e_versions = {}.
+00027830: 2020 2020 2020 2020 6c61 7465 7374 5f64          latest_d
+00027840: 6174 6173 6f75 7263 655f 7665 7273 696f  atasource_versio
+00027850: 6e73 203d 207b 7d0a 0a20 2020 2023 2049  ns = {}..    # I
+00027860: 6620 7765 2068 6176 6520 6461 7461 736f  f we have dataso
+00027870: 7572 6365 7320 7573 696e 6720 5645 5253  urces using VERS
+00027880: 494f 4e2c 206c 6574 2773 2074 7279 2074  ION, let's try t
+00027890: 6f20 6765 7420 7468 6520 6c61 7465 7374  o get the latest
+000278a0: 2076 6572 7369 6f6e 0a20 2020 2064 6570   version.    dep
+000278b0: 656e 6465 6e63 6965 735f 6772 6170 6820  endencies_graph 
+000278c0: 3d20 6177 6169 7420 6275 696c 645f 6772  = await build_gr
+000278d0: 6170 6828 0a20 2020 2020 2020 2066 696c  aph(.        fil
+000278e0: 656e 616d 6573 2c0a 2020 2020 2020 2020  enames,.        
+000278f0: 7462 5f63 6c69 656e 742c 0a20 2020 2020  tb_client,.     
+00027900: 2020 2064 6972 5f70 6174 683d 666f 6c64     dir_path=fold
+00027910: 6572 2c0a 2020 2020 2020 2020 7265 736f  er,.        reso
+00027920: 7572 6365 5f76 6572 7369 6f6e 733d 6c61  urce_versions=la
+00027930: 7465 7374 5f64 6174 6173 6f75 7263 655f  test_datasource_
+00027940: 7665 7273 696f 6e73 2c0a 2020 2020 2020  versions,.      
+00027950: 2020 776f 726b 7370 6163 655f 6d61 703d    workspace_map=
+00027960: 776f 726b 7370 6163 655f 6d61 702c 0a20  workspace_map,. 
+00027970: 2020 2020 2020 2070 726f 6365 7373 5f64         process_d
+00027980: 6570 656e 6465 6e63 6965 733d 7075 7368  ependencies=push
+00027990: 5f64 6570 732c 0a20 2020 2020 2020 2076  _deps,.        v
+000279a0: 6572 626f 7365 3d76 6572 626f 7365 2c0a  erbose=verbose,.
+000279b0: 2020 2020 2020 2020 776f 726b 7370 6163          workspac
+000279c0: 655f 6c69 625f 7061 7468 733d 776f 726b  e_lib_paths=work
+000279d0: 7370 6163 655f 6c69 625f 7061 7468 732c  space_lib_paths,
+000279e0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
+000279f0: 5f77 733d 6375 7272 656e 745f 7773 2c0a  _ws=current_ws,.
+00027a00: 2020 2020 2020 2020 6368 616e 6765 643d          changed=
+00027a10: 6368 616e 6765 642c 0a20 2020 2020 2020  changed,.       
+00027a20: 206f 6e6c 795f 6368 616e 6765 733d 6f6e   only_changes=on
+00027a30: 6c79 5f63 6861 6e67 6573 206f 7220 2864  ly_changes or (d
+00027a40: 6570 6c6f 796d 656e 742e 6973 5f67 6974  eployment.is_git
+00027a50: 5f72 656c 6561 7365 2061 6e64 2068 6173  _release and has
+00027a60: 5f73 656d 7665 7229 2c0a 2020 2020 2020  _semver),.      
+00027a70: 2020 666f 726b 5f64 6f77 6e73 7472 6561    fork_downstrea
+00027a80: 6d3d 666f 726b 5f64 6f77 6e73 7472 6561  m=fork_downstrea
+00027a90: 6d2c 0a20 2020 2020 2020 2069 735f 696e  m,.        is_in
+00027aa0: 7465 726e 616c 3d69 735f 696e 7465 726e  ternal=is_intern
+00027ab0: 616c 2c0a 2020 2020 290a 0a20 2020 2069  al,.    )..    i
+00027ac0: 6620 6465 6275 673a 0a20 2020 2020 2020  f debug:.       
+00027ad0: 2070 702e 7070 7269 6e74 2864 6570 656e   pp.pprint(depen
+00027ae0: 6465 6e63 6965 735f 6772 6170 682e 746f  dencies_graph.to
+00027af0: 5f72 756e 290a 0a20 2020 2069 6620 7665  _run)..    if ve
+00027b00: 7262 6f73 653a 0a20 2020 2020 2020 2063  rbose:.        c
+00027b10: 6c69 636b 2e65 6368 6f28 4665 6564 6261  lick.echo(Feedba
+00027b20: 636b 4d61 6e61 6765 722e 696e 666f 5f62  ckManager.info_b
+00027b30: 7569 6c64 696e 675f 6465 7065 6e64 656e  uilding_dependen
+00027b40: 6369 6573 2829 290a 0a20 2020 2064 6570  cies())..    dep
+00027b50: 6c6f 796d 656e 742e 7072 6570 6172 696e  loyment.preparin
+00027b60: 675f 6465 7065 6e64 656e 6369 6573 2863  g_dependencies(c
+00027b70: 6861 6e67 6564 2c20 6465 7065 6e64 656e  hanged, dependen
+00027b80: 6369 6573 5f67 7261 7068 2e64 6570 5f6d  cies_graph.dep_m
+00027b90: 6170 2c20 6c61 7465 7374 5f64 6174 6173  ap, latest_datas
+00027ba0: 6f75 7263 655f 7665 7273 696f 6e73 290a  ource_versions).
+00027bb0: 0a20 2020 2064 6566 2073 686f 756c 645f  .    def should_
+00027bc0: 7075 7368 5f66 696c 6528 0a20 2020 2020  push_file(.     
+00027bd0: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
+00027be0: 2020 2020 2020 7265 6d6f 7465 5f72 6573        remote_res
+00027bf0: 6f75 7263 655f 6e61 6d65 733a 204c 6973  ource_names: Lis
+00027c00: 745b 7374 725d 2c0a 2020 2020 2020 2020  t[str],.        
+00027c10: 6c61 7465 7374 5f64 6174 6173 6f75 7263  latest_datasourc
+00027c20: 655f 7665 7273 696f 6e73 3a20 4469 6374  e_versions: Dict
+00027c30: 5b73 7472 2c20 416e 795d 2c0a 2020 2020  [str, Any],.    
+00027c40: 2020 2020 666f 7263 653a 2062 6f6f 6c2c      force: bool,
+00027c50: 0a20 2020 2020 2020 2072 756e 5f74 6573  .        run_tes
+00027c60: 7473 3a20 626f 6f6c 2c0a 2020 2020 2920  ts: bool,.    ) 
+00027c70: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00027c80: 2022 2222 0a20 2020 2020 2020 2046 756e   """.        Fun
+00027c90: 6374 696f 6e20 746f 206b 6e6f 7720 6966  ction to know if
+00027ca0: 2077 6520 6e65 6564 2074 6f20 7275 6e20   we need to run 
+00027cb0: 6120 6669 6c65 206f 7220 6e6f 740a 2020  a file or not.  
+00027cc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00027cd0: 2020 6966 206e 616d 6520 6e6f 7420 696e    if name not in
+00027ce0: 2072 656d 6f74 655f 7265 736f 7572 6365   remote_resource
+00027cf0: 5f6e 616d 6573 3a0a 2020 2020 2020 2020  _names:.        
+00027d00: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00027d10: 2020 2020 2020 2020 2320 5768 656e 2077          # When w
+00027d20: 6520 6e65 6564 2074 6f20 7472 7920 746f  e need to try to
+00027d30: 2070 7573 6820 6120 6669 6c65 2077 6865   push a file whe
+00027d40: 6e20 6974 2064 6f65 736e 2774 2065 7869  n it doesn't exi
+00027d50: 7374 2061 6e64 2074 6865 2076 6572 7369  st and the versi
+00027d60: 6f6e 2069 7320 6469 6666 6572 656e 7420  on is different 
+00027d70: 7468 6174 2074 6865 2065 7869 7374 696e  that the existin
+00027d80: 6720 6f6e 650a 2020 2020 2020 2020 7265  g one.        re
+00027d90: 736f 7572 6365 5f66 756c 6c5f 6e61 6d65  source_full_name
+00027da0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00027db0: 2066 227b 6e61 6d65 7d5f 5f76 7b6c 6174   f"{name}__v{lat
+00027dc0: 6573 745f 6461 7461 736f 7572 6365 5f76  est_datasource_v
+00027dd0: 6572 7369 6f6e 732e 6765 7428 6e61 6d65  ersions.get(name
+00027de0: 297d 2220 6966 206e 616d 6520 696e 206c  )}" if name in l
+00027df0: 6174 6573 745f 6461 7461 736f 7572 6365  atest_datasource
+00027e00: 5f76 6572 7369 6f6e 7320 656c 7365 206e  _versions else n
+00027e10: 616d 650a 2020 2020 2020 2020 290a 2020  ame.        ).  
+00027e20: 2020 2020 2020 6966 2072 6573 6f75 7263        if resourc
+00027e30: 655f 6675 6c6c 5f6e 616d 6520 6e6f 7420  e_full_name not 
+00027e40: 696e 2065 7869 7374 696e 675f 7265 736f  in existing_reso
+00027e50: 7572 6365 733a 0a20 2020 2020 2020 2020  urces:.         
+00027e60: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00027e70: 2020 2020 2020 2069 6620 666f 7263 6520         if force 
+00027e80: 6f72 2072 756e 5f74 6573 7473 3a0a 2020  or run_tests:.  
+00027e90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00027ea0: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+00027eb0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00027ec0: 6173 796e 6320 6465 6620 7075 7368 280a  async def push(.
+00027ed0: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
+00027ee0: 722c 0a20 2020 2020 2020 2074 6f5f 7275  r,.        to_ru
+00027ef0: 6e3a 2044 6963 745b 7374 722c 2044 6963  n: Dict[str, Dic
+00027f00: 745b 7374 722c 2041 6e79 5d5d 2c0a 2020  t[str, Any]],.  
+00027f10: 2020 2020 2020 7265 736f 7572 6365 5f76        resource_v
+00027f20: 6572 7369 6f6e 733a 2044 6963 745b 7374  ersions: Dict[st
+00027f30: 722c 2041 6e79 5d2c 0a20 2020 2020 2020  r, Any],.       
+00027f40: 206c 6174 6573 745f 6461 7461 736f 7572   latest_datasour
+00027f50: 6365 5f76 6572 7369 6f6e 733a 2044 6963  ce_versions: Dic
+00027f60: 745b 7374 722c 2041 6e79 5d2c 0a20 2020  t[str, Any],.   
+00027f70: 2020 2020 2064 7279 5f72 756e 3a20 626f       dry_run: bo
+00027f80: 6f6c 2c0a 2020 2020 2020 2020 666f 726b  ol,.        fork
+00027f90: 5f64 6f77 6e73 7472 6561 6d3a 204f 7074  _downstream: Opt
+00027fa0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4661  ional[bool] = Fa
+00027fb0: 6c73 652c 0a20 2020 2020 2020 2066 6f72  lse,.        for
+00027fc0: 6b3a 204f 7074 696f 6e61 6c5b 626f 6f6c  k: Optional[bool
+00027fd0: 5d20 3d20 4661 6c73 652c 0a20 2020 2029  ] = False,.    )
+00027fe0: 3a0a 2020 2020 2020 2020 6966 206e 616d  :.        if nam
+00027ff0: 6520 696e 2074 6f5f 7275 6e3a 0a20 2020  e in to_run:.   
+00028000: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00028010: 6472 795f 7275 6e3a 0a20 2020 2020 2020  dry_run:.       
+00028020: 2020 2020 2020 2020 2069 6620 7368 6f75           if shou
+00028030: 6c64 5f70 7573 685f 6669 6c65 286e 616d  ld_push_file(nam
+00028040: 652c 2072 656d 6f74 655f 7265 736f 7572  e, remote_resour
+00028050: 6365 5f6e 616d 6573 2c20 6c61 7465 7374  ce_names, latest
+00028060: 5f64 6174 6173 6f75 7263 655f 7665 7273  _datasource_vers
+00028070: 696f 6e73 2c20 666f 7263 652c 2072 756e  ions, force, run
+00028080: 5f74 6573 7473 293a 0a20 2020 2020 2020  _tests):.       
+00028090: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000280a0: 6e61 6d65 206e 6f74 2069 6e20 7265 736f  name not in reso
+000280b0: 7572 6365 5f76 6572 7369 6f6e 733a 0a20  urce_versions:. 
+000280c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000280d0: 2020 2020 2020 2076 6572 7369 6f6e 203d         version =
+000280e0: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
+000280f0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00028100: 616d 6520 696e 206c 6174 6573 745f 6461  ame in latest_da
+00028110: 7461 736f 7572 6365 5f76 6572 7369 6f6e  tasource_version
+00028120: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00028130: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00028140: 6572 7369 6f6e 203d 2066 2228 767b 6c61  ersion = f"(v{la
+00028150: 7465 7374 5f64 6174 6173 6f75 7263 655f  test_datasource_
+00028160: 7665 7273 696f 6e73 5b6e 616d 655d 7d29  versions[name]})
+00028170: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00028180: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00028190: 6563 686f 2846 6565 6462 6163 6b4d 616e  echo(FeedbackMan
+000281a0: 6167 6572 2e69 6e66 6f5f 7072 6f63 6573  ager.info_proces
+000281b0: 7369 6e67 5f6e 6577 5f72 6573 6f75 7263  sing_new_resourc
+000281c0: 6528 6e61 6d65 3d6e 616d 652c 2076 6572  e(name=name, ver
+000281d0: 7369 6f6e 3d76 6572 7369 6f6e 2929 0a20  sion=version)). 
+000281e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00028200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028210: 2063 6c69 636b 2e65 6368 6f28 0a20 2020   click.echo(.   
 00028220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028230: 2046 6565 6462 6163 6b4d 616e 6167 6572   FeedbackManager
-00028240: 2e69 6e66 6f5f 7072 6f63 6573 7369 6e67  .info_processing
-00028250: 5f72 6573 6f75 7263 6528 0a20 2020 2020  _resource(.     
-00028260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028270: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00028280: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00028230: 2020 2020 2020 2020 2046 6565 6462 6163           Feedbac
+00028240: 6b4d 616e 6167 6572 2e69 6e66 6f5f 7072  kManager.info_pr
+00028250: 6f63 6573 7369 6e67 5f72 6573 6f75 7263  ocessing_resourc
+00028260: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00028270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028280: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
 00028290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000282a0: 2020 2020 2020 7665 7273 696f 6e3d 6c61        version=la
-000282b0: 7465 7374 5f64 6174 6173 6f75 7263 655f  test_datasource_
-000282c0: 7665 7273 696f 6e73 5b6e 616d 655d 2c0a  versions[name],.
-000282d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000282a0: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+000282b0: 7273 696f 6e3d 6c61 7465 7374 5f64 6174  rsion=latest_dat
+000282c0: 6173 6f75 7263 655f 7665 7273 696f 6e73  asource_versions
+000282d0: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
 000282e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000282f0: 6c61 7465 7374 5f76 6572 7369 6f6e 3d72  latest_version=r
-00028300: 6573 6f75 7263 655f 7665 7273 696f 6e73  esource_versions
-00028310: 2e67 6574 286e 616d 6529 2c0a 2020 2020  .get(name),.    
-00028320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028330: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00028340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028350: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00028360: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00028370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028380: 2020 2020 2061 7761 6974 2065 7865 635f       await exec_
-00028390: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
+000282f0: 2020 2020 2020 2020 6c61 7465 7374 5f76          latest_v
+00028300: 6572 7369 6f6e 3d72 6573 6f75 7263 655f  ersion=resource_
+00028310: 7665 7273 696f 6e73 2e67 6574 286e 616d  versions.get(nam
+00028320: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00028330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00028350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00028360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028370: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00028380: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+00028390: 6974 2065 7865 635f 6669 6c65 280a 2020  it exec_file(.  
 000283a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283b0: 2020 636f 6e66 6967 2c0a 2020 2020 2020    config,.      
-000283c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283d0: 2020 2020 2020 746f 5f72 756e 5b6e 616d        to_run[nam
-000283e0: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+000283b0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+000283c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000283d0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+000283e0: 5f72 756e 5b6e 616d 655d 2c0a 2020 2020  _run[name],.    
 000283f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028400: 7462 5f63 6c69 656e 742c 0a20 2020 2020  tb_client,.     
-00028410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028420: 2020 2020 2020 2066 6f72 6365 2c0a 2020         force,.  
-00028430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028440: 2020 2020 2020 2020 2020 6368 6563 6b2c            check,
-00028450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028460: 2020 2020 2020 2020 2020 2020 2064 6562               deb
-00028470: 7567 2061 6e64 2076 6572 626f 7365 2c0a  ug and verbose,.
-00028480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028490: 2020 2020 2020 2020 2020 2020 706f 7075              popu
-000284a0: 6c61 7465 2c0a 2020 2020 2020 2020 2020  late,.          
+00028400: 2020 2020 2020 2020 7462 5f63 6c69 656e          tb_clien
+00028410: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00028420: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00028430: 6f72 6365 2c0a 2020 2020 2020 2020 2020  orce,.          
+00028440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028450: 2020 6368 6563 6b2c 0a20 2020 2020 2020    check,.       
+00028460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028470: 2020 2020 2064 6562 7567 2061 6e64 2076       debug and v
+00028480: 6572 626f 7365 2c0a 2020 2020 2020 2020  erbose,.        
+00028490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000284a0: 2020 2020 706f 7075 6c61 7465 2c0a 2020      populate,.  
 000284b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284c0: 2020 706f 7075 6c61 7465 5f73 7562 7365    populate_subse
-000284d0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-000284e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000284f0: 6f70 756c 6174 655f 636f 6e64 6974 696f  opulate_conditio
-00028500: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00028510: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00028520: 6e6c 696e 6b5f 6f6e 5f70 6f70 756c 6174  nlink_on_populat
-00028530: 655f 6572 726f 722c 0a20 2020 2020 2020  e_error,.       
-00028540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028550: 2020 2020 2077 6169 742c 0a20 2020 2020       wait,.     
-00028560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028570: 2020 2020 2020 2075 7365 725f 746f 6b65         user_toke
-00028580: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00028590: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000285a0: 7665 7272 6964 655f 6461 7461 736f 7572  verride_datasour
-000285b0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+000284c0: 2020 2020 2020 2020 2020 706f 7075 6c61            popula
+000284d0: 7465 5f73 7562 7365 742c 0a20 2020 2020  te_subset,.     
+000284e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000284f0: 2020 2020 2020 2070 6f70 756c 6174 655f         populate_
+00028500: 636f 6e64 6974 696f 6e2c 0a20 2020 2020  condition,.     
+00028510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028520: 2020 2020 2020 2075 6e6c 696e 6b5f 6f6e         unlink_on
+00028530: 5f70 6f70 756c 6174 655f 6572 726f 722c  _populate_error,
+00028540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028550: 2020 2020 2020 2020 2020 2020 2077 6169               wai
+00028560: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00028570: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00028580: 7365 725f 746f 6b65 6e2c 0a20 2020 2020  ser_token,.     
+00028590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000285a0: 2020 2020 2020 206f 7665 7272 6964 655f         override_
+000285b0: 6461 7461 736f 7572 6365 2c0a 2020 2020  datasource,.    
 000285c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000285d0: 6967 6e6f 7265 5f73 716c 5f65 7272 6f72  ignore_sql_error
-000285e0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000285f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00028600: 6b69 705f 636f 6e66 6972 6d61 7469 6f6e  kip_confirmation
-00028610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00028620: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-00028630: 6c79 5f72 6573 706f 6e73 655f 7469 6d65  ly_response_time
-00028640: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00028650: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00028660: 696d 656f 7574 2c0a 2020 2020 2020 2020  imeout,.        
+000285d0: 2020 2020 2020 2020 6967 6e6f 7265 5f73          ignore_s
+000285e0: 716c 5f65 7272 6f72 732c 0a20 2020 2020  ql_errors,.     
+000285f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028600: 2020 2020 2020 2073 6b69 705f 636f 6e66         skip_conf
+00028610: 6972 6d61 7469 6f6e 2c0a 2020 2020 2020  irmation,.      
+00028620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028630: 2020 2020 2020 6f6e 6c79 5f72 6573 706f        only_respo
+00028640: 6e73 655f 7469 6d65 732c 0a20 2020 2020  nse_times,.     
+00028650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028660: 2020 2020 2020 2074 696d 656f 7574 2c0a         timeout,.
 00028670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028680: 2020 2020 7275 6e5f 7465 7374 732c 0a20      run_tests,. 
-00028690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000286a0: 2020 2020 2020 2020 2020 2061 735f 7374             as_st
-000286b0: 616e 6461 7264 2c0a 2020 2020 2020 2020  andard,.        
+00028680: 2020 2020 2020 2020 2020 2020 7275 6e5f              run_
+00028690: 7465 7374 732c 0a20 2020 2020 2020 2020  tests,.         
+000286a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000286b0: 2020 2061 735f 7374 616e 6461 7264 2c0a     as_standard,.
 000286c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000286d0: 2020 2020 7465 7374 735f 746f 5f72 756e      tests_to_run
-000286e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000286f0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00028700: 7374 735f 7361 6d70 6c65 5f62 795f 7061  sts_sample_by_pa
-00028710: 7261 6d73 2c0a 2020 2020 2020 2020 2020  rams,.          
+000286d0: 2020 2020 2020 2020 2020 2020 7465 7374              test
+000286e0: 735f 746f 5f72 756e 2c0a 2020 2020 2020  s_to_run,.      
+000286f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028700: 2020 2020 2020 7465 7374 735f 7361 6d70        tests_samp
+00028710: 6c65 5f62 795f 7061 7261 6d73 2c0a 2020  le_by_params,.  
 00028720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028730: 2020 7465 7374 735f 6669 6c74 6572 5f62    tests_filter_b
-00028740: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-00028750: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00028760: 6573 7473 5f66 6169 6c66 6173 742c 0a20  ests_failfast,. 
-00028770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028780: 2020 2020 2020 2020 2020 2074 6573 7473             tests
-00028790: 5f69 676e 6f72 655f 6f72 6465 722c 0a20  _ignore_order,. 
-000287a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000287b0: 2020 2020 2020 2020 2020 2074 6573 7473             tests
-000287c0: 5f76 616c 6964 6174 655f 7072 6f63 6573  _validate_proces
-000287d0: 7365 645f 6279 7465 732c 0a20 2020 2020  sed_bytes,.     
-000287e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000287f0: 2020 2020 2020 2074 6573 7473 5f63 6865         tests_che
-00028800: 636b 5f72 6571 7565 7374 735f 6672 6f6d  ck_requests_from
-00028810: 5f62 7261 6e63 682c 0a20 2020 2020 2020  _branch,.       
-00028820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028830: 2020 2020 2063 7572 7265 6e74 5f77 732c       current_ws,
-00028840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028850: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00028860: 6b5f 646f 776e 7374 7265 616d 2c0a 2020  k_downstream,.  
-00028870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028880: 2020 2020 2020 2020 2020 666f 726b 2c0a            fork,.
-00028890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000288a0: 2020 2020 2020 2020 2020 2020 6769 745f              git_
-000288b0: 7265 6c65 6173 652c 0a20 2020 2020 2020  release,.       
-000288c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000288d0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000288e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000288f0: 7420 7275 6e5f 7465 7374 733a 0a20 2020  t run_tests:.   
-00028900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028910: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-00028920: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+00028730: 2020 2020 2020 2020 2020 7465 7374 735f            tests_
+00028740: 6669 6c74 6572 5f62 792c 0a20 2020 2020  filter_by,.     
+00028750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028760: 2020 2020 2020 2074 6573 7473 5f66 6169         tests_fai
+00028770: 6c66 6173 742c 0a20 2020 2020 2020 2020  lfast,.         
+00028780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028790: 2020 2074 6573 7473 5f69 676e 6f72 655f     tests_ignore_
+000287a0: 6f72 6465 722c 0a20 2020 2020 2020 2020  order,.         
+000287b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000287c0: 2020 2074 6573 7473 5f76 616c 6964 6174     tests_validat
+000287d0: 655f 7072 6f63 6573 7365 645f 6279 7465  e_processed_byte
+000287e0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000287f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00028800: 6573 7473 5f63 6865 636b 5f72 6571 7565  ests_check_reque
+00028810: 7374 735f 6672 6f6d 5f62 7261 6e63 682c  sts_from_branch,
+00028820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028830: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00028840: 7265 6e74 5f77 732c 0a20 2020 2020 2020  rent_ws,.       
+00028850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028860: 2020 2020 2066 6f72 6b5f 646f 776e 7374       fork_downst
+00028870: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
+00028880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028890: 2020 666f 726b 2c0a 2020 2020 2020 2020    fork,.        
+000288a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000288b0: 2020 2020 6769 745f 7265 6c65 6173 652c      git_release,
+000288c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000288d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000288e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000288f0: 2020 2069 6620 6e6f 7420 7275 6e5f 7465     if not run_te
+00028900: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
+00028910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028920: 2063 6c69 636b 2e65 6368 6f28 0a20 2020   click.echo(.   
 00028930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028940: 2020 2020 2046 6565 6462 6163 6b4d 616e       FeedbackMan
-00028950: 6167 6572 2e73 7563 6365 7373 5f63 7265  ager.success_cre
-00028960: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
+00028940: 2020 2020 2020 2020 2020 2020 2046 6565               Fee
+00028950: 6462 6163 6b4d 616e 6167 6572 2e73 7563  dbackManager.suc
+00028960: 6365 7373 5f63 7265 6174 6528 0a20 2020  cess_create(.   
 00028970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028980: 2020 2020 2020 2020 206e 616d 653d 280a           name=(.
-00028990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028990: 206e 616d 653d 280a 2020 2020 2020 2020   name=(.        
 000289a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000289b0: 2020 2020 2020 2020 6e61 6d65 0a20 2020          name.   
-000289c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000289b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000289c0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
 000289d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000289e0: 2020 2020 2069 6620 746f 5f72 756e 5b6e       if to_run[n
-000289f0: 616d 655d 5b22 7665 7273 696f 6e22 5d20  ame]["version"] 
-00028a00: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
+000289e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000289f0: 746f 5f72 756e 5b6e 616d 655d 5b22 7665  to_run[name]["ve
+00028a00: 7273 696f 6e22 5d20 6973 204e 6f6e 650a  rsion"] is None.
 00028a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00028a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a30: 656c 7365 2066 277b 6e61 6d65 7d5f 5f76  else f'{name}__v
-00028a40: 7b74 6f5f 7275 6e5b 6e61 6d65 5d5b 2276  {to_run[name]["v
-00028a50: 6572 7369 6f6e 225d 7d27 0a20 2020 2020  ersion"]}'.     
-00028a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00028a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028a30: 2020 2020 2020 2020 656c 7365 2066 277b          else f'{
+00028a40: 6e61 6d65 7d5f 5f76 7b74 6f5f 7275 6e5b  name}__v{to_run[
+00028a50: 6e61 6d65 5d5b 2276 6572 7369 6f6e 225d  name]["version"]
+00028a60: 7d27 0a20 2020 2020 2020 2020 2020 2020  }'.             
+00028a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028a80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 00028a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028aa0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00028ab0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00028ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028ad0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00028ae0: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-00028af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b00: 2020 2020 6578 6365 7074 696f 6e20 3d20      exception = 
-00028b10: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
-00028b20: 6572 726f 725f 7075 7368 5f66 696c 655f  error_push_file_
-00028b30: 6578 6365 7074 696f 6e28 0a20 2020 2020  exception(.     
-00028b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b50: 2020 2020 2020 2066 696c 656e 616d 653d         filename=
-00028b60: 746f 5f72 756e 5b6e 616d 655d 5b22 6669  to_run[name]["fi
-00028b70: 6c65 6e61 6d65 225d 2c20 6572 726f 723d  lename"], error=
-00028b80: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00028b90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00028ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028bb0: 2020 2020 7261 6973 6520 636c 6963 6b2e      raise click.
-00028bc0: 436c 6963 6b45 7863 6570 7469 6f6e 2865  ClickException(e
-00028bd0: 7863 6570 7469 6f6e 290a 2020 2020 2020  xception).      
-00028be0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00028bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c00: 2020 2020 6966 2072 6169 7365 5f6f 6e5f      if raise_on_
-00028c10: 6578 6973 7473 3a0a 2020 2020 2020 2020  exists:.        
+00028aa0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00028ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028ac0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00028ad0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00028ae0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00028af0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00028b00: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00028b10: 7074 696f 6e20 3d20 4665 6564 6261 636b  ption = Feedback
+00028b20: 4d61 6e61 6765 722e 6572 726f 725f 7075  Manager.error_pu
+00028b30: 7368 5f66 696c 655f 6578 6365 7074 696f  sh_file_exceptio
+00028b40: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00028b50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00028b60: 696c 656e 616d 653d 746f 5f72 756e 5b6e  ilename=to_run[n
+00028b70: 616d 655d 5b22 6669 6c65 6e61 6d65 225d  ame]["filename"]
+00028b80: 2c20 6572 726f 723d 650a 2020 2020 2020  , error=e.      
+00028b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028ba0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00028bb0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00028bc0: 6520 636c 6963 6b2e 436c 6963 6b45 7863  e click.ClickExc
+00028bd0: 6570 7469 6f6e 2865 7863 6570 7469 6f6e  eption(exception
+00028be0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00028bf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00028c00: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00028c10: 6169 7365 5f6f 6e5f 6578 6973 7473 3a0a  aise_on_exists:.
 00028c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c30: 7261 6973 6520 416c 7265 6164 7945 7869  raise AlreadyExi
-00028c40: 7374 7345 7863 6570 7469 6f6e 280a 2020  stsException(.  
-00028c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c60: 2020 2020 2020 2020 2020 4665 6564 6261            Feedba
-00028c70: 636b 4d61 6e61 6765 722e 7761 726e 696e  ckManager.warnin
-00028c80: 675f 6e61 6d65 5f61 6c72 6561 6479 5f65  g_name_already_e
-00028c90: 7869 7374 7328 0a20 2020 2020 2020 2020  xists(.         
+00028c30: 2020 2020 2020 2020 7261 6973 6520 416c          raise Al
+00028c40: 7265 6164 7945 7869 7374 7345 7863 6570  readyExistsExcep
+00028c50: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00028c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028c70: 2020 4665 6564 6261 636b 4d61 6e61 6765    FeedbackManage
+00028c80: 722e 7761 726e 696e 675f 6e61 6d65 5f61  r.warning_name_a
+00028c90: 6c72 6561 6479 5f65 7869 7374 7328 0a20  lready_exists(. 
 00028ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028cb0: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
-00028cc0: 2069 6620 746f 5f72 756e 5b6e 616d 655d   if to_run[name]
-00028cd0: 5b22 7665 7273 696f 6e22 5d20 6973 204e  ["version"] is N
-00028ce0: 6f6e 6520 656c 7365 2066 277b 6e61 6d65  one else f'{name
-00028cf0: 7d5f 5f76 7b74 6f5f 7275 6e5b 6e61 6d65  }__v{to_run[name
-00028d00: 5d5b 2276 6572 7369 6f6e 225d 7d27 0a20  ]["version"]}'. 
-00028d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028d20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00028d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028d40: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00028d50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00028d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028d70: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-00028d80: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+00028cb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00028cc0: 616d 653d 6e61 6d65 2069 6620 746f 5f72  ame=name if to_r
+00028cd0: 756e 5b6e 616d 655d 5b22 7665 7273 696f  un[name]["versio
+00028ce0: 6e22 5d20 6973 204e 6f6e 6520 656c 7365  n"] is None else
+00028cf0: 2066 277b 6e61 6d65 7d5f 5f76 7b74 6f5f   f'{name}__v{to_
+00028d00: 7275 6e5b 6e61 6d65 5d5b 2276 6572 7369  run[name]["versi
+00028d10: 6f6e 225d 7d27 0a20 2020 2020 2020 2020  on"]}'.         
+00028d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d30: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00028d40: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00028d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00028d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d80: 2063 6c69 636b 2e65 6368 6f28 0a20 2020   click.echo(.   
 00028d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028da0: 2046 6565 6462 6163 6b4d 616e 6167 6572   FeedbackManager
-00028db0: 2e77 6172 6e69 6e67 5f6e 616d 655f 616c  .warning_name_al
-00028dc0: 7265 6164 795f 6578 6973 7473 280a 2020  ready_exists(.  
-00028dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028de0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00028df0: 6d65 3d6e 616d 6520 6966 2074 6f5f 7275  me=name if to_ru
-00028e00: 6e5b 6e61 6d65 5d5b 2276 6572 7369 6f6e  n[name]["version
-00028e10: 225d 2069 7320 4e6f 6e65 2065 6c73 6520  "] is None else 
-00028e20: 6627 7b6e 616d 657d 5f5f 767b 746f 5f72  f'{name}__v{to_r
-00028e30: 756e 5b6e 616d 655d 5b22 7665 7273 696f  un[name]["versio
-00028e40: 6e22 5d7d 270a 2020 2020 2020 2020 2020  n"]}'.          
+00028da0: 2020 2020 2020 2020 2046 6565 6462 6163           Feedbac
+00028db0: 6b4d 616e 6167 6572 2e77 6172 6e69 6e67  kManager.warning
+00028dc0: 5f6e 616d 655f 616c 7265 6164 795f 6578  _name_already_ex
+00028dd0: 6973 7473 280a 2020 2020 2020 2020 2020  ists(.          
+00028de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028df0: 2020 2020 2020 6e61 6d65 3d6e 616d 6520        name=name 
+00028e00: 6966 2074 6f5f 7275 6e5b 6e61 6d65 5d5b  if to_run[name][
+00028e10: 2276 6572 7369 6f6e 225d 2069 7320 4e6f  "version"] is No
+00028e20: 6e65 2065 6c73 6520 6627 7b6e 616d 657d  ne else f'{name}
+00028e30: 5f5f 767b 746f 5f72 756e 5b6e 616d 655d  __v{to_run[name]
+00028e40: 5b22 7665 7273 696f 6e22 5d7d 270a 2020  ["version"]}'.  
 00028e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028e60: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00028e70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00028e80: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00028e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ea0: 6966 2073 686f 756c 645f 7075 7368 5f66  if should_push_f
-00028eb0: 696c 6528 6e61 6d65 2c20 7265 6d6f 7465  ile(name, remote
-00028ec0: 5f72 6573 6f75 7263 655f 6e61 6d65 732c  _resource_names,
-00028ed0: 206c 6174 6573 745f 6461 7461 736f 7572   latest_datasour
-00028ee0: 6365 5f76 6572 7369 6f6e 732c 2066 6f72  ce_versions, for
-00028ef0: 6365 2c20 7275 6e5f 7465 7374 7329 3a0a  ce, run_tests):.
-00028f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028f10: 2020 2020 6966 206e 616d 6520 6e6f 7420      if name not 
-00028f20: 696e 2072 6573 6f75 7263 655f 7665 7273  in resource_vers
-00028f30: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-00028f40: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-00028f50: 7273 696f 6e20 3d20 2222 0a20 2020 2020  rsion = "".     
-00028f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028f70: 2020 2069 6620 6e61 6d65 2069 6e20 6c61     if name in la
-00028f80: 7465 7374 5f64 6174 6173 6f75 7263 655f  test_datasource_
-00028f90: 7665 7273 696f 6e73 3a0a 2020 2020 2020  versions:.      
-00028fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028fb0: 2020 2020 2020 7665 7273 696f 6e20 3d20        version = 
-00028fc0: 6622 2876 7b6c 6174 6573 745f 6461 7461  f"(v{latest_data
-00028fd0: 736f 7572 6365 5f76 6572 7369 6f6e 735b  source_versions[
-00028fe0: 6e61 6d65 5d7d 2922 0a20 2020 2020 2020  name]})".       
-00028ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029000: 2063 6c69 636b 2e65 6368 6f28 4665 6564   click.echo(Feed
-00029010: 6261 636b 4d61 6e61 6765 722e 696e 666f  backManager.info
-00029020: 5f64 7279 5f70 726f 6365 7373 696e 675f  _dry_processing_
-00029030: 6e65 775f 7265 736f 7572 6365 286e 616d  new_resource(nam
-00029040: 653d 6e61 6d65 2c20 7665 7273 696f 6e3d  e=name, version=
-00029050: 7665 7273 696f 6e29 290a 2020 2020 2020  version)).      
-00029060: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00029070: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00029080: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-00029090: 6b2e 6563 686f 280a 2020 2020 2020 2020  k.echo(.        
+00028e60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00028e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028e80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00028e90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00028ea0: 2020 2020 2020 2020 6966 2073 686f 756c          if shoul
+00028eb0: 645f 7075 7368 5f66 696c 6528 6e61 6d65  d_push_file(name
+00028ec0: 2c20 7265 6d6f 7465 5f72 6573 6f75 7263  , remote_resourc
+00028ed0: 655f 6e61 6d65 732c 206c 6174 6573 745f  e_names, latest_
+00028ee0: 6461 7461 736f 7572 6365 5f76 6572 7369  datasource_versi
+00028ef0: 6f6e 732c 2066 6f72 6365 2c20 7275 6e5f  ons, force, run_
+00028f00: 7465 7374 7329 3a0a 2020 2020 2020 2020  tests):.        
+00028f10: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00028f20: 616d 6520 6e6f 7420 696e 2072 6573 6f75  ame not in resou
+00028f30: 7263 655f 7665 7273 696f 6e73 3a0a 2020  rce_versions:.  
+00028f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028f50: 2020 2020 2020 7665 7273 696f 6e20 3d20        version = 
+00028f60: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00028f70: 2020 2020 2020 2020 2020 2069 6620 6e61             if na
+00028f80: 6d65 2069 6e20 6c61 7465 7374 5f64 6174  me in latest_dat
+00028f90: 6173 6f75 7263 655f 7665 7273 696f 6e73  asource_versions
+00028fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00028fb0: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+00028fc0: 7273 696f 6e20 3d20 6622 2876 7b6c 6174  rsion = f"(v{lat
+00028fd0: 6573 745f 6461 7461 736f 7572 6365 5f76  est_datasource_v
+00028fe0: 6572 7369 6f6e 735b 6e61 6d65 5d7d 2922  ersions[name]})"
+00028ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029000: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
+00029010: 6368 6f28 4665 6564 6261 636b 4d61 6e61  cho(FeedbackMana
+00029020: 6765 722e 696e 666f 5f64 7279 5f70 726f  ger.info_dry_pro
+00029030: 6365 7373 696e 675f 6e65 775f 7265 736f  cessing_new_reso
+00029040: 7572 6365 286e 616d 653d 6e61 6d65 2c20  urce(name=name, 
+00029050: 7665 7273 696f 6e3d 7665 7273 696f 6e29  version=version)
+00029060: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00029070: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00029080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029090: 2020 2020 636c 6963 6b2e 6563 686f 280a      click.echo(.
 000290a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000290b0: 2020 2020 4665 6564 6261 636b 4d61 6e61      FeedbackMana
-000290c0: 6765 722e 696e 666f 5f64 7279 5f70 726f  ger.info_dry_pro
-000290d0: 6365 7373 696e 675f 7265 736f 7572 6365  cessing_resource
-000290e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000290b0: 2020 2020 2020 2020 2020 2020 4665 6564              Feed
+000290c0: 6261 636b 4d61 6e61 6765 722e 696e 666f  backManager.info
+000290d0: 5f64 7279 5f70 726f 6365 7373 696e 675f  _dry_processing_
+000290e0: 7265 736f 7572 6365 280a 2020 2020 2020  resource(.      
 000290f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029100: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
-00029110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029120: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00029130: 7369 6f6e 3d6c 6174 6573 745f 6461 7461  sion=latest_data
-00029140: 736f 7572 6365 5f76 6572 7369 6f6e 735b  source_versions[
-00029150: 6e61 6d65 5d2c 0a20 2020 2020 2020 2020  name],.         
+00029100: 2020 2020 2020 2020 2020 6e61 6d65 3d6e            name=n
+00029110: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00029120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029130: 2020 2020 2076 6572 7369 6f6e 3d6c 6174       version=lat
+00029140: 6573 745f 6461 7461 736f 7572 6365 5f76  est_datasource_v
+00029150: 6572 7369 6f6e 735b 6e61 6d65 5d2c 0a20  ersions[name],. 
 00029160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029170: 2020 2020 2020 206c 6174 6573 745f 7665         latest_ve
-00029180: 7273 696f 6e3d 7265 736f 7572 6365 5f76  rsion=resource_v
-00029190: 6572 7369 6f6e 732e 6765 7428 6e61 6d65  ersions.get(name
-000291a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000291b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000291c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000291d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000291e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000291f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029200: 2020 2020 2063 6c69 636b 2e65 6368 6f28       click.echo(
-00029210: 4665 6564 6261 636b 4d61 6e61 6765 722e  FeedbackManager.
-00029220: 7761 726e 696e 675f 6472 795f 6e61 6d65  warning_dry_name
-00029230: 5f61 6c72 6561 6479 5f65 7869 7374 7328  _already_exists(
-00029240: 6e61 6d65 3d6e 616d 6529 290a 0a20 2020  name=name))..   
-00029250: 2061 7379 6e63 2064 6566 2070 7573 685f   async def push_
-00029260: 6669 6c65 7328 0a20 2020 2020 2020 2064  files(.        d
-00029270: 6570 656e 6465 6e63 795f 6772 6170 683a  ependency_graph:
-00029280: 2047 7261 7068 4465 7065 6e64 656e 6369   GraphDependenci
-00029290: 6573 2c0a 2020 2020 2020 2020 6472 795f  es,.        dry_
-000292a0: 7275 6e3a 2062 6f6f 6c20 3d20 4661 6c73  run: bool = Fals
-000292b0: 652c 0a20 2020 2020 2020 2063 6865 636b  e,.        check
-000292c0: 5f62 6163 6b66 696c 6c5f 7265 7175 6972  _backfill_requir
-000292d0: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
-000292e0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000292f0: 2065 6e64 706f 696e 7473 5f64 6570 5f6d   endpoints_dep_m
-00029300: 6170 203d 2064 6963 7428 290a 2020 2020  ap = dict().    
-00029310: 2020 2020 7072 6f63 6573 7365 6420 3d20      processed = 
-00029320: 7365 7428 290a 0a20 2020 2020 2020 2064  set()..        d
-00029330: 6570 656e 6465 6e63 6965 735f 6772 6170  ependencies_grap
-00029340: 6820 3d20 6465 7065 6e64 656e 6379 5f67  h = dependency_g
-00029350: 7261 7068 2e64 6570 5f6d 6170 0a20 2020  raph.dep_map.   
-00029360: 2020 2020 2072 6573 6f75 7263 6573 5f74       resources_t
-00029370: 6f5f 7275 6e20 3d20 6465 7065 6e64 656e  o_run = dependen
-00029380: 6379 5f67 7261 7068 2e74 6f5f 7275 6e0a  cy_graph.to_run.
-00029390: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000293a0: 666f 726b 5f64 6f77 6e73 7472 6561 6d3a  fork_downstream:
-000293b0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-000293c0: 6972 7374 2c20 7765 2077 696c 6c20 6465  irst, we will de
-000293d0: 706c 6f79 2074 6865 2061 6c6c 2074 6865  ploy the all the
-000293e0: 2072 6573 6f75 7263 6573 2066 6f6c 6c6f   resources follo
-000293f0: 7769 6e67 2074 6865 2064 6570 656e 6465  wing the depende
-00029400: 6e63 7920 6772 6170 6820 6578 6365 7074  ncy graph except
-00029410: 2066 6f72 2074 6865 2065 6e64 706f 696e   for the endpoin
-00029420: 7473 0a20 2020 2020 2020 2020 2020 2067  ts.            g
-00029430: 726f 7570 7320 3d20 5b67 726f 7570 2066  roups = [group f
-00029440: 6f72 2067 726f 7570 2069 6e20 746f 706f  or group in topo
-00029450: 736f 7274 2864 6570 656e 6465 6e63 6965  sort(dependencie
-00029460: 735f 6772 6170 6829 5d0a 2020 2020 2020  s_graph)].      
-00029470: 2020 2020 2020 666f 7220 6772 6f75 7020        for group 
-00029480: 696e 2067 726f 7570 733a 0a20 2020 2020  in groups:.     
-00029490: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-000294a0: 616d 6520 696e 2067 726f 7570 3a0a 2020  ame in group:.  
-000294b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000294c0: 2020 6966 206e 616d 6520 696e 2070 726f    if name in pro
-000294d0: 6365 7373 6564 3a0a 2020 2020 2020 2020  cessed:.        
+00029170: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00029180: 6174 6573 745f 7665 7273 696f 6e3d 7265  atest_version=re
+00029190: 736f 7572 6365 5f76 6572 7369 6f6e 732e  source_versions.
+000291a0: 6765 7428 6e61 6d65 292c 0a20 2020 2020  get(name),.     
+000291b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000291c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000291d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000291e0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000291f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00029200: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+00029210: 636b 2e65 6368 6f28 4665 6564 6261 636b  ck.echo(Feedback
+00029220: 4d61 6e61 6765 722e 7761 726e 696e 675f  Manager.warning_
+00029230: 6472 795f 6e61 6d65 5f61 6c72 6561 6479  dry_name_already
+00029240: 5f65 7869 7374 7328 6e61 6d65 3d6e 616d  _exists(name=nam
+00029250: 6529 290a 0a20 2020 2061 7379 6e63 2064  e))..    async d
+00029260: 6566 2070 7573 685f 6669 6c65 7328 0a20  ef push_files(. 
+00029270: 2020 2020 2020 2064 6570 656e 6465 6e63         dependenc
+00029280: 795f 6772 6170 683a 2047 7261 7068 4465  y_graph: GraphDe
+00029290: 7065 6e64 656e 6369 6573 2c0a 2020 2020  pendencies,.    
+000292a0: 2020 2020 6472 795f 7275 6e3a 2062 6f6f      dry_run: boo
+000292b0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+000292c0: 2020 2063 6865 636b 5f62 6163 6b66 696c     check_backfil
+000292d0: 6c5f 7265 7175 6972 6564 3a20 626f 6f6c  l_required: bool
+000292e0: 203d 2046 616c 7365 2c0a 2020 2020 293a   = False,.    ):
+000292f0: 0a20 2020 2020 2020 2065 6e64 706f 696e  .        endpoin
+00029300: 7473 5f64 6570 5f6d 6170 203d 2064 6963  ts_dep_map = dic
+00029310: 7428 290a 2020 2020 2020 2020 7072 6f63  t().        proc
+00029320: 6573 7365 6420 3d20 7365 7428 290a 0a20  essed = set().. 
+00029330: 2020 2020 2020 2064 6570 656e 6465 6e63         dependenc
+00029340: 6965 735f 6772 6170 6820 3d20 6465 7065  ies_graph = depe
+00029350: 6e64 656e 6379 5f67 7261 7068 2e64 6570  ndency_graph.dep
+00029360: 5f6d 6170 0a20 2020 2020 2020 2072 6573  _map.        res
+00029370: 6f75 7263 6573 5f74 6f5f 7275 6e20 3d20  ources_to_run = 
+00029380: 6465 7065 6e64 656e 6379 5f67 7261 7068  dependency_graph
+00029390: 2e74 6f5f 7275 6e0a 0a20 2020 2020 2020  .to_run..       
+000293a0: 2069 6620 6e6f 7420 666f 726b 5f64 6f77   if not fork_dow
+000293b0: 6e73 7472 6561 6d3a 0a20 2020 2020 2020  nstream:.       
+000293c0: 2020 2020 2023 2046 6972 7374 2c20 7765       # First, we
+000293d0: 2077 696c 6c20 6465 706c 6f79 2074 6865   will deploy the
+000293e0: 2061 6c6c 2074 6865 2072 6573 6f75 7263   all the resourc
+000293f0: 6573 2066 6f6c 6c6f 7769 6e67 2074 6865  es following the
+00029400: 2064 6570 656e 6465 6e63 7920 6772 6170   dependency grap
+00029410: 6820 6578 6365 7074 2066 6f72 2074 6865  h except for the
+00029420: 2065 6e64 706f 696e 7473 0a20 2020 2020   endpoints.     
+00029430: 2020 2020 2020 2067 726f 7570 7320 3d20         groups = 
+00029440: 5b67 726f 7570 2066 6f72 2067 726f 7570  [group for group
+00029450: 2069 6e20 746f 706f 736f 7274 2864 6570   in toposort(dep
+00029460: 656e 6465 6e63 6965 735f 6772 6170 6829  endencies_graph)
+00029470: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00029480: 7220 6772 6f75 7020 696e 2067 726f 7570  r group in group
+00029490: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000294a0: 2020 2066 6f72 206e 616d 6520 696e 2067     for name in g
+000294b0: 726f 7570 3a0a 2020 2020 2020 2020 2020  roup:.          
+000294c0: 2020 2020 2020 2020 2020 6966 206e 616d            if nam
+000294d0: 6520 696e 2070 726f 6365 7373 6564 3a0a  e in processed:.
 000294e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000294f0: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-00029500: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00029510: 2069 735f 656e 6470 6f69 6e74 5f77 6974   is_endpoint_wit
-00029520: 685f 6e6f 5f64 6570 656e 6465 6e63 6965  h_no_dependencie
-00029530: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00029540: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-00029550: 7263 6573 5f74 6f5f 7275 6e2e 6765 7428  rces_to_run.get(
-00029560: 6e61 6d65 2c20 7b7d 292c 0a20 2020 2020  name, {}),.     
-00029570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029580: 2020 2064 6570 656e 6465 6e63 6965 735f     dependencies_
-00029590: 6772 6170 682c 0a20 2020 2020 2020 2020  graph,.         
-000295a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000295b0: 6573 6f75 7263 6573 5f74 6f5f 7275 6e2c  esources_to_run,
-000295c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000295d0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+000294f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00029500: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00029510: 2020 2020 2020 6966 2069 735f 656e 6470        if is_endp
+00029520: 6f69 6e74 5f77 6974 685f 6e6f 5f64 6570  oint_with_no_dep
+00029530: 656e 6465 6e63 6965 7328 0a20 2020 2020  endencies(.     
+00029540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029550: 2020 2072 6573 6f75 7263 6573 5f74 6f5f     resources_to_
+00029560: 7275 6e2e 6765 7428 6e61 6d65 2c20 7b7d  run.get(name, {}
+00029570: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00029580: 2020 2020 2020 2020 2020 2064 6570 656e             depen
+00029590: 6465 6e63 6965 735f 6772 6170 682c 0a20  dencies_graph,. 
+000295a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000295b0: 2020 2020 2020 2072 6573 6f75 7263 6573         resources
+000295c0: 5f74 6f5f 7275 6e2c 0a20 2020 2020 2020  _to_run,.       
+000295d0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 000295e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000295f0: 656e 6470 6f69 6e74 735f 6465 705f 6d61  endpoints_dep_ma
-00029600: 705b 6e61 6d65 5d20 3d20 6465 7065 6e64  p[name] = depend
-00029610: 656e 6369 6573 5f67 7261 7068 5b6e 616d  encies_graph[nam
-00029620: 655d 0a20 2020 2020 2020 2020 2020 2020  e].             
-00029630: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00029640: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-00029650: 2020 2020 2020 2020 2061 7761 6974 2070           await p
-00029660: 7573 6828 0a20 2020 2020 2020 2020 2020  ush(.           
-00029670: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00029680: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00029690: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-000296a0: 7263 6573 5f74 6f5f 7275 6e2c 0a20 2020  rces_to_run,.   
-000296b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000296c0: 2020 2020 2072 6573 6f75 7263 655f 7665       resource_ve
-000296d0: 7273 696f 6e73 2c0a 2020 2020 2020 2020  rsions,.        
+000295f0: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+00029600: 735f 6465 705f 6d61 705b 6e61 6d65 5d20  s_dep_map[name] 
+00029610: 3d20 6465 7065 6e64 656e 6369 6573 5f67  = dependencies_g
+00029620: 7261 7068 5b6e 616d 655d 0a20 2020 2020  raph[name].     
+00029630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029640: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+00029650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029660: 2061 7761 6974 2070 7573 6828 0a20 2020   await push(.   
+00029670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029680: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
+00029690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000296a0: 2020 2072 6573 6f75 7263 6573 5f74 6f5f     resources_to_
+000296b0: 7275 6e2c 0a20 2020 2020 2020 2020 2020  run,.           
+000296c0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+000296d0: 6f75 7263 655f 7665 7273 696f 6e73 2c0a  ource_versions,.
 000296e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000296f0: 6c61 7465 7374 5f64 6174 6173 6f75 7263  latest_datasourc
-00029700: 655f 7665 7273 696f 6e73 2c0a 2020 2020  e_versions,.    
-00029710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029720: 2020 2020 6472 795f 7275 6e2c 0a20 2020      dry_run,.   
-00029730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029740: 2020 2020 2066 6f72 6b5f 646f 776e 7374       fork_downst
-00029750: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
-00029760: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00029770: 726b 2c0a 2020 2020 2020 2020 2020 2020  rk,.            
-00029780: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00029790: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000297a0: 6f63 6573 7365 642e 6164 6428 6e61 6d65  ocessed.add(name
-000297b0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-000297c0: 2054 6865 6e2c 2077 6520 7769 6c6c 2064   Then, we will d
-000297d0: 6570 6c6f 7920 7468 6520 656e 6470 6f69  eploy the endpoi
-000297e0: 6e74 7320 7468 6174 2061 7265 206f 6e20  nts that are on 
-000297f0: 7468 6520 6465 7065 6e64 656e 6379 2067  the dependency g
-00029800: 7261 7068 0a20 2020 2020 2020 2020 2020  raph.           
-00029810: 2067 726f 7570 7320 3d20 5b67 726f 7570   groups = [group
-00029820: 2066 6f72 2067 726f 7570 2069 6e20 746f   for group in to
-00029830: 706f 736f 7274 2865 6e64 706f 696e 7473  posort(endpoints
-00029840: 5f64 6570 5f6d 6170 295d 0a20 2020 2020  _dep_map)].     
-00029850: 2020 2020 2020 2066 6f72 2067 726f 7570         for group
-00029860: 2069 6e20 6772 6f75 7073 3a0a 2020 2020   in groups:.    
-00029870: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00029880: 6e61 6d65 2069 6e20 6772 6f75 703a 0a20  name in group:. 
-00029890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000298a0: 2020 2069 6620 6e61 6d65 206e 6f74 2069     if name not i
-000298b0: 6e20 7072 6f63 6573 7365 643a 0a20 2020  n processed:.   
-000298c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000298d0: 2020 2020 2061 7761 6974 2070 7573 6828       await push(
-000298e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000298f0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00029900: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00029910: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00029920: 6573 6f75 7263 6573 5f74 6f5f 7275 6e2c  esources_to_run,
-00029930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029940: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00029950: 6f75 7263 655f 7665 7273 696f 6e73 2c0a  ource_versions,.
-00029960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029970: 2020 2020 2020 2020 2020 2020 6c61 7465              late
-00029980: 7374 5f64 6174 6173 6f75 7263 655f 7665  st_datasource_ve
-00029990: 7273 696f 6e73 2c0a 2020 2020 2020 2020  rsions,.        
+000296f0: 2020 2020 2020 2020 6c61 7465 7374 5f64          latest_d
+00029700: 6174 6173 6f75 7263 655f 7665 7273 696f  atasource_versio
+00029710: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00029720: 2020 2020 2020 2020 2020 2020 6472 795f              dry_
+00029730: 7275 6e2c 0a20 2020 2020 2020 2020 2020  run,.           
+00029740: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00029750: 6b5f 646f 776e 7374 7265 616d 2c0a 2020  k_downstream,.  
+00029760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029770: 2020 2020 2020 666f 726b 2c0a 2020 2020        fork,.    
+00029780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029790: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000297a0: 2020 2020 2020 7072 6f63 6573 7365 642e        processed.
+000297b0: 6164 6428 6e61 6d65 290a 0a20 2020 2020  add(name)..     
+000297c0: 2020 2020 2020 2023 2054 6865 6e2c 2077         # Then, w
+000297d0: 6520 7769 6c6c 2064 6570 6c6f 7920 7468  e will deploy th
+000297e0: 6520 656e 6470 6f69 6e74 7320 7468 6174  e endpoints that
+000297f0: 2061 7265 206f 6e20 7468 6520 6465 7065   are on the depe
+00029800: 6e64 656e 6379 2067 7261 7068 0a20 2020  ndency graph.   
+00029810: 2020 2020 2020 2020 2067 726f 7570 7320           groups 
+00029820: 3d20 5b67 726f 7570 2066 6f72 2067 726f  = [group for gro
+00029830: 7570 2069 6e20 746f 706f 736f 7274 2865  up in toposort(e
+00029840: 6e64 706f 696e 7473 5f64 6570 5f6d 6170  ndpoints_dep_map
+00029850: 295d 0a20 2020 2020 2020 2020 2020 2066  )].            f
+00029860: 6f72 2067 726f 7570 2069 6e20 6772 6f75  or group in grou
+00029870: 7073 3a0a 2020 2020 2020 2020 2020 2020  ps:.            
+00029880: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
+00029890: 6772 6f75 703a 0a20 2020 2020 2020 2020  group:.         
+000298a0: 2020 2020 2020 2020 2020 2069 6620 6e61             if na
+000298b0: 6d65 206e 6f74 2069 6e20 7072 6f63 6573  me not in proces
+000298c0: 7365 643a 0a20 2020 2020 2020 2020 2020  sed:.           
+000298d0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+000298e0: 6974 2070 7573 6828 0a20 2020 2020 2020  it push(.       
+000298f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029900: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
+00029910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029920: 2020 2020 2020 2072 6573 6f75 7263 6573         resources
+00029930: 5f74 6f5f 7275 6e2c 0a20 2020 2020 2020  _to_run,.       
+00029940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029950: 2020 2020 2072 6573 6f75 7263 655f 7665       resource_ve
+00029960: 7273 696f 6e73 2c0a 2020 2020 2020 2020  rsions,.        
+00029970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029980: 2020 2020 6c61 7465 7374 5f64 6174 6173      latest_datas
+00029990: 6f75 7263 655f 7665 7273 696f 6e73 2c0a  ource_versions,.
 000299a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299b0: 2020 2020 6472 795f 7275 6e2c 0a20 2020      dry_run,.   
-000299c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299d0: 2020 2020 2020 2020 2066 6f72 6b5f 646f           fork_do
-000299e0: 776e 7374 7265 616d 2c0a 2020 2020 2020  wnstream,.      
-000299f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a00: 2020 2020 2020 666f 726b 2c0a 2020 2020        fork,.    
-00029a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00029a30: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00029a40: 6f63 6573 7365 642e 6164 6428 6e61 6d65  ocessed.add(name
-00029a50: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00029a60: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00029a70: 6973 2077 696c 6c20 6765 6e65 7261 7465  is will generate
-00029a80: 2074 6865 2067 7261 7068 2066 726f 6d20   the graph from 
-00029a90: 7269 6768 7420 746f 206c 6566 7420 616e  right to left an
-00029aa0: 6420 7769 6c6c 2066 696c 6c20 7468 6520  d will fill the 
-00029ab0: 6761 7073 206f 6620 7468 6520 6465 7065  gaps of the depe
-00029ac0: 6e64 656e 6369 6573 0a20 2020 2020 2020  ndencies.       
-00029ad0: 2020 2020 2023 2049 6620 7765 2068 6176       # If we hav
-00029ae0: 6520 6120 6772 6170 6820 6c69 6b65 2074  e a graph like t
-00029af0: 6869 733a 0a20 2020 2020 2020 2020 2020  his:.           
-00029b00: 2023 2041 202d 3e20 4220 2d3e 2043 0a20   # A -> B -> C. 
-00029b10: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
-00029b20: 7765 206f 6e6c 7920 6d6f 6469 6679 2041  we only modify A
-00029b30: 2c20 7468 6520 6e6f 726d 616c 2064 6570  , the normal dep
-00029b40: 656e 6465 6e63 6965 7320 6772 6170 6820  endencies graph 
-00029b50: 7769 6c6c 206f 6e6c 7920 636f 6e74 6169  will only contai
-00029b60: 6e20 6120 6e6f 6465 206c 696b 6520 5f7b  n a node like _{
-00029b70: 4120 3d3e 2042 7d0a 2020 2020 2020 2020  A => B}.        
-00029b80: 2020 2020 2320 4275 7420 7765 206e 6565      # But we nee
-00029b90: 6420 6120 6772 6170 6820 7468 6174 2063  d a graph that c
-00029ba0: 6f6e 7461 696e 7320 412c 2042 2061 6e64  ontains A, B and
-00029bb0: 2043 2061 6e64 2074 6865 2064 6570 656e   C and the depen
-00029bc0: 6465 6e63 6965 7320 6265 7477 6565 6e20  dencies between 
-00029bd0: 7468 656d 2074 6f20 6465 706c 6f79 2074  them to deploy t
-00029be0: 6865 6d20 696e 2074 6865 2072 6967 6874  hem in the right
-00029bf0: 206f 7264 6572 0a20 2020 2020 2020 2020   order.         
-00029c00: 2020 2064 6570 656e 6465 6e63 6965 735f     dependencies_
-00029c10: 6772 6170 685f 666f 726b 5f64 6f77 6e73  graph_fork_downs
-00029c20: 7472 6561 6d2c 2072 6573 6f75 7263 6573  tream, resources
-00029c30: 5f74 6f5f 7275 6e5f 666f 726b 5f64 6f77  _to_run_fork_dow
-00029c40: 6e73 7472 6561 6d20 3d20 6765 6e65 7261  nstream = genera
-00029c50: 7465 5f66 6f72 6b64 6f77 6e73 7472 6561  te_forkdownstrea
-00029c60: 6d5f 6772 6170 6828 0a20 2020 2020 2020  m_graph(.       
-00029c70: 2020 2020 2020 2020 2064 6570 656e 6465           depende
-00029c80: 6e63 795f 6772 6170 682e 616c 6c5f 6465  ncy_graph.all_de
-00029c90: 705f 6d61 702c 0a20 2020 2020 2020 2020  p_map,.         
-00029ca0: 2020 2020 2020 2064 6570 656e 6465 6e63         dependenc
-00029cb0: 795f 6772 6170 682e 616c 6c5f 7265 736f  y_graph.all_reso
-00029cc0: 7572 6365 732c 0a20 2020 2020 2020 2020  urces,.         
-00029cd0: 2020 2020 2020 2072 6573 6f75 7263 6573         resources
-00029ce0: 5f74 6f5f 7275 6e2c 0a20 2020 2020 2020  _to_run,.       
-00029cf0: 2020 2020 2020 2020 206c 6973 7428 6465           list(de
-00029d00: 7065 6e64 656e 6379 5f67 7261 7068 2e64  pendency_graph.d
-00029d10: 6570 5f6d 6170 2e6b 6579 7328 2929 2c0a  ep_map.keys()),.
-00029d20: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00029d30: 2020 2020 2020 2020 2020 2023 2046 6972             # Fir
-00029d40: 7374 2c20 7765 2077 696c 6c20 6465 706c  st, we will depl
-00029d50: 6f79 2074 6865 2064 6174 6173 6f75 7263  oy the datasourc
-00029d60: 6573 2074 6861 7420 6e65 6564 2074 6f20  es that need to 
-00029d70: 6265 2064 6570 6c6f 7965 642e 0a20 2020  be deployed..   
-00029d80: 2020 2020 2020 2020 2023 2057 6520 6e65           # We ne
-00029d90: 6564 2074 6f20 6465 706c 6f79 2074 6865  ed to deploy the
-00029da0: 2064 6174 6173 6f75 7263 6573 2066 726f   datasources fro
-00029db0: 6d20 6c65 6674 2074 6f20 7269 6768 7420  m left to right 
-00029dc0: 6173 2073 6f6d 6520 6461 7461 736f 7572  as some datasour
-00029dd0: 6365 7320 6d69 6768 7420 6861 7665 204d  ces might have M
-00029de0: 5620 7468 6174 2064 6570 656e 6420 6f6e  V that depend on
-00029df0: 2074 6865 2063 6f6c 756d 6e20 7479 7065   the column type
-00029e00: 7320 6f66 2070 7265 7669 6f75 7320 6461  s of previous da
-00029e10: 7461 736f 7572 6365 732e 2045 783a 2060  tasources. Ex: `
-00029e20: 7465 7374 5f63 6861 6e67 655f 636f 6c75  test_change_colu
-00029e30: 6d6e 5f74 7970 655f 6c61 6e64 696e 675f  mn_type_landing_
-00029e40: 6461 7461 736f 7572 6365 6020 7465 7374  datasource` test
-00029e50: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
-00029e60: 7570 7320 3d20 5b67 726f 7570 2066 6f72  ups = [group for
-00029e70: 2067 726f 7570 2069 6e20 746f 706f 736f   group in toposo
-00029e80: 7274 2864 6570 656e 6465 6e63 6965 735f  rt(dependencies_
-00029e90: 6772 6170 685f 666f 726b 5f64 6f77 6e73  graph_fork_downs
-00029ea0: 7472 6561 6d29 5d0a 2020 2020 2020 2020  tream)].        
-00029eb0: 2020 2020 6772 6f75 7073 2e72 6576 6572      groups.rever
-00029ec0: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-00029ed0: 2066 6f72 2067 726f 7570 2069 6e20 6772   for group in gr
-00029ee0: 6f75 7073 3a0a 2020 2020 2020 2020 2020  oups:.          
-00029ef0: 2020 2020 2020 666f 7220 6e61 6d65 2069        for name i
-00029f00: 6e20 6772 6f75 703a 0a20 2020 2020 2020  n group:.       
-00029f10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00029f20: 6e61 6d65 2069 6e20 7072 6f63 6573 7365  name in processe
-00029f30: 6420 6f72 206e 6f74 2069 735f 6461 7461  d or not is_data
-00029f40: 736f 7572 6365 2872 6573 6f75 7263 6573  source(resources
-00029f50: 5f74 6f5f 7275 6e5f 666f 726b 5f64 6f77  _to_run_fork_dow
-00029f60: 6e73 7472 6561 6d5b 6e61 6d65 5d29 3a0a  nstream[name]):.
-00029f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029f80: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00029f90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00029fa0: 2020 2020 2020 2320 4966 2074 6865 2072        # If the r
-00029fb0: 6573 6f75 7263 6520 6973 206e 6577 2c20  esource is new, 
-00029fc0: 7765 2077 696c 6c20 7573 6520 7468 6520  we will use the 
-00029fd0: 6e6f 726d 616c 2072 6573 6f75 7263 6520  normal resource 
-00029fe0: 696e 666f 726d 6174 696f 6e20 746f 2064  information to d
-00029ff0: 6570 6c6f 7920 6974 0a20 2020 2020 2020  eploy it.       
-0002a000: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-0002a010: 6869 7320 6973 206d 6f73 746c 7920 7573  his is mostly us
-0002a020: 6564 2066 6f72 2064 6174 6173 6f75 7263  ed for datasourc
-0002a030: 6573 2077 6974 6820 636f 6e6e 6563 7469  es with connecti
-0002a040: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
-0002a050: 2020 2020 2020 2020 2023 2041 7420 7468           # At th
-0002a060: 6520 6d6f 6d65 6e74 2c20 6072 6573 6f75  e moment, `resou
-0002a070: 7263 6573 5f74 6f5f 7275 6e5f 666f 726b  rces_to_run_fork
-0002a080: 5f64 6f77 6e73 7472 6561 6d60 2069 7320  _downstream` is 
-0002a090: 6765 6e65 7261 7465 6420 6279 2060 616c  generated by `al
-0002a0a0: 6c5f 7265 736f 7572 6365 7360 2061 6e64  l_resources` and
-0002a0b0: 2074 6869 7320 6973 2067 656e 6572 6174   this is generat
-0002a0c0: 6564 2075 7369 6e67 2074 6865 2070 6172  ed using the par
-0002a0d0: 616d 6574 6572 2060 736b 6970 5f63 6f6e  ameter `skip_con
-0002a0e0: 6e65 6374 6f72 733d 5472 7565 600a 2020  nectors=True`.  
-0002a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a100: 2020 2320 544f 444f 3a20 5368 6f75 6c64    # TODO: Should
-0002a110: 2074 6865 2060 7265 736f 7572 6365 735f   the `resources_
-0002a120: 746f 5f72 756e 5f66 6f72 6b5f 646f 776e  to_run_fork_down
-0002a130: 7374 7265 616d 6020 6265 2067 656e 6572  stream` be gener
-0002a140: 6174 6564 2075 7369 6e67 2074 6865 2060  ated using the `
-0002a150: 736b 6970 5f63 6f6e 6e65 6374 6f72 7360  skip_connectors`
-0002a160: 2070 6172 616d 6574 6572 3f0a 2020 2020   parameter?.    
-0002a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a180: 6966 2069 735f 6e65 7728 6e61 6d65 2c20  if is_new(name, 
-0002a190: 6368 616e 6765 642c 2064 6570 656e 6465  changed, depende
-0002a1a0: 6e63 6965 735f 6772 6170 685f 666f 726b  ncies_graph_fork
-0002a1b0: 5f64 6f77 6e73 7472 6561 6d2c 2064 6570  _downstream, dep
-0002a1c0: 656e 6465 6e63 6965 735f 6772 6170 685f  endencies_graph_
-0002a1d0: 666f 726b 5f64 6f77 6e73 7472 6561 6d29  fork_downstream)
-0002a1e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002a1f0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0002a200: 7075 7368 280a 2020 2020 2020 2020 2020  push(.          
+000299b0: 2020 2020 2020 2020 2020 2020 6472 795f              dry_
+000299c0: 7275 6e2c 0a20 2020 2020 2020 2020 2020  run,.           
+000299d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000299e0: 2066 6f72 6b5f 646f 776e 7374 7265 616d   fork_downstream
+000299f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029a00: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00029a10: 726b 2c0a 2020 2020 2020 2020 2020 2020  rk,.            
+00029a20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00029a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029a40: 2020 2020 2020 7072 6f63 6573 7365 642e        processed.
+00029a50: 6164 6428 6e61 6d65 290a 2020 2020 2020  add(name).      
+00029a60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00029a70: 2020 2020 2320 5468 6973 2077 696c 6c20      # This will 
+00029a80: 6765 6e65 7261 7465 2074 6865 2067 7261  generate the gra
+00029a90: 7068 2066 726f 6d20 7269 6768 7420 746f  ph from right to
+00029aa0: 206c 6566 7420 616e 6420 7769 6c6c 2066   left and will f
+00029ab0: 696c 6c20 7468 6520 6761 7073 206f 6620  ill the gaps of 
+00029ac0: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00029ad0: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+00029ae0: 6620 7765 2068 6176 6520 6120 6772 6170  f we have a grap
+00029af0: 6820 6c69 6b65 2074 6869 733a 0a20 2020  h like this:.   
+00029b00: 2020 2020 2020 2020 2023 2041 202d 3e20           # A -> 
+00029b10: 4220 2d3e 2043 0a20 2020 2020 2020 2020  B -> C.         
+00029b20: 2020 2023 2049 6620 7765 206f 6e6c 7920     # If we only 
+00029b30: 6d6f 6469 6679 2041 2c20 7468 6520 6e6f  modify A, the no
+00029b40: 726d 616c 2064 6570 656e 6465 6e63 6965  rmal dependencie
+00029b50: 7320 6772 6170 6820 7769 6c6c 206f 6e6c  s graph will onl
+00029b60: 7920 636f 6e74 6169 6e20 6120 6e6f 6465  y contain a node
+00029b70: 206c 696b 6520 5f7b 4120 3d3e 2042 7d0a   like _{A => B}.
+00029b80: 2020 2020 2020 2020 2020 2020 2320 4275              # Bu
+00029b90: 7420 7765 206e 6565 6420 6120 6772 6170  t we need a grap
+00029ba0: 6820 7468 6174 2063 6f6e 7461 696e 7320  h that contains 
+00029bb0: 412c 2042 2061 6e64 2043 2061 6e64 2074  A, B and C and t
+00029bc0: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
+00029bd0: 6265 7477 6565 6e20 7468 656d 2074 6f20  between them to 
+00029be0: 6465 706c 6f79 2074 6865 6d20 696e 2074  deploy them in t
+00029bf0: 6865 2072 6967 6874 206f 7264 6572 0a20  he right order. 
+00029c00: 2020 2020 2020 2020 2020 2064 6570 656e             depen
+00029c10: 6465 6e63 6965 735f 6772 6170 685f 666f  dencies_graph_fo
+00029c20: 726b 5f64 6f77 6e73 7472 6561 6d2c 2072  rk_downstream, r
+00029c30: 6573 6f75 7263 6573 5f74 6f5f 7275 6e5f  esources_to_run_
+00029c40: 666f 726b 5f64 6f77 6e73 7472 6561 6d20  fork_downstream 
+00029c50: 3d20 6765 6e65 7261 7465 5f66 6f72 6b64  = generate_forkd
+00029c60: 6f77 6e73 7472 6561 6d5f 6772 6170 6828  ownstream_graph(
+00029c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029c80: 2064 6570 656e 6465 6e63 795f 6772 6170   dependency_grap
+00029c90: 682e 616c 6c5f 6465 705f 6d61 702c 0a20  h.all_dep_map,. 
+00029ca0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00029cb0: 6570 656e 6465 6e63 795f 6772 6170 682e  ependency_graph.
+00029cc0: 616c 6c5f 7265 736f 7572 6365 732c 0a20  all_resources,. 
+00029cd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00029ce0: 6573 6f75 7263 6573 5f74 6f5f 7275 6e2c  esources_to_run,
+00029cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029d00: 206c 6973 7428 6465 7065 6e64 656e 6379   list(dependency
+00029d10: 5f67 7261 7068 2e64 6570 5f6d 6170 2e6b  _graph.dep_map.k
+00029d20: 6579 7328 2929 2c0a 2020 2020 2020 2020  eys()),.        
+00029d30: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00029d40: 2020 2023 2046 6972 7374 2c20 7765 2077     # First, we w
+00029d50: 696c 6c20 6465 706c 6f79 2074 6865 2064  ill deploy the d
+00029d60: 6174 6173 6f75 7263 6573 2074 6861 7420  atasources that 
+00029d70: 6e65 6564 2074 6f20 6265 2064 6570 6c6f  need to be deplo
+00029d80: 7965 642e 0a20 2020 2020 2020 2020 2020  yed..           
+00029d90: 2023 2057 6520 6e65 6564 2074 6f20 6465   # We need to de
+00029da0: 706c 6f79 2074 6865 2064 6174 6173 6f75  ploy the datasou
+00029db0: 7263 6573 2066 726f 6d20 6c65 6674 2074  rces from left t
+00029dc0: 6f20 7269 6768 7420 6173 2073 6f6d 6520  o right as some 
+00029dd0: 6461 7461 736f 7572 6365 7320 6d69 6768  datasources migh
+00029de0: 7420 6861 7665 204d 5620 7468 6174 2064  t have MV that d
+00029df0: 6570 656e 6420 6f6e 2074 6865 2063 6f6c  epend on the col
+00029e00: 756d 6e20 7479 7065 7320 6f66 2070 7265  umn types of pre
+00029e10: 7669 6f75 7320 6461 7461 736f 7572 6365  vious datasource
+00029e20: 732e 2045 783a 2060 7465 7374 5f63 6861  s. Ex: `test_cha
+00029e30: 6e67 655f 636f 6c75 6d6e 5f74 7970 655f  nge_column_type_
+00029e40: 6c61 6e64 696e 675f 6461 7461 736f 7572  landing_datasour
+00029e50: 6365 6020 7465 7374 0a20 2020 2020 2020  ce` test.       
+00029e60: 2020 2020 2067 726f 7570 7320 3d20 5b67       groups = [g
+00029e70: 726f 7570 2066 6f72 2067 726f 7570 2069  roup for group i
+00029e80: 6e20 746f 706f 736f 7274 2864 6570 656e  n toposort(depen
+00029e90: 6465 6e63 6965 735f 6772 6170 685f 666f  dencies_graph_fo
+00029ea0: 726b 5f64 6f77 6e73 7472 6561 6d29 5d0a  rk_downstream)].
+00029eb0: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00029ec0: 7073 2e72 6576 6572 7365 2829 0a20 2020  ps.reverse().   
+00029ed0: 2020 2020 2020 2020 2066 6f72 2067 726f           for gro
+00029ee0: 7570 2069 6e20 6772 6f75 7073 3a0a 2020  up in groups:.  
+00029ef0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00029f00: 7220 6e61 6d65 2069 6e20 6772 6f75 703a  r name in group:
+00029f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029f20: 2020 2020 2069 6620 6e61 6d65 2069 6e20       if name in 
+00029f30: 7072 6f63 6573 7365 6420 6f72 206e 6f74  processed or not
+00029f40: 2069 735f 6461 7461 736f 7572 6365 2872   is_datasource(r
+00029f50: 6573 6f75 7263 6573 5f74 6f5f 7275 6e5f  esources_to_run_
+00029f60: 666f 726b 5f64 6f77 6e73 7472 6561 6d5b  fork_downstream[
+00029f70: 6e61 6d65 5d29 3a0a 2020 2020 2020 2020  name]):.        
+00029f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029f90: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
+00029fa0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00029fb0: 4966 2074 6865 2072 6573 6f75 7263 6520  If the resource 
+00029fc0: 6973 206e 6577 2c20 7765 2077 696c 6c20  is new, we will 
+00029fd0: 7573 6520 7468 6520 6e6f 726d 616c 2072  use the normal r
+00029fe0: 6573 6f75 7263 6520 696e 666f 726d 6174  esource informat
+00029ff0: 696f 6e20 746f 2064 6570 6c6f 7920 6974  ion to deploy it
+0002a000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a010: 2020 2020 2023 2054 6869 7320 6973 206d       # This is m
+0002a020: 6f73 746c 7920 7573 6564 2066 6f72 2064  ostly used for d
+0002a030: 6174 6173 6f75 7263 6573 2077 6974 6820  atasources with 
+0002a040: 636f 6e6e 6563 7469 6f6e 732e 0a20 2020  connections..   
+0002a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a060: 2023 2041 7420 7468 6520 6d6f 6d65 6e74   # At the moment
+0002a070: 2c20 6072 6573 6f75 7263 6573 5f74 6f5f  , `resources_to_
+0002a080: 7275 6e5f 666f 726b 5f64 6f77 6e73 7472  run_fork_downstr
+0002a090: 6561 6d60 2069 7320 6765 6e65 7261 7465  eam` is generate
+0002a0a0: 6420 6279 2060 616c 6c5f 7265 736f 7572  d by `all_resour
+0002a0b0: 6365 7360 2061 6e64 2074 6869 7320 6973  ces` and this is
+0002a0c0: 2067 656e 6572 6174 6564 2075 7369 6e67   generated using
+0002a0d0: 2074 6865 2070 6172 616d 6574 6572 2060   the parameter `
+0002a0e0: 736b 6970 5f63 6f6e 6e65 6374 6f72 733d  skip_connectors=
+0002a0f0: 5472 7565 600a 2020 2020 2020 2020 2020  True`.          
+0002a100: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
+0002a110: 3a20 5368 6f75 6c64 2074 6865 2060 7265  : Should the `re
+0002a120: 736f 7572 6365 735f 746f 5f72 756e 5f66  sources_to_run_f
+0002a130: 6f72 6b5f 646f 776e 7374 7265 616d 6020  ork_downstream` 
+0002a140: 6265 2067 656e 6572 6174 6564 2075 7369  be generated usi
+0002a150: 6e67 2074 6865 2060 736b 6970 5f63 6f6e  ng the `skip_con
+0002a160: 6e65 6374 6f72 7360 2070 6172 616d 6574  nectors` paramet
+0002a170: 6572 3f0a 2020 2020 2020 2020 2020 2020  er?.            
+0002a180: 2020 2020 2020 2020 6966 2069 735f 6e65          if is_ne
+0002a190: 7728 6e61 6d65 2c20 6368 616e 6765 642c  w(name, changed,
+0002a1a0: 2064 6570 656e 6465 6e63 6965 735f 6772   dependencies_gr
+0002a1b0: 6170 685f 666f 726b 5f64 6f77 6e73 7472  aph_fork_downstr
+0002a1c0: 6561 6d2c 2064 6570 656e 6465 6e63 6965  eam, dependencie
+0002a1d0: 735f 6772 6170 685f 666f 726b 5f64 6f77  s_graph_fork_dow
+0002a1e0: 6e73 7472 6561 6d29 3a0a 2020 2020 2020  nstream):.      
+0002a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a200: 2020 6177 6169 7420 7075 7368 280a 2020    await push(.  
 0002a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a220: 2020 6e61 6d65 2c0a 2020 2020 2020 2020    name,.        
+0002a220: 2020 2020 2020 2020 2020 6e61 6d65 2c0a            name,.
 0002a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a240: 2020 2020 7265 736f 7572 6365 735f 746f      resources_to
-0002a250: 5f72 756e 2c0a 2020 2020 2020 2020 2020  _run,.          
+0002a240: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0002a250: 7572 6365 735f 746f 5f72 756e 2c0a 2020  urces_to_run,.  
 0002a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a270: 2020 7265 736f 7572 6365 5f76 6572 7369    resource_versi
-0002a280: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+0002a270: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0002a280: 6365 5f76 6572 7369 6f6e 732c 0a20 2020  ce_versions,.   
 0002a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a2a0: 206c 6174 6573 745f 6461 7461 736f 7572   latest_datasour
-0002a2b0: 6365 5f76 6572 7369 6f6e 732c 0a20 2020  ce_versions,.   
-0002a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a2d0: 2020 2020 2020 2020 2064 7279 5f72 756e           dry_run
-0002a2e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002a2f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002a300: 726b 5f64 6f77 6e73 7472 6561 6d2c 0a20  rk_downstream,. 
-0002a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a320: 2020 2020 2020 2020 2020 2066 6f72 6b2c             fork,
-0002a330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a340: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0002a350: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0002a360: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0002a370: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-0002a380: 6620 7765 2061 7265 2074 7279 696e 6720  f we are trying 
-0002a390: 746f 206d 6f64 6966 7920 6120 4b61 666b  to modify a Kafk
-0002a3a0: 6120 6f72 2043 444b 2064 6174 6173 6f75  a or CDK datasou
-0002a3b0: 7263 652c 2077 6520 6e65 6564 2074 6f20  rce, we need to 
-0002a3c0: 696e 666f 726d 2074 6865 2075 7365 7220  inform the user 
-0002a3d0: 7468 6174 2074 6865 2072 6573 6f75 7263  that the resourc
-0002a3e0: 6520 6e65 6564 7320 746f 2062 6520 706f  e needs to be po
-0002a3f0: 7374 2d72 656c 6561 7365 640a 2020 2020  st-released.    
-0002a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a410: 2020 2020 6b61 666b 615f 636f 6e6e 6563      kafka_connec
-0002a420: 7469 6f6e 5f6e 616d 6520 3d20 280a 2020  tion_name = (.  
-0002a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a440: 2020 2020 2020 2020 2020 7265 736f 7572            resour
-0002a450: 6365 735f 746f 5f72 756e 5f66 6f72 6b5f  ces_to_run_fork_
-0002a460: 646f 776e 7374 7265 616d 5b6e 616d 655d  downstream[name]
-0002a470: 2e67 6574 2822 7061 7261 6d73 222c 207b  .get("params", {
-0002a480: 7d29 2e67 6574 2822 6b61 666b 615f 636f  }).get("kafka_co
-0002a490: 6e6e 6563 7469 6f6e 5f6e 616d 6522 290a  nnection_name").
-0002a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a4b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0002a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a4d0: 2020 7365 7276 6963 6520 3d20 7265 736f    service = reso
-0002a4e0: 7572 6365 735f 746f 5f72 756e 5f66 6f72  urces_to_run_for
-0002a4f0: 6b5f 646f 776e 7374 7265 616d 5b6e 616d  k_downstream[nam
-0002a500: 655d 2e67 6574 2822 7061 7261 6d73 222c  e].get("params",
-0002a510: 207b 7d29 2e67 6574 2822 696d 706f 7274   {}).get("import
-0002a520: 5f73 6572 7669 6365 2229 0a20 2020 2020  _service").     
-0002a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a540: 2020 2069 6620 7265 6c65 6173 655f 6372     if release_cr
-0002a550: 6561 7465 6420 616e 6420 286b 6166 6b61  eated and (kafka
-0002a560: 5f63 6f6e 6e65 6374 696f 6e5f 6e61 6d65  _connection_name
-0002a570: 206f 7220 7365 7276 6963 6529 3a0a 2020   or service):.  
-0002a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a590: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
-0002a5a0: 746f 7220 3d20 224b 6166 6b61 2220 6966  tor = "Kafka" if
-0002a5b0: 206b 6166 6b61 5f63 6f6e 6e65 6374 696f   kafka_connectio
-0002a5c0: 6e5f 6e61 6d65 2065 6c73 6520 7365 7276  n_name else serv
-0002a5d0: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
+0002a2a0: 2020 2020 2020 2020 206c 6174 6573 745f           latest_
+0002a2b0: 6461 7461 736f 7572 6365 5f76 6572 7369  datasource_versi
+0002a2c0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+0002a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a2e0: 2064 7279 5f72 756e 2c0a 2020 2020 2020   dry_run,.      
+0002a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a300: 2020 2020 2020 666f 726b 5f64 6f77 6e73        fork_downs
+0002a310: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
+0002a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a330: 2020 2066 6f72 6b2c 0a20 2020 2020 2020     fork,.       
+0002a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a350: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0002a360: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0002a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a380: 2020 2020 2023 2049 6620 7765 2061 7265       # If we are
+0002a390: 2074 7279 696e 6720 746f 206d 6f64 6966   trying to modif
+0002a3a0: 7920 6120 4b61 666b 6120 6f72 2043 444b  y a Kafka or CDK
+0002a3b0: 2064 6174 6173 6f75 7263 652c 2077 6520   datasource, we 
+0002a3c0: 6e65 6564 2074 6f20 696e 666f 726d 2074  need to inform t
+0002a3d0: 6865 2075 7365 7220 7468 6174 2074 6865  he user that the
+0002a3e0: 2072 6573 6f75 7263 6520 6e65 6564 7320   resource needs 
+0002a3f0: 746f 2062 6520 706f 7374 2d72 656c 6561  to be post-relea
+0002a400: 7365 640a 2020 2020 2020 2020 2020 2020  sed.            
+0002a410: 2020 2020 2020 2020 2020 2020 6b61 666b              kafk
+0002a420: 615f 636f 6e6e 6563 7469 6f6e 5f6e 616d  a_connection_nam
+0002a430: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
+0002a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a450: 2020 7265 736f 7572 6365 735f 746f 5f72    resources_to_r
+0002a460: 756e 5f66 6f72 6b5f 646f 776e 7374 7265  un_fork_downstre
+0002a470: 616d 5b6e 616d 655d 2e67 6574 2822 7061  am[name].get("pa
+0002a480: 7261 6d73 222c 207b 7d29 2e67 6574 2822  rams", {}).get("
+0002a490: 6b61 666b 615f 636f 6e6e 6563 7469 6f6e  kafka_connection
+0002a4a0: 5f6e 616d 6522 290a 2020 2020 2020 2020  _name").        
+0002a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a4c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002a4d0: 2020 2020 2020 2020 2020 7365 7276 6963            servic
+0002a4e0: 6520 3d20 7265 736f 7572 6365 735f 746f  e = resources_to
+0002a4f0: 5f72 756e 5f66 6f72 6b5f 646f 776e 7374  _run_fork_downst
+0002a500: 7265 616d 5b6e 616d 655d 2e67 6574 2822  ream[name].get("
+0002a510: 7061 7261 6d73 222c 207b 7d29 2e67 6574  params", {}).get
+0002a520: 2822 696d 706f 7274 5f73 6572 7669 6365  ("import_service
+0002a530: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0002a540: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0002a550: 6c65 6173 655f 6372 6561 7465 6420 616e  lease_created an
+0002a560: 6420 286b 6166 6b61 5f63 6f6e 6e65 6374  d (kafka_connect
+0002a570: 696f 6e5f 6e61 6d65 206f 7220 7365 7276  ion_name or serv
+0002a580: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
+0002a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a5a0: 2020 636f 6e6e 6563 746f 7220 3d20 224b    connector = "K
+0002a5b0: 6166 6b61 2220 6966 206b 6166 6b61 5f63  afka" if kafka_c
+0002a5c0: 6f6e 6e65 6374 696f 6e5f 6e61 6d65 2065  onnection_name e
+0002a5d0: 6c73 6520 7365 7276 6963 650a 2020 2020  lse service.    
 0002a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a5f0: 6572 726f 725f 6d73 6720 3d20 4665 6564  error_msg = Feed
-0002a600: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
-0002a610: 725f 636f 6e6e 6563 746f 725f 7265 7175  r_connector_requ
-0002a620: 6972 655f 706f 7374 5f72 656c 6561 7365  ire_post_release
-0002a630: 2863 6f6e 6e65 6374 6f72 3d63 6f6e 6e65  (connector=conne
-0002a640: 6374 6f72 290a 2020 2020 2020 2020 2020  ctor).          
+0002a5f0: 2020 2020 2020 2020 6572 726f 725f 6d73          error_ms
+0002a600: 6720 3d20 4665 6564 6261 636b 4d61 6e61  g = FeedbackMana
+0002a610: 6765 722e 6572 726f 725f 636f 6e6e 6563  ger.error_connec
+0002a620: 746f 725f 7265 7175 6972 655f 706f 7374  tor_require_post
+0002a630: 5f72 656c 6561 7365 2863 6f6e 6e65 6374  _release(connect
+0002a640: 6f72 3d63 6f6e 6e65 6374 6f72 290a 2020  or=connector).  
 0002a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a660: 2020 7261 6973 6520 636c 6963 6b2e 436c    raise click.Cl
-0002a670: 6963 6b45 7863 6570 7469 6f6e 2865 7272  ickException(err
-0002a680: 6f72 5f6d 7367 290a 0a20 2020 2020 2020  or_msg)..       
-0002a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a6a0: 2023 2049 6620 7765 2061 7265 2070 7573   # If we are pus
-0002a6b0: 6869 6e67 2061 206d 6f64 6966 6965 6420  hing a modified 
-0002a6c0: 6461 7461 736f 7572 6365 2c20 696e 666f  datasource, info
-0002a6d0: 726d 2061 626f 7574 2074 6865 2062 6163  rm about the bac
-0002a6e0: 6b66 696c 6c60 600a 2020 2020 2020 2020  kfill``.        
+0002a660: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0002a670: 636c 6963 6b2e 436c 6963 6b45 7863 6570  click.ClickExcep
+0002a680: 7469 6f6e 2865 7272 6f72 5f6d 7367 290a  tion(error_msg).
+0002a690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a6a0: 2020 2020 2020 2020 2023 2049 6620 7765           # If we
+0002a6b0: 2061 7265 2070 7573 6869 6e67 2061 206d   are pushing a m
+0002a6c0: 6f64 6966 6965 6420 6461 7461 736f 7572  odified datasour
+0002a6d0: 6365 2c20 696e 666f 726d 2061 626f 7574  ce, inform about
+0002a6e0: 2074 6865 2062 6163 6b66 696c 6c60 600a   the backfill``.
 0002a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a700: 6966 2063 6865 636b 5f62 6163 6b66 696c  if check_backfil
-0002a710: 6c5f 7265 7175 6972 6564 2061 6e64 2061  l_required and a
-0002a720: 7574 6f5f 7072 6f6d 6f74 6520 616e 6420  uto_promote and 
-0002a730: 7265 6c65 6173 655f 6372 6561 7465 643a  release_created:
-0002a740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a750: 2020 2020 2020 2020 2020 2020 2065 7272               err
-0002a760: 6f72 5f6d 7367 203d 2046 6565 6462 6163  or_msg = Feedbac
-0002a770: 6b4d 616e 6167 6572 2e65 7272 6f72 5f63  kManager.error_c
-0002a780: 6865 636b 5f62 6163 6b66 696c 6c5f 7265  heck_backfill_re
-0002a790: 7175 6972 6564 2872 6573 6f75 7263 655f  quired(resource_
-0002a7a0: 6e61 6d65 3d6e 616d 6529 0a20 2020 2020  name=name).     
-0002a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a7c0: 2020 2020 2020 2072 6169 7365 2063 6c69         raise cli
-0002a7d0: 636b 2e43 6c69 636b 4578 6365 7074 696f  ck.ClickExceptio
-0002a7e0: 6e28 6572 726f 725f 6d73 6729 0a0a 2020  n(error_msg)..  
-0002a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a800: 2020 2020 2020 6177 6169 7420 7075 7368        await push
-0002a810: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002a820: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0002a830: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0002a700: 2020 2020 2020 2020 6966 2063 6865 636b          if check
+0002a710: 5f62 6163 6b66 696c 6c5f 7265 7175 6972  _backfill_requir
+0002a720: 6564 2061 6e64 2061 7574 6f5f 7072 6f6d  ed and auto_prom
+0002a730: 6f74 6520 616e 6420 7265 6c65 6173 655f  ote and release_
+0002a740: 6372 6561 7465 643a 0a20 2020 2020 2020  created:.       
+0002a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a760: 2020 2020 2065 7272 6f72 5f6d 7367 203d       error_msg =
+0002a770: 2046 6565 6462 6163 6b4d 616e 6167 6572   FeedbackManager
+0002a780: 2e65 7272 6f72 5f63 6865 636b 5f62 6163  .error_check_bac
+0002a790: 6b66 696c 6c5f 7265 7175 6972 6564 2872  kfill_required(r
+0002a7a0: 6573 6f75 7263 655f 6e61 6d65 3d6e 616d  esource_name=nam
+0002a7b0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0002a7c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002a7d0: 6169 7365 2063 6c69 636b 2e43 6c69 636b  aise click.Click
+0002a7e0: 4578 6365 7074 696f 6e28 6572 726f 725f  Exception(error_
+0002a7f0: 6d73 6729 0a0a 2020 2020 2020 2020 2020  msg)..          
+0002a800: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+0002a810: 6169 7420 7075 7368 280a 2020 2020 2020  ait push(.      
+0002a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a830: 2020 2020 2020 6e61 6d65 2c0a 2020 2020        name,.    
 0002a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a850: 7265 736f 7572 6365 735f 746f 5f72 756e  resources_to_run
-0002a860: 5f66 6f72 6b5f 646f 776e 7374 7265 616d  _fork_downstream
-0002a870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002a880: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0002a890: 736f 7572 6365 5f76 6572 7369 6f6e 732c  source_versions,
-0002a8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a8b0: 2020 2020 2020 2020 2020 2020 206c 6174               lat
-0002a8c0: 6573 745f 6461 7461 736f 7572 6365 5f76  est_datasource_v
-0002a8d0: 6572 7369 6f6e 732c 0a20 2020 2020 2020  ersions,.       
-0002a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a8f0: 2020 2020 2064 7279 5f72 756e 2c0a 2020       dry_run,.  
-0002a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a910: 2020 2020 2020 2020 2020 666f 726b 5f64            fork_d
-0002a920: 6f77 6e73 7472 6561 6d2c 0a20 2020 2020  ownstream,.     
-0002a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a940: 2020 2020 2020 2066 6f72 6b2c 0a20 2020         fork,.   
-0002a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a960: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0002a970: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-0002a980: 7373 6564 2e61 6464 286e 616d 6529 0a0a  ssed.add(name)..
-0002a990: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
-0002a9a0: 772c 2077 6520 7769 6c6c 2063 7265 6174  w, we will creat
-0002a9b0: 6520 6120 6d61 7020 6f66 2061 6c6c 2074  e a map of all t
-0002a9c0: 6865 2065 6e64 706f 696e 7473 2061 6e64  he endpoints and
-0002a9d0: 2074 6865 7265 2064 6570 656e 6465 6e63   there dependenc
-0002a9e0: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-0002a9f0: 2320 5765 2061 7265 2075 7369 6e67 2074  # We are using t
-0002aa00: 6865 2066 6f72 6b64 6f77 6e73 7472 6561  he forkdownstrea
-0002aa10: 6d20 6772 6170 6820 746f 2067 6574 2074  m graph to get t
-0002aa20: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
-0002aa30: 6f66 2074 6865 2065 6e64 706f 696e 7473  of the endpoints
-0002aa40: 2061 7320 7468 6520 6e6f 726d 616c 2064   as the normal d
-0002aa50: 6570 656e 6465 6e63 6965 7320 6772 6170  ependencies grap
-0002aa60: 6820 6f6e 6c79 2063 6f6e 7461 696e 7320  h only contains 
-0002aa70: 7468 6520 7265 736f 7572 6365 7320 7468  the resources th
-0002aa80: 6174 2061 7265 2067 6f69 6e67 2074 6f20  at are going to 
-0002aa90: 6265 2064 6570 6c6f 7965 640a 2020 2020  be deployed.    
-0002aaa0: 2020 2020 2020 2020 2320 4275 7420 646f          # But do
-0002aab0: 6573 206e 6f74 2069 6e63 6c75 6465 2074  es not include t
-0002aac0: 6865 206d 6973 7369 6e67 2067 6170 730a  he missing gaps.
-0002aad0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-0002aae0: 2077 6520 6861 7665 2045 4e44 504f 494e   we have ENDPOIN
-0002aaf0: 545f 4120 2d2d 2d2d 3e20 4d56 5f50 4950  T_A ----> MV_PIP
-0002ab00: 455f 4220 2d2d 2d2d 2d3e 2044 4154 4153  E_B -----> DATAS
-0002ab10: 4f55 5243 455f 4220 2d2d 2d2d 2d2d 3e20  OURCE_B ------> 
-0002ab20: 454e 4450 4f49 4e54 5f43 0a20 2020 2020  ENDPOINT_C.     
-0002ab30: 2020 2020 2020 2023 2057 6865 7265 2065         # Where e
-0002ab40: 6e64 706f 696e 7420 4120 6973 2062 6569  ndpoint A is bei
-0002ab50: 6e67 2075 7365 6420 696e 2074 6865 204d  ng used in the M
-0002ab60: 565f 5049 5045 5f42 2c20 6966 2077 6520  V_PIPE_B, if we 
-0002ab70: 6f6e 6c79 206d 6f64 6966 7920 7468 6520  only modify the 
-0002ab80: 656e 6470 6f69 6e74 2041 0a20 2020 2020  endpoint A.     
-0002ab90: 2020 2020 2020 2023 2054 6865 2064 6570         # The dep
-0002aba0: 656e 6465 6e63 6965 7320 6772 6170 6820  endencies graph 
-0002abb0: 7769 6c6c 206f 6e6c 7920 636f 6e74 6169  will only contai
-0002abc0: 6e20 7468 6520 656e 6470 6f69 6e74 2041  n the endpoint A
-0002abd0: 2061 6e64 2074 6865 204d 565f 5049 5045   and the MV_PIPE
-0002abe0: 5f42 2c20 6275 7420 6e6f 7420 7468 6520  _B, but not the 
-0002abf0: 4441 5441 534f 5552 4345 5f42 2061 6e64  DATASOURCE_B and
-0002ac00: 2074 6865 2045 4e44 504f 494e 545f 430a   the ENDPOINT_C.
-0002ac10: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-0002ac20: 7073 203d 205b 6772 6f75 7020 666f 7220  ps = [group for 
-0002ac30: 6772 6f75 7020 696e 2074 6f70 6f73 6f72  group in toposor
-0002ac40: 7428 6465 7065 6e64 656e 6369 6573 5f67  t(dependencies_g
-0002ac50: 7261 7068 5f66 6f72 6b5f 646f 776e 7374  raph_fork_downst
-0002ac60: 7265 616d 295d 0a20 2020 2020 2020 2020  ream)].         
-0002ac70: 2020 2066 6f72 2067 726f 7570 2069 6e20     for group in 
-0002ac80: 6772 6f75 7073 3a0a 2020 2020 2020 2020  groups:.        
-0002ac90: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
-0002aca0: 2069 6e20 6772 6f75 703a 0a20 2020 2020   in group:.     
-0002acb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002acc0: 6620 6e61 6d65 2069 6e20 7072 6f63 6573  f name in proces
-0002acd0: 7365 6420 6f72 206e 6f74 2069 735f 656e  sed or not is_en
-0002ace0: 6470 6f69 6e74 2872 6573 6f75 7263 6573  dpoint(resources
-0002acf0: 5f74 6f5f 7275 6e5f 666f 726b 5f64 6f77  _to_run_fork_dow
-0002ad00: 6e73 7472 6561 6d5b 6e61 6d65 5d29 3a0a  nstream[name]):.
-0002ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ad20: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0002ad30: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002ad40: 2020 2020 2020 656e 6470 6f69 6e74 735f        endpoints_
-0002ad50: 6465 705f 6d61 705b 6e61 6d65 5d20 3d20  dep_map[name] = 
-0002ad60: 6465 7065 6e64 656e 6369 6573 5f67 7261  dependencies_gra
-0002ad70: 7068 5f66 6f72 6b5f 646f 776e 7374 7265  ph_fork_downstre
-0002ad80: 616d 5b6e 616d 655d 0a0a 2020 2020 2020  am[name]..      
-0002ad90: 2020 2020 2020 2320 4e6f 7720 7468 6174        # Now that
-0002ada0: 2077 6520 6861 7665 2074 6865 2064 6570   we have the dep
-0002adb0: 656e 6465 6e63 6965 7320 6f66 2074 6865  endencies of the
-0002adc0: 2065 6e64 706f 696e 7473 2c20 7765 206e   endpoints, we n
-0002add0: 6565 6420 746f 2063 6865 636b 2074 6861  eed to check tha
-0002ade0: 7420 7468 6520 7265 736f 7572 6365 7320  t the resources 
-0002adf0: 6861 7320 6e6f 7420 6265 656e 2064 6570  has not been dep
-0002ae00: 6c6f 7965 6420 7965 7420 616e 6420 6f6e  loyed yet and on
-0002ae10: 6c79 2063 6172 6520 6162 6f75 7420 7468  ly care about th
-0002ae20: 6520 656e 6470 6f69 6e74 7320 7468 6174  e endpoints that
-0002ae30: 2064 6570 656e 6420 6f6e 2065 6e64 706f   depend on endpo
-0002ae40: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
-0002ae50: 2067 726f 7570 7320 3d20 5b67 726f 7570   groups = [group
-0002ae60: 2066 6f72 2067 726f 7570 2069 6e20 746f   for group in to
-0002ae70: 706f 736f 7274 2865 6e64 706f 696e 7473  posort(endpoints
-0002ae80: 5f64 6570 5f6d 6170 295d 0a0a 2020 2020  _dep_map)]..    
-0002ae90: 2020 2020 2020 2020 2320 4173 2077 6520          # As we 
-0002aea0: 6861 7665 2075 7365 6420 7468 6520 666f  have used the fo
-0002aeb0: 726b 646f 776e 7374 7265 616d 2067 7261  rkdownstream gra
-0002aec0: 7068 2074 6f20 6765 7420 7468 6520 6465  ph to get the de
-0002aed0: 7065 6e64 656e 6369 6573 206f 6620 7468  pendencies of th
-0002aee0: 6520 656e 6470 6f69 6e74 732c 2077 6520  e endpoints, we 
-0002aef0: 6861 7665 2061 6c6c 2074 6865 2064 6570  have all the dep
-0002af00: 656e 6465 6e63 6965 7320 6f66 2074 6865  endencies of the
-0002af10: 2065 6e64 706f 696e 7473 0a20 2020 2020   endpoints.     
-0002af20: 2020 2020 2020 2023 2042 7574 2077 6520         # But we 
-0002af30: 6e65 6564 2074 6f20 6465 706c 6f79 2074  need to deploy t
-0002af40: 6865 2065 6e64 706f 696e 7473 2061 6e64  he endpoints and
-0002af50: 2074 6865 2064 6570 656e 6465 6e63 6965   the dependencie
-0002af60: 7320 6f66 2074 6865 2065 6e64 706f 696e  s of the endpoin
-0002af70: 7473 2066 726f 6d20 6c65 6674 2074 6f20  ts from left to 
-0002af80: 7269 6768 740a 2020 2020 2020 2020 2020  right.          
-0002af90: 2020 2320 536f 2077 6520 6e65 6564 2074    # So we need t
-0002afa0: 6f20 7265 7665 7273 6520 7468 6520 6772  o reverse the gr
-0002afb0: 6f75 7073 0a20 2020 2020 2020 2020 2020  oups.           
-0002afc0: 2067 726f 7570 732e 7265 7665 7273 6528   groups.reverse(
-0002afd0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0002afe0: 7220 6772 6f75 7020 696e 2067 726f 7570  r group in group
-0002aff0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0002b000: 2020 2066 6f72 206e 616d 6520 696e 2067     for name in g
-0002b010: 726f 7570 3a0a 2020 2020 2020 2020 2020  roup:.          
-0002b020: 2020 2020 2020 2020 2020 6966 206e 616d            if nam
-0002b030: 6520 696e 2070 726f 6365 7373 6564 206f  e in processed o
-0002b040: 7220 6e6f 7420 6973 5f65 6e64 706f 696e  r not is_endpoin
-0002b050: 7428 7265 736f 7572 6365 735f 746f 5f72  t(resources_to_r
-0002b060: 756e 5f66 6f72 6b5f 646f 776e 7374 7265  un_fork_downstre
-0002b070: 616d 5b6e 616d 655d 293a 0a20 2020 2020  am[name]):.     
-0002b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b090: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
-0002b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b0b0: 2061 7761 6974 2070 7573 6828 0a20 2020   await push(.   
-0002b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b0d0: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
-0002b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b0f0: 2020 2072 6573 6f75 7263 6573 5f74 6f5f     resources_to_
-0002b100: 7275 6e5f 666f 726b 5f64 6f77 6e73 7472  run_fork_downstr
-0002b110: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
-0002b120: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0002b130: 6f75 7263 655f 7665 7273 696f 6e73 2c0a  ource_versions,.
-0002b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b150: 2020 2020 2020 2020 6c61 7465 7374 5f64          latest_d
-0002b160: 6174 6173 6f75 7263 655f 7665 7273 696f  atasource_versio
-0002b170: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-0002b180: 2020 2020 2020 2020 2020 2020 6472 795f              dry_
-0002b190: 7275 6e2c 0a20 2020 2020 2020 2020 2020  run,.           
-0002b1a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0002b1b0: 6b5f 646f 776e 7374 7265 616d 2c0a 2020  k_downstream,.  
-0002b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b1d0: 2020 2020 2020 666f 726b 2c0a 2020 2020        fork,.    
-0002b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b1f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002b200: 2020 2020 2020 7072 6f63 6573 7365 642e        processed.
-0002b210: 6164 6428 6e61 6d65 290a 0a20 2020 2020  add(name)..     
-0002b220: 2020 2020 2020 2023 204e 6f77 2077 6520         # Now we 
-0002b230: 7368 6f75 6c64 2068 6176 6520 7468 6520  should have the 
-0002b240: 656e 6470 6f69 6e74 7320 616e 6420 6461  endpoints and da
-0002b250: 7461 736f 7572 6365 7320 6465 706c 6f79  tasources deploy
-0002b260: 6564 2c20 7765 2063 616e 2064 6570 6c6f  ed, we can deplo
-0002b270: 7920 7468 6520 7265 7374 206f 6620 7468  y the rest of th
-0002b280: 6520 7069 7065 7320 2863 6f70 7920 2620  e pipes (copy & 
-0002b290: 7369 6e6b 7329 0a20 2020 2020 2020 2020  sinks).         
-0002b2a0: 2020 2023 2057 6520 6e65 6564 2074 6f20     # We need to 
-0002b2b0: 7265 6c79 206f 6e20 7468 6520 666f 726b  rely on the fork
-0002b2c0: 646f 776e 7374 7265 616d 2067 7261 7068  downstream graph
-0002b2d0: 2061 7320 6974 2063 6f6e 7461 696e 7320   as it contains 
-0002b2e0: 616c 6c20 7468 6520 6d6f 6469 6669 6564  all the modified
-0002b2f0: 2070 6970 6573 2061 7320 7765 6c6c 2061   pipes as well a
-0002b300: 7320 7468 6520 6465 7065 6e64 656e 6369  s the dependenci
-0002b310: 6573 206f 6620 7468 6520 7069 7065 730a  es of the pipes.
-0002b320: 2020 2020 2020 2020 2020 2020 2320 496e              # In
-0002b330: 2074 6869 7320 6361 7365 2c20 7765 2064   this case, we d
-0002b340: 6f6e 2774 206e 6565 6420 746f 2067 656e  on't need to gen
-0002b350: 6572 6174 6520 6120 6e65 7720 6772 6170  erate a new grap
-0002b360: 6820 6173 2077 6520 6469 6420 666f 7220  h as we did for 
-0002b370: 7468 6520 656e 6470 6f69 6e74 7320 6173  the endpoints as
-0002b380: 2074 6865 2070 6970 6573 2061 7265 206e   the pipes are n
-0002b390: 6f74 2067 6f69 6e67 2074 6f20 6265 2075  ot going to be u
-0002b3a0: 7365 6420 6173 2064 6570 656e 6465 6e63  sed as dependenc
-0002b3b0: 6965 7320 616e 6420 7468 6520 6461 7461  ies and the data
-0002b3c0: 736f 7572 6365 7320 6172 6520 616c 7265  sources are alre
-0002b3d0: 6164 7920 6465 706c 6f79 6564 0a20 2020  ady deployed.   
-0002b3e0: 2020 2020 2020 2020 2067 726f 7570 7320           groups 
-0002b3f0: 3d20 5b67 726f 7570 2066 6f72 2067 726f  = [group for gro
-0002b400: 7570 2069 6e20 746f 706f 736f 7274 2864  up in toposort(d
-0002b410: 6570 656e 6465 6e63 6965 735f 6772 6170  ependencies_grap
-0002b420: 685f 666f 726b 5f64 6f77 6e73 7472 6561  h_fork_downstrea
-0002b430: 6d29 5d0a 2020 2020 2020 2020 2020 2020  m)].            
-0002b440: 666f 7220 6772 6f75 7020 696e 2067 726f  for group in gro
-0002b450: 7570 733a 0a20 2020 2020 2020 2020 2020  ups:.           
-0002b460: 2020 2020 2066 6f72 206e 616d 6520 696e       for name in
-0002b470: 2067 726f 7570 3a0a 2020 2020 2020 2020   group:.        
-0002b480: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0002b490: 616d 6520 696e 2070 726f 6365 7373 6564  ame in processed
-0002b4a0: 206f 7220 6973 5f6d 6174 6572 6961 6c69   or is_materiali
-0002b4b0: 7a65 6428 7265 736f 7572 6365 735f 746f  zed(resources_to
-0002b4c0: 5f72 756e 5f66 6f72 6b5f 646f 776e 7374  _run_fork_downst
-0002b4d0: 7265 616d 2e67 6574 286e 616d 6529 293a  ream.get(name)):
-0002b4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b4f0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0002b500: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-0002b510: 2020 2020 2020 2061 7761 6974 2070 7573         await pus
-0002b520: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
-0002b530: 2020 2020 2020 2020 2020 206e 616d 652c             name,
-0002b540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b550: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-0002b560: 6573 5f74 6f5f 7275 6e5f 666f 726b 5f64  es_to_run_fork_d
-0002b570: 6f77 6e73 7472 6561 6d2c 0a20 2020 2020  ownstream,.     
-0002b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b590: 2020 2072 6573 6f75 7263 655f 7665 7273     resource_vers
-0002b5a0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-0002b5b0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0002b5c0: 7465 7374 5f64 6174 6173 6f75 7263 655f  test_datasource_
-0002b5d0: 7665 7273 696f 6e73 2c0a 2020 2020 2020  versions,.      
-0002b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b5f0: 2020 6472 795f 7275 6e2c 0a20 2020 2020    dry_run,.     
-0002b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b610: 2020 2066 6f72 6b5f 646f 776e 7374 7265     fork_downstre
-0002b620: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
-0002b630: 2020 2020 2020 2020 2020 2020 666f 726b              fork
-0002b640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002b650: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0002b660: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-0002b670: 6573 7365 642e 6164 6428 6e61 6d65 290a  essed.add(name).
-0002b680: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0002b690: 696e 616c 6c79 2c20 7765 206e 6565 6420  inally, we need 
-0002b6a0: 746f 2064 6570 6c6f 7920 7468 6520 6d61  to deploy the ma
-0002b6b0: 7465 7269 616c 697a 6564 2076 6965 7773  terialized views
-0002b6c0: 2066 726f 6d20 7269 6768 7420 746f 206c   from right to l
-0002b6d0: 6566 742e 0a20 2020 2020 2020 2020 2020  eft..           
-0002b6e0: 2023 2057 6520 6e65 6564 2074 6f20 7265   # We need to re
-0002b6f0: 6c79 206f 6e20 7468 6520 666f 726b 646f  ly on the forkdo
-0002b700: 776e 7374 7265 616d 2067 7261 7068 2061  wnstream graph a
-0002b710: 7320 6974 2063 6f6e 7461 696e 7320 616c  s it contains al
-0002b720: 6c20 7468 6520 6d6f 6469 6669 6564 206d  l the modified m
-0002b730: 6174 6572 6961 6c69 7a65 6420 7669 6577  aterialized view
-0002b740: 7320 6173 2077 656c 6c20 6173 2074 6865  s as well as the
-0002b750: 2064 6570 656e 6465 6e63 6965 7320 6f66   dependencies of
-0002b760: 2074 6865 206d 6174 6572 6961 6c69 7a65   the materialize
-0002b770: 6420 7669 6577 730a 2020 2020 2020 2020  d views.        
-0002b780: 2020 2020 2320 496e 2074 6869 7320 6361      # In this ca
-0002b790: 7365 2c20 7765 2064 6f6e 2774 206e 6565  se, we don't nee
-0002b7a0: 6420 746f 2067 656e 6572 6174 6520 6120  d to generate a 
-0002b7b0: 6e65 7720 6772 6170 6820 6173 2077 6520  new graph as we 
-0002b7c0: 6469 6420 666f 7220 7468 6520 656e 6470  did for the endp
-0002b7d0: 6f69 6e74 7320 6173 2074 6865 2070 6970  oints as the pip
-0002b7e0: 6573 2061 7265 206e 6f74 2067 6f69 6e67  es are not going
-0002b7f0: 2074 6f20 6265 2075 7365 6420 6173 2064   to be used as d
-0002b800: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
-0002b810: 7468 6520 6461 7461 736f 7572 6365 7320  the datasources 
-0002b820: 6172 6520 616c 7265 6164 7920 6465 706c  are already depl
-0002b830: 6f79 6564 0a20 2020 2020 2020 2020 2020  oyed.           
-0002b840: 2067 726f 7570 7320 3d20 5b67 726f 7570   groups = [group
-0002b850: 2066 6f72 2067 726f 7570 2069 6e20 746f   for group in to
-0002b860: 706f 736f 7274 2864 6570 656e 6465 6e63  posort(dependenc
-0002b870: 6965 735f 6772 6170 685f 666f 726b 5f64  ies_graph_fork_d
-0002b880: 6f77 6e73 7472 6561 6d29 5d0a 2020 2020  ownstream)].    
-0002b890: 2020 2020 2020 2020 666f 7220 6772 6f75          for grou
-0002b8a0: 7020 696e 2067 726f 7570 733a 0a20 2020  p in groups:.   
-0002b8b0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0002b8c0: 206e 616d 6520 696e 2067 726f 7570 3a0a   name in group:.
-0002b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b8e0: 2020 2020 6966 206e 616d 6520 696e 2070      if name in p
-0002b8f0: 726f 6365 7373 6564 206f 7220 6e6f 7420  rocessed or not 
-0002b900: 6973 5f6d 6174 6572 6961 6c69 7a65 6428  is_materialized(
-0002b910: 7265 736f 7572 6365 735f 746f 5f72 756e  resources_to_run
-0002b920: 5f66 6f72 6b5f 646f 776e 7374 7265 616d  _fork_downstream
-0002b930: 2e67 6574 286e 616d 6529 293a 0a20 2020  .get(name)):.   
-0002b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b950: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-0002b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b970: 2020 2061 7761 6974 2070 7573 6828 0a20     await push(. 
-0002b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b990: 2020 2020 2020 206e 616d 652c 0a20 2020         name,.   
-0002b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b9b0: 2020 2020 2072 6573 6f75 7263 6573 5f74       resources_t
-0002b9c0: 6f5f 7275 6e5f 666f 726b 5f64 6f77 6e73  o_run_fork_downs
-0002b9d0: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
-0002b9e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0002b9f0: 6573 6f75 7263 655f 7665 7273 696f 6e73  esource_versions
-0002ba00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002ba10: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
-0002ba20: 5f64 6174 6173 6f75 7263 655f 7665 7273  _datasource_vers
-0002ba30: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-0002ba40: 2020 2020 2020 2020 2020 2020 2020 6472                dr
-0002ba50: 795f 7275 6e2c 0a20 2020 2020 2020 2020  y_run,.         
-0002ba60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0002ba70: 6f72 6b5f 646f 776e 7374 7265 616d 2c0a  ork_downstream,.
-0002ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ba90: 2020 2020 2020 2020 666f 726b 2c0a 2020          fork,.  
-0002baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bab0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0002bac0: 2020 2020 2020 2020 7072 6f63 6573 7365          processe
-0002bad0: 642e 6164 6428 6e61 6d65 290a 0a20 2020  d.add(name)..   
-0002bae0: 2069 6620 6465 706c 6f79 6d65 6e74 2e69   if deployment.i
-0002baf0: 735f 6769 745f 7265 6c65 6173 653a 0a20  s_git_release:. 
-0002bb00: 2020 2020 2020 2064 6570 6c6f 796d 656e         deploymen
-0002bb10: 742e 6465 706c 6f79 696e 675f 6472 795f  t.deploying_dry_
-0002bb20: 7275 6e28 290a 2020 2020 2020 2020 6177  run().        aw
-0002bb30: 6169 7420 7075 7368 5f66 696c 6573 2864  ait push_files(d
-0002bb40: 6570 656e 6465 6e63 6965 735f 6772 6170  ependencies_grap
-0002bb50: 682c 2064 7279 5f72 756e 3d54 7275 652c  h, dry_run=True,
-0002bb60: 2063 6865 636b 5f62 6163 6b66 696c 6c5f   check_backfill_
-0002bb70: 7265 7175 6972 6564 3d63 6865 636b 5f62  required=check_b
-0002bb80: 6163 6b66 696c 6c5f 7265 7175 6972 6564  ackfill_required
-0002bb90: 290a 0a20 2020 2020 2020 2061 7761 6974  )..        await
-0002bba0: 2064 6570 6c6f 796d 656e 742e 6465 6c65   deployment.dele
-0002bbb0: 7465 5f72 6573 6f75 7263 6573 2864 656c  te_resources(del
-0002bbc0: 6574 6564 2c20 7069 7065 732c 2064 7279  eted, pipes, dry
-0002bbd0: 5f72 756e 3d54 7275 6529 0a20 2020 2020  _run=True).     
-0002bbe0: 2020 2069 6620 6e6f 7420 6465 706c 6f79     if not deploy
-0002bbf0: 6d65 6e74 2e64 7279 5f72 756e 3a0a 2020  ment.dry_run:.  
-0002bc00: 2020 2020 2020 2020 2020 6465 706c 6f79            deploy
-0002bc10: 6d65 6e74 2e64 6570 6c6f 7969 6e67 2829  ment.deploying()
-0002bc20: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-0002bc30: 6974 2070 7573 685f 6669 6c65 7328 6465  it push_files(de
-0002bc40: 7065 6e64 656e 6369 6573 5f67 7261 7068  pendencies_graph
-0002bc50: 2c20 6472 795f 7275 6e29 0a20 2020 2020  , dry_run).     
-0002bc60: 2020 2020 2020 2061 7761 6974 2064 6570         await dep
-0002bc70: 6c6f 796d 656e 742e 6465 6c65 7465 5f72  loyment.delete_r
-0002bc80: 6573 6f75 7263 6573 2864 656c 6574 6564  esources(deleted
-0002bc90: 2c20 7069 7065 7329 0a20 2020 2065 6c73  , pipes).    els
-0002bca0: 653a 0a20 2020 2020 2020 2061 7761 6974  e:.        await
-0002bcb0: 2070 7573 685f 6669 6c65 7328 6465 7065   push_files(depe
-0002bcc0: 6e64 656e 6369 6573 5f67 7261 7068 2c20  ndencies_graph, 
-0002bcd0: 6472 795f 7275 6e29 0a0a 2020 2020 6966  dry_run)..    if
-0002bce0: 206e 6f74 2064 7279 5f72 756e 2061 6e64   not dry_run and
-0002bcf0: 206e 6f74 2072 756e 5f74 6573 7473 3a0a   not run_tests:.
-0002bd00: 2020 2020 2020 2020 6966 2075 706c 6f61          if uploa
-0002bd10: 645f 6669 7874 7572 6573 3a0a 2020 2020  d_fixtures:.    
-0002bd20: 2020 2020 2020 2020 636c 6963 6b2e 6563          click.ec
-0002bd30: 686f 2846 6565 6462 6163 6b4d 616e 6167  ho(FeedbackManag
-0002bd40: 6572 2e69 6e66 6f5f 7075 7368 696e 675f  er.info_pushing_
-0002bd50: 6669 7874 7572 6573 2829 290a 0a20 2020  fixtures())..   
-0002bd60: 2020 2020 2020 2020 2023 2057 6520 6e65           # We ne
-0002bd70: 6564 2074 6f20 7570 6c6f 6164 2074 6865  ed to upload the
-0002bd80: 2066 6978 7475 7265 7320 6576 656e 2069   fixtures even i
-0002bd90: 6620 7468 6572 6520 6973 206e 6f20 6368  f there is no ch
-0002bda0: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
-0002bdb0: 2069 6620 6973 5f62 7261 6e63 683a 0a20   if is_branch:. 
-0002bdc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0002bdd0: 696c 656e 616d 6573 203d 2067 6574 5f70  ilenames = get_p
-0002bde0: 726f 6a65 6374 5f66 696c 656e 616d 6573  roject_filenames
-0002bdf0: 2866 6f6c 6465 722c 2077 6974 685f 7665  (folder, with_ve
-0002be00: 6e64 6f72 3d54 7275 6529 0a20 2020 2020  ndor=True).     
-0002be10: 2020 2020 2020 2020 2020 2064 6570 656e             depen
-0002be20: 6465 6e63 6965 735f 6772 6170 6820 3d20  dencies_graph = 
-0002be30: 6177 6169 7420 6275 696c 645f 6772 6170  await build_grap
-0002be40: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
-0002be50: 2020 2020 2020 2066 696c 656e 616d 6573         filenames
-0002be60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002be70: 2020 2020 2020 7462 5f63 6c69 656e 742c        tb_client,
-0002be80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002be90: 2020 2020 2064 6972 5f70 6174 683d 666f       dir_path=fo
-0002bea0: 6c64 6572 2c0a 2020 2020 2020 2020 2020  lder,.          
-0002beb0: 2020 2020 2020 2020 2020 7265 736f 7572            resour
-0002bec0: 6365 5f76 6572 7369 6f6e 733d 6c61 7465  ce_versions=late
-0002bed0: 7374 5f64 6174 6173 6f75 7263 655f 7665  st_datasource_ve
-0002bee0: 7273 696f 6e73 2c0a 2020 2020 2020 2020  rsions,.        
-0002bef0: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0002bf00: 7370 6163 655f 6d61 703d 776f 726b 7370  space_map=worksp
-0002bf10: 6163 655f 6d61 702c 0a20 2020 2020 2020  ace_map,.       
-0002bf20: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-0002bf30: 6365 7373 5f64 6570 656e 6465 6e63 6965  cess_dependencie
-0002bf40: 733d 7075 7368 5f64 6570 732c 0a20 2020  s=push_deps,.   
-0002bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bf60: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-0002bf70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002bf80: 2020 2020 2020 776f 726b 7370 6163 655f        workspace_
-0002bf90: 6c69 625f 7061 7468 733d 776f 726b 7370  lib_paths=worksp
-0002bfa0: 6163 655f 6c69 625f 7061 7468 732c 0a20  ace_lib_paths,. 
-0002bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bfc0: 2020 2063 7572 7265 6e74 5f77 733d 6375     current_ws=cu
-0002bfd0: 7272 656e 745f 7773 2c0a 2020 2020 2020  rrent_ws,.      
-0002bfe0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0002bff0: 2020 2020 2020 2020 2070 726f 6365 7373           process
-0002c000: 6564 203d 2073 6574 2829 0a20 2020 2020  ed = set().     
-0002c010: 2020 2020 2020 2066 6f72 2067 726f 7570         for group
-0002c020: 2069 6e20 746f 706f 736f 7274 2864 6570   in toposort(dep
-0002c030: 656e 6465 6e63 6965 735f 6772 6170 682e  endencies_graph.
-0002c040: 6465 705f 6d61 7029 3a0a 2020 2020 2020  dep_map):.      
-0002c050: 2020 2020 2020 2020 2020 666f 7220 6620            for f 
-0002c060: 696e 2067 726f 7570 3a0a 2020 2020 2020  in group:.      
-0002c070: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0002c080: 6d65 203d 206f 732e 7061 7468 2e62 6173  me = os.path.bas
-0002c090: 656e 616d 6528 6629 0a20 2020 2020 2020  ename(f).       
-0002c0a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0002c0b0: 6e61 6d65 206e 6f74 2069 6e20 7072 6f63  name not in proc
-0002c0c0: 6573 7365 643a 0a20 2020 2020 2020 2020  essed:.         
-0002c0d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002c0e0: 6620 6e61 6d65 2069 6e20 6465 7065 6e64  f name in depend
-0002c0f0: 656e 6369 6573 5f67 7261 7068 2e74 6f5f  encies_graph.to_
-0002c100: 7275 6e3a 0a20 2020 2020 2020 2020 2020  run:.           
+0002a850: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0002a860: 735f 746f 5f72 756e 5f66 6f72 6b5f 646f  s_to_run_fork_do
+0002a870: 776e 7374 7265 616d 2c0a 2020 2020 2020  wnstream,.      
+0002a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a890: 2020 2020 2020 7265 736f 7572 6365 5f76        resource_v
+0002a8a0: 6572 7369 6f6e 732c 0a20 2020 2020 2020  ersions,.       
+0002a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a8c0: 2020 2020 206c 6174 6573 745f 6461 7461       latest_data
+0002a8d0: 736f 7572 6365 5f76 6572 7369 6f6e 732c  source_versions,
+0002a8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a8f0: 2020 2020 2020 2020 2020 2020 2064 7279               dry
+0002a900: 5f72 756e 2c0a 2020 2020 2020 2020 2020  _run,.          
+0002a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a920: 2020 666f 726b 5f64 6f77 6e73 7472 6561    fork_downstrea
+0002a930: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
+0002a940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002a950: 6f72 6b2c 0a20 2020 2020 2020 2020 2020  ork,.           
+0002a960: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0002a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a980: 2020 2070 726f 6365 7373 6564 2e61 6464     processed.add
+0002a990: 286e 616d 6529 0a0a 2020 2020 2020 2020  (name)..        
+0002a9a0: 2020 2020 2320 4e6f 772c 2077 6520 7769      # Now, we wi
+0002a9b0: 6c6c 2063 7265 6174 6520 6120 6d61 7020  ll create a map 
+0002a9c0: 6f66 2061 6c6c 2074 6865 2065 6e64 706f  of all the endpo
+0002a9d0: 696e 7473 2061 6e64 2074 6865 7265 2064  ints and there d
+0002a9e0: 6570 656e 6465 6e63 6965 730a 2020 2020  ependencies.    
+0002a9f0: 2020 2020 2020 2020 2320 5765 2061 7265          # We are
+0002aa00: 2075 7369 6e67 2074 6865 2066 6f72 6b64   using the forkd
+0002aa10: 6f77 6e73 7472 6561 6d20 6772 6170 6820  ownstream graph 
+0002aa20: 746f 2067 6574 2074 6865 2064 6570 656e  to get the depen
+0002aa30: 6465 6e63 6965 7320 6f66 2074 6865 2065  dencies of the e
+0002aa40: 6e64 706f 696e 7473 2061 7320 7468 6520  ndpoints as the 
+0002aa50: 6e6f 726d 616c 2064 6570 656e 6465 6e63  normal dependenc
+0002aa60: 6965 7320 6772 6170 6820 6f6e 6c79 2063  ies graph only c
+0002aa70: 6f6e 7461 696e 7320 7468 6520 7265 736f  ontains the reso
+0002aa80: 7572 6365 7320 7468 6174 2061 7265 2067  urces that are g
+0002aa90: 6f69 6e67 2074 6f20 6265 2064 6570 6c6f  oing to be deplo
+0002aaa0: 7965 640a 2020 2020 2020 2020 2020 2020  yed.            
+0002aab0: 2320 4275 7420 646f 6573 206e 6f74 2069  # But does not i
+0002aac0: 6e63 6c75 6465 2074 6865 206d 6973 7369  nclude the missi
+0002aad0: 6e67 2067 6170 730a 2020 2020 2020 2020  ng gaps.        
+0002aae0: 2020 2020 2320 4966 2077 6520 6861 7665      # If we have
+0002aaf0: 2045 4e44 504f 494e 545f 4120 2d2d 2d2d   ENDPOINT_A ----
+0002ab00: 3e20 4d56 5f50 4950 455f 4220 2d2d 2d2d  > MV_PIPE_B ----
+0002ab10: 2d3e 2044 4154 4153 4f55 5243 455f 4220  -> DATASOURCE_B 
+0002ab20: 2d2d 2d2d 2d2d 3e20 454e 4450 4f49 4e54  ------> ENDPOINT
+0002ab30: 5f43 0a20 2020 2020 2020 2020 2020 2023  _C.            #
+0002ab40: 2057 6865 7265 2065 6e64 706f 696e 7420   Where endpoint 
+0002ab50: 4120 6973 2062 6569 6e67 2075 7365 6420  A is being used 
+0002ab60: 696e 2074 6865 204d 565f 5049 5045 5f42  in the MV_PIPE_B
+0002ab70: 2c20 6966 2077 6520 6f6e 6c79 206d 6f64  , if we only mod
+0002ab80: 6966 7920 7468 6520 656e 6470 6f69 6e74  ify the endpoint
+0002ab90: 2041 0a20 2020 2020 2020 2020 2020 2023   A.            #
+0002aba0: 2054 6865 2064 6570 656e 6465 6e63 6965   The dependencie
+0002abb0: 7320 6772 6170 6820 7769 6c6c 206f 6e6c  s graph will onl
+0002abc0: 7920 636f 6e74 6169 6e20 7468 6520 656e  y contain the en
+0002abd0: 6470 6f69 6e74 2041 2061 6e64 2074 6865  dpoint A and the
+0002abe0: 204d 565f 5049 5045 5f42 2c20 6275 7420   MV_PIPE_B, but 
+0002abf0: 6e6f 7420 7468 6520 4441 5441 534f 5552  not the DATASOUR
+0002ac00: 4345 5f42 2061 6e64 2074 6865 2045 4e44  CE_B and the END
+0002ac10: 504f 494e 545f 430a 2020 2020 2020 2020  POINT_C.        
+0002ac20: 2020 2020 6772 6f75 7073 203d 205b 6772      groups = [gr
+0002ac30: 6f75 7020 666f 7220 6772 6f75 7020 696e  oup for group in
+0002ac40: 2074 6f70 6f73 6f72 7428 6465 7065 6e64   toposort(depend
+0002ac50: 656e 6369 6573 5f67 7261 7068 5f66 6f72  encies_graph_for
+0002ac60: 6b5f 646f 776e 7374 7265 616d 295d 0a20  k_downstream)]. 
+0002ac70: 2020 2020 2020 2020 2020 2066 6f72 2067             for g
+0002ac80: 726f 7570 2069 6e20 6772 6f75 7073 3a0a  roup in groups:.
+0002ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002aca0: 666f 7220 6e61 6d65 2069 6e20 6772 6f75  for name in grou
+0002acb0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+0002acc0: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
+0002acd0: 6e20 7072 6f63 6573 7365 6420 6f72 206e  n processed or n
+0002ace0: 6f74 2069 735f 656e 6470 6f69 6e74 2872  ot is_endpoint(r
+0002acf0: 6573 6f75 7263 6573 5f74 6f5f 7275 6e5f  esources_to_run_
+0002ad00: 666f 726b 5f64 6f77 6e73 7472 6561 6d5b  fork_downstream[
+0002ad10: 6e61 6d65 5d29 3a0a 2020 2020 2020 2020  name]):.        
+0002ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ad30: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
+0002ad40: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0002ad50: 6470 6f69 6e74 735f 6465 705f 6d61 705b  dpoints_dep_map[
+0002ad60: 6e61 6d65 5d20 3d20 6465 7065 6e64 656e  name] = dependen
+0002ad70: 6369 6573 5f67 7261 7068 5f66 6f72 6b5f  cies_graph_fork_
+0002ad80: 646f 776e 7374 7265 616d 5b6e 616d 655d  downstream[name]
+0002ad90: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0002ada0: 4e6f 7720 7468 6174 2077 6520 6861 7665  Now that we have
+0002adb0: 2074 6865 2064 6570 656e 6465 6e63 6965   the dependencie
+0002adc0: 7320 6f66 2074 6865 2065 6e64 706f 696e  s of the endpoin
+0002add0: 7473 2c20 7765 206e 6565 6420 746f 2063  ts, we need to c
+0002ade0: 6865 636b 2074 6861 7420 7468 6520 7265  heck that the re
+0002adf0: 736f 7572 6365 7320 6861 7320 6e6f 7420  sources has not 
+0002ae00: 6265 656e 2064 6570 6c6f 7965 6420 7965  been deployed ye
+0002ae10: 7420 616e 6420 6f6e 6c79 2063 6172 6520  t and only care 
+0002ae20: 6162 6f75 7420 7468 6520 656e 6470 6f69  about the endpoi
+0002ae30: 6e74 7320 7468 6174 2064 6570 656e 6420  nts that depend 
+0002ae40: 6f6e 2065 6e64 706f 696e 7473 0a20 2020  on endpoints.   
+0002ae50: 2020 2020 2020 2020 2067 726f 7570 7320           groups 
+0002ae60: 3d20 5b67 726f 7570 2066 6f72 2067 726f  = [group for gro
+0002ae70: 7570 2069 6e20 746f 706f 736f 7274 2865  up in toposort(e
+0002ae80: 6e64 706f 696e 7473 5f64 6570 5f6d 6170  ndpoints_dep_map
+0002ae90: 295d 0a0a 2020 2020 2020 2020 2020 2020  )]..            
+0002aea0: 2320 4173 2077 6520 6861 7665 2075 7365  # As we have use
+0002aeb0: 6420 7468 6520 666f 726b 646f 776e 7374  d the forkdownst
+0002aec0: 7265 616d 2067 7261 7068 2074 6f20 6765  ream graph to ge
+0002aed0: 7420 7468 6520 6465 7065 6e64 656e 6369  t the dependenci
+0002aee0: 6573 206f 6620 7468 6520 656e 6470 6f69  es of the endpoi
+0002aef0: 6e74 732c 2077 6520 6861 7665 2061 6c6c  nts, we have all
+0002af00: 2074 6865 2064 6570 656e 6465 6e63 6965   the dependencie
+0002af10: 7320 6f66 2074 6865 2065 6e64 706f 696e  s of the endpoin
+0002af20: 7473 0a20 2020 2020 2020 2020 2020 2023  ts.            #
+0002af30: 2042 7574 2077 6520 6e65 6564 2074 6f20   But we need to 
+0002af40: 6465 706c 6f79 2074 6865 2065 6e64 706f  deploy the endpo
+0002af50: 696e 7473 2061 6e64 2074 6865 2064 6570  ints and the dep
+0002af60: 656e 6465 6e63 6965 7320 6f66 2074 6865  endencies of the
+0002af70: 2065 6e64 706f 696e 7473 2066 726f 6d20   endpoints from 
+0002af80: 6c65 6674 2074 6f20 7269 6768 740a 2020  left to right.  
+0002af90: 2020 2020 2020 2020 2020 2320 536f 2077            # So w
+0002afa0: 6520 6e65 6564 2074 6f20 7265 7665 7273  e need to revers
+0002afb0: 6520 7468 6520 6772 6f75 7073 0a20 2020  e the groups.   
+0002afc0: 2020 2020 2020 2020 2067 726f 7570 732e           groups.
+0002afd0: 7265 7665 7273 6528 290a 2020 2020 2020  reverse().      
+0002afe0: 2020 2020 2020 666f 7220 6772 6f75 7020        for group 
+0002aff0: 696e 2067 726f 7570 733a 0a20 2020 2020  in groups:.     
+0002b000: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+0002b010: 616d 6520 696e 2067 726f 7570 3a0a 2020  ame in group:.  
+0002b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b030: 2020 6966 206e 616d 6520 696e 2070 726f    if name in pro
+0002b040: 6365 7373 6564 206f 7220 6e6f 7420 6973  cessed or not is
+0002b050: 5f65 6e64 706f 696e 7428 7265 736f 7572  _endpoint(resour
+0002b060: 6365 735f 746f 5f72 756e 5f66 6f72 6b5f  ces_to_run_fork_
+0002b070: 646f 776e 7374 7265 616d 5b6e 616d 655d  downstream[name]
+0002b080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002b090: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0002b0a0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+0002b0b0: 2020 2020 2020 2020 2061 7761 6974 2070           await p
+0002b0c0: 7573 6828 0a20 2020 2020 2020 2020 2020  ush(.           
+0002b0d0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0002b0e0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002b0f0: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0002b100: 7263 6573 5f74 6f5f 7275 6e5f 666f 726b  rces_to_run_fork
+0002b110: 5f64 6f77 6e73 7472 6561 6d2c 0a20 2020  _downstream,.   
+0002b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b130: 2020 2020 2072 6573 6f75 7263 655f 7665       resource_ve
+0002b140: 7273 696f 6e73 2c0a 2020 2020 2020 2020  rsions,.        
+0002b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b160: 6c61 7465 7374 5f64 6174 6173 6f75 7263  latest_datasourc
+0002b170: 655f 7665 7273 696f 6e73 2c0a 2020 2020  e_versions,.    
+0002b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b190: 2020 2020 6472 795f 7275 6e2c 0a20 2020      dry_run,.   
+0002b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b1b0: 2020 2020 2066 6f72 6b5f 646f 776e 7374       fork_downst
+0002b1c0: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
+0002b1d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0002b1e0: 726b 2c0a 2020 2020 2020 2020 2020 2020  rk,.            
+0002b1f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002b200: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0002b210: 6f63 6573 7365 642e 6164 6428 6e61 6d65  ocessed.add(name
+0002b220: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+0002b230: 204e 6f77 2077 6520 7368 6f75 6c64 2068   Now we should h
+0002b240: 6176 6520 7468 6520 656e 6470 6f69 6e74  ave the endpoint
+0002b250: 7320 616e 6420 6461 7461 736f 7572 6365  s and datasource
+0002b260: 7320 6465 706c 6f79 6564 2c20 7765 2063  s deployed, we c
+0002b270: 616e 2064 6570 6c6f 7920 7468 6520 7265  an deploy the re
+0002b280: 7374 206f 6620 7468 6520 7069 7065 7320  st of the pipes 
+0002b290: 2863 6f70 7920 2620 7369 6e6b 7329 0a20  (copy & sinks). 
+0002b2a0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+0002b2b0: 6e65 6564 2074 6f20 7265 6c79 206f 6e20  need to rely on 
+0002b2c0: 7468 6520 666f 726b 646f 776e 7374 7265  the forkdownstre
+0002b2d0: 616d 2067 7261 7068 2061 7320 6974 2063  am graph as it c
+0002b2e0: 6f6e 7461 696e 7320 616c 6c20 7468 6520  ontains all the 
+0002b2f0: 6d6f 6469 6669 6564 2070 6970 6573 2061  modified pipes a
+0002b300: 7320 7765 6c6c 2061 7320 7468 6520 6465  s well as the de
+0002b310: 7065 6e64 656e 6369 6573 206f 6620 7468  pendencies of th
+0002b320: 6520 7069 7065 730a 2020 2020 2020 2020  e pipes.        
+0002b330: 2020 2020 2320 496e 2074 6869 7320 6361      # In this ca
+0002b340: 7365 2c20 7765 2064 6f6e 2774 206e 6565  se, we don't nee
+0002b350: 6420 746f 2067 656e 6572 6174 6520 6120  d to generate a 
+0002b360: 6e65 7720 6772 6170 6820 6173 2077 6520  new graph as we 
+0002b370: 6469 6420 666f 7220 7468 6520 656e 6470  did for the endp
+0002b380: 6f69 6e74 7320 6173 2074 6865 2070 6970  oints as the pip
+0002b390: 6573 2061 7265 206e 6f74 2067 6f69 6e67  es are not going
+0002b3a0: 2074 6f20 6265 2075 7365 6420 6173 2064   to be used as d
+0002b3b0: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
+0002b3c0: 7468 6520 6461 7461 736f 7572 6365 7320  the datasources 
+0002b3d0: 6172 6520 616c 7265 6164 7920 6465 706c  are already depl
+0002b3e0: 6f79 6564 0a20 2020 2020 2020 2020 2020  oyed.           
+0002b3f0: 2067 726f 7570 7320 3d20 5b67 726f 7570   groups = [group
+0002b400: 2066 6f72 2067 726f 7570 2069 6e20 746f   for group in to
+0002b410: 706f 736f 7274 2864 6570 656e 6465 6e63  posort(dependenc
+0002b420: 6965 735f 6772 6170 685f 666f 726b 5f64  ies_graph_fork_d
+0002b430: 6f77 6e73 7472 6561 6d29 5d0a 2020 2020  ownstream)].    
+0002b440: 2020 2020 2020 2020 666f 7220 6772 6f75          for grou
+0002b450: 7020 696e 2067 726f 7570 733a 0a20 2020  p in groups:.   
+0002b460: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0002b470: 206e 616d 6520 696e 2067 726f 7570 3a0a   name in group:.
+0002b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b490: 2020 2020 6966 206e 616d 6520 696e 2070      if name in p
+0002b4a0: 726f 6365 7373 6564 206f 7220 6973 5f6d  rocessed or is_m
+0002b4b0: 6174 6572 6961 6c69 7a65 6428 7265 736f  aterialized(reso
+0002b4c0: 7572 6365 735f 746f 5f72 756e 5f66 6f72  urces_to_run_for
+0002b4d0: 6b5f 646f 776e 7374 7265 616d 2e67 6574  k_downstream.get
+0002b4e0: 286e 616d 6529 293a 0a20 2020 2020 2020  (name)):.       
+0002b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b500: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+0002b510: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0002b520: 7761 6974 2070 7573 6828 0a20 2020 2020  wait push(.     
+0002b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b540: 2020 206e 616d 652c 0a20 2020 2020 2020     name,.       
+0002b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b560: 2072 6573 6f75 7263 6573 5f74 6f5f 7275   resources_to_ru
+0002b570: 6e5f 666f 726b 5f64 6f77 6e73 7472 6561  n_fork_downstrea
+0002b580: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
+0002b590: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0002b5a0: 7263 655f 7665 7273 696f 6e73 2c0a 2020  rce_versions,.  
+0002b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b5c0: 2020 2020 2020 6c61 7465 7374 5f64 6174        latest_dat
+0002b5d0: 6173 6f75 7263 655f 7665 7273 696f 6e73  asource_versions
+0002b5e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002b5f0: 2020 2020 2020 2020 2020 6472 795f 7275            dry_ru
+0002b600: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0002b610: 2020 2020 2020 2020 2020 2066 6f72 6b5f             fork_
+0002b620: 646f 776e 7374 7265 616d 2c0a 2020 2020  downstream,.    
+0002b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b640: 2020 2020 666f 726b 2c0a 2020 2020 2020      fork,.      
+0002b650: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0002b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b670: 2020 2020 7072 6f63 6573 7365 642e 6164      processed.ad
+0002b680: 6428 6e61 6d65 290a 0a20 2020 2020 2020  d(name)..       
+0002b690: 2020 2020 2023 2046 696e 616c 6c79 2c20       # Finally, 
+0002b6a0: 7765 206e 6565 6420 746f 2064 6570 6c6f  we need to deplo
+0002b6b0: 7920 7468 6520 6d61 7465 7269 616c 697a  y the materializ
+0002b6c0: 6564 2076 6965 7773 2066 726f 6d20 7269  ed views from ri
+0002b6d0: 6768 7420 746f 206c 6566 742e 0a20 2020  ght to left..   
+0002b6e0: 2020 2020 2020 2020 2023 2057 6520 6e65           # We ne
+0002b6f0: 6564 2074 6f20 7265 6c79 206f 6e20 7468  ed to rely on th
+0002b700: 6520 666f 726b 646f 776e 7374 7265 616d  e forkdownstream
+0002b710: 2067 7261 7068 2061 7320 6974 2063 6f6e   graph as it con
+0002b720: 7461 696e 7320 616c 6c20 7468 6520 6d6f  tains all the mo
+0002b730: 6469 6669 6564 206d 6174 6572 6961 6c69  dified materiali
+0002b740: 7a65 6420 7669 6577 7320 6173 2077 656c  zed views as wel
+0002b750: 6c20 6173 2074 6865 2064 6570 656e 6465  l as the depende
+0002b760: 6e63 6965 7320 6f66 2074 6865 206d 6174  ncies of the mat
+0002b770: 6572 6961 6c69 7a65 6420 7669 6577 730a  erialized views.
+0002b780: 2020 2020 2020 2020 2020 2020 2320 496e              # In
+0002b790: 2074 6869 7320 6361 7365 2c20 7765 2064   this case, we d
+0002b7a0: 6f6e 2774 206e 6565 6420 746f 2067 656e  on't need to gen
+0002b7b0: 6572 6174 6520 6120 6e65 7720 6772 6170  erate a new grap
+0002b7c0: 6820 6173 2077 6520 6469 6420 666f 7220  h as we did for 
+0002b7d0: 7468 6520 656e 6470 6f69 6e74 7320 6173  the endpoints as
+0002b7e0: 2074 6865 2070 6970 6573 2061 7265 206e   the pipes are n
+0002b7f0: 6f74 2067 6f69 6e67 2074 6f20 6265 2075  ot going to be u
+0002b800: 7365 6420 6173 2064 6570 656e 6465 6e63  sed as dependenc
+0002b810: 6965 7320 616e 6420 7468 6520 6461 7461  ies and the data
+0002b820: 736f 7572 6365 7320 6172 6520 616c 7265  sources are alre
+0002b830: 6164 7920 6465 706c 6f79 6564 0a20 2020  ady deployed.   
+0002b840: 2020 2020 2020 2020 2067 726f 7570 7320           groups 
+0002b850: 3d20 5b67 726f 7570 2066 6f72 2067 726f  = [group for gro
+0002b860: 7570 2069 6e20 746f 706f 736f 7274 2864  up in toposort(d
+0002b870: 6570 656e 6465 6e63 6965 735f 6772 6170  ependencies_grap
+0002b880: 685f 666f 726b 5f64 6f77 6e73 7472 6561  h_fork_downstrea
+0002b890: 6d29 5d0a 2020 2020 2020 2020 2020 2020  m)].            
+0002b8a0: 666f 7220 6772 6f75 7020 696e 2067 726f  for group in gro
+0002b8b0: 7570 733a 0a20 2020 2020 2020 2020 2020  ups:.           
+0002b8c0: 2020 2020 2066 6f72 206e 616d 6520 696e       for name in
+0002b8d0: 2067 726f 7570 3a0a 2020 2020 2020 2020   group:.        
+0002b8e0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0002b8f0: 616d 6520 696e 2070 726f 6365 7373 6564  ame in processed
+0002b900: 206f 7220 6e6f 7420 6973 5f6d 6174 6572   or not is_mater
+0002b910: 6961 6c69 7a65 6428 7265 736f 7572 6365  ialized(resource
+0002b920: 735f 746f 5f72 756e 5f66 6f72 6b5f 646f  s_to_run_fork_do
+0002b930: 776e 7374 7265 616d 2e67 6574 286e 616d  wnstream.get(nam
+0002b940: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
+0002b950: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0002b960: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
+0002b970: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0002b980: 2070 7573 6828 0a20 2020 2020 2020 2020   push(.         
+0002b990: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0002b9a0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0002b9b0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0002b9c0: 6f75 7263 6573 5f74 6f5f 7275 6e5f 666f  ources_to_run_fo
+0002b9d0: 726b 5f64 6f77 6e73 7472 6561 6d2c 0a20  rk_downstream,. 
+0002b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b9f0: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
+0002ba00: 7665 7273 696f 6e73 2c0a 2020 2020 2020  versions,.      
+0002ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ba20: 2020 6c61 7465 7374 5f64 6174 6173 6f75    latest_datasou
+0002ba30: 7263 655f 7665 7273 696f 6e73 2c0a 2020  rce_versions,.  
+0002ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ba50: 2020 2020 2020 6472 795f 7275 6e2c 0a20        dry_run,. 
+0002ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ba70: 2020 2020 2020 2066 6f72 6b5f 646f 776e         fork_down
+0002ba80: 7374 7265 616d 2c0a 2020 2020 2020 2020  stream,.        
+0002ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002baa0: 666f 726b 2c0a 2020 2020 2020 2020 2020  fork,.          
+0002bab0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0002bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bad0: 7072 6f63 6573 7365 642e 6164 6428 6e61  processed.add(na
+0002bae0: 6d65 290a 0a20 2020 2069 6620 6465 706c  me)..    if depl
+0002baf0: 6f79 6d65 6e74 2e69 735f 6769 745f 7265  oyment.is_git_re
+0002bb00: 6c65 6173 653a 0a20 2020 2020 2020 2064  lease:.        d
+0002bb10: 6570 6c6f 796d 656e 742e 6465 706c 6f79  eployment.deploy
+0002bb20: 696e 675f 6472 795f 7275 6e28 290a 2020  ing_dry_run().  
+0002bb30: 2020 2020 2020 6177 6169 7420 7075 7368        await push
+0002bb40: 5f66 696c 6573 2864 6570 656e 6465 6e63  _files(dependenc
+0002bb50: 6965 735f 6772 6170 682c 2064 7279 5f72  ies_graph, dry_r
+0002bb60: 756e 3d54 7275 652c 2063 6865 636b 5f62  un=True, check_b
+0002bb70: 6163 6b66 696c 6c5f 7265 7175 6972 6564  ackfill_required
+0002bb80: 3d63 6865 636b 5f62 6163 6b66 696c 6c5f  =check_backfill_
+0002bb90: 7265 7175 6972 6564 290a 0a20 2020 2020  required)..     
+0002bba0: 2020 2061 7761 6974 2064 6570 6c6f 796d     await deploym
+0002bbb0: 656e 742e 6465 6c65 7465 5f72 6573 6f75  ent.delete_resou
+0002bbc0: 7263 6573 2864 656c 6574 6564 2c20 7069  rces(deleted, pi
+0002bbd0: 7065 732c 2064 7279 5f72 756e 3d54 7275  pes, dry_run=Tru
+0002bbe0: 6529 0a20 2020 2020 2020 2069 6620 6e6f  e).        if no
+0002bbf0: 7420 6465 706c 6f79 6d65 6e74 2e64 7279  t deployment.dry
+0002bc00: 5f72 756e 3a0a 2020 2020 2020 2020 2020  _run:.          
+0002bc10: 2020 6465 706c 6f79 6d65 6e74 2e64 6570    deployment.dep
+0002bc20: 6c6f 7969 6e67 2829 0a20 2020 2020 2020  loying().       
+0002bc30: 2020 2020 2061 7761 6974 2070 7573 685f       await push_
+0002bc40: 6669 6c65 7328 6465 7065 6e64 656e 6369  files(dependenci
+0002bc50: 6573 5f67 7261 7068 2c20 6472 795f 7275  es_graph, dry_ru
+0002bc60: 6e29 0a20 2020 2020 2020 2020 2020 2061  n).            a
+0002bc70: 7761 6974 2064 6570 6c6f 796d 656e 742e  wait deployment.
+0002bc80: 6465 6c65 7465 5f72 6573 6f75 7263 6573  delete_resources
+0002bc90: 2864 656c 6574 6564 2c20 7069 7065 7329  (deleted, pipes)
+0002bca0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0002bcb0: 2020 2061 7761 6974 2070 7573 685f 6669     await push_fi
+0002bcc0: 6c65 7328 6465 7065 6e64 656e 6369 6573  les(dependencies
+0002bcd0: 5f67 7261 7068 2c20 6472 795f 7275 6e29  _graph, dry_run)
+0002bce0: 0a0a 2020 2020 6966 206e 6f74 2064 7279  ..    if not dry
+0002bcf0: 5f72 756e 2061 6e64 206e 6f74 2072 756e  _run and not run
+0002bd00: 5f74 6573 7473 3a0a 2020 2020 2020 2020  _tests:.        
+0002bd10: 6966 2075 706c 6f61 645f 6669 7874 7572  if upload_fixtur
+0002bd20: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0002bd30: 636c 6963 6b2e 6563 686f 2846 6565 6462  click.echo(Feedb
+0002bd40: 6163 6b4d 616e 6167 6572 2e69 6e66 6f5f  ackManager.info_
+0002bd50: 7075 7368 696e 675f 6669 7874 7572 6573  pushing_fixtures
+0002bd60: 2829 290a 0a20 2020 2020 2020 2020 2020  ())..           
+0002bd70: 2023 2057 6520 6e65 6564 2074 6f20 7570   # We need to up
+0002bd80: 6c6f 6164 2074 6865 2066 6978 7475 7265  load the fixture
+0002bd90: 7320 6576 656e 2069 6620 7468 6572 6520  s even if there 
+0002bda0: 6973 206e 6f20 6368 616e 6765 0a20 2020  is no change.   
+0002bdb0: 2020 2020 2020 2020 2069 6620 6973 5f62           if is_b
+0002bdc0: 7261 6e63 683a 0a20 2020 2020 2020 2020  ranch:.         
+0002bdd0: 2020 2020 2020 2066 696c 656e 616d 6573         filenames
+0002bde0: 203d 2067 6574 5f70 726f 6a65 6374 5f66   = get_project_f
+0002bdf0: 696c 656e 616d 6573 2866 6f6c 6465 722c  ilenames(folder,
+0002be00: 2077 6974 685f 7665 6e64 6f72 3d54 7275   with_vendor=Tru
+0002be10: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0002be20: 2020 2064 6570 656e 6465 6e63 6965 735f     dependencies_
+0002be30: 6772 6170 6820 3d20 6177 6169 7420 6275  graph = await bu
+0002be40: 696c 645f 6772 6170 6828 0a20 2020 2020  ild_graph(.     
+0002be50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002be60: 696c 656e 616d 6573 2c0a 2020 2020 2020  ilenames,.      
+0002be70: 2020 2020 2020 2020 2020 2020 2020 7462                tb
+0002be80: 5f63 6c69 656e 742c 0a20 2020 2020 2020  _client,.       
+0002be90: 2020 2020 2020 2020 2020 2020 2064 6972               dir
+0002bea0: 5f70 6174 683d 666f 6c64 6572 2c0a 2020  _path=folder,.  
+0002beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bec0: 2020 7265 736f 7572 6365 5f76 6572 7369    resource_versi
+0002bed0: 6f6e 733d 6c61 7465 7374 5f64 6174 6173  ons=latest_datas
+0002bee0: 6f75 7263 655f 7665 7273 696f 6e73 2c0a  ource_versions,.
+0002bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bf00: 2020 2020 776f 726b 7370 6163 655f 6d61      workspace_ma
+0002bf10: 703d 776f 726b 7370 6163 655f 6d61 702c  p=workspace_map,
+0002bf20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bf30: 2020 2020 2070 726f 6365 7373 5f64 6570       process_dep
+0002bf40: 656e 6465 6e63 6965 733d 7075 7368 5f64  endencies=push_d
+0002bf50: 6570 732c 0a20 2020 2020 2020 2020 2020  eps,.           
+0002bf60: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+0002bf70: 3d76 6572 626f 7365 2c0a 2020 2020 2020  =verbose,.      
+0002bf80: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+0002bf90: 726b 7370 6163 655f 6c69 625f 7061 7468  rkspace_lib_path
+0002bfa0: 733d 776f 726b 7370 6163 655f 6c69 625f  s=workspace_lib_
+0002bfb0: 7061 7468 732c 0a20 2020 2020 2020 2020  paths,.         
+0002bfc0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+0002bfd0: 6e74 5f77 733d 6375 7272 656e 745f 7773  nt_ws=current_ws
+0002bfe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002bff0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0002c000: 2070 726f 6365 7373 6564 203d 2073 6574   processed = set
+0002c010: 2829 0a20 2020 2020 2020 2020 2020 2066  ().            f
+0002c020: 6f72 2067 726f 7570 2069 6e20 746f 706f  or group in topo
+0002c030: 736f 7274 2864 6570 656e 6465 6e63 6965  sort(dependencie
+0002c040: 735f 6772 6170 682e 6465 705f 6d61 7029  s_graph.dep_map)
+0002c050: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002c060: 2020 666f 7220 6620 696e 2067 726f 7570    for f in group
+0002c070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002c080: 2020 2020 2020 6e61 6d65 203d 206f 732e        name = os.
+0002c090: 7061 7468 2e62 6173 656e 616d 6528 6629  path.basename(f)
+0002c0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c0b0: 2020 2020 2069 6620 6e61 6d65 206e 6f74       if name not
+0002c0c0: 2069 6e20 7072 6f63 6573 7365 643a 0a20   in processed:. 
+0002c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c0e0: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
+0002c0f0: 6e20 6465 7065 6e64 656e 6369 6573 5f67  n dependencies_g
+0002c100: 7261 7068 2e74 6f5f 7275 6e3a 0a20 2020  raph.to_run:.   
 0002c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c120: 2061 7761 6974 2063 6865 636b 5f66 6978   await check_fix
-0002c130: 7475 7265 735f 6461 7461 280a 2020 2020  tures_data(.    
-0002c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c150: 2020 2020 2020 2020 2020 2020 7462 5f63              tb_c
-0002c160: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
+0002c120: 2020 2020 2020 2020 2061 7761 6974 2063           await c
+0002c130: 6865 636b 5f66 6978 7475 7265 735f 6461  heck_fixtures_da
+0002c140: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
+0002c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c160: 2020 2020 7462 5f63 6c69 656e 742c 0a20      tb_client,. 
 0002c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c180: 2020 2020 2020 2064 6570 656e 6465 6e63         dependenc
-0002c190: 6965 735f 6772 6170 682e 746f 5f72 756e  ies_graph.to_run
-0002c1a0: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
+0002c180: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0002c190: 6570 656e 6465 6e63 6965 735f 6772 6170  ependencies_grap
+0002c1a0: 682e 746f 5f72 756e 5b6e 616d 655d 2c0a  h.to_run[name],.
 0002c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c1c0: 2020 2020 2020 2020 6465 6275 672c 0a20          debug,. 
-0002c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c1e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0002c1f0: 6f6c 6465 722c 0a20 2020 2020 2020 2020  older,.         
+0002c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c1d0: 6465 6275 672c 0a20 2020 2020 2020 2020  debug,.         
+0002c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c1f0: 2020 2020 2020 2066 6f6c 6465 722c 0a20         folder,. 
 0002c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c210: 2020 2020 2020 2066 6f72 6365 2c0a 2020         force,.  
-0002c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c230: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-0002c240: 6465 3d22 6170 7065 6e64 2220 6966 2069  de="append" if i
-0002c250: 735f 6272 616e 6368 2065 6c73 6520 2272  s_branch else "r
-0002c260: 6570 6c61 6365 222c 0a20 2020 2020 2020  eplace",.       
-0002c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c280: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0002c210: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002c220: 6f72 6365 2c0a 2020 2020 2020 2020 2020  orce,.          
+0002c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c240: 2020 2020 2020 6d6f 6465 3d22 6170 7065        mode="appe
+0002c250: 6e64 2220 6966 2069 735f 6272 616e 6368  nd" if is_branch
+0002c260: 2065 6c73 6520 2272 6570 6c61 6365 222c   else "replace",
+0002c270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c280: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
 0002c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c2a0: 2020 2070 726f 6365 7373 6564 2e61 6464     processed.add
-0002c2b0: 286e 616d 6529 0a20 2020 2020 2020 2020  (name).         
-0002c2c0: 2020 2066 6f72 2066 2069 6e20 6465 7065     for f in depe
-0002c2d0: 6e64 656e 6369 6573 5f67 7261 7068 2e74  ndencies_graph.t
-0002c2e0: 6f5f 7275 6e3a 0a20 2020 2020 2020 2020  o_run:.         
-0002c2f0: 2020 2020 2020 2069 6620 6620 6e6f 7420         if f not 
-0002c300: 696e 2070 726f 6365 7373 6564 3a0a 2020  in processed:.  
-0002c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c320: 2020 6177 6169 7420 6368 6563 6b5f 6669    await check_fi
-0002c330: 7874 7572 6573 5f64 6174 6128 0a20 2020  xtures_data(.   
-0002c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c350: 2020 2020 2074 625f 636c 6965 6e74 2c0a       tb_client,.
-0002c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c370: 2020 2020 2020 2020 6465 7065 6e64 656e          dependen
-0002c380: 6369 6573 5f67 7261 7068 2e74 6f5f 7275  cies_graph.to_ru
-0002c390: 6e5b 665d 2c0a 2020 2020 2020 2020 2020  n[f],.          
-0002c3a0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0002c3b0: 6275 672c 0a20 2020 2020 2020 2020 2020  bug,.           
-0002c3c0: 2020 2020 2020 2020 2020 2020 2066 6f6c               fol
-0002c3d0: 6465 722c 0a20 2020 2020 2020 2020 2020  der,.           
-0002c3e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0002c3f0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
-0002c400: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-0002c410: 3d22 6170 7065 6e64 2220 6966 2069 735f  ="append" if is_
-0002c420: 6272 616e 6368 2065 6c73 6520 2272 6570  branch else "rep
-0002c430: 6c61 6365 222c 0a20 2020 2020 2020 2020  lace",.         
-0002c440: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002c450: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0002c460: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-0002c470: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002c480: 2020 2063 6c69 636b 2e65 6368 6f28 4665     click.echo(Fe
-0002c490: 6564 6261 636b 4d61 6e61 6765 722e 696e  edbackManager.in
-0002c4a0: 666f 5f6e 6f74 5f70 7573 6869 6e67 5f66  fo_not_pushing_f
-0002c4b0: 6978 7475 7265 7328 2929 0a0a 2020 2020  ixtures())..    
-0002c4c0: 6177 6169 7420 6465 706c 6f79 6d65 6e74  await deployment
-0002c4d0: 2e75 7064 6174 655f 7265 6c65 6173 6528  .update_release(
-0002c4e0: 6861 735f 7365 6d76 6572 3d68 6173 5f73  has_semver=has_s
-0002c4f0: 656d 7665 722c 2072 656c 6561 7365 5f63  emver, release_c
-0002c500: 7265 6174 6564 3d72 656c 6561 7365 5f63  reated=release_c
-0002c510: 7265 6174 6564 290a 0a20 2020 2072 6574  reated)..    ret
-0002c520: 7572 6e20 6465 7065 6e64 656e 6369 6573  urn dependencies
-0002c530: 5f67 7261 7068 2e74 6f5f 7275 6e0a 0a0a  _graph.to_run...
-0002c540: 6173 796e 6320 6465 6620 6368 6563 6b5f  async def check_
-0002c550: 6669 7874 7572 6573 5f64 6174 6128 0a20  fixtures_data(. 
-0002c560: 2020 2063 6c69 656e 743a 2054 696e 7942     client: TinyB
-0002c570: 2c20 7265 736f 7572 6365 3a20 4469 6374  , resource: Dict
-0002c580: 5b73 7472 2c20 416e 795d 2c20 6465 6275  [str, Any], debu
-0002c590: 673a 2062 6f6f 6c2c 2066 6f6c 6465 723a  g: bool, folder:
-0002c5a0: 2073 7472 203d 2022 222c 2066 6f72 6365   str = "", force
-0002c5b0: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-0002c5c0: 6d6f 6465 3a20 7374 7220 3d20 2272 6570  mode: str = "rep
-0002c5d0: 6c61 6365 220a 293a 0a20 2020 2069 6620  lace".):.    if 
-0002c5e0: 6465 6275 673a 0a20 2020 2020 2020 2063  debug:.        c
-0002c5f0: 6c69 636b 2e65 6368 6f28 4665 6564 6261  lick.echo(Feedba
-0002c600: 636b 4d61 6e61 6765 722e 696e 666f 5f63  ckManager.info_c
-0002c610: 6865 636b 696e 675f 6669 6c65 2866 696c  hecking_file(fil
-0002c620: 653d 7070 2e70 666f 726d 6174 2872 6573  e=pp.pformat(res
-0002c630: 6f75 7263 6529 2929 0a20 2020 2069 6620  ource))).    if 
-0002c640: 7265 736f 7572 6365 5b22 7265 736f 7572  resource["resour
-0002c650: 6365 225d 2069 6e20 5b22 7069 7065 7322  ce"] in ["pipes"
-0002c660: 2c20 2274 6f6b 656e 7322 5d3a 0a20 2020  , "tokens"]:.   
-0002c670: 2020 2020 2070 6173 730a 2020 2020 656c       pass.    el
-0002c680: 6966 2072 6573 6f75 7263 655b 2272 6573  if resource["res
-0002c690: 6f75 7263 6522 5d20 3d3d 2022 6461 7461  ource"] == "data
-0002c6a0: 736f 7572 6365 7322 3a0a 2020 2020 2020  sources":.      
-0002c6b0: 2020 6461 7461 736f 7572 6365 5f6e 616d    datasource_nam
-0002c6c0: 6520 3d20 7265 736f 7572 6365 5b22 7061  e = resource["pa
-0002c6d0: 7261 6d73 225d 5b22 6e61 6d65 225d 0a20  rams"]["name"]. 
-0002c6e0: 2020 2020 2020 206e 616d 6520 3d20 6f73         name = os
-0002c6f0: 2e70 6174 682e 6261 7365 6e61 6d65 2872  .path.basename(r
-0002c700: 6573 6f75 7263 655b 2266 696c 656e 616d  esource["filenam
-0002c710: 6522 5d29 2e72 7370 6c69 7428 222e 222c  e"]).rsplit(".",
-0002c720: 2031 295b 305d 0a20 2020 2020 2020 2066   1)[0].        f
-0002c730: 6978 7475 7265 5f70 6174 6820 3d20 5061  ixture_path = Pa
-0002c740: 7468 2866 6f6c 6465 7229 202f 2022 6669  th(folder) / "fi
-0002c750: 7874 7572 6573 2220 2f20 6622 7b6e 616d  xtures" / f"{nam
-0002c760: 657d 2e63 7376 220a 0a20 2020 2020 2020  e}.csv"..       
-0002c770: 2069 6620 6e6f 7420 6669 7874 7572 655f   if not fixture_
-0002c780: 7061 7468 2e65 7869 7374 7328 293a 0a20  path.exists():. 
-0002c790: 2020 2020 2020 2020 2020 2066 6978 7475             fixtu
-0002c7a0: 7265 5f70 6174 6820 3d20 5061 7468 2866  re_path = Path(f
-0002c7b0: 6f6c 6465 7229 202f 2022 6461 7461 736f  older) / "dataso
-0002c7c0: 7572 6365 7322 202f 2022 6669 7874 7572  urces" / "fixtur
-0002c7d0: 6573 2220 2f20 6622 7b6e 616d 657d 2e63  es" / f"{name}.c
-0002c7e0: 7376 220a 2020 2020 2020 2020 6966 206e  sv".        if n
-0002c7f0: 6f74 2066 6978 7475 7265 5f70 6174 682e  ot fixture_path.
-0002c800: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-0002c810: 2020 2020 2020 6669 7874 7572 655f 7061        fixture_pa
-0002c820: 7468 203d 2050 6174 6828 666f 6c64 6572  th = Path(folder
-0002c830: 2920 2f20 2264 6174 6173 6f75 7263 6573  ) / "datasources
-0002c840: 2220 2f20 2266 6978 7475 7265 7322 202f  " / "fixtures" /
-0002c850: 2066 227b 6e61 6d65 7d2e 6e64 6a73 6f6e   f"{name}.ndjson
-0002c860: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-0002c870: 2066 6978 7475 7265 5f70 6174 682e 6578   fixture_path.ex
-0002c880: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
-0002c890: 2020 2020 6669 7874 7572 655f 7061 7468      fixture_path
-0002c8a0: 203d 2050 6174 6828 666f 6c64 6572 2920   = Path(folder) 
-0002c8b0: 2f20 2264 6174 6173 6f75 7263 6573 2220  / "datasources" 
-0002c8c0: 2f20 2266 6978 7475 7265 7322 202f 2066  / "fixtures" / f
-0002c8d0: 227b 6e61 6d65 7d2e 7061 7271 7565 7422  "{name}.parquet"
-0002c8e0: 0a20 2020 2020 2020 2069 6620 6669 7874  .        if fixt
-0002c8f0: 7572 655f 7061 7468 2e65 7869 7374 7328  ure_path.exists(
-0002c900: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-0002c910: 204c 6574 2773 2076 616c 6964 6174 6520   Let's validate 
-0002c920: 6f6e 6c79 2077 6865 6e20 7768 656e 2077  only when when w
-0002c930: 6520 6172 6520 676f 696e 6720 746f 2072  e are going to r
-0002c940: 6570 6c61 6365 2074 6865 2061 6374 7561  eplace the actua
-0002c950: 6c20 6461 7461 0a20 2020 2020 2020 2020  l data.         
-0002c960: 2020 2072 6573 756c 7420 3d20 6177 6169     result = awai
-0002c970: 7420 636c 6965 6e74 2e71 7565 7279 2873  t client.query(s
-0002c980: 716c 3d66 2253 454c 4543 5420 636f 756e  ql=f"SELECT coun
-0002c990: 7428 2920 6173 2063 2046 524f 4d20 7b64  t() as c FROM {d
-0002c9a0: 6174 6173 6f75 7263 655f 6e61 6d65 7d20  atasource_name} 
-0002c9b0: 464f 524d 4154 204a 534f 4e22 290a 2020  FORMAT JSON").  
-0002c9c0: 2020 2020 2020 2020 2020 636f 756e 7420            count 
-0002c9d0: 3d20 7265 7375 6c74 5b22 6461 7461 225d  = result["data"]
-0002c9e0: 5b30 5d5b 2263 225d 0a0a 2020 2020 2020  [0]["c"]..      
-0002c9f0: 2020 2020 2020 6966 2063 6f75 6e74 203e        if count >
-0002ca00: 2030 2061 6e64 206e 6f74 2066 6f72 6365   0 and not force
-0002ca10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002ca20: 2020 7261 6973 6520 636c 6963 6b2e 436c    raise click.Cl
-0002ca30: 6963 6b45 7863 6570 7469 6f6e 280a 2020  ickException(.  
-0002ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca50: 2020 4665 6564 6261 636b 4d61 6e61 6765    FeedbackManage
-0002ca60: 722e 6572 726f 725f 7075 7368 5f66 6978  r.error_push_fix
-0002ca70: 7475 7265 5f77 696c 6c5f 7265 706c 6163  ture_will_replac
-0002ca80: 655f 6461 7461 2864 6174 6173 6f75 7263  e_data(datasourc
-0002ca90: 653d 6461 7461 736f 7572 6365 5f6e 616d  e=datasource_nam
-0002caa0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0002cab0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0002cac0: 2020 636c 6963 6b2e 6563 686f 280a 2020    click.echo(.  
-0002cad0: 2020 2020 2020 2020 2020 2020 2020 4665                Fe
-0002cae0: 6564 6261 636b 4d61 6e61 6765 722e 696e  edbackManager.in
-0002caf0: 666f 5f63 6865 636b 696e 675f 6669 6c65  fo_checking_file
-0002cb00: 5f73 697a 6528 0a20 2020 2020 2020 2020  _size(.         
-0002cb10: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-0002cb20: 616d 653d 7265 736f 7572 6365 5b22 6669  ame=resource["fi
-0002cb30: 6c65 6e61 6d65 225d 2c20 7369 7a65 3d73  lename"], size=s
-0002cb40: 697a 656f 665f 666d 7428 6f73 2e73 7461  izeof_fmt(os.sta
-0002cb50: 7428 6669 7874 7572 655f 7061 7468 292e  t(fixture_path).
-0002cb60: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
-0002cb70: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0002cb80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002cb90: 2020 2020 2073 7973 2e73 7464 6f75 742e       sys.stdout.
-0002cba0: 666c 7573 6828 290a 2020 2020 2020 2020  flush().        
-0002cbb0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0002cbc0: 2020 2020 2020 2020 2061 7761 6974 2063           await c
-0002cbd0: 6c69 656e 742e 6461 7461 736f 7572 6365  lient.datasource
-0002cbe0: 5f61 7070 656e 645f 6461 7461 280a 2020  _append_data(.  
-0002cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cc00: 2020 6461 7461 736f 7572 6365 5f6e 616d    datasource_nam
-0002cc10: 653d 7265 736f 7572 6365 5b22 7061 7261  e=resource["para
-0002cc20: 6d73 225d 5b22 6e61 6d65 225d 2c0a 2020  ms"]["name"],.  
-0002cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cc40: 2020 6669 6c65 3d66 6978 7475 7265 5f70    file=fixture_p
-0002cc50: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0002cc60: 2020 2020 2020 2020 206d 6f64 653d 6d6f           mode=mo
-0002cc70: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-0002cc80: 2020 2020 2020 2020 666f 726d 6174 3d66          format=f
-0002cc90: 6978 7475 7265 5f70 6174 682e 7375 6666  ixture_path.suff
-0002cca0: 6978 5b31 3a5d 2c0a 2020 2020 2020 2020  ix[1:],.        
-0002ccb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0002ccc0: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-0002ccd0: 6563 686f 2846 6565 6462 6163 6b4d 616e  echo(FeedbackMan
-0002cce0: 6167 6572 2e73 7563 6365 7373 5f70 726f  ager.success_pro
-0002ccf0: 6365 7373 696e 675f 6461 7461 2829 290a  cessing_data()).
-0002cd00: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0002cd10: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0002cd20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002cd30: 2020 2072 6169 7365 2063 6c69 636b 2e43     raise click.C
-0002cd40: 6c69 636b 4578 6365 7074 696f 6e28 4665  lickException(Fe
-0002cd50: 6564 6261 636b 4d61 6e61 6765 722e 6572  edbackManager.er
-0002cd60: 726f 725f 7072 6f63 6573 7369 6e67 5f62  ror_processing_b
-0002cd70: 6c6f 636b 7328 6572 726f 723d 6529 290a  locks(error=e)).
-0002cd80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0002cd90: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-0002cda0: 2e65 6368 6f28 4665 6564 6261 636b 4d61  .echo(FeedbackMa
-0002cdb0: 6e61 6765 722e 7761 726e 696e 675f 6669  nager.warning_fi
-0002cdc0: 7874 7572 655f 6e6f 745f 666f 756e 6428  xture_not_found(
-0002cdd0: 6461 7461 736f 7572 6365 5f6e 616d 653d  datasource_name=
-0002cde0: 6e61 6d65 2929 0a20 2020 2065 6c73 653a  name)).    else:
-0002cdf0: 0a20 2020 2020 2020 2072 6169 7365 2063  .        raise c
-0002ce00: 6c69 636b 2e43 6c69 636b 4578 6365 7074  lick.ClickExcept
-0002ce10: 696f 6e28 4665 6564 6261 636b 4d61 6e61  ion(FeedbackMana
-0002ce20: 6765 722e 6572 726f 725f 756e 6b6e 6f77  ger.error_unknow
-0002ce30: 6e5f 7265 736f 7572 6365 2872 6573 6f75  n_resource(resou
-0002ce40: 7263 653d 7265 736f 7572 6365 5b22 7265  rce=resource["re
-0002ce50: 736f 7572 6365 225d 2929 0a0a 0a44 4154  source"]))...DAT
-0002ce60: 4146 494c 455f 4e45 575f 4c49 4e45 203d  AFILE_NEW_LINE =
-0002ce70: 2022 5c6e 220a 4441 5441 4649 4c45 5f49   "\n".DATAFILE_I
-0002ce80: 4e44 454e 5420 3d20 2220 2220 2a20 340a  NDENT = " " * 4.
-0002ce90: 0a0a 6465 6620 666f 726d 6174 5f73 6368  ..def format_sch
-0002cea0: 656d 6128 6669 6c65 5f70 6172 7473 3a20  ema(file_parts: 
-0002ceb0: 4c69 7374 5b73 7472 5d2c 206e 6f64 653a  List[str], node:
-0002cec0: 2044 6963 745b 7374 722c 2041 6e79 5d29   Dict[str, Any])
-0002ced0: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
-0002cee0: 2020 2069 6620 2273 6368 656d 6122 2069     if "schema" i
-0002cef0: 6e20 6e6f 6465 2061 6e64 206e 6f64 655b  n node and node[
-0002cf00: 2273 6368 656d 6122 5d3a 0a20 2020 2020  "schema"]:.     
-0002cf10: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
-0002cf20: 7065 6e64 2822 5343 4845 4d41 203e 2229  pend("SCHEMA >")
-0002cf30: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
-0002cf40: 7274 732e 6170 7065 6e64 2844 4154 4146  rts.append(DATAF
-0002cf50: 494c 455f 4e45 575f 4c49 4e45 290a 2020  ILE_NEW_LINE).  
-0002cf60: 2020 2020 2020 636f 6c75 6d6e 7320 3d20        columns = 
-0002cf70: 7363 6865 6d61 5f74 6f5f 7371 6c5f 636f  schema_to_sql_co
-0002cf80: 6c75 6d6e 7328 6e6f 6465 5b22 636f 6c75  lumns(node["colu
-0002cf90: 6d6e 7322 5d29 0a20 2020 2020 2020 2066  mns"]).        f
-0002cfa0: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002cfb0: 2866 222c 7b44 4154 4146 494c 455f 4e45  (f",{DATAFILE_NE
-0002cfc0: 575f 4c49 4e45 7d22 2e6a 6f69 6e28 6d61  W_LINE}".join(ma
-0002cfd0: 7028 6c61 6d62 6461 2078 3a20 6622 2020  p(lambda x: f"  
-0002cfe0: 2020 7b78 7d22 2c20 636f 6c75 6d6e 7329    {x}", columns)
-0002cff0: 2929 0a20 2020 2020 2020 2066 696c 655f  )).        file_
-0002d000: 7061 7274 732e 6170 7065 6e64 2844 4154  parts.append(DAT
-0002d010: 4146 494c 455f 4e45 575f 4c49 4e45 290a  AFILE_NEW_LINE).
-0002d020: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
-0002d030: 7473 2e61 7070 656e 6428 4441 5441 4649  ts.append(DATAFI
-0002d040: 4c45 5f4e 4557 5f4c 494e 4529 0a0a 2020  LE_NEW_LINE)..  
-0002d050: 2020 7265 7475 726e 2066 696c 655f 7061    return file_pa
-0002d060: 7274 730a 0a0a 6465 6620 666f 726d 6174  rts...def format
-0002d070: 5f69 6e64 6963 6573 2866 696c 655f 7061  _indices(file_pa
-0002d080: 7274 733a 204c 6973 745b 7374 725d 2c20  rts: List[str], 
-0002d090: 6e6f 6465 3a20 4469 6374 5b73 7472 2c20  node: Dict[str, 
-0002d0a0: 416e 795d 2920 2d3e 204c 6973 745b 7374  Any]) -> List[st
-0002d0b0: 725d 3a0a 2020 2020 6966 2022 696e 6465  r]:.    if "inde
-0002d0c0: 7865 7322 2069 6e20 6e6f 6465 2061 6e64  xes" in node and
-0002d0d0: 206e 6f64 655b 2269 6e64 6578 6573 225d   node["indexes"]
-0002d0e0: 3a0a 2020 2020 2020 2020 696e 6465 7865  :.        indexe
-0002d0f0: 7320 3d20 6e6f 6465 5b22 696e 6465 7865  s = node["indexe
-0002d100: 7322 5d0a 2020 2020 2020 2020 6669 6c65  s"].        file
-0002d110: 5f70 6172 7473 2e61 7070 656e 6428 2249  _parts.append("I
-0002d120: 4e44 4558 4553 203e 2229 0a20 2020 2020  NDEXES >").     
-0002d130: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
-0002d140: 7065 6e64 2844 4154 4146 494c 455f 4e45  pend(DATAFILE_NE
-0002d150: 575f 4c49 4e45 290a 2020 2020 2020 2020  W_LINE).        
-0002d160: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
-0002d170: 6428 6622 7b44 4154 4146 494c 455f 4e45  d(f"{DATAFILE_NE
-0002d180: 575f 4c49 4e45 7d22 2e6a 6f69 6e28 6d61  W_LINE}".join(ma
-0002d190: 7028 6c61 6d62 6461 2069 6e64 6578 3a20  p(lambda index: 
-0002d1a0: 6622 2020 2020 7b69 6e64 6578 2e74 6f5f  f"    {index.to_
-0002d1b0: 6461 7461 6669 6c65 2829 7d22 2c20 696e  datafile()}", in
-0002d1c0: 6465 7865 7329 2929 0a20 2020 2020 2020  dexes))).       
-0002d1d0: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
-0002d1e0: 6e64 2844 4154 4146 494c 455f 4e45 575f  nd(DATAFILE_NEW_
-0002d1f0: 4c49 4e45 290a 2020 2020 2020 2020 6669  LINE).        fi
-0002d200: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
-0002d210: 4441 5441 4649 4c45 5f4e 4557 5f4c 494e  DATAFILE_NEW_LIN
-0002d220: 4529 0a0a 2020 2020 7265 7475 726e 2066  E)..    return f
-0002d230: 696c 655f 7061 7274 730a 0a0a 6465 6620  ile_parts...def 
-0002d240: 666f 726d 6174 5f64 6174 615f 636f 6e6e  format_data_conn
-0002d250: 6563 746f 7228 6669 6c65 5f70 6172 7473  ector(file_parts
-0002d260: 3a20 4c69 7374 5b73 7472 5d2c 206e 6f64  : List[str], nod
-0002d270: 653a 2044 6963 745b 7374 722c 2041 6e79  e: Dict[str, Any
-0002d280: 5d29 202d 3e20 4c69 7374 5b73 7472 5d3a  ]) -> List[str]:
-0002d290: 0a20 2020 206c 6c20 3d20 6c65 6e28 6669  .    ll = len(fi
-0002d2a0: 6c65 5f70 6172 7473 290a 2020 2020 7175  le_parts).    qu
-0002d2b0: 6f74 6573 203d 2022 2727 220a 2020 2020  otes = "''".    
-0002d2c0: 5b66 696c 655f 7061 7274 732e 6170 7065  [file_parts.appe
-0002d2d0: 6e64 2866 227b 6b2e 7570 7065 7228 297d  nd(f"{k.upper()}
-0002d2e0: 207b 7620 6f72 2071 756f 7465 737d 7b44   {v or quotes}{D
-0002d2f0: 4154 4146 494c 455f 4e45 575f 4c49 4e45  ATAFILE_NEW_LINE
-0002d300: 7d22 2920 666f 7220 6b2c 2076 2069 6e20  }") for k, v in 
-0002d310: 6e6f 6465 2e69 7465 6d73 2829 2069 6620  node.items() if 
-0002d320: 226b 6166 6b61 2220 696e 206b 5d20 2023  "kafka" in k]  #
-0002d330: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-0002d340: 2020 6966 206c 6c20 3c20 6c65 6e28 6669    if ll < len(fi
-0002d350: 6c65 5f70 6172 7473 293a 0a20 2020 2020  le_parts):.     
-0002d360: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
-0002d370: 7065 6e64 2844 4154 4146 494c 455f 4e45  pend(DATAFILE_NE
-0002d380: 575f 4c49 4e45 290a 2020 2020 7265 7475  W_LINE).    retu
-0002d390: 726e 2066 696c 655f 7061 7274 730a 0a0a  rn file_parts...
-0002d3a0: 6465 6620 666f 726d 6174 5f69 6d70 6f72  def format_impor
-0002d3b0: 745f 7365 7474 696e 6773 2866 696c 655f  t_settings(file_
-0002d3c0: 7061 7274 733a 204c 6973 745b 7374 725d  parts: List[str]
-0002d3d0: 2c20 6e6f 6465 3a20 4469 6374 5b73 7472  , node: Dict[str
-0002d3e0: 2c20 416e 795d 2920 2d3e 204c 6973 745b  , Any]) -> List[
-0002d3f0: 7374 725d 3a0a 2020 2020 6c6c 203d 206c  str]:.    ll = l
-0002d400: 656e 2866 696c 655f 7061 7274 7329 0a20  en(file_parts). 
-0002d410: 2020 205b 6669 6c65 5f70 6172 7473 2e61     [file_parts.a
-0002d420: 7070 656e 6428 6622 7b6b 2e75 7070 6572  ppend(f"{k.upper
-0002d430: 2829 7d20 7b76 7d7b 4441 5441 4649 4c45  ()} {v}{DATAFILE
-0002d440: 5f4e 4557 5f4c 494e 457d 2229 2066 6f72  _NEW_LINE}") for
-0002d450: 206b 2c20 7620 696e 206e 6f64 652e 6974   k, v in node.it
-0002d460: 656d 7328 2920 6966 2022 696d 706f 7274  ems() if "import
-0002d470: 5f22 2069 6e20 6b5d 2020 2320 7479 7065  _" in k]  # type
-0002d480: 3a20 6967 6e6f 7265 0a20 2020 2069 6620  : ignore.    if 
-0002d490: 6c6c 203c 206c 656e 2866 696c 655f 7061  ll < len(file_pa
-0002d4a0: 7274 7329 3a0a 2020 2020 2020 2020 6669  rts):.        fi
-0002d4b0: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
-0002d4c0: 4441 5441 4649 4c45 5f4e 4557 5f4c 494e  DATAFILE_NEW_LIN
-0002d4d0: 4529 0a20 2020 2072 6574 7572 6e20 6669  E).    return fi
-0002d4e0: 6c65 5f70 6172 7473 0a0a 0a64 6566 2066  le_parts...def f
-0002d4f0: 6f72 6d61 745f 696e 636c 7564 6528 6669  ormat_include(fi
-0002d500: 6c65 5f70 6172 7473 3a20 4c69 7374 5b73  le_parts: List[s
-0002d510: 7472 5d2c 2064 6f63 3a20 4461 7461 6669  tr], doc: Datafi
-0002d520: 6c65 2c20 756e 726f 6c6c 5f69 6e63 6c75  le, unroll_inclu
-0002d530: 6465 733a 2062 6f6f 6c20 3d20 4661 6c73  des: bool = Fals
-0002d540: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-0002d550: 0a20 2020 2069 6620 756e 726f 6c6c 5f69  .    if unroll_i
-0002d560: 6e63 6c75 6465 733a 0a20 2020 2020 2020  ncludes:.       
-0002d570: 2072 6574 7572 6e20 6669 6c65 5f70 6172   return file_par
-0002d580: 7473 0a0a 2020 2020 6173 7365 7274 2064  ts..    assert d
-0002d590: 6f63 2e72 6177 2069 7320 6e6f 7420 4e6f  oc.raw is not No
-0002d5a0: 6e65 0a0a 2020 2020 696e 636c 7564 6520  ne..    include 
-0002d5b0: 3d20 5b6c 696e 6520 666f 7220 6c69 6e65  = [line for line
-0002d5c0: 2069 6e20 646f 632e 7261 7720 6966 2022   in doc.raw if "
-0002d5d0: 494e 434c 5544 4522 2069 6e20 6c69 6e65  INCLUDE" in line
-0002d5e0: 2061 6e64 2022 2e69 6e63 6c22 2069 6e20   and ".incl" in 
-0002d5f0: 6c69 6e65 5d0a 2020 2020 6966 206c 656e  line].    if len
-0002d600: 2869 6e63 6c75 6465 293a 0a20 2020 2020  (include):.     
-0002d610: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
-0002d620: 7065 6e64 2869 6e63 6c75 6465 5b30 5d29  pend(include[0])
-0002d630: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
-0002d640: 7274 732e 6170 7065 6e64 2844 4154 4146  rts.append(DATAF
-0002d650: 494c 455f 4e45 575f 4c49 4e45 290a 2020  ILE_NEW_LINE).  
-0002d660: 2020 7265 7475 726e 2066 696c 655f 7061    return file_pa
-0002d670: 7274 730a 0a0a 6173 796e 6320 6465 6620  rts...async def 
-0002d680: 666f 726d 6174 5f64 6174 6173 6f75 7263  format_datasourc
-0002d690: 6528 0a20 2020 2066 696c 656e 616d 653a  e(.    filename:
-0002d6a0: 2073 7472 2c0a 2020 2020 756e 726f 6c6c   str,.    unroll
-0002d6b0: 5f69 6e63 6c75 6465 733a 2062 6f6f 6c20  _includes: bool 
-0002d6c0: 3d20 4661 6c73 652c 0a20 2020 2066 6f72  = False,.    for
-0002d6d0: 5f64 6966 663a 2062 6f6f 6c20 3d20 4661  _diff: bool = Fa
-0002d6e0: 6c73 652c 0a20 2020 2063 6c69 656e 743a  lse,.    client:
-0002d6f0: 204f 7074 696f 6e61 6c5b 5469 6e79 425d   Optional[TinyB]
-0002d700: 203d 204e 6f6e 652c 0a20 2020 2072 6570   = None,.    rep
-0002d710: 6c61 6365 5f69 6e63 6c75 6465 733a 2062  lace_includes: b
-0002d720: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0002d730: 2064 6174 6166 696c 653a 204f 7074 696f   datafile: Optio
-0002d740: 6e61 6c5b 4461 7461 6669 6c65 5d20 3d20  nal[Datafile] = 
-0002d750: 4e6f 6e65 2c0a 2020 2020 666f 725f 6465  None,.    for_de
-0002d760: 706c 6f79 5f64 6966 663a 2062 6f6f 6c20  ploy_diff: bool 
-0002d770: 3d20 4661 6c73 652c 0a20 2020 2073 6b69  = False,.    ski
-0002d780: 705f 6576 616c 3a20 626f 6f6c 203d 2046  p_eval: bool = F
-0002d790: 616c 7365 2c0a 2920 2d3e 2073 7472 3a0a  alse,.) -> str:.
-0002d7a0: 2020 2020 6966 2064 6174 6166 696c 653a      if datafile:
-0002d7b0: 0a20 2020 2020 2020 2064 6f63 203d 2064  .        doc = d
-0002d7c0: 6174 6166 696c 650a 2020 2020 656c 7365  atafile.    else
-0002d7d0: 3a0a 2020 2020 2020 2020 646f 6320 3d20  :.        doc = 
-0002d7e0: 7061 7273 655f 6461 7461 736f 7572 6365  parse_datasource
-0002d7f0: 2866 696c 656e 616d 652c 2072 6570 6c61  (filename, repla
-0002d800: 6365 5f69 6e63 6c75 6465 733d 7265 706c  ce_includes=repl
-0002d810: 6163 655f 696e 636c 7564 6573 2c20 736b  ace_includes, sk
-0002d820: 6970 5f65 7661 6c3d 736b 6970 5f65 7661  ip_eval=skip_eva
-0002d830: 6c29 0a0a 2020 2020 6669 6c65 5f70 6172  l)..    file_par
-0002d840: 7473 3a20 4c69 7374 5b73 7472 5d20 3d20  ts: List[str] = 
-0002d850: 5b5d 0a20 2020 2069 6620 666f 725f 6469  [].    if for_di
-0002d860: 6666 3a0a 2020 2020 2020 2020 6973 5f6b  ff:.        is_k
-0002d870: 6166 6b61 203d 2022 6b61 666b 615f 636f  afka = "kafka_co
-0002d880: 6e6e 6563 7469 6f6e 5f6e 616d 6522 2069  nnection_name" i
-0002d890: 6e20 646f 632e 6e6f 6465 735b 305d 0a20  n doc.nodes[0]. 
-0002d8a0: 2020 2020 2020 2069 6620 6973 5f6b 6166         if is_kaf
-0002d8b0: 6b61 3a0a 2020 2020 2020 2020 2020 2020  ka:.            
-0002d8c0: 6b61 666b 615f 6d65 7461 6461 7461 5f63  kafka_metadata_c
-0002d8d0: 6f6c 756d 6e73 203d 205b 0a20 2020 2020  olumns = [.     
-0002d8e0: 2020 2020 2020 2020 2020 2022 5f5f 7661             "__va
-0002d8f0: 6c75 6522 2c0a 2020 2020 2020 2020 2020  lue",.          
-0002d900: 2020 2020 2020 225f 5f68 6561 6465 7273        "__headers
-0002d910: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0002d920: 2020 2022 5f5f 746f 7069 6322 2c0a 2020     "__topic",.  
-0002d930: 2020 2020 2020 2020 2020 2020 2020 225f                "_
-0002d940: 5f70 6172 7469 7469 6f6e 222c 0a20 2020  _partition",.   
-0002d950: 2020 2020 2020 2020 2020 2020 2022 5f5f               "__
-0002d960: 6f66 6673 6574 222c 0a20 2020 2020 2020  offset",.       
-0002d970: 2020 2020 2020 2020 2022 5f5f 7469 6d65           "__time
-0002d980: 7374 616d 7022 2c0a 2020 2020 2020 2020  stamp",.        
-0002d990: 2020 2020 2020 2020 225f 5f6b 6579 222c          "__key",
-0002d9a0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-0002d9b0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0002d9c0: 6e73 203d 205b 6320 666f 7220 6320 696e  ns = [c for c in
-0002d9d0: 2064 6f63 2e6e 6f64 6573 5b30 5d5b 2263   doc.nodes[0]["c
-0002d9e0: 6f6c 756d 6e73 225d 2069 6620 635b 226e  olumns"] if c["n
-0002d9f0: 616d 6522 5d20 6e6f 7420 696e 206b 6166  ame"] not in kaf
-0002da00: 6b61 5f6d 6574 6164 6174 615f 636f 6c75  ka_metadata_colu
-0002da10: 6d6e 735d 0a20 2020 2020 2020 2020 2020  mns].           
-0002da20: 2064 6f63 2e6e 6f64 6573 5b30 5d2e 7570   doc.nodes[0].up
-0002da30: 6461 7465 280a 2020 2020 2020 2020 2020  date(.          
-0002da40: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0002da50: 2020 2020 2020 2020 2020 2020 2263 6f6c              "col
-0002da60: 756d 6e73 223a 2063 6f6c 756d 6e73 2c0a  umns": columns,.
-0002da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002da80: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
-0002da90: 2020 2020 2020 2020 666f 726d 6174 5f76          format_v
-0002daa0: 6572 7369 6f6e 2866 696c 655f 7061 7274  ersion(file_part
-0002dab0: 732c 2064 6f63 290a 2020 2020 2020 2020  s, doc).        
-0002dac0: 6966 2066 6f72 5f64 6570 6c6f 795f 6469  if for_deploy_di
-0002dad0: 6666 3a0a 2020 2020 2020 2020 2020 2020  ff:.            
-0002dae0: 666f 726d 6174 5f64 6573 6372 6970 7469  format_descripti
-0002daf0: 6f6e 2866 696c 655f 7061 7274 732c 2064  on(file_parts, d
-0002db00: 6f63 290a 2020 2020 2020 2020 666f 726d  oc).        form
-0002db10: 6174 5f74 6f6b 656e 7328 6669 6c65 5f70  at_tokens(file_p
-0002db20: 6172 7473 2c20 646f 6329 0a20 2020 2020  arts, doc).     
-0002db30: 2020 2066 6f72 6d61 745f 7363 6865 6d61     format_schema
-0002db40: 2866 696c 655f 7061 7274 732c 2064 6f63  (file_parts, doc
-0002db50: 2e6e 6f64 6573 5b30 5d29 0a20 2020 2020  .nodes[0]).     
-0002db60: 2020 2066 6f72 6d61 745f 696e 6469 6365     format_indice
-0002db70: 7328 6669 6c65 5f70 6172 7473 2c20 646f  s(file_parts, do
-0002db80: 632e 6e6f 6465 735b 305d 290a 2020 2020  c.nodes[0]).    
-0002db90: 2020 2020 6177 6169 7420 666f 726d 6174      await format
-0002dba0: 5f65 6e67 696e 6528 6669 6c65 5f70 6172  _engine(file_par
-0002dbb0: 7473 2c20 646f 632e 6e6f 6465 735b 305d  ts, doc.nodes[0]
-0002dbc0: 2c20 6f6e 6c79 5f74 746c 3d54 7275 6520  , only_ttl=True 
-0002dbd0: 6966 206e 6f74 2066 6f72 5f64 6570 6c6f  if not for_deplo
-0002dbe0: 795f 6469 6666 2065 6c73 6520 4661 6c73  y_diff else Fals
-0002dbf0: 652c 2063 6c69 656e 743d 636c 6965 6e74  e, client=client
-0002dc00: 290a 2020 2020 2020 2020 6966 2066 6f72  ).        if for
-0002dc10: 5f64 6570 6c6f 795f 6469 6666 3a0a 2020  _deploy_diff:.  
-0002dc20: 2020 2020 2020 2020 2020 666f 726d 6174            format
-0002dc30: 5f69 6d70 6f72 745f 7365 7474 696e 6773  _import_settings
-0002dc40: 2866 696c 655f 7061 7274 732c 2064 6f63  (file_parts, doc
-0002dc50: 2e6e 6f64 6573 5b30 5d29 0a20 2020 2020  .nodes[0]).     
-0002dc60: 2020 2066 6f72 6d61 745f 7368 6172 6564     format_shared
-0002dc70: 5f77 6974 6828 6669 6c65 5f70 6172 7473  _with(file_parts
-0002dc80: 2c20 646f 6329 0a0a 2020 2020 656c 7365  , doc)..    else
-0002dc90: 3a0a 2020 2020 2020 2020 666f 726d 6174  :.        format
-0002dca0: 5f73 6f75 7263 6573 2866 696c 655f 7061  _sources(file_pa
-0002dcb0: 7274 732c 2064 6f63 290a 2020 2020 2020  rts, doc).      
-0002dcc0: 2020 666f 726d 6174 5f6d 6169 6e74 6169    format_maintai
-0002dcd0: 6e65 7228 6669 6c65 5f70 6172 7473 2c20  ner(file_parts, 
-0002dce0: 646f 6329 0a20 2020 2020 2020 2066 6f72  doc).        for
-0002dcf0: 6d61 745f 7665 7273 696f 6e28 6669 6c65  mat_version(file
-0002dd00: 5f70 6172 7473 2c20 646f 6329 0a20 2020  _parts, doc).   
-0002dd10: 2020 2020 2066 6f72 6d61 745f 6465 7363       format_desc
-0002dd20: 7269 7074 696f 6e28 6669 6c65 5f70 6172  ription(file_par
-0002dd30: 7473 2c20 646f 6329 0a20 2020 2020 2020  ts, doc).       
-0002dd40: 2066 6f72 6d61 745f 746f 6b65 6e73 2866   format_tokens(f
-0002dd50: 696c 655f 7061 7274 732c 2064 6f63 290a  ile_parts, doc).
-0002dd60: 2020 2020 2020 2020 666f 726d 6174 5f73          format_s
-0002dd70: 6368 656d 6128 6669 6c65 5f70 6172 7473  chema(file_parts
-0002dd80: 2c20 646f 632e 6e6f 6465 735b 305d 290a  , doc.nodes[0]).
-0002dd90: 2020 2020 2020 2020 666f 726d 6174 5f69          format_i
-0002dda0: 6e64 6963 6573 2866 696c 655f 7061 7274  ndices(file_part
-0002ddb0: 732c 2064 6f63 2e6e 6f64 6573 5b30 5d29  s, doc.nodes[0])
-0002ddc0: 0a20 2020 2020 2020 2061 7761 6974 2066  .        await f
-0002ddd0: 6f72 6d61 745f 656e 6769 6e65 2866 696c  ormat_engine(fil
-0002dde0: 655f 7061 7274 732c 2064 6f63 2e6e 6f64  e_parts, doc.nod
-0002ddf0: 6573 5b30 5d29 0a20 2020 2020 2020 2066  es[0]).        f
-0002de00: 6f72 6d61 745f 696e 636c 7564 6528 6669  ormat_include(fi
-0002de10: 6c65 5f70 6172 7473 2c20 646f 632c 2075  le_parts, doc, u
-0002de20: 6e72 6f6c 6c5f 696e 636c 7564 6573 3d75  nroll_includes=u
-0002de30: 6e72 6f6c 6c5f 696e 636c 7564 6573 290a  nroll_includes).
-0002de40: 2020 2020 2020 2020 666f 726d 6174 5f64          format_d
-0002de50: 6174 615f 636f 6e6e 6563 746f 7228 6669  ata_connector(fi
-0002de60: 6c65 5f70 6172 7473 2c20 646f 632e 6e6f  le_parts, doc.no
-0002de70: 6465 735b 305d 290a 2020 2020 2020 2020  des[0]).        
-0002de80: 666f 726d 6174 5f69 6d70 6f72 745f 7365  format_import_se
-0002de90: 7474 696e 6773 2866 696c 655f 7061 7274  ttings(file_part
-0002dea0: 732c 2064 6f63 2e6e 6f64 6573 5b30 5d29  s, doc.nodes[0])
-0002deb0: 0a20 2020 2020 2020 2066 6f72 6d61 745f  .        format_
-0002dec0: 7368 6172 6564 5f77 6974 6828 6669 6c65  shared_with(file
-0002ded0: 5f70 6172 7473 2c20 646f 6329 0a20 2020  _parts, doc).   
-0002dee0: 2072 6573 756c 7420 3d20 2222 2e6a 6f69   result = "".joi
-0002def0: 6e28 6669 6c65 5f70 6172 7473 290a 2020  n(file_parts).  
-0002df00: 2020 7265 7375 6c74 203d 2072 6573 756c    result = resul
-0002df10: 742e 7273 7472 6970 2822 5c6e 2229 202b  t.rstrip("\n") +
-0002df20: 2022 5c6e 220a 2020 2020 7265 7475 726e   "\n".    return
-0002df30: 2072 6573 756c 740a 0a0a 6465 6620 666f   result...def fo
-0002df40: 726d 6174 5f76 6572 7369 6f6e 2866 696c  rmat_version(fil
-0002df50: 655f 7061 7274 733a 204c 6973 745b 7374  e_parts: List[st
-0002df60: 725d 2c20 646f 633a 2044 6174 6166 696c  r], doc: Datafil
-0002df70: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-0002df80: 0a20 2020 2076 6572 7369 6f6e 203d 2064  .    version = d
-0002df90: 6f63 2e76 6572 7369 6f6e 2069 6620 646f  oc.version if do
-0002dfa0: 632e 7665 7273 696f 6e20 6973 206e 6f74  c.version is not
-0002dfb0: 204e 6f6e 6520 656c 7365 2022 220a 2020   None else "".  
-0002dfc0: 2020 6966 2076 6572 7369 6f6e 2021 3d20    if version != 
-0002dfd0: 2222 3a0a 2020 2020 2020 2020 6669 6c65  "":.        file
-0002dfe0: 5f70 6172 7473 2e61 7070 656e 6428 6622  _parts.append(f"
-0002dff0: 5645 5253 494f 4e20 7b76 6572 7369 6f6e  VERSION {version
-0002e000: 7d22 290a 2020 2020 2020 2020 6669 6c65  }").        file
-0002e010: 5f70 6172 7473 2e61 7070 656e 6428 4441  _parts.append(DA
-0002e020: 5441 4649 4c45 5f4e 4557 5f4c 494e 4529  TAFILE_NEW_LINE)
-0002e030: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
-0002e040: 7274 732e 6170 7065 6e64 2844 4154 4146  rts.append(DATAF
-0002e050: 494c 455f 4e45 575f 4c49 4e45 290a 2020  ILE_NEW_LINE).  
-0002e060: 2020 7265 7475 726e 2066 696c 655f 7061    return file_pa
-0002e070: 7274 730a 0a0a 6465 6620 666f 726d 6174  rts...def format
-0002e080: 5f6d 6169 6e74 6169 6e65 7228 6669 6c65  _maintainer(file
-0002e090: 5f70 6172 7473 3a20 4c69 7374 5b73 7472  _parts: List[str
-0002e0a0: 5d2c 2064 6f63 3a20 4461 7461 6669 6c65  ], doc: Datafile
-0002e0b0: 2920 2d3e 204c 6973 745b 7374 725d 3a0a  ) -> List[str]:.
-0002e0c0: 2020 2020 6d61 696e 7461 696e 6572 203d      maintainer =
-0002e0d0: 2064 6f63 2e6d 6169 6e74 6169 6e65 7220   doc.maintainer 
-0002e0e0: 6966 2064 6f63 2e6d 6169 6e74 6169 6e65  if doc.maintaine
-0002e0f0: 7220 6973 206e 6f74 204e 6f6e 6520 656c  r is not None el
-0002e100: 7365 2022 220a 2020 2020 6966 206d 6169  se "".    if mai
-0002e110: 6e74 6169 6e65 723a 0a20 2020 2020 2020  ntainer:.       
-0002e120: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
-0002e130: 6e64 2866 224d 4149 4e54 4149 4e45 5220  nd(f"MAINTAINER 
-0002e140: 7b6d 6169 6e74 6169 6e65 727d 2229 0a20  {maintainer}"). 
-0002e150: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002e160: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
-0002e170: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
-0002e180: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
-0002e190: 7070 656e 6428 4441 5441 4649 4c45 5f4e  ppend(DATAFILE_N
-0002e1a0: 4557 5f4c 494e 4529 0a20 2020 2072 6574  EW_LINE).    ret
-0002e1b0: 7572 6e20 6669 6c65 5f70 6172 7473 0a0a  urn file_parts..
-0002e1c0: 0a64 6566 2066 6f72 6d61 745f 736f 7572  .def format_sour
-0002e1d0: 6365 7328 6669 6c65 5f70 6172 7473 3a20  ces(file_parts: 
-0002e1e0: 4c69 7374 5b73 7472 5d2c 2064 6f63 3a20  List[str], doc: 
-0002e1f0: 4461 7461 6669 6c65 2920 2d3e 204c 6973  Datafile) -> Lis
-0002e200: 745b 7374 725d 3a0a 2020 2020 666f 7220  t[str]:.    for 
-0002e210: 736f 7572 6365 2069 6e20 646f 632e 736f  source in doc.so
-0002e220: 7572 6365 733a 0a20 2020 2020 2020 2066  urces:.        f
-0002e230: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002e240: 2866 2253 4f55 5243 4520 7b73 6f75 7263  (f"SOURCE {sourc
-0002e250: 657d 2229 0a20 2020 2020 2020 2066 696c  e}").        fil
-0002e260: 655f 7061 7274 732e 6170 7065 6e64 2844  e_parts.append(D
-0002e270: 4154 4146 494c 455f 4e45 575f 4c49 4e45  ATAFILE_NEW_LINE
-0002e280: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
-0002e290: 655f 7061 7274 730a 0a0a 6465 6620 666f  e_parts...def fo
-0002e2a0: 726d 6174 5f64 6573 6372 6970 7469 6f6e  rmat_description
-0002e2b0: 2866 696c 655f 7061 7274 733a 204c 6973  (file_parts: Lis
-0002e2c0: 745b 7374 725d 2c20 646f 633a 2041 6e79  t[str], doc: Any
-0002e2d0: 2920 2d3e 204c 6973 745b 7374 725d 3a0a  ) -> List[str]:.
-0002e2e0: 2020 2020 6465 7363 7269 7074 696f 6e20      description 
-0002e2f0: 3d20 646f 632e 6465 7363 7269 7074 696f  = doc.descriptio
-0002e300: 6e20 6966 2064 6f63 2e64 6573 6372 6970  n if doc.descrip
-0002e310: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
-0002e320: 2065 6c73 6520 2222 0a20 2020 2069 6620   else "".    if 
-0002e330: 6465 7363 7269 7074 696f 6e3a 0a20 2020  description:.   
-0002e340: 2020 2020 2066 696c 655f 7061 7274 732e       file_parts.
-0002e350: 6170 7065 6e64 2822 4445 5343 5249 5054  append("DESCRIPT
-0002e360: 494f 4e20 3e22 290a 2020 2020 2020 2020  ION >").        
-0002e370: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
-0002e380: 6428 4441 5441 4649 4c45 5f4e 4557 5f4c  d(DATAFILE_NEW_L
-0002e390: 494e 4529 0a20 2020 2020 2020 205b 6669  INE).        [fi
-0002e3a0: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
-0002e3b0: 6622 7b44 4154 4146 494c 455f 494e 4445  f"{DATAFILE_INDE
-0002e3c0: 4e54 7d7b 642e 7374 7269 7028 297d 5c6e  NT}{d.strip()}\n
-0002e3d0: 2229 2066 6f72 2064 2069 6e20 6465 7363  ") for d in desc
-0002e3e0: 7269 7074 696f 6e2e 7370 6c69 7428 4441  ription.split(DA
-0002e3f0: 5441 4649 4c45 5f4e 4557 5f4c 494e 4529  TAFILE_NEW_LINE)
-0002e400: 2069 6620 642e 7374 7269 7028 295d 2020   if d.strip()]  
-0002e410: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
-0002e420: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002e430: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
-0002e440: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
-0002e450: 7265 7475 726e 2066 696c 655f 7061 7274  return file_part
-0002e460: 730a 0a0a 6465 6620 666f 726d 6174 5f74  s...def format_t
-0002e470: 6f6b 656e 7328 6669 6c65 5f70 6172 7473  okens(file_parts
-0002e480: 3a20 4c69 7374 5b73 7472 5d2c 2064 6f63  : List[str], doc
-0002e490: 3a20 4461 7461 6669 6c65 2920 2d3e 204c  : Datafile) -> L
-0002e4a0: 6973 745b 7374 725d 3a0a 2020 2020 666f  ist[str]:.    fo
-0002e4b0: 7220 746f 6b65 6e20 696e 2064 6f63 2e74  r token in doc.t
-0002e4c0: 6f6b 656e 733a 0a20 2020 2020 2020 2066  okens:.        f
-0002e4d0: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002e4e0: 2866 2754 4f4b 454e 2022 7b74 6f6b 656e  (f'TOKEN "{token
-0002e4f0: 5b22 746f 6b65 6e5f 6e61 6d65 225d 7d22  ["token_name"]}"
-0002e500: 207b 746f 6b65 6e5b 2270 6572 6d69 7373   {token["permiss
-0002e510: 696f 6e73 225d 7d27 290a 2020 2020 2020  ions"]}').      
-0002e520: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
-0002e530: 656e 6428 4441 5441 4649 4c45 5f4e 4557  end(DATAFILE_NEW
-0002e540: 5f4c 494e 4529 0a20 2020 2069 6620 6c65  _LINE).    if le
-0002e550: 6e28 646f 632e 746f 6b65 6e73 293a 0a20  n(doc.tokens):. 
-0002e560: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002e570: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
-0002e580: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
-0002e590: 7265 7475 726e 2066 696c 655f 7061 7274  return file_part
-0002e5a0: 730a 0a0a 6465 6620 666f 726d 6174 5f6e  s...def format_n
-0002e5b0: 6f64 655f 7371 6c28 0a20 2020 2066 696c  ode_sql(.    fil
-0002e5c0: 655f 7061 7274 733a 204c 6973 745b 7374  e_parts: List[st
-0002e5d0: 725d 2c20 6e6f 6465 3a20 4469 6374 5b73  r], node: Dict[s
-0002e5e0: 7472 2c20 416e 795d 2c20 6c69 6e65 5f6c  tr, Any], line_l
-0002e5f0: 656e 6774 683a 204f 7074 696f 6e61 6c5b  ength: Optional[
-0002e600: 696e 745d 203d 204e 6f6e 652c 206c 6f77  int] = None, low
-0002e610: 6572 5f6b 6579 776f 7264 733a 2062 6f6f  er_keywords: boo
-0002e620: 6c20 3d20 4661 6c73 650a 2920 2d3e 204c  l = False.) -> L
-0002e630: 6973 745b 7374 725d 3a0a 2020 2020 6669  ist[str]:.    fi
-0002e640: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
-0002e650: 2253 514c 203e 2229 0a20 2020 2066 696c  "SQL >").    fil
-0002e660: 655f 7061 7274 732e 6170 7065 6e64 2844  e_parts.append(D
-0002e670: 4154 4146 494c 455f 4e45 575f 4c49 4e45  ATAFILE_NEW_LINE
-0002e680: 290a 2020 2020 6669 6c65 5f70 6172 7473  ).    file_parts
-0002e690: 2e61 7070 656e 6428 666f 726d 6174 5f73  .append(format_s
-0002e6a0: 716c 286e 6f64 655b 2273 716c 225d 2c20  ql(node["sql"], 
-0002e6b0: 4441 5441 4649 4c45 5f49 4e44 454e 542c  DATAFILE_INDENT,
-0002e6c0: 206c 696e 655f 6c65 6e67 7468 3d6c 696e   line_length=lin
-0002e6d0: 655f 6c65 6e67 7468 2c20 6c6f 7765 725f  e_length, lower_
-0002e6e0: 6b65 7977 6f72 6473 3d6c 6f77 6572 5f6b  keywords=lower_k
-0002e6f0: 6579 776f 7264 7329 290a 2020 2020 6669  eywords)).    fi
-0002e700: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
-0002e710: 4441 5441 4649 4c45 5f4e 4557 5f4c 494e  DATAFILE_NEW_LIN
-0002e720: 4529 0a20 2020 2066 696c 655f 7061 7274  E).    file_part
-0002e730: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
-0002e740: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
-0002e750: 7265 7475 726e 2066 696c 655f 7061 7274  return file_part
-0002e760: 730a 0a0a 6465 6620 666f 726d 6174 5f73  s...def format_s
-0002e770: 6861 7265 645f 7769 7468 2866 696c 655f  hared_with(file_
-0002e780: 7061 7274 733a 204c 6973 745b 7374 725d  parts: List[str]
-0002e790: 2c20 646f 633a 2044 6174 6166 696c 6529  , doc: Datafile)
-0002e7a0: 202d 3e20 4c69 7374 5b73 7472 5d3a 0a20   -> List[str]:. 
-0002e7b0: 2020 2069 6620 646f 632e 7368 6172 6564     if doc.shared
-0002e7c0: 5f77 6974 683a 0a20 2020 2020 2020 2066  _with:.        f
-0002e7d0: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002e7e0: 2822 5348 4152 4544 5f57 4954 4820 3e22  ("SHARED_WITH >"
-0002e7f0: 290a 2020 2020 2020 2020 6669 6c65 5f70  ).        file_p
-0002e800: 6172 7473 2e61 7070 656e 6428 4441 5441  arts.append(DATA
-0002e810: 4649 4c45 5f4e 4557 5f4c 494e 4529 0a20  FILE_NEW_LINE). 
-0002e820: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002e830: 732e 6170 7065 6e64 2822 5c6e 222e 6a6f  s.append("\n".jo
-0002e840: 696e 285b 6622 7b44 4154 4146 494c 455f  in([f"{DATAFILE_
-0002e850: 494e 4445 4e54 7d7b 776f 726b 7370 6163  INDENT}{workspac
-0002e860: 655f 6e61 6d65 7d22 2066 6f72 2077 6f72  e_name}" for wor
-0002e870: 6b73 7061 6365 5f6e 616d 6520 696e 2064  kspace_name in d
-0002e880: 6f63 2e73 6861 7265 645f 7769 7468 5d29  oc.shared_with])
-0002e890: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
-0002e8a0: 655f 7061 7274 730a 0a0a 6173 796e 6320  e_parts...async 
-0002e8b0: 6465 6620 666f 726d 6174 5f65 6e67 696e  def format_engin
-0002e8c0: 6528 0a20 2020 2066 696c 655f 7061 7274  e(.    file_part
-0002e8d0: 733a 204c 6973 745b 7374 725d 2c20 6e6f  s: List[str], no
-0002e8e0: 6465 3a20 4469 6374 5b73 7472 2c20 416e  de: Dict[str, An
-0002e8f0: 795d 2c20 6f6e 6c79 5f74 746c 3a20 626f  y], only_ttl: bo
-0002e900: 6f6c 203d 2046 616c 7365 2c20 636c 6965  ol = False, clie
-0002e910: 6e74 3a20 4f70 7469 6f6e 616c 5b54 696e  nt: Optional[Tin
-0002e920: 7942 5d20 3d20 4e6f 6e65 0a29 202d 3e20  yB] = None.) -> 
-0002e930: 4c69 7374 5b73 7472 5d3a 0a20 2020 2069  List[str]:.    i
-0002e940: 6620 6f6e 6c79 5f74 746c 3a0a 2020 2020  f only_ttl:.    
-0002e950: 2020 2020 6966 206e 6f64 652e 6765 7428      if node.get(
-0002e960: 2265 6e67 696e 6522 2c20 4e6f 6e65 293a  "engine", None):
-0002e970: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0002e980: 2061 7267 2069 6e20 736f 7274 6564 286e   arg in sorted(n
-0002e990: 6f64 655b 2265 6e67 696e 6522 5d2e 6765  ode["engine"].ge
-0002e9a0: 7428 2261 7267 7322 2c20 5b5d 2929 3a0a  t("args", [])):.
-0002e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e9c0: 6966 2061 7267 5b30 5d2e 7570 7065 7228  if arg[0].upper(
-0002e9d0: 2920 3d3d 2022 5454 4c22 3a0a 2020 2020  ) == "TTL":.    
-0002e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e9f0: 656c 656d 203d 2022 2c20 222e 6a6f 696e  elem = ", ".join
-0002ea00: 285b 782e 7374 7269 7028 2920 666f 7220  ([x.strip() for 
-0002ea10: 7820 696e 2061 7267 5b31 5d2e 7370 6c69  x in arg[1].spli
-0002ea20: 7428 222c 2229 5d29 0a20 2020 2020 2020  t(",")]).       
-0002ea30: 2020 2020 2020 2020 2020 2020 2074 7279               try
-0002ea40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002ea50: 2020 2020 2020 2020 2020 6966 2063 6c69            if cli
-0002ea60: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
+0002c2a0: 2020 2020 2020 2020 2020 2070 726f 6365             proce
+0002c2b0: 7373 6564 2e61 6464 286e 616d 6529 0a20  ssed.add(name). 
+0002c2c0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0002c2d0: 2069 6e20 6465 7065 6e64 656e 6369 6573   in dependencies
+0002c2e0: 5f67 7261 7068 2e74 6f5f 7275 6e3a 0a20  _graph.to_run:. 
+0002c2f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002c300: 6620 6620 6e6f 7420 696e 2070 726f 6365  f f not in proce
+0002c310: 7373 6564 3a0a 2020 2020 2020 2020 2020  ssed:.          
+0002c320: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0002c330: 6368 6563 6b5f 6669 7874 7572 6573 5f64  check_fixtures_d
+0002c340: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
+0002c350: 2020 2020 2020 2020 2020 2020 2074 625f               tb_
+0002c360: 636c 6965 6e74 2c0a 2020 2020 2020 2020  client,.        
+0002c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c380: 6465 7065 6e64 656e 6369 6573 5f67 7261  dependencies_gra
+0002c390: 7068 2e74 6f5f 7275 6e5b 665d 2c0a 2020  ph.to_run[f],.  
+0002c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c3b0: 2020 2020 2020 6465 6275 672c 0a20 2020        debug,.   
+0002c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c3d0: 2020 2020 2066 6f6c 6465 722c 0a20 2020       folder,.   
+0002c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c3f0: 2020 2020 2066 6f72 6365 2c0a 2020 2020       force,.    
+0002c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c410: 2020 2020 6d6f 6465 3d22 6170 7065 6e64      mode="append
+0002c420: 2220 6966 2069 735f 6272 616e 6368 2065  " if is_branch e
+0002c430: 6c73 6520 2272 6570 6c61 6365 222c 0a20  lse "replace",. 
+0002c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c450: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+0002c460: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+0002c470: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+0002c480: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+0002c490: 2e65 6368 6f28 4665 6564 6261 636b 4d61  .echo(FeedbackMa
+0002c4a0: 6e61 6765 722e 696e 666f 5f6e 6f74 5f70  nager.info_not_p
+0002c4b0: 7573 6869 6e67 5f66 6978 7475 7265 7328  ushing_fixtures(
+0002c4c0: 2929 0a0a 2020 2020 6177 6169 7420 6465  ))..    await de
+0002c4d0: 706c 6f79 6d65 6e74 2e75 7064 6174 655f  ployment.update_
+0002c4e0: 7265 6c65 6173 6528 6861 735f 7365 6d76  release(has_semv
+0002c4f0: 6572 3d68 6173 5f73 656d 7665 722c 2072  er=has_semver, r
+0002c500: 656c 6561 7365 5f63 7265 6174 6564 3d72  elease_created=r
+0002c510: 656c 6561 7365 5f63 7265 6174 6564 290a  elease_created).
+0002c520: 0a20 2020 2072 6574 7572 6e20 6465 7065  .    return depe
+0002c530: 6e64 656e 6369 6573 5f67 7261 7068 2e74  ndencies_graph.t
+0002c540: 6f5f 7275 6e0a 0a0a 6173 796e 6320 6465  o_run...async de
+0002c550: 6620 6368 6563 6b5f 6669 7874 7572 6573  f check_fixtures
+0002c560: 5f64 6174 6128 0a20 2020 2063 6c69 656e  _data(.    clien
+0002c570: 743a 2054 696e 7942 2c20 7265 736f 7572  t: TinyB, resour
+0002c580: 6365 3a20 4469 6374 5b73 7472 2c20 416e  ce: Dict[str, An
+0002c590: 795d 2c20 6465 6275 673a 2062 6f6f 6c2c  y], debug: bool,
+0002c5a0: 2066 6f6c 6465 723a 2073 7472 203d 2022   folder: str = "
+0002c5b0: 222c 2066 6f72 6365 3a20 626f 6f6c 203d  ", force: bool =
+0002c5c0: 2046 616c 7365 2c20 6d6f 6465 3a20 7374   False, mode: st
+0002c5d0: 7220 3d20 2272 6570 6c61 6365 220a 293a  r = "replace".):
+0002c5e0: 0a20 2020 2069 6620 6465 6275 673a 0a20  .    if debug:. 
+0002c5f0: 2020 2020 2020 2063 6c69 636b 2e65 6368         click.ech
+0002c600: 6f28 4665 6564 6261 636b 4d61 6e61 6765  o(FeedbackManage
+0002c610: 722e 696e 666f 5f63 6865 636b 696e 675f  r.info_checking_
+0002c620: 6669 6c65 2866 696c 653d 7070 2e70 666f  file(file=pp.pfo
+0002c630: 726d 6174 2872 6573 6f75 7263 6529 2929  rmat(resource)))
+0002c640: 0a20 2020 2069 6620 7265 736f 7572 6365  .    if resource
+0002c650: 5b22 7265 736f 7572 6365 225d 2069 6e20  ["resource"] in 
+0002c660: 5b22 7069 7065 7322 2c20 2274 6f6b 656e  ["pipes", "token
+0002c670: 7322 5d3a 0a20 2020 2020 2020 2070 6173  s"]:.        pas
+0002c680: 730a 2020 2020 656c 6966 2072 6573 6f75  s.    elif resou
+0002c690: 7263 655b 2272 6573 6f75 7263 6522 5d20  rce["resource"] 
+0002c6a0: 3d3d 2022 6461 7461 736f 7572 6365 7322  == "datasources"
+0002c6b0: 3a0a 2020 2020 2020 2020 6461 7461 736f  :.        dataso
+0002c6c0: 7572 6365 5f6e 616d 6520 3d20 7265 736f  urce_name = reso
+0002c6d0: 7572 6365 5b22 7061 7261 6d73 225d 5b22  urce["params"]["
+0002c6e0: 6e61 6d65 225d 0a20 2020 2020 2020 206e  name"].        n
+0002c6f0: 616d 6520 3d20 6f73 2e70 6174 682e 6261  ame = os.path.ba
+0002c700: 7365 6e61 6d65 2872 6573 6f75 7263 655b  sename(resource[
+0002c710: 2266 696c 656e 616d 6522 5d29 2e72 7370  "filename"]).rsp
+0002c720: 6c69 7428 222e 222c 2031 295b 305d 0a20  lit(".", 1)[0]. 
+0002c730: 2020 2020 2020 2066 6978 7475 7265 5f70         fixture_p
+0002c740: 6174 6820 3d20 5061 7468 2866 6f6c 6465  ath = Path(folde
+0002c750: 7229 202f 2022 6669 7874 7572 6573 2220  r) / "fixtures" 
+0002c760: 2f20 6622 7b6e 616d 657d 2e63 7376 220a  / f"{name}.csv".
+0002c770: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0002c780: 6669 7874 7572 655f 7061 7468 2e65 7869  fixture_path.exi
+0002c790: 7374 7328 293a 0a20 2020 2020 2020 2020  sts():.         
+0002c7a0: 2020 2066 6978 7475 7265 5f70 6174 6820     fixture_path 
+0002c7b0: 3d20 5061 7468 2866 6f6c 6465 7229 202f  = Path(folder) /
+0002c7c0: 2022 6461 7461 736f 7572 6365 7322 202f   "datasources" /
+0002c7d0: 2022 6669 7874 7572 6573 2220 2f20 6622   "fixtures" / f"
+0002c7e0: 7b6e 616d 657d 2e63 7376 220a 2020 2020  {name}.csv".    
+0002c7f0: 2020 2020 6966 206e 6f74 2066 6978 7475      if not fixtu
+0002c800: 7265 5f70 6174 682e 6578 6973 7473 2829  re_path.exists()
+0002c810: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+0002c820: 7874 7572 655f 7061 7468 203d 2050 6174  xture_path = Pat
+0002c830: 6828 666f 6c64 6572 2920 2f20 2264 6174  h(folder) / "dat
+0002c840: 6173 6f75 7263 6573 2220 2f20 2266 6978  asources" / "fix
+0002c850: 7475 7265 7322 202f 2066 227b 6e61 6d65  tures" / f"{name
+0002c860: 7d2e 6e64 6a73 6f6e 220a 2020 2020 2020  }.ndjson".      
+0002c870: 2020 6966 206e 6f74 2066 6978 7475 7265    if not fixture
+0002c880: 5f70 6174 682e 6578 6973 7473 2829 3a0a  _path.exists():.
+0002c890: 2020 2020 2020 2020 2020 2020 6669 7874              fixt
+0002c8a0: 7572 655f 7061 7468 203d 2050 6174 6828  ure_path = Path(
+0002c8b0: 666f 6c64 6572 2920 2f20 2264 6174 6173  folder) / "datas
+0002c8c0: 6f75 7263 6573 2220 2f20 2266 6978 7475  ources" / "fixtu
+0002c8d0: 7265 7322 202f 2066 227b 6e61 6d65 7d2e  res" / f"{name}.
+0002c8e0: 7061 7271 7565 7422 0a20 2020 2020 2020  parquet".       
+0002c8f0: 2069 6620 6669 7874 7572 655f 7061 7468   if fixture_path
+0002c900: 2e65 7869 7374 7328 293a 0a20 2020 2020  .exists():.     
+0002c910: 2020 2020 2020 2023 204c 6574 2773 2076         # Let's v
+0002c920: 616c 6964 6174 6520 6f6e 6c79 2077 6865  alidate only whe
+0002c930: 6e20 7768 656e 2077 6520 6172 6520 676f  n when we are go
+0002c940: 696e 6720 746f 2072 6570 6c61 6365 2074  ing to replace t
+0002c950: 6865 2061 6374 7561 6c20 6461 7461 0a20  he actual data. 
+0002c960: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002c970: 7420 3d20 6177 6169 7420 636c 6965 6e74  t = await client
+0002c980: 2e71 7565 7279 2873 716c 3d66 2253 454c  .query(sql=f"SEL
+0002c990: 4543 5420 636f 756e 7428 2920 6173 2063  ECT count() as c
+0002c9a0: 2046 524f 4d20 7b64 6174 6173 6f75 7263   FROM {datasourc
+0002c9b0: 655f 6e61 6d65 7d20 464f 524d 4154 204a  e_name} FORMAT J
+0002c9c0: 534f 4e22 290a 2020 2020 2020 2020 2020  SON").          
+0002c9d0: 2020 636f 756e 7420 3d20 7265 7375 6c74    count = result
+0002c9e0: 5b22 6461 7461 225d 5b30 5d5b 2263 225d  ["data"][0]["c"]
+0002c9f0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0002ca00: 2063 6f75 6e74 203e 2030 2061 6e64 206e   count > 0 and n
+0002ca10: 6f74 2066 6f72 6365 3a0a 2020 2020 2020  ot force:.      
+0002ca20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0002ca30: 636c 6963 6b2e 436c 6963 6b45 7863 6570  click.ClickExcep
+0002ca40: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0002ca50: 2020 2020 2020 2020 2020 4665 6564 6261            Feedba
+0002ca60: 636b 4d61 6e61 6765 722e 6572 726f 725f  ckManager.error_
+0002ca70: 7075 7368 5f66 6978 7475 7265 5f77 696c  push_fixture_wil
+0002ca80: 6c5f 7265 706c 6163 655f 6461 7461 2864  l_replace_data(d
+0002ca90: 6174 6173 6f75 7263 653d 6461 7461 736f  atasource=dataso
+0002caa0: 7572 6365 5f6e 616d 6529 0a20 2020 2020  urce_name).     
+0002cab0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0002cac0: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+0002cad0: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
+0002cae0: 2020 2020 2020 4665 6564 6261 636b 4d61        FeedbackMa
+0002caf0: 6e61 6765 722e 696e 666f 5f63 6865 636b  nager.info_check
+0002cb00: 696e 675f 6669 6c65 5f73 697a 6528 0a20  ing_file_size(. 
+0002cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cb20: 2020 2066 696c 656e 616d 653d 7265 736f     filename=reso
+0002cb30: 7572 6365 5b22 6669 6c65 6e61 6d65 225d  urce["filename"]
+0002cb40: 2c20 7369 7a65 3d73 697a 656f 665f 666d  , size=sizeof_fm
+0002cb50: 7428 6f73 2e73 7461 7428 6669 7874 7572  t(os.stat(fixtur
+0002cb60: 655f 7061 7468 292e 7374 5f73 697a 6529  e_path).st_size)
+0002cb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cb80: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+0002cb90: 0a20 2020 2020 2020 2020 2020 2073 7973  .            sys
+0002cba0: 2e73 7464 6f75 742e 666c 7573 6828 290a  .stdout.flush().
+0002cbb0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0002cbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cbd0: 2061 7761 6974 2063 6c69 656e 742e 6461   await client.da
+0002cbe0: 7461 736f 7572 6365 5f61 7070 656e 645f  tasource_append_
+0002cbf0: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
+0002cc00: 2020 2020 2020 2020 2020 6461 7461 736f            dataso
+0002cc10: 7572 6365 5f6e 616d 653d 7265 736f 7572  urce_name=resour
+0002cc20: 6365 5b22 7061 7261 6d73 225d 5b22 6e61  ce["params"]["na
+0002cc30: 6d65 225d 2c0a 2020 2020 2020 2020 2020  me"],.          
+0002cc40: 2020 2020 2020 2020 2020 6669 6c65 3d66            file=f
+0002cc50: 6978 7475 7265 5f70 6174 682c 0a20 2020  ixture_path,.   
+0002cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cc70: 206d 6f64 653d 6d6f 6465 2c0a 2020 2020   mode=mode,.    
+0002cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cc90: 666f 726d 6174 3d66 6978 7475 7265 5f70  format=fixture_p
+0002cca0: 6174 682e 7375 6666 6978 5b31 3a5d 2c0a  ath.suffix[1:],.
+0002ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ccc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002ccd0: 2020 636c 6963 6b2e 6563 686f 2846 6565    click.echo(Fee
+0002cce0: 6462 6163 6b4d 616e 6167 6572 2e73 7563  dbackManager.suc
+0002ccf0: 6365 7373 5f70 726f 6365 7373 696e 675f  cess_processing_
+0002cd00: 6461 7461 2829 290a 2020 2020 2020 2020  data()).        
+0002cd10: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0002cd20: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+0002cd30: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0002cd40: 2063 6c69 636b 2e43 6c69 636b 4578 6365   click.ClickExce
+0002cd50: 7074 696f 6e28 4665 6564 6261 636b 4d61  ption(FeedbackMa
+0002cd60: 6e61 6765 722e 6572 726f 725f 7072 6f63  nager.error_proc
+0002cd70: 6573 7369 6e67 5f62 6c6f 636b 7328 6572  essing_blocks(er
+0002cd80: 726f 723d 6529 290a 0a20 2020 2020 2020  ror=e))..       
+0002cd90: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002cda0: 2020 2063 6c69 636b 2e65 6368 6f28 4665     click.echo(Fe
+0002cdb0: 6564 6261 636b 4d61 6e61 6765 722e 7761  edbackManager.wa
+0002cdc0: 726e 696e 675f 6669 7874 7572 655f 6e6f  rning_fixture_no
+0002cdd0: 745f 666f 756e 6428 6461 7461 736f 7572  t_found(datasour
+0002cde0: 6365 5f6e 616d 653d 6e61 6d65 2929 0a20  ce_name=name)). 
+0002cdf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002ce00: 2072 6169 7365 2063 6c69 636b 2e43 6c69   raise click.Cli
+0002ce10: 636b 4578 6365 7074 696f 6e28 4665 6564  ckException(Feed
+0002ce20: 6261 636b 4d61 6e61 6765 722e 6572 726f  backManager.erro
+0002ce30: 725f 756e 6b6e 6f77 6e5f 7265 736f 7572  r_unknown_resour
+0002ce40: 6365 2872 6573 6f75 7263 653d 7265 736f  ce(resource=reso
+0002ce50: 7572 6365 5b22 7265 736f 7572 6365 225d  urce["resource"]
+0002ce60: 2929 0a0a 0a44 4154 4146 494c 455f 4e45  ))...DATAFILE_NE
+0002ce70: 575f 4c49 4e45 203d 2022 5c6e 220a 4441  W_LINE = "\n".DA
+0002ce80: 5441 4649 4c45 5f49 4e44 454e 5420 3d20  TAFILE_INDENT = 
+0002ce90: 2220 2220 2a20 340a 0a0a 6465 6620 666f  " " * 4...def fo
+0002cea0: 726d 6174 5f73 6368 656d 6128 6669 6c65  rmat_schema(file
+0002ceb0: 5f70 6172 7473 3a20 4c69 7374 5b73 7472  _parts: List[str
+0002cec0: 5d2c 206e 6f64 653a 2044 6963 745b 7374  ], node: Dict[st
+0002ced0: 722c 2041 6e79 5d29 202d 3e20 4c69 7374  r, Any]) -> List
+0002cee0: 5b73 7472 5d3a 0a20 2020 2069 6620 2273  [str]:.    if "s
+0002cef0: 6368 656d 6122 2069 6e20 6e6f 6465 2061  chema" in node a
+0002cf00: 6e64 206e 6f64 655b 2273 6368 656d 6122  nd node["schema"
+0002cf10: 5d3a 0a20 2020 2020 2020 2066 696c 655f  ]:.        file_
+0002cf20: 7061 7274 732e 6170 7065 6e64 2822 5343  parts.append("SC
+0002cf30: 4845 4d41 203e 2229 0a20 2020 2020 2020  HEMA >").       
+0002cf40: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
+0002cf50: 6e64 2844 4154 4146 494c 455f 4e45 575f  nd(DATAFILE_NEW_
+0002cf60: 4c49 4e45 290a 2020 2020 2020 2020 636f  LINE).        co
+0002cf70: 6c75 6d6e 7320 3d20 7363 6865 6d61 5f74  lumns = schema_t
+0002cf80: 6f5f 7371 6c5f 636f 6c75 6d6e 7328 6e6f  o_sql_columns(no
+0002cf90: 6465 5b22 636f 6c75 6d6e 7322 5d29 0a20  de["columns"]). 
+0002cfa0: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002cfb0: 732e 6170 7065 6e64 2866 222c 7b44 4154  s.append(f",{DAT
+0002cfc0: 4146 494c 455f 4e45 575f 4c49 4e45 7d22  AFILE_NEW_LINE}"
+0002cfd0: 2e6a 6f69 6e28 6d61 7028 6c61 6d62 6461  .join(map(lambda
+0002cfe0: 2078 3a20 6622 2020 2020 7b78 7d22 2c20   x: f"    {x}", 
+0002cff0: 636f 6c75 6d6e 7329 2929 0a20 2020 2020  columns))).     
+0002d000: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
+0002d010: 7065 6e64 2844 4154 4146 494c 455f 4e45  pend(DATAFILE_NE
+0002d020: 575f 4c49 4e45 290a 2020 2020 2020 2020  W_LINE).        
+0002d030: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
+0002d040: 6428 4441 5441 4649 4c45 5f4e 4557 5f4c  d(DATAFILE_NEW_L
+0002d050: 494e 4529 0a0a 2020 2020 7265 7475 726e  INE)..    return
+0002d060: 2066 696c 655f 7061 7274 730a 0a0a 6465   file_parts...de
+0002d070: 6620 666f 726d 6174 5f69 6e64 6963 6573  f format_indices
+0002d080: 2866 696c 655f 7061 7274 733a 204c 6973  (file_parts: Lis
+0002d090: 745b 7374 725d 2c20 6e6f 6465 3a20 4469  t[str], node: Di
+0002d0a0: 6374 5b73 7472 2c20 416e 795d 2920 2d3e  ct[str, Any]) ->
+0002d0b0: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+0002d0c0: 6966 2022 696e 6465 7865 7322 2069 6e20  if "indexes" in 
+0002d0d0: 6e6f 6465 2061 6e64 206e 6f64 655b 2269  node and node["i
+0002d0e0: 6e64 6578 6573 225d 3a0a 2020 2020 2020  ndexes"]:.      
+0002d0f0: 2020 696e 6465 7865 7320 3d20 6e6f 6465    indexes = node
+0002d100: 5b22 696e 6465 7865 7322 5d0a 2020 2020  ["indexes"].    
+0002d110: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
+0002d120: 7070 656e 6428 2249 4e44 4558 4553 203e  ppend("INDEXES >
+0002d130: 2229 0a20 2020 2020 2020 2066 696c 655f  ").        file_
+0002d140: 7061 7274 732e 6170 7065 6e64 2844 4154  parts.append(DAT
+0002d150: 4146 494c 455f 4e45 575f 4c49 4e45 290a  AFILE_NEW_LINE).
+0002d160: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
+0002d170: 7473 2e61 7070 656e 6428 6622 7b44 4154  ts.append(f"{DAT
+0002d180: 4146 494c 455f 4e45 575f 4c49 4e45 7d22  AFILE_NEW_LINE}"
+0002d190: 2e6a 6f69 6e28 6d61 7028 6c61 6d62 6461  .join(map(lambda
+0002d1a0: 2069 6e64 6578 3a20 6622 2020 2020 7b69   index: f"    {i
+0002d1b0: 6e64 6578 2e74 6f5f 6461 7461 6669 6c65  ndex.to_datafile
+0002d1c0: 2829 7d22 2c20 696e 6465 7865 7329 2929  ()}", indexes)))
+0002d1d0: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
+0002d1e0: 7274 732e 6170 7065 6e64 2844 4154 4146  rts.append(DATAF
+0002d1f0: 494c 455f 4e45 575f 4c49 4e45 290a 2020  ILE_NEW_LINE).  
+0002d200: 2020 2020 2020 6669 6c65 5f70 6172 7473        file_parts
+0002d210: 2e61 7070 656e 6428 4441 5441 4649 4c45  .append(DATAFILE
+0002d220: 5f4e 4557 5f4c 494e 4529 0a0a 2020 2020  _NEW_LINE)..    
+0002d230: 7265 7475 726e 2066 696c 655f 7061 7274  return file_part
+0002d240: 730a 0a0a 6465 6620 666f 726d 6174 5f64  s...def format_d
+0002d250: 6174 615f 636f 6e6e 6563 746f 7228 6669  ata_connector(fi
+0002d260: 6c65 5f70 6172 7473 3a20 4c69 7374 5b73  le_parts: List[s
+0002d270: 7472 5d2c 206e 6f64 653a 2044 6963 745b  tr], node: Dict[
+0002d280: 7374 722c 2041 6e79 5d29 202d 3e20 4c69  str, Any]) -> Li
+0002d290: 7374 5b73 7472 5d3a 0a20 2020 206c 6c20  st[str]:.    ll 
+0002d2a0: 3d20 6c65 6e28 6669 6c65 5f70 6172 7473  = len(file_parts
+0002d2b0: 290a 2020 2020 7175 6f74 6573 203d 2022  ).    quotes = "
+0002d2c0: 2727 220a 2020 2020 5b66 696c 655f 7061  ''".    [file_pa
+0002d2d0: 7274 732e 6170 7065 6e64 2866 227b 6b2e  rts.append(f"{k.
+0002d2e0: 7570 7065 7228 297d 207b 7620 6f72 2071  upper()} {v or q
+0002d2f0: 756f 7465 737d 7b44 4154 4146 494c 455f  uotes}{DATAFILE_
+0002d300: 4e45 575f 4c49 4e45 7d22 2920 666f 7220  NEW_LINE}") for 
+0002d310: 6b2c 2076 2069 6e20 6e6f 6465 2e69 7465  k, v in node.ite
+0002d320: 6d73 2829 2069 6620 226b 6166 6b61 2220  ms() if "kafka" 
+0002d330: 696e 206b 5d20 2023 2074 7970 653a 2069  in k]  # type: i
+0002d340: 676e 6f72 650a 2020 2020 6966 206c 6c20  gnore.    if ll 
+0002d350: 3c20 6c65 6e28 6669 6c65 5f70 6172 7473  < len(file_parts
+0002d360: 293a 0a20 2020 2020 2020 2066 696c 655f  ):.        file_
+0002d370: 7061 7274 732e 6170 7065 6e64 2844 4154  parts.append(DAT
+0002d380: 4146 494c 455f 4e45 575f 4c49 4e45 290a  AFILE_NEW_LINE).
+0002d390: 2020 2020 7265 7475 726e 2066 696c 655f      return file_
+0002d3a0: 7061 7274 730a 0a0a 6465 6620 666f 726d  parts...def form
+0002d3b0: 6174 5f69 6d70 6f72 745f 7365 7474 696e  at_import_settin
+0002d3c0: 6773 2866 696c 655f 7061 7274 733a 204c  gs(file_parts: L
+0002d3d0: 6973 745b 7374 725d 2c20 6e6f 6465 3a20  ist[str], node: 
+0002d3e0: 4469 6374 5b73 7472 2c20 416e 795d 2920  Dict[str, Any]) 
+0002d3f0: 2d3e 204c 6973 745b 7374 725d 3a0a 2020  -> List[str]:.  
+0002d400: 2020 6c6c 203d 206c 656e 2866 696c 655f    ll = len(file_
+0002d410: 7061 7274 7329 0a20 2020 205b 6669 6c65  parts).    [file
+0002d420: 5f70 6172 7473 2e61 7070 656e 6428 6622  _parts.append(f"
+0002d430: 7b6b 2e75 7070 6572 2829 7d20 7b76 7d7b  {k.upper()} {v}{
+0002d440: 4441 5441 4649 4c45 5f4e 4557 5f4c 494e  DATAFILE_NEW_LIN
+0002d450: 457d 2229 2066 6f72 206b 2c20 7620 696e  E}") for k, v in
+0002d460: 206e 6f64 652e 6974 656d 7328 2920 6966   node.items() if
+0002d470: 2022 696d 706f 7274 5f22 2069 6e20 6b5d   "import_" in k]
+0002d480: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+0002d490: 0a20 2020 2069 6620 6c6c 203c 206c 656e  .    if ll < len
+0002d4a0: 2866 696c 655f 7061 7274 7329 3a0a 2020  (file_parts):.  
+0002d4b0: 2020 2020 2020 6669 6c65 5f70 6172 7473        file_parts
+0002d4c0: 2e61 7070 656e 6428 4441 5441 4649 4c45  .append(DATAFILE
+0002d4d0: 5f4e 4557 5f4c 494e 4529 0a20 2020 2072  _NEW_LINE).    r
+0002d4e0: 6574 7572 6e20 6669 6c65 5f70 6172 7473  eturn file_parts
+0002d4f0: 0a0a 0a64 6566 2066 6f72 6d61 745f 696e  ...def format_in
+0002d500: 636c 7564 6528 6669 6c65 5f70 6172 7473  clude(file_parts
+0002d510: 3a20 4c69 7374 5b73 7472 5d2c 2064 6f63  : List[str], doc
+0002d520: 3a20 4461 7461 6669 6c65 2c20 756e 726f  : Datafile, unro
+0002d530: 6c6c 5f69 6e63 6c75 6465 733a 2062 6f6f  ll_includes: boo
+0002d540: 6c20 3d20 4661 6c73 6529 202d 3e20 4c69  l = False) -> Li
+0002d550: 7374 5b73 7472 5d3a 0a20 2020 2069 6620  st[str]:.    if 
+0002d560: 756e 726f 6c6c 5f69 6e63 6c75 6465 733a  unroll_includes:
+0002d570: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002d580: 6669 6c65 5f70 6172 7473 0a0a 2020 2020  file_parts..    
+0002d590: 6173 7365 7274 2064 6f63 2e72 6177 2069  assert doc.raw i
+0002d5a0: 7320 6e6f 7420 4e6f 6e65 0a0a 2020 2020  s not None..    
+0002d5b0: 696e 636c 7564 6520 3d20 5b6c 696e 6520  include = [line 
+0002d5c0: 666f 7220 6c69 6e65 2069 6e20 646f 632e  for line in doc.
+0002d5d0: 7261 7720 6966 2022 494e 434c 5544 4522  raw if "INCLUDE"
+0002d5e0: 2069 6e20 6c69 6e65 2061 6e64 2022 2e69   in line and ".i
+0002d5f0: 6e63 6c22 2069 6e20 6c69 6e65 5d0a 2020  ncl" in line].  
+0002d600: 2020 6966 206c 656e 2869 6e63 6c75 6465    if len(include
+0002d610: 293a 0a20 2020 2020 2020 2066 696c 655f  ):.        file_
+0002d620: 7061 7274 732e 6170 7065 6e64 2869 6e63  parts.append(inc
+0002d630: 6c75 6465 5b30 5d29 0a20 2020 2020 2020  lude[0]).       
+0002d640: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
+0002d650: 6e64 2844 4154 4146 494c 455f 4e45 575f  nd(DATAFILE_NEW_
+0002d660: 4c49 4e45 290a 2020 2020 7265 7475 726e  LINE).    return
+0002d670: 2066 696c 655f 7061 7274 730a 0a0a 6173   file_parts...as
+0002d680: 796e 6320 6465 6620 666f 726d 6174 5f64  ync def format_d
+0002d690: 6174 6173 6f75 7263 6528 0a20 2020 2066  atasource(.    f
+0002d6a0: 696c 656e 616d 653a 2073 7472 2c0a 2020  ilename: str,.  
+0002d6b0: 2020 756e 726f 6c6c 5f69 6e63 6c75 6465    unroll_include
+0002d6c0: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
+0002d6d0: 0a20 2020 2066 6f72 5f64 6966 663a 2062  .    for_diff: b
+0002d6e0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0002d6f0: 2063 6c69 656e 743a 204f 7074 696f 6e61   client: Optiona
+0002d700: 6c5b 5469 6e79 425d 203d 204e 6f6e 652c  l[TinyB] = None,
+0002d710: 0a20 2020 2072 6570 6c61 6365 5f69 6e63  .    replace_inc
+0002d720: 6c75 6465 733a 2062 6f6f 6c20 3d20 4661  ludes: bool = Fa
+0002d730: 6c73 652c 0a20 2020 2064 6174 6166 696c  lse,.    datafil
+0002d740: 653a 204f 7074 696f 6e61 6c5b 4461 7461  e: Optional[Data
+0002d750: 6669 6c65 5d20 3d20 4e6f 6e65 2c0a 2020  file] = None,.  
+0002d760: 2020 666f 725f 6465 706c 6f79 5f64 6966    for_deploy_dif
+0002d770: 663a 2062 6f6f 6c20 3d20 4661 6c73 652c  f: bool = False,
+0002d780: 0a20 2020 2073 6b69 705f 6576 616c 3a20  .    skip_eval: 
+0002d790: 626f 6f6c 203d 2046 616c 7365 2c0a 2920  bool = False,.) 
+0002d7a0: 2d3e 2073 7472 3a0a 2020 2020 6966 2064  -> str:.    if d
+0002d7b0: 6174 6166 696c 653a 0a20 2020 2020 2020  atafile:.       
+0002d7c0: 2064 6f63 203d 2064 6174 6166 696c 650a   doc = datafile.
+0002d7d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0002d7e0: 2020 646f 6320 3d20 7061 7273 655f 6461    doc = parse_da
+0002d7f0: 7461 736f 7572 6365 2866 696c 656e 616d  tasource(filenam
+0002d800: 652c 2072 6570 6c61 6365 5f69 6e63 6c75  e, replace_inclu
+0002d810: 6465 733d 7265 706c 6163 655f 696e 636c  des=replace_incl
+0002d820: 7564 6573 2c20 736b 6970 5f65 7661 6c3d  udes, skip_eval=
+0002d830: 736b 6970 5f65 7661 6c29 0a0a 2020 2020  skip_eval)..    
+0002d840: 6669 6c65 5f70 6172 7473 3a20 4c69 7374  file_parts: List
+0002d850: 5b73 7472 5d20 3d20 5b5d 0a20 2020 2069  [str] = [].    i
+0002d860: 6620 666f 725f 6469 6666 3a0a 2020 2020  f for_diff:.    
+0002d870: 2020 2020 6973 5f6b 6166 6b61 203d 2022      is_kafka = "
+0002d880: 6b61 666b 615f 636f 6e6e 6563 7469 6f6e  kafka_connection
+0002d890: 5f6e 616d 6522 2069 6e20 646f 632e 6e6f  _name" in doc.no
+0002d8a0: 6465 735b 305d 0a20 2020 2020 2020 2069  des[0].        i
+0002d8b0: 6620 6973 5f6b 6166 6b61 3a0a 2020 2020  f is_kafka:.    
+0002d8c0: 2020 2020 2020 2020 6b61 666b 615f 6d65          kafka_me
+0002d8d0: 7461 6461 7461 5f63 6f6c 756d 6e73 203d  tadata_columns =
+0002d8e0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0002d8f0: 2020 2022 5f5f 7661 6c75 6522 2c0a 2020     "__value",.  
+0002d900: 2020 2020 2020 2020 2020 2020 2020 225f                "_
+0002d910: 5f68 6561 6465 7273 222c 0a20 2020 2020  _headers",.     
+0002d920: 2020 2020 2020 2020 2020 2022 5f5f 746f             "__to
+0002d930: 7069 6322 2c0a 2020 2020 2020 2020 2020  pic",.          
+0002d940: 2020 2020 2020 225f 5f70 6172 7469 7469        "__partiti
+0002d950: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+0002d960: 2020 2020 2022 5f5f 6f66 6673 6574 222c       "__offset",
+0002d970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d980: 2022 5f5f 7469 6d65 7374 616d 7022 2c0a   "__timestamp",.
+0002d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d9a0: 225f 5f6b 6579 222c 0a20 2020 2020 2020  "__key",.       
+0002d9b0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0002d9c0: 2020 2063 6f6c 756d 6e73 203d 205b 6320     columns = [c 
+0002d9d0: 666f 7220 6320 696e 2064 6f63 2e6e 6f64  for c in doc.nod
+0002d9e0: 6573 5b30 5d5b 2263 6f6c 756d 6e73 225d  es[0]["columns"]
+0002d9f0: 2069 6620 635b 226e 616d 6522 5d20 6e6f   if c["name"] no
+0002da00: 7420 696e 206b 6166 6b61 5f6d 6574 6164  t in kafka_metad
+0002da10: 6174 615f 636f 6c75 6d6e 735d 0a20 2020  ata_columns].   
+0002da20: 2020 2020 2020 2020 2064 6f63 2e6e 6f64           doc.nod
+0002da30: 6573 5b30 5d2e 7570 6461 7465 280a 2020  es[0].update(.  
+0002da40: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+0002da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002da60: 2020 2020 2263 6f6c 756d 6e73 223a 2063      "columns": c
+0002da70: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+0002da80: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0002da90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002daa0: 666f 726d 6174 5f76 6572 7369 6f6e 2866  format_version(f
+0002dab0: 696c 655f 7061 7274 732c 2064 6f63 290a  ile_parts, doc).
+0002dac0: 2020 2020 2020 2020 6966 2066 6f72 5f64          if for_d
+0002dad0: 6570 6c6f 795f 6469 6666 3a0a 2020 2020  eploy_diff:.    
+0002dae0: 2020 2020 2020 2020 666f 726d 6174 5f64          format_d
+0002daf0: 6573 6372 6970 7469 6f6e 2866 696c 655f  escription(file_
+0002db00: 7061 7274 732c 2064 6f63 290a 2020 2020  parts, doc).    
+0002db10: 2020 2020 666f 726d 6174 5f74 6f6b 656e      format_token
+0002db20: 7328 6669 6c65 5f70 6172 7473 2c20 646f  s(file_parts, do
+0002db30: 6329 0a20 2020 2020 2020 2066 6f72 6d61  c).        forma
+0002db40: 745f 7363 6865 6d61 2866 696c 655f 7061  t_schema(file_pa
+0002db50: 7274 732c 2064 6f63 2e6e 6f64 6573 5b30  rts, doc.nodes[0
+0002db60: 5d29 0a20 2020 2020 2020 2066 6f72 6d61  ]).        forma
+0002db70: 745f 696e 6469 6365 7328 6669 6c65 5f70  t_indices(file_p
+0002db80: 6172 7473 2c20 646f 632e 6e6f 6465 735b  arts, doc.nodes[
+0002db90: 305d 290a 2020 2020 2020 2020 6177 6169  0]).        awai
+0002dba0: 7420 666f 726d 6174 5f65 6e67 696e 6528  t format_engine(
+0002dbb0: 6669 6c65 5f70 6172 7473 2c20 646f 632e  file_parts, doc.
+0002dbc0: 6e6f 6465 735b 305d 2c20 6f6e 6c79 5f74  nodes[0], only_t
+0002dbd0: 746c 3d54 7275 6520 6966 206e 6f74 2066  tl=True if not f
+0002dbe0: 6f72 5f64 6570 6c6f 795f 6469 6666 2065  or_deploy_diff e
+0002dbf0: 6c73 6520 4661 6c73 652c 2063 6c69 656e  lse False, clien
+0002dc00: 743d 636c 6965 6e74 290a 2020 2020 2020  t=client).      
+0002dc10: 2020 6966 2066 6f72 5f64 6570 6c6f 795f    if for_deploy_
+0002dc20: 6469 6666 3a0a 2020 2020 2020 2020 2020  diff:.          
+0002dc30: 2020 666f 726d 6174 5f69 6d70 6f72 745f    format_import_
+0002dc40: 7365 7474 696e 6773 2866 696c 655f 7061  settings(file_pa
+0002dc50: 7274 732c 2064 6f63 2e6e 6f64 6573 5b30  rts, doc.nodes[0
+0002dc60: 5d29 0a20 2020 2020 2020 2066 6f72 6d61  ]).        forma
+0002dc70: 745f 7368 6172 6564 5f77 6974 6828 6669  t_shared_with(fi
+0002dc80: 6c65 5f70 6172 7473 2c20 646f 6329 0a0a  le_parts, doc)..
+0002dc90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0002dca0: 2020 666f 726d 6174 5f73 6f75 7263 6573    format_sources
+0002dcb0: 2866 696c 655f 7061 7274 732c 2064 6f63  (file_parts, doc
+0002dcc0: 290a 2020 2020 2020 2020 666f 726d 6174  ).        format
+0002dcd0: 5f6d 6169 6e74 6169 6e65 7228 6669 6c65  _maintainer(file
+0002dce0: 5f70 6172 7473 2c20 646f 6329 0a20 2020  _parts, doc).   
+0002dcf0: 2020 2020 2066 6f72 6d61 745f 7665 7273       format_vers
+0002dd00: 696f 6e28 6669 6c65 5f70 6172 7473 2c20  ion(file_parts, 
+0002dd10: 646f 6329 0a20 2020 2020 2020 2066 6f72  doc).        for
+0002dd20: 6d61 745f 6465 7363 7269 7074 696f 6e28  mat_description(
+0002dd30: 6669 6c65 5f70 6172 7473 2c20 646f 6329  file_parts, doc)
+0002dd40: 0a20 2020 2020 2020 2066 6f72 6d61 745f  .        format_
+0002dd50: 746f 6b65 6e73 2866 696c 655f 7061 7274  tokens(file_part
+0002dd60: 732c 2064 6f63 290a 2020 2020 2020 2020  s, doc).        
+0002dd70: 666f 726d 6174 5f73 6368 656d 6128 6669  format_schema(fi
+0002dd80: 6c65 5f70 6172 7473 2c20 646f 632e 6e6f  le_parts, doc.no
+0002dd90: 6465 735b 305d 290a 2020 2020 2020 2020  des[0]).        
+0002dda0: 666f 726d 6174 5f69 6e64 6963 6573 2866  format_indices(f
+0002ddb0: 696c 655f 7061 7274 732c 2064 6f63 2e6e  ile_parts, doc.n
+0002ddc0: 6f64 6573 5b30 5d29 0a20 2020 2020 2020  odes[0]).       
+0002ddd0: 2061 7761 6974 2066 6f72 6d61 745f 656e   await format_en
+0002dde0: 6769 6e65 2866 696c 655f 7061 7274 732c  gine(file_parts,
+0002ddf0: 2064 6f63 2e6e 6f64 6573 5b30 5d29 0a20   doc.nodes[0]). 
+0002de00: 2020 2020 2020 2066 6f72 6d61 745f 696e         format_in
+0002de10: 636c 7564 6528 6669 6c65 5f70 6172 7473  clude(file_parts
+0002de20: 2c20 646f 632c 2075 6e72 6f6c 6c5f 696e  , doc, unroll_in
+0002de30: 636c 7564 6573 3d75 6e72 6f6c 6c5f 696e  cludes=unroll_in
+0002de40: 636c 7564 6573 290a 2020 2020 2020 2020  cludes).        
+0002de50: 666f 726d 6174 5f64 6174 615f 636f 6e6e  format_data_conn
+0002de60: 6563 746f 7228 6669 6c65 5f70 6172 7473  ector(file_parts
+0002de70: 2c20 646f 632e 6e6f 6465 735b 305d 290a  , doc.nodes[0]).
+0002de80: 2020 2020 2020 2020 666f 726d 6174 5f69          format_i
+0002de90: 6d70 6f72 745f 7365 7474 696e 6773 2866  mport_settings(f
+0002dea0: 696c 655f 7061 7274 732c 2064 6f63 2e6e  ile_parts, doc.n
+0002deb0: 6f64 6573 5b30 5d29 0a20 2020 2020 2020  odes[0]).       
+0002dec0: 2066 6f72 6d61 745f 7368 6172 6564 5f77   format_shared_w
+0002ded0: 6974 6828 6669 6c65 5f70 6172 7473 2c20  ith(file_parts, 
+0002dee0: 646f 6329 0a20 2020 2072 6573 756c 7420  doc).    result 
+0002def0: 3d20 2222 2e6a 6f69 6e28 6669 6c65 5f70  = "".join(file_p
+0002df00: 6172 7473 290a 2020 2020 7265 7375 6c74  arts).    result
+0002df10: 203d 2072 6573 756c 742e 7273 7472 6970   = result.rstrip
+0002df20: 2822 5c6e 2229 202b 2022 5c6e 220a 2020  ("\n") + "\n".  
+0002df30: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0002df40: 0a0a 6465 6620 666f 726d 6174 5f76 6572  ..def format_ver
+0002df50: 7369 6f6e 2866 696c 655f 7061 7274 733a  sion(file_parts:
+0002df60: 204c 6973 745b 7374 725d 2c20 646f 633a   List[str], doc:
+0002df70: 2044 6174 6166 696c 6529 202d 3e20 4c69   Datafile) -> Li
+0002df80: 7374 5b73 7472 5d3a 0a20 2020 2076 6572  st[str]:.    ver
+0002df90: 7369 6f6e 203d 2064 6f63 2e76 6572 7369  sion = doc.versi
+0002dfa0: 6f6e 2069 6620 646f 632e 7665 7273 696f  on if doc.versio
+0002dfb0: 6e20 6973 206e 6f74 204e 6f6e 6520 656c  n is not None el
+0002dfc0: 7365 2022 220a 2020 2020 6966 2076 6572  se "".    if ver
+0002dfd0: 7369 6f6e 2021 3d20 2222 3a0a 2020 2020  sion != "":.    
+0002dfe0: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
+0002dff0: 7070 656e 6428 6622 5645 5253 494f 4e20  ppend(f"VERSION 
+0002e000: 7b76 6572 7369 6f6e 7d22 290a 2020 2020  {version}").    
+0002e010: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
+0002e020: 7070 656e 6428 4441 5441 4649 4c45 5f4e  ppend(DATAFILE_N
+0002e030: 4557 5f4c 494e 4529 0a20 2020 2020 2020  EW_LINE).       
+0002e040: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
+0002e050: 6e64 2844 4154 4146 494c 455f 4e45 575f  nd(DATAFILE_NEW_
+0002e060: 4c49 4e45 290a 2020 2020 7265 7475 726e  LINE).    return
+0002e070: 2066 696c 655f 7061 7274 730a 0a0a 6465   file_parts...de
+0002e080: 6620 666f 726d 6174 5f6d 6169 6e74 6169  f format_maintai
+0002e090: 6e65 7228 6669 6c65 5f70 6172 7473 3a20  ner(file_parts: 
+0002e0a0: 4c69 7374 5b73 7472 5d2c 2064 6f63 3a20  List[str], doc: 
+0002e0b0: 4461 7461 6669 6c65 2920 2d3e 204c 6973  Datafile) -> Lis
+0002e0c0: 745b 7374 725d 3a0a 2020 2020 6d61 696e  t[str]:.    main
+0002e0d0: 7461 696e 6572 203d 2064 6f63 2e6d 6169  tainer = doc.mai
+0002e0e0: 6e74 6169 6e65 7220 6966 2064 6f63 2e6d  ntainer if doc.m
+0002e0f0: 6169 6e74 6169 6e65 7220 6973 206e 6f74  aintainer is not
+0002e100: 204e 6f6e 6520 656c 7365 2022 220a 2020   None else "".  
+0002e110: 2020 6966 206d 6169 6e74 6169 6e65 723a    if maintainer:
+0002e120: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
+0002e130: 7274 732e 6170 7065 6e64 2866 224d 4149  rts.append(f"MAI
+0002e140: 4e54 4149 4e45 5220 7b6d 6169 6e74 6169  NTAINER {maintai
+0002e150: 6e65 727d 2229 0a20 2020 2020 2020 2066  ner}").        f
+0002e160: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002e170: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
+0002e180: 4e45 290a 2020 2020 2020 2020 6669 6c65  NE).        file
+0002e190: 5f70 6172 7473 2e61 7070 656e 6428 4441  _parts.append(DA
+0002e1a0: 5441 4649 4c45 5f4e 4557 5f4c 494e 4529  TAFILE_NEW_LINE)
+0002e1b0: 0a20 2020 2072 6574 7572 6e20 6669 6c65  .    return file
+0002e1c0: 5f70 6172 7473 0a0a 0a64 6566 2066 6f72  _parts...def for
+0002e1d0: 6d61 745f 736f 7572 6365 7328 6669 6c65  mat_sources(file
+0002e1e0: 5f70 6172 7473 3a20 4c69 7374 5b73 7472  _parts: List[str
+0002e1f0: 5d2c 2064 6f63 3a20 4461 7461 6669 6c65  ], doc: Datafile
+0002e200: 2920 2d3e 204c 6973 745b 7374 725d 3a0a  ) -> List[str]:.
+0002e210: 2020 2020 666f 7220 736f 7572 6365 2069      for source i
+0002e220: 6e20 646f 632e 736f 7572 6365 733a 0a20  n doc.sources:. 
+0002e230: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002e240: 732e 6170 7065 6e64 2866 2253 4f55 5243  s.append(f"SOURC
+0002e250: 4520 7b73 6f75 7263 657d 2229 0a20 2020  E {source}").   
+0002e260: 2020 2020 2066 696c 655f 7061 7274 732e       file_parts.
+0002e270: 6170 7065 6e64 2844 4154 4146 494c 455f  append(DATAFILE_
+0002e280: 4e45 575f 4c49 4e45 290a 2020 2020 7265  NEW_LINE).    re
+0002e290: 7475 726e 2066 696c 655f 7061 7274 730a  turn file_parts.
+0002e2a0: 0a0a 6465 6620 666f 726d 6174 5f64 6573  ..def format_des
+0002e2b0: 6372 6970 7469 6f6e 2866 696c 655f 7061  cription(file_pa
+0002e2c0: 7274 733a 204c 6973 745b 7374 725d 2c20  rts: List[str], 
+0002e2d0: 646f 633a 2041 6e79 2920 2d3e 204c 6973  doc: Any) -> Lis
+0002e2e0: 745b 7374 725d 3a0a 2020 2020 6465 7363  t[str]:.    desc
+0002e2f0: 7269 7074 696f 6e20 3d20 646f 632e 6465  ription = doc.de
+0002e300: 7363 7269 7074 696f 6e20 6966 2064 6f63  scription if doc
+0002e310: 2e64 6573 6372 6970 7469 6f6e 2069 7320  .description is 
+0002e320: 6e6f 7420 4e6f 6e65 2065 6c73 6520 2222  not None else ""
+0002e330: 0a20 2020 2069 6620 6465 7363 7269 7074  .    if descript
+0002e340: 696f 6e3a 0a20 2020 2020 2020 2066 696c  ion:.        fil
+0002e350: 655f 7061 7274 732e 6170 7065 6e64 2822  e_parts.append("
+0002e360: 4445 5343 5249 5054 494f 4e20 3e22 290a  DESCRIPTION >").
+0002e370: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
+0002e380: 7473 2e61 7070 656e 6428 4441 5441 4649  ts.append(DATAFI
+0002e390: 4c45 5f4e 4557 5f4c 494e 4529 0a20 2020  LE_NEW_LINE).   
+0002e3a0: 2020 2020 205b 6669 6c65 5f70 6172 7473       [file_parts
+0002e3b0: 2e61 7070 656e 6428 6622 7b44 4154 4146  .append(f"{DATAF
+0002e3c0: 494c 455f 494e 4445 4e54 7d7b 642e 7374  ILE_INDENT}{d.st
+0002e3d0: 7269 7028 297d 5c6e 2229 2066 6f72 2064  rip()}\n") for d
+0002e3e0: 2069 6e20 6465 7363 7269 7074 696f 6e2e   in description.
+0002e3f0: 7370 6c69 7428 4441 5441 4649 4c45 5f4e  split(DATAFILE_N
+0002e400: 4557 5f4c 494e 4529 2069 6620 642e 7374  EW_LINE) if d.st
+0002e410: 7269 7028 295d 2020 2320 7479 7065 3a20  rip()]  # type: 
+0002e420: 6967 6e6f 7265 0a20 2020 2020 2020 2066  ignore.        f
+0002e430: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002e440: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
+0002e450: 4e45 290a 2020 2020 7265 7475 726e 2066  NE).    return f
+0002e460: 696c 655f 7061 7274 730a 0a0a 6465 6620  ile_parts...def 
+0002e470: 666f 726d 6174 5f74 6f6b 656e 7328 6669  format_tokens(fi
+0002e480: 6c65 5f70 6172 7473 3a20 4c69 7374 5b73  le_parts: List[s
+0002e490: 7472 5d2c 2064 6f63 3a20 4461 7461 6669  tr], doc: Datafi
+0002e4a0: 6c65 2920 2d3e 204c 6973 745b 7374 725d  le) -> List[str]
+0002e4b0: 3a0a 2020 2020 666f 7220 746f 6b65 6e20  :.    for token 
+0002e4c0: 696e 2064 6f63 2e74 6f6b 656e 733a 0a20  in doc.tokens:. 
+0002e4d0: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002e4e0: 732e 6170 7065 6e64 2866 2754 4f4b 454e  s.append(f'TOKEN
+0002e4f0: 2022 7b74 6f6b 656e 5b22 746f 6b65 6e5f   "{token["token_
+0002e500: 6e61 6d65 225d 7d22 207b 746f 6b65 6e5b  name"]}" {token[
+0002e510: 2270 6572 6d69 7373 696f 6e73 225d 7d27  "permissions"]}'
+0002e520: 290a 2020 2020 2020 2020 6669 6c65 5f70  ).        file_p
+0002e530: 6172 7473 2e61 7070 656e 6428 4441 5441  arts.append(DATA
+0002e540: 4649 4c45 5f4e 4557 5f4c 494e 4529 0a20  FILE_NEW_LINE). 
+0002e550: 2020 2069 6620 6c65 6e28 646f 632e 746f     if len(doc.to
+0002e560: 6b65 6e73 293a 0a20 2020 2020 2020 2066  kens):.        f
+0002e570: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002e580: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
+0002e590: 4e45 290a 2020 2020 7265 7475 726e 2066  NE).    return f
+0002e5a0: 696c 655f 7061 7274 730a 0a0a 6465 6620  ile_parts...def 
+0002e5b0: 666f 726d 6174 5f6e 6f64 655f 7371 6c28  format_node_sql(
+0002e5c0: 0a20 2020 2066 696c 655f 7061 7274 733a  .    file_parts:
+0002e5d0: 204c 6973 745b 7374 725d 2c20 6e6f 6465   List[str], node
+0002e5e0: 3a20 4469 6374 5b73 7472 2c20 416e 795d  : Dict[str, Any]
+0002e5f0: 2c20 6c69 6e65 5f6c 656e 6774 683a 204f  , line_length: O
+0002e600: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0002e610: 6f6e 652c 206c 6f77 6572 5f6b 6579 776f  one, lower_keywo
+0002e620: 7264 733a 2062 6f6f 6c20 3d20 4661 6c73  rds: bool = Fals
+0002e630: 650a 2920 2d3e 204c 6973 745b 7374 725d  e.) -> List[str]
+0002e640: 3a0a 2020 2020 6669 6c65 5f70 6172 7473  :.    file_parts
+0002e650: 2e61 7070 656e 6428 2253 514c 203e 2229  .append("SQL >")
+0002e660: 0a20 2020 2066 696c 655f 7061 7274 732e  .    file_parts.
+0002e670: 6170 7065 6e64 2844 4154 4146 494c 455f  append(DATAFILE_
+0002e680: 4e45 575f 4c49 4e45 290a 2020 2020 6669  NEW_LINE).    fi
+0002e690: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
+0002e6a0: 666f 726d 6174 5f73 716c 286e 6f64 655b  format_sql(node[
+0002e6b0: 2273 716c 225d 2c20 4441 5441 4649 4c45  "sql"], DATAFILE
+0002e6c0: 5f49 4e44 454e 542c 206c 696e 655f 6c65  _INDENT, line_le
+0002e6d0: 6e67 7468 3d6c 696e 655f 6c65 6e67 7468  ngth=line_length
+0002e6e0: 2c20 6c6f 7765 725f 6b65 7977 6f72 6473  , lower_keywords
+0002e6f0: 3d6c 6f77 6572 5f6b 6579 776f 7264 7329  =lower_keywords)
+0002e700: 290a 2020 2020 6669 6c65 5f70 6172 7473  ).    file_parts
+0002e710: 2e61 7070 656e 6428 4441 5441 4649 4c45  .append(DATAFILE
+0002e720: 5f4e 4557 5f4c 494e 4529 0a20 2020 2066  _NEW_LINE).    f
+0002e730: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002e740: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
+0002e750: 4e45 290a 2020 2020 7265 7475 726e 2066  NE).    return f
+0002e760: 696c 655f 7061 7274 730a 0a0a 6465 6620  ile_parts...def 
+0002e770: 666f 726d 6174 5f73 6861 7265 645f 7769  format_shared_wi
+0002e780: 7468 2866 696c 655f 7061 7274 733a 204c  th(file_parts: L
+0002e790: 6973 745b 7374 725d 2c20 646f 633a 2044  ist[str], doc: D
+0002e7a0: 6174 6166 696c 6529 202d 3e20 4c69 7374  atafile) -> List
+0002e7b0: 5b73 7472 5d3a 0a20 2020 2069 6620 646f  [str]:.    if do
+0002e7c0: 632e 7368 6172 6564 5f77 6974 683a 0a20  c.shared_with:. 
+0002e7d0: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002e7e0: 732e 6170 7065 6e64 2822 5348 4152 4544  s.append("SHARED
+0002e7f0: 5f57 4954 4820 3e22 290a 2020 2020 2020  _WITH >").      
+0002e800: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
+0002e810: 656e 6428 4441 5441 4649 4c45 5f4e 4557  end(DATAFILE_NEW
+0002e820: 5f4c 494e 4529 0a20 2020 2020 2020 2066  _LINE).        f
+0002e830: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002e840: 2822 5c6e 222e 6a6f 696e 285b 6622 7b44  ("\n".join([f"{D
+0002e850: 4154 4146 494c 455f 494e 4445 4e54 7d7b  ATAFILE_INDENT}{
+0002e860: 776f 726b 7370 6163 655f 6e61 6d65 7d22  workspace_name}"
+0002e870: 2066 6f72 2077 6f72 6b73 7061 6365 5f6e   for workspace_n
+0002e880: 616d 6520 696e 2064 6f63 2e73 6861 7265  ame in doc.share
+0002e890: 645f 7769 7468 5d29 290a 2020 2020 7265  d_with])).    re
+0002e8a0: 7475 726e 2066 696c 655f 7061 7274 730a  turn file_parts.
+0002e8b0: 0a0a 6173 796e 6320 6465 6620 666f 726d  ..async def form
+0002e8c0: 6174 5f65 6e67 696e 6528 0a20 2020 2066  at_engine(.    f
+0002e8d0: 696c 655f 7061 7274 733a 204c 6973 745b  ile_parts: List[
+0002e8e0: 7374 725d 2c20 6e6f 6465 3a20 4469 6374  str], node: Dict
+0002e8f0: 5b73 7472 2c20 416e 795d 2c20 6f6e 6c79  [str, Any], only
+0002e900: 5f74 746c 3a20 626f 6f6c 203d 2046 616c  _ttl: bool = Fal
+0002e910: 7365 2c20 636c 6965 6e74 3a20 4f70 7469  se, client: Opti
+0002e920: 6f6e 616c 5b54 696e 7942 5d20 3d20 4e6f  onal[TinyB] = No
+0002e930: 6e65 0a29 202d 3e20 4c69 7374 5b73 7472  ne.) -> List[str
+0002e940: 5d3a 0a20 2020 2069 6620 6f6e 6c79 5f74  ]:.    if only_t
+0002e950: 746c 3a0a 2020 2020 2020 2020 6966 206e  tl:.        if n
+0002e960: 6f64 652e 6765 7428 2265 6e67 696e 6522  ode.get("engine"
+0002e970: 2c20 4e6f 6e65 293a 0a20 2020 2020 2020  , None):.       
+0002e980: 2020 2020 2066 6f72 2061 7267 2069 6e20       for arg in 
+0002e990: 736f 7274 6564 286e 6f64 655b 2265 6e67  sorted(node["eng
+0002e9a0: 696e 6522 5d2e 6765 7428 2261 7267 7322  ine"].get("args"
+0002e9b0: 2c20 5b5d 2929 3a0a 2020 2020 2020 2020  , [])):.        
+0002e9c0: 2020 2020 2020 2020 6966 2061 7267 5b30          if arg[0
+0002e9d0: 5d2e 7570 7065 7228 2920 3d3d 2022 5454  ].upper() == "TT
+0002e9e0: 4c22 3a0a 2020 2020 2020 2020 2020 2020  L":.            
+0002e9f0: 2020 2020 2020 2020 656c 656d 203d 2022          elem = "
+0002ea00: 2c20 222e 6a6f 696e 285b 782e 7374 7269  , ".join([x.stri
+0002ea10: 7028 2920 666f 7220 7820 696e 2061 7267  p() for x in arg
+0002ea20: 5b31 5d2e 7370 6c69 7428 222c 2229 5d29  [1].split(",")])
+0002ea30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ea40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0002ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ea60: 2020 6966 2063 6c69 656e 743a 0a20 2020    if client:.   
 0002ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ea80: 2074 746c 5f73 716c 203d 2061 7761 6974   ttl_sql = await
-0002ea90: 2063 6c69 656e 742e 7371 6c5f 6765 745f   client.sql_get_
-0002eaa0: 666f 726d 6174 2866 2273 656c 6563 7420  format(f"select 
-0002eab0: 7b65 6c65 6d7d 222c 2077 6974 685f 636c  {elem}", with_cl
-0002eac0: 6963 6b68 6f75 7365 5f66 6f72 6d61 743d  ickhouse_format=
-0002ead0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0002ea80: 2020 2020 2020 2020 2074 746c 5f73 716c           ttl_sql
+0002ea90: 203d 2061 7761 6974 2063 6c69 656e 742e   = await client.
+0002eaa0: 7371 6c5f 6765 745f 666f 726d 6174 2866  sql_get_format(f
+0002eab0: 2273 656c 6563 7420 7b65 6c65 6d7d 222c  "select {elem}",
+0002eac0: 2077 6974 685f 636c 6963 6b68 6f75 7365   with_clickhouse
+0002ead0: 5f66 6f72 6d61 743d 5472 7565 290a 2020  _format=True).  
 0002eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002eaf0: 2020 666f 726d 6174 7465 645f 7474 6c20    formatted_ttl 
-0002eb00: 3d20 7474 6c5f 7371 6c5b 373a 5d0a 2020  = ttl_sql[7:].  
-0002eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002eb20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0002eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002eb40: 2020 2020 2020 2020 666f 726d 6174 7465          formatte
-0002eb50: 645f 7474 6c20 3d20 656c 656d 0a20 2020  d_ttl = elem.   
-0002eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002eb70: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0002eb80: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-0002eb90: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
-0002eba0: 7474 6564 5f74 746c 203d 2065 6c65 6d0a  tted_ttl = elem.
-0002ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ebc0: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
-0002ebd0: 7070 656e 6428 6622 454e 4749 4e45 5f7b  ppend(f"ENGINE_{
-0002ebe0: 6172 675b 305d 2e75 7070 6572 2829 7d20  arg[0].upper()} 
-0002ebf0: 7b66 6f72 6d61 7474 6564 5f74 746c 7d22  {formatted_ttl}"
-0002ec00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002ec10: 2020 2020 2020 6669 6c65 5f70 6172 7473        file_parts
-0002ec20: 2e61 7070 656e 6428 4441 5441 4649 4c45  .append(DATAFILE
-0002ec30: 5f4e 4557 5f4c 494e 4529 0a20 2020 2020  _NEW_LINE).     
-0002ec40: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002ec50: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
-0002ec60: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
-0002ec70: 2020 2020 7265 7475 726e 2066 696c 655f      return file_
-0002ec80: 7061 7274 730a 2020 2020 656c 7365 3a0a  parts.    else:.
-0002ec90: 2020 2020 2020 2020 6966 206e 6f64 652e          if node.
-0002eca0: 6765 7428 2265 6e67 696e 6522 2c20 4e6f  get("engine", No
-0002ecb0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-0002ecc0: 2065 6d70 7479 203d 2027 2222 270a 2020   empty = '""'.  
-0002ecd0: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
-0002ece0: 6172 7473 2e61 7070 656e 6428 6627 454e  arts.append(f'EN
-0002ecf0: 4749 4e45 207b 6e6f 6465 5b22 656e 6769  GINE {node["engi
-0002ed00: 6e65 225d 5b22 7479 7065 225d 7d27 2069  ne"]["type"]}' i
-0002ed10: 6620 6e6f 6465 2e67 6574 2822 656e 6769  f node.get("engi
-0002ed20: 6e65 222c 207b 7d29 2e67 6574 2822 7479  ne", {}).get("ty
-0002ed30: 7065 2229 2065 6c73 6520 656d 7074 7929  pe") else empty)
-0002ed40: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-0002ed50: 655f 7061 7274 732e 6170 7065 6e64 2844  e_parts.append(D
-0002ed60: 4154 4146 494c 455f 4e45 575f 4c49 4e45  ATAFILE_NEW_LINE
-0002ed70: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0002ed80: 7220 6172 6720 696e 2073 6f72 7465 6428  r arg in sorted(
-0002ed90: 6e6f 6465 5b22 656e 6769 6e65 225d 2e67  node["engine"].g
-0002eda0: 6574 2822 6172 6773 222c 205b 5d29 293a  et("args", [])):
-0002edb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002edc0: 2065 6c65 6d20 3d20 222c 2022 2e6a 6f69   elem = ", ".joi
-0002edd0: 6e28 5b78 2e73 7472 6970 2829 2066 6f72  n([x.strip() for
-0002ede0: 2078 2069 6e20 6172 675b 315d 2e73 706c   x in arg[1].spl
-0002edf0: 6974 2822 2c22 295d 290a 2020 2020 2020  it(",")]).      
-0002ee00: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
-0002ee10: 6172 7473 2e61 7070 656e 6428 6622 454e  arts.append(f"EN
-0002ee20: 4749 4e45 5f7b 6172 675b 305d 2e75 7070  GINE_{arg[0].upp
-0002ee30: 6572 2829 7d20 7b65 6c65 6d20 6966 2065  er()} {elem if e
-0002ee40: 6c65 6d20 656c 7365 2065 6d70 7479 7d22  lem else empty}"
-0002ee50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002ee60: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
-0002ee70: 656e 6428 4441 5441 4649 4c45 5f4e 4557  end(DATAFILE_NEW
-0002ee80: 5f4c 494e 4529 0a20 2020 2020 2020 2020  _LINE).         
-0002ee90: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
-0002eea0: 7065 6e64 2844 4154 4146 494c 455f 4e45  pend(DATAFILE_NE
-0002eeb0: 575f 4c49 4e45 290a 2020 2020 2020 2020  W_LINE).        
-0002eec0: 7265 7475 726e 2066 696c 655f 7061 7274  return file_part
-0002eed0: 730a 0a0a 6173 796e 6320 6465 6620 666f  s...async def fo
-0002eee0: 726d 6174 5f6e 6f64 655f 7479 7065 2866  rmat_node_type(f
-0002eef0: 696c 655f 7061 7274 733a 204c 6973 745b  ile_parts: List[
-0002ef00: 7374 725d 2c20 6e6f 6465 3a20 4469 6374  str], node: Dict
-0002ef10: 5b73 7472 2c20 416e 795d 2920 2d3e 204c  [str, Any]) -> L
-0002ef20: 6973 745b 7374 725d 3a0a 2020 2020 6e6f  ist[str]:.    no
-0002ef30: 6465 5f74 7970 6520 3d20 6e6f 6465 2e67  de_type = node.g
-0002ef40: 6574 2822 7479 7065 222c 2022 2229 2e6c  et("type", "").l
-0002ef50: 6f77 6572 2829 0a20 2020 206e 6f64 655f  ower().    node_
-0002ef60: 7479 7065 5f75 7070 6572 203d 2066 2254  type_upper = f"T
-0002ef70: 5950 4520 7b6e 6f64 655f 7479 7065 2e75  YPE {node_type.u
-0002ef80: 7070 6572 2829 7d22 0a0a 2020 2020 2320  pper()}"..    # 
-0002ef90: 4d61 7465 7269 616c 697a 6564 2070 6970  Materialized pip
-0002efa0: 650a 2020 2020 6966 206e 6f64 655f 7479  e.    if node_ty
-0002efb0: 7065 203d 3d20 5069 7065 4e6f 6465 5479  pe == PipeNodeTy
-0002efc0: 7065 732e 4d41 5445 5249 414c 495a 4544  pes.MATERIALIZED
-0002efd0: 3a0a 2020 2020 2020 2020 6669 6c65 5f70  :.        file_p
-0002efe0: 6172 7473 2e61 7070 656e 6428 6e6f 6465  arts.append(node
-0002eff0: 5f74 7970 655f 7570 7065 7229 0a20 2020  _type_upper).   
-0002f000: 2020 2020 2066 696c 655f 7061 7274 732e       file_parts.
-0002f010: 6170 7065 6e64 2844 4154 4146 494c 455f  append(DATAFILE_
-0002f020: 4e45 575f 4c49 4e45 290a 2020 2020 2020  NEW_LINE).      
-0002f030: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
-0002f040: 656e 6428 6627 4441 5441 534f 5552 4345  end(f'DATASOURCE
-0002f050: 207b 6e6f 6465 5b22 6461 7461 736f 7572   {node["datasour
-0002f060: 6365 225d 7d27 290a 2020 2020 2020 2020  ce"]}').        
-0002f070: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
-0002f080: 6428 4441 5441 4649 4c45 5f4e 4557 5f4c  d(DATAFILE_NEW_L
-0002f090: 494e 4529 0a20 2020 2020 2020 2061 7761  INE).        awa
-0002f0a0: 6974 2066 6f72 6d61 745f 656e 6769 6e65  it format_engine
-0002f0b0: 2866 696c 655f 7061 7274 732c 206e 6f64  (file_parts, nod
-0002f0c0: 6529 0a0a 2020 2020 2320 436f 7079 2070  e)..    # Copy p
-0002f0d0: 6970 650a 2020 2020 6966 206e 6f64 655f  ipe.    if node_
-0002f0e0: 7479 7065 203d 3d20 5069 7065 4e6f 6465  type == PipeNode
-0002f0f0: 5479 7065 732e 434f 5059 3a0a 2020 2020  Types.COPY:.    
-0002f100: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
-0002f110: 7070 656e 6428 6e6f 6465 5f74 7970 655f  ppend(node_type_
-0002f120: 7570 7065 7229 0a20 2020 2020 2020 2066  upper).        f
-0002f130: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002f140: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
-0002f150: 4e45 290a 2020 2020 2020 2020 6669 6c65  NE).        file
-0002f160: 5f70 6172 7473 2e61 7070 656e 6428 6627  _parts.append(f'
-0002f170: 5441 5247 4554 5f44 4154 4153 4f55 5243  TARGET_DATASOURC
-0002f180: 4520 7b6e 6f64 655b 2274 6172 6765 745f  E {node["target_
-0002f190: 6461 7461 736f 7572 6365 225d 7d27 290a  datasource"]}').
-0002f1a0: 2020 2020 2020 2020 6966 2043 6f70 7950          if CopyP
-0002f1b0: 6172 616d 6574 6572 732e 434f 5059 5f53  arameters.COPY_S
-0002f1c0: 4348 4544 554c 4520 696e 206e 6f64 6520  CHEDULE in node 
-0002f1d0: 616e 6420 6e6f 6465 5b43 6f70 7950 6172  and node[CopyPar
-0002f1e0: 616d 6574 6572 732e 434f 5059 5f53 4348  ameters.COPY_SCH
-0002f1f0: 4544 554c 455d 3a0a 2020 2020 2020 2020  EDULE]:.        
-0002f200: 2020 2020 6973 5f6f 6e64 656d 616e 6420      is_ondemand 
-0002f210: 3d20 6e6f 6465 5b43 6f70 7950 6172 616d  = node[CopyParam
-0002f220: 6574 6572 732e 434f 5059 5f53 4348 4544  eters.COPY_SCHED
-0002f230: 554c 455d 2e6c 6f77 6572 2829 203d 3d20  ULE].lower() == 
-0002f240: 4f4e 5f44 454d 414e 440a 2020 2020 2020  ON_DEMAND.      
-0002f250: 2020 2020 2020 6669 6c65 5f70 6172 7473        file_parts
-0002f260: 2e61 7070 656e 6428 4441 5441 4649 4c45  .append(DATAFILE
-0002f270: 5f4e 4557 5f4c 494e 4529 0a20 2020 2020  _NEW_LINE).     
-0002f280: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002f290: 732e 6170 7065 6e64 280a 2020 2020 2020  s.append(.      
-0002f2a0: 2020 2020 2020 2020 2020 6622 7b43 6f70            f"{Cop
-0002f2b0: 7950 6172 616d 6574 6572 732e 434f 5059  yParameters.COPY
-0002f2c0: 5f53 4348 4544 554c 452e 7570 7065 7228  _SCHEDULE.upper(
-0002f2d0: 297d 207b 4f4e 5f44 454d 414e 4420 6966  )} {ON_DEMAND if
-0002f2e0: 2069 735f 6f6e 6465 6d61 6e64 2065 6c73   is_ondemand els
-0002f2f0: 6520 6e6f 6465 5b43 6f70 7950 6172 616d  e node[CopyParam
-0002f300: 6574 6572 732e 434f 5059 5f53 4348 4544  eters.COPY_SCHED
-0002f310: 554c 455d 7d22 0a20 2020 2020 2020 2020  ULE]}".         
-0002f320: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-0002f330: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-0002f340: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002f350: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
-0002f360: 4e45 290a 2020 2020 2020 2020 2020 2020  NE).            
-0002f370: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
-0002f380: 6428 6622 7b43 6f70 7950 6172 616d 6574  d(f"{CopyParamet
-0002f390: 6572 732e 434f 5059 5f53 4348 4544 554c  ers.COPY_SCHEDUL
-0002f3a0: 452e 7570 7065 7228 297d 207b 4f4e 5f44  E.upper()} {ON_D
-0002f3b0: 454d 414e 447d 2229 0a20 2020 2020 2020  EMAND}").       
-0002f3c0: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
-0002f3d0: 6e64 2844 4154 4146 494c 455f 4e45 575f  nd(DATAFILE_NEW_
-0002f3e0: 4c49 4e45 290a 0a20 2020 2023 2053 696e  LINE)..    # Sin
-0002f3f0: 6b20 7069 7065 0a20 2020 2069 6620 4578  k pipe.    if Ex
-0002f400: 706f 7274 5265 706c 6163 656d 656e 7473  portReplacements
-0002f410: 2e69 735f 6578 706f 7274 5f6e 6f64 6528  .is_export_node(
-0002f420: 6e6f 6465 293a 0a20 2020 2020 2020 2066  node):.        f
-0002f430: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
-0002f440: 286e 6f64 655f 7479 7065 5f75 7070 6572  (node_type_upper
-0002f450: 290a 2020 2020 2020 2020 6578 706f 7274  ).        export
-0002f460: 5f70 6172 616d 7320 3d20 4578 706f 7274  _params = Export
-0002f470: 5265 706c 6163 656d 656e 7473 2e67 6574  Replacements.get
-0002f480: 5f70 6172 616d 735f 6672 6f6d 5f64 6174  _params_from_dat
-0002f490: 6166 696c 6528 6e6f 6465 290a 2020 2020  afile(node).    
-0002f4a0: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
-0002f4b0: 7070 656e 6428 4441 5441 4649 4c45 5f4e  ppend(DATAFILE_N
-0002f4c0: 4557 5f4c 494e 4529 0a20 2020 2020 2020  EW_LINE).       
-0002f4d0: 2066 6f72 2070 6172 616d 2c20 7661 6c75   for param, valu
-0002f4e0: 6520 696e 2065 7870 6f72 745f 7061 7261  e in export_para
-0002f4f0: 6d73 2e69 7465 6d73 2829 3a0a 2020 2020  ms.items():.    
-0002f500: 2020 2020 2020 2020 6966 2070 6172 616d          if param
-0002f510: 203d 3d20 2273 6368 6564 756c 655f 6372   == "schedule_cr
-0002f520: 6f6e 2220 616e 6420 6e6f 7420 7661 6c75  on" and not valu
-0002f530: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002f540: 2020 2076 616c 7565 203d 204f 4e5f 4445     value = ON_DE
-0002f550: 4d41 4e44 0a20 2020 2020 2020 2020 2020  MAND.           
-0002f560: 2064 6174 6166 696c 655f 6b65 7920 3d20   datafile_key = 
-0002f570: 4578 706f 7274 5265 706c 6163 656d 656e  ExportReplacemen
-0002f580: 7473 2e67 6574 5f64 6174 6166 696c 655f  ts.get_datafile_
-0002f590: 6b65 7928 7061 7261 6d29 0a20 2020 2020  key(param).     
-0002f5a0: 2020 2020 2020 2069 6620 6461 7461 6669         if datafi
-0002f5b0: 6c65 5f6b 6579 3a0a 2020 2020 2020 2020  le_key:.        
-0002f5c0: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
-0002f5d0: 7473 2e61 7070 656e 6428 6622 7b64 6174  ts.append(f"{dat
-0002f5e0: 6166 696c 655f 6b65 797d 207b 7661 6c75  afile_key} {valu
-0002f5f0: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-0002f600: 2020 2020 2066 696c 655f 7061 7274 732e       file_parts.
-0002f610: 6170 7065 6e64 2844 4154 4146 494c 455f  append(DATAFILE_
-0002f620: 4e45 575f 4c49 4e45 290a 0a20 2020 2072  NEW_LINE)..    r
-0002f630: 6574 7572 6e20 6669 6c65 5f70 6172 7473  eturn file_parts
-0002f640: 0a0a 0a64 6566 2066 6f72 6d61 745f 7069  ...def format_pi
-0002f650: 7065 5f69 6e63 6c75 6465 2866 696c 655f  pe_include(file_
-0002f660: 7061 7274 733a 204c 6973 745b 7374 725d  parts: List[str]
-0002f670: 2c20 6e6f 6465 3a20 4469 6374 5b73 7472  , node: Dict[str
-0002f680: 2c20 416e 795d 2c20 696e 636c 7564 6573  , Any], includes
-0002f690: 3a20 4469 6374 5b73 7472 2c20 416e 795d  : Dict[str, Any]
-0002f6a0: 2920 2d3e 204c 6973 745b 7374 725d 3a0a  ) -> List[str]:.
-0002f6b0: 2020 2020 6966 2069 6e63 6c75 6465 733a      if includes:
-0002f6c0: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
-0002f6d0: 7620 696e 2069 6e63 6c75 6465 732e 636f  v in includes.co
-0002f6e0: 7079 2829 2e69 7465 6d73 2829 3a0a 2020  py().items():.  
-0002f6f0: 2020 2020 2020 2020 2020 6966 206e 6f64            if nod
-0002f700: 655b 226e 616d 6522 5d20 696e 2076 3a0a  e["name"] in v:.
-0002f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f720: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
-0002f730: 6428 6622 494e 434c 5544 4520 7b6b 7d22  d(f"INCLUDE {k}"
-0002f740: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002f750: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
-0002f760: 656e 6428 4441 5441 4649 4c45 5f4e 4557  end(DATAFILE_NEW
-0002f770: 5f4c 494e 4529 0a20 2020 2020 2020 2020  _LINE).         
-0002f780: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
-0002f790: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
-0002f7a0: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
-0002f7b0: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-0002f7c0: 696e 636c 7564 6573 5b6b 5d0a 2020 2020  includes[k].    
-0002f7d0: 7265 7475 726e 2066 696c 655f 7061 7274  return file_part
-0002f7e0: 730a 0a0a 6173 796e 6320 6465 6620 666f  s...async def fo
-0002f7f0: 726d 6174 5f6e 6f64 6528 0a20 2020 2066  rmat_node(.    f
-0002f800: 696c 655f 7061 7274 733a 204c 6973 745b  ile_parts: List[
-0002f810: 7374 725d 2c0a 2020 2020 6e6f 6465 3a20  str],.    node: 
-0002f820: 4469 6374 5b73 7472 2c20 416e 795d 2c0a  Dict[str, Any],.
-0002f830: 2020 2020 696e 636c 7564 6573 3a20 4469      includes: Di
-0002f840: 6374 5b73 7472 2c20 416e 795d 2c0a 2020  ct[str, Any],.  
-0002f850: 2020 6c69 6e65 5f6c 656e 6774 683a 204f    line_length: O
-0002f860: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0002f870: 6f6e 652c 0a20 2020 2075 6e72 6f6c 6c5f  one,.    unroll_
-0002f880: 696e 636c 7564 6573 3a20 626f 6f6c 203d  includes: bool =
-0002f890: 2046 616c 7365 2c0a 2020 2020 6c6f 7765   False,.    lowe
-0002f8a0: 725f 6b65 7977 6f72 6473 3a20 626f 6f6c  r_keywords: bool
-0002f8b0: 203d 2046 616c 7365 2c0a 2920 2d3e 204e   = False,.) -> N
-0002f8c0: 6f6e 653a 0a20 2020 2069 6620 6e6f 7420  one:.    if not 
-0002f8d0: 756e 726f 6c6c 5f69 6e63 6c75 6465 733a  unroll_includes:
-0002f8e0: 0a20 2020 2020 2020 2066 6f72 6d61 745f  .        format_
-0002f8f0: 7069 7065 5f69 6e63 6c75 6465 2866 696c  pipe_include(fil
-0002f900: 655f 7061 7274 732c 206e 6f64 652c 2069  e_parts, node, i
-0002f910: 6e63 6c75 6465 7329 0a20 2020 2069 7465  ncludes).    ite
-0002f920: 6d20 3d20 5b6b 2066 6f72 206b 2c20 5f20  m = [k for k, _ 
-0002f930: 696e 2069 6e63 6c75 6465 732e 6974 656d  in includes.item
-0002f940: 7328 2920 6966 206e 6f64 655b 226e 616d  s() if node["nam
-0002f950: 6522 5d2e 7374 7269 7028 2920 696e 206b  e"].strip() in k
-0002f960: 5d0a 2020 2020 6966 2069 7465 6d20 616e  ].    if item an
-0002f970: 6420 6e6f 7420 756e 726f 6c6c 5f69 6e63  d not unroll_inc
-0002f980: 6c75 6465 733a 0a20 2020 2020 2020 2072  ludes:.        r
-0002f990: 6574 7572 6e0a 0a20 2020 2066 696c 655f  eturn..    file_
-0002f9a0: 7061 7274 732e 6170 7065 6e64 2866 274e  parts.append(f'N
-0002f9b0: 4f44 4520 7b6e 6f64 655b 226e 616d 6522  ODE {node["name"
-0002f9c0: 5d2e 7374 7269 7028 297d 2729 0a20 2020  ].strip()}').   
-0002f9d0: 2066 696c 655f 7061 7274 732e 6170 7065   file_parts.appe
-0002f9e0: 6e64 2844 4154 4146 494c 455f 4e45 575f  nd(DATAFILE_NEW_
-0002f9f0: 4c49 4e45 290a 0a20 2020 2066 726f 6d20  LINE)..    from 
-0002fa00: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
-0002fa10: 7274 206e 616d 6564 7475 706c 650a 0a20  rt namedtuple.. 
-0002fa20: 2020 2044 6f63 203d 206e 616d 6564 7475     Doc = namedtu
-0002fa30: 706c 6528 2244 6f63 222c 205b 2264 6573  ple("Doc", ["des
-0002fa40: 6372 6970 7469 6f6e 225d 290a 2020 2020  cription"]).    
-0002fa50: 666f 726d 6174 5f64 6573 6372 6970 7469  format_descripti
-0002fa60: 6f6e 2866 696c 655f 7061 7274 732c 2044  on(file_parts, D
-0002fa70: 6f63 286e 6f64 652e 6765 7428 2264 6573  oc(node.get("des
-0002fa80: 6372 6970 7469 6f6e 222c 2022 2229 2929  cription", "")))
-0002fa90: 0a20 2020 2066 6f72 6d61 745f 6e6f 6465  .    format_node
-0002faa0: 5f73 716c 2866 696c 655f 7061 7274 732c  _sql(file_parts,
-0002fab0: 206e 6f64 652c 206c 696e 655f 6c65 6e67   node, line_leng
-0002fac0: 7468 3d6c 696e 655f 6c65 6e67 7468 2c20  th=line_length, 
-0002fad0: 6c6f 7765 725f 6b65 7977 6f72 6473 3d6c  lower_keywords=l
-0002fae0: 6f77 6572 5f6b 6579 776f 7264 7329 0a20  ower_keywords). 
-0002faf0: 2020 2061 7761 6974 2066 6f72 6d61 745f     await format_
-0002fb00: 6e6f 6465 5f74 7970 6528 6669 6c65 5f70  node_type(file_p
-0002fb10: 6172 7473 2c20 6e6f 6465 290a 0a0a 6173  arts, node)...as
-0002fb20: 796e 6320 6465 6620 666f 726d 6174 5f70  ync def format_p
-0002fb30: 6970 6528 0a20 2020 2066 696c 656e 616d  ipe(.    filenam
-0002fb40: 653a 2073 7472 2c0a 2020 2020 6c69 6e65  e: str,.    line
-0002fb50: 5f6c 656e 6774 683a 204f 7074 696f 6e61  _length: Optiona
-0002fb60: 6c5b 696e 745d 2c0a 2020 2020 756e 726f  l[int],.    unro
-0002fb70: 6c6c 5f69 6e63 6c75 6465 733a 2062 6f6f  ll_includes: boo
-0002fb80: 6c20 3d20 4661 6c73 652c 0a20 2020 2072  l = False,.    r
-0002fb90: 6570 6c61 6365 5f69 6e63 6c75 6465 733a  eplace_includes:
-0002fba0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0002fbb0: 2020 2064 6174 6166 696c 653a 204f 7074     datafile: Opt
-0002fbc0: 696f 6e61 6c5b 4461 7461 6669 6c65 5d20  ional[Datafile] 
-0002fbd0: 3d20 4e6f 6e65 2c0a 2020 2020 666f 725f  = None,.    for_
-0002fbe0: 6465 706c 6f79 5f64 6966 663a 2062 6f6f  deploy_diff: boo
-0002fbf0: 6c20 3d20 4661 6c73 652c 0a20 2020 2073  l = False,.    s
-0002fc00: 6b69 705f 6576 616c 3a20 626f 6f6c 203d  kip_eval: bool =
-0002fc10: 2046 616c 7365 2c0a 2920 2d3e 2073 7472   False,.) -> str
-0002fc20: 3a0a 2020 2020 6966 2064 6174 6166 696c  :.    if datafil
-0002fc30: 653a 0a20 2020 2020 2020 2064 6f63 203d  e:.        doc =
-0002fc40: 2064 6174 6166 696c 650a 2020 2020 656c   datafile.    el
-0002fc50: 7365 3a0a 2020 2020 2020 2020 646f 6320  se:.        doc 
-0002fc60: 3d20 7061 7273 655f 7069 7065 2866 696c  = parse_pipe(fil
-0002fc70: 656e 616d 652c 2072 6570 6c61 6365 5f69  ename, replace_i
-0002fc80: 6e63 6c75 6465 733d 7265 706c 6163 655f  ncludes=replace_
-0002fc90: 696e 636c 7564 6573 2c20 736b 6970 5f65  includes, skip_e
-0002fca0: 7661 6c3d 736b 6970 5f65 7661 6c29 0a0a  val=skip_eval)..
-0002fcb0: 2020 2020 6669 6c65 5f70 6172 7473 3a20      file_parts: 
-0002fcc0: 4c69 7374 5b73 7472 5d20 3d20 5b5d 0a20  List[str] = []. 
-0002fcd0: 2020 2066 6f72 6d61 745f 736f 7572 6365     format_source
-0002fce0: 7328 6669 6c65 5f70 6172 7473 2c20 646f  s(file_parts, do
-0002fcf0: 6329 0a20 2020 2066 6f72 6d61 745f 6d61  c).    format_ma
-0002fd00: 696e 7461 696e 6572 2866 696c 655f 7061  intainer(file_pa
-0002fd10: 7274 732c 2064 6f63 290a 2020 2020 666f  rts, doc).    fo
-0002fd20: 726d 6174 5f76 6572 7369 6f6e 2866 696c  rmat_version(fil
-0002fd30: 655f 7061 7274 732c 2064 6f63 290a 2020  e_parts, doc).  
-0002fd40: 2020 666f 726d 6174 5f64 6573 6372 6970    format_descrip
-0002fd50: 7469 6f6e 2866 696c 655f 7061 7274 732c  tion(file_parts,
-0002fd60: 2064 6f63 290a 2020 2020 666f 726d 6174   doc).    format
-0002fd70: 5f74 6f6b 656e 7328 6669 6c65 5f70 6172  _tokens(file_par
-0002fd80: 7473 2c20 646f 6329 0a20 2020 2069 6620  ts, doc).    if 
-0002fd90: 646f 632e 696e 636c 7564 6573 2061 6e64  doc.includes and
-0002fda0: 206e 6f74 2075 6e72 6f6c 6c5f 696e 636c   not unroll_incl
-0002fdb0: 7564 6573 3a0a 2020 2020 2020 2020 666f  udes:.        fo
-0002fdc0: 7220 6b20 696e 2064 6f63 2e69 6e63 6c75  r k in doc.inclu
-0002fdd0: 6465 733a 0a20 2020 2020 2020 2020 2020  des:.           
-0002fde0: 2023 2057 6520 6669 6c74 6572 206f 6e6c   # We filter onl
-0002fdf0: 7920 7468 6520 696e 636c 7564 6520 6669  y the include fi
-0002fe00: 6c65 7320 6173 2077 6520 6375 7272 656e  les as we curren
-0002fe10: 746c 7920 6861 7665 2032 2069 7465 6d73  tly have 2 items
-0002fe20: 2066 6f72 2065 6163 6820 696e 636c 7564   for each includ
-0002fe30: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-0002fe40: 7b20 2769 6e63 6c75 6465 5f66 696c 652e  { 'include_file.
-0002fe50: 696e 636c 273a 2027 4669 7273 7420 6e6f  incl': 'First no
-0002fe60: 6465 206f 6620 7468 6520 696e 636c 7564  de of the includ
-0002fe70: 6522 207d 0a20 2020 2020 2020 2020 2020  e" }.           
-0002fe80: 2023 207b 2027 6669 7273 7420 6e6f 6465   # { 'first node
-0002fe90: 206f 6620 7468 6520 7069 7065 2061 6674   of the pipe aft
-0002fea0: 6572 2074 6865 2069 6e63 6c75 6465 273a  er the include':
-0002feb0: 207d 0a20 2020 2020 2020 2020 2020 2069   }.            i
-0002fec0: 6620 222e 696e 636c 2220 6e6f 7420 696e  f ".incl" not in
-0002fed0: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
-0002fee0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-0002fef0: 2020 2020 2020 2020 2020 2320 5765 2067            # We g
-0002ff00: 6574 2061 6c6c 2074 6865 206e 6f64 6573  et all the nodes
-0002ff10: 2069 6e73 6964 6520 7468 6520 696e 636c   inside the incl
-0002ff20: 7564 6520 616e 6420 7265 6d6f 7665 2074  ude and remove t
-0002ff30: 6865 6d20 6672 6f6d 2074 6865 2075 6e72  hem from the unr
-0002ff40: 6f6c 6c65 6420 7069 7065 2061 7320 7765  olled pipe as we
-0002ff50: 2077 616e 7420 7468 696e 6773 2075 6e72   want things unr
-0002ff60: 6f6c 6c65 640a 2020 2020 2020 2020 2020  olled.          
-0002ff70: 2020 696e 636c 7564 655f 7061 7261 6d65    include_parame
-0002ff80: 7465 7273 203d 205f 756e 7175 6f74 6528  ters = _unquote(
-0002ff90: 6b29 0a0a 2020 2020 2020 2020 2020 2020  k)..            
-0002ffa0: 2320 4966 2074 6865 7920 7573 6520 616e  # If they use an
-0002ffb0: 2069 6e63 6c75 6465 2077 6974 6820 7061   include with pa
-0002ffc0: 7261 6d65 7465 7273 206c 696b 6520 6049  rameters like `I
-0002ffd0: 4e43 4c55 4445 2022 7878 782e 696e 636c  NCLUDE "xxx.incl
-0002ffe0: 2220 2247 524f 5550 5f43 4f4c 3d70 6174  " "GROUP_COL=pat
-0002fff0: 6822 2022 4d41 5445 5249 414c 495a 4544  h" "MATERIALIZED
-00030000: 5f56 4945 573d 7370 6565 645f 696e 7369  _VIEW=speed_insi
-00030010: 6768 7473 5f70 6174 685f 6461 696c 795f  ghts_path_daily_
-00030020: 6d76 2260 600a 2020 2020 2020 2020 2020  mv"``.          
-00030030: 2020 2320 5765 206a 7573 7420 7761 6e74    # We just want
-00030040: 2074 6865 2066 696c 6520 6e61 6d65 2074   the file name t
-00030050: 6f20 7461 6b65 206e 6f64 6573 0a20 2020  o take nodes.   
-00030060: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00030070: 5f66 696c 6520 3d20 696e 636c 7564 655f  _file = include_
-00030080: 7061 7261 6d65 7465 7273 2e73 706c 6974  parameters.split
-00030090: 2827 2227 295b 305d 0a20 2020 2020 2020  ('"')[0].       
-000300a0: 2020 2020 2069 6e63 6c75 6465 5f66 696c       include_fil
-000300b0: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
-000300c0: 2020 2020 2020 5061 7468 286f 732e 7061        Path(os.pa
-000300d0: 7468 2e64 6972 6e61 6d65 2866 696c 656e  th.dirname(filen
-000300e0: 616d 6529 2920 2f20 6576 616c 5f76 6172  ame)) / eval_var
-000300f0: 2869 6e63 6c75 6465 5f66 696c 6529 0a20  (include_file). 
-00030100: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00030110: 6620 222e 2220 696e 2069 6e63 6c75 6465  f "." in include
-00030120: 5f66 696c 650a 2020 2020 2020 2020 2020  _file.          
-00030130: 2020 2020 2020 656c 7365 2065 7661 6c5f        else eval_
-00030140: 7661 7228 696e 636c 7564 655f 6669 6c65  var(include_file
-00030150: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00030160: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-00030170: 7564 6564 5f70 6970 6520 3d20 7061 7273  uded_pipe = pars
-00030180: 655f 7069 7065 2869 6e63 6c75 6465 5f66  e_pipe(include_f
-00030190: 696c 652c 2073 6b69 705f 6576 616c 3d73  ile, skip_eval=s
-000301a0: 6b69 705f 6576 616c 290a 2020 2020 2020  kip_eval).      
-000301b0: 2020 2020 2020 7069 7065 5f6e 6f64 6573        pipe_nodes
-000301c0: 203d 2064 6f63 2e6e 6f64 6573 2e63 6f70   = doc.nodes.cop
-000301d0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-000301e0: 666f 7220 696e 636c 7564 6564 5f6e 6f64  for included_nod
-000301f0: 6520 696e 2069 6e63 6c75 6465 645f 7069  e in included_pi
-00030200: 7065 2e6e 6f64 6573 2e63 6f70 7928 293a  pe.nodes.copy():
-00030210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030220: 2075 6e72 6f6c 6c65 645f 696e 636c 7564   unrolled_includ
-00030230: 6564 5f6e 6f64 6520 3d20 6e65 7874 280a  ed_node = next(.
-00030240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030250: 2020 2020 286e 6f64 6520 666f 7220 6e6f      (node for no
-00030260: 6465 2069 6e20 7069 7065 5f6e 6f64 6573  de in pipe_nodes
-00030270: 2069 6620 6e6f 6465 5b22 6e61 6d65 225d   if node["name"]
-00030280: 203d 3d20 696e 636c 7564 6564 5f6e 6f64   == included_nod
-00030290: 655b 226e 616d 6522 5d29 2c20 4e6f 6e65  e["name"]), None
-000302a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000302b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000302c0: 2020 2069 6620 756e 726f 6c6c 6564 5f69     if unrolled_i
-000302d0: 6e63 6c75 6465 645f 6e6f 6465 3a0a 2020  ncluded_node:.  
-000302e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000302f0: 2020 646f 632e 6e6f 6465 732e 7265 6d6f    doc.nodes.remo
-00030300: 7665 2875 6e72 6f6c 6c65 645f 696e 636c  ve(unrolled_incl
-00030310: 7564 6564 5f6e 6f64 6529 0a20 2020 2066  uded_node).    f
-00030320: 6f72 206e 6f64 6520 696e 2064 6f63 2e6e  or node in doc.n
-00030330: 6f64 6573 3a0a 2020 2020 2020 2020 6177  odes:.        aw
-00030340: 6169 7420 666f 726d 6174 5f6e 6f64 6528  ait format_node(
-00030350: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00030360: 655f 7061 7274 732c 0a20 2020 2020 2020  e_parts,.       
-00030370: 2020 2020 206e 6f64 652c 0a20 2020 2020       node,.     
-00030380: 2020 2020 2020 2064 6f63 2e69 6e63 6c75         doc.inclu
-00030390: 6465 732c 0a20 2020 2020 2020 2020 2020  des,.           
-000303a0: 206c 696e 655f 6c65 6e67 7468 3d6c 696e   line_length=lin
-000303b0: 655f 6c65 6e67 7468 2c0a 2020 2020 2020  e_length,.      
-000303c0: 2020 2020 2020 756e 726f 6c6c 5f69 6e63        unroll_inc
-000303d0: 6c75 6465 733d 756e 726f 6c6c 5f69 6e63  ludes=unroll_inc
-000303e0: 6c75 6465 732c 0a20 2020 2020 2020 2020  ludes,.         
-000303f0: 2020 206c 6f77 6572 5f6b 6579 776f 7264     lower_keyword
-00030400: 733d 5472 7565 2069 6620 666f 725f 6465  s=True if for_de
-00030410: 706c 6f79 5f64 6966 6620 656c 7365 2046  ploy_diff else F
-00030420: 616c 7365 2c0a 2020 2020 2020 2020 290a  alse,.        ).
-00030430: 0a20 2020 2069 6620 6e6f 7420 756e 726f  .    if not unro
-00030440: 6c6c 5f69 6e63 6c75 6465 733a 0a20 2020  ll_includes:.   
-00030450: 2020 2020 2066 6f72 206b 2c20 5f20 696e       for k, _ in
-00030460: 2064 6f63 2e69 6e63 6c75 6465 732e 6974   doc.includes.it
-00030470: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00030480: 2020 2069 6620 222e 696e 636c 2220 6e6f     if ".incl" no
-00030490: 7420 696e 206b 3a0a 2020 2020 2020 2020  t in k:.        
-000304a0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-000304b0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-000304c0: 655f 7061 7274 732e 6170 7065 6e64 2866  e_parts.append(f
-000304d0: 2249 4e43 4c55 4445 207b 6b7d 2229 0a20  "INCLUDE {k}"). 
-000304e0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-000304f0: 7061 7274 732e 6170 7065 6e64 2844 4154  parts.append(DAT
-00030500: 4146 494c 455f 4e45 575f 4c49 4e45 290a  AFILE_NEW_LINE).
-00030510: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00030520: 5f70 6172 7473 2e61 7070 656e 6428 4441  _parts.append(DA
-00030530: 5441 4649 4c45 5f4e 4557 5f4c 494e 4529  TAFILE_NEW_LINE)
-00030540: 0a0a 2020 2020 7265 7375 6c74 203d 2022  ..    result = "
-00030550: 222e 6a6f 696e 2866 696c 655f 7061 7274  ".join(file_part
-00030560: 7329 0a20 2020 2072 6573 756c 7420 3d20  s).    result = 
-00030570: 7265 7375 6c74 2e72 7374 7269 7028 225c  result.rstrip("\
-00030580: 6e22 2920 2b20 225c 6e22 0a20 2020 2072  n") + "\n".    r
-00030590: 6574 7572 6e20 7265 7375 6c74 0a0a 0a64  eturn result...d
-000305a0: 6566 2066 6f72 6d61 745f 7371 6c28 7371  ef format_sql(sq
-000305b0: 6c3a 2073 7472 2c20 4441 5441 4649 4c45  l: str, DATAFILE
-000305c0: 5f49 4e44 454e 543a 2073 7472 2c20 6c69  _INDENT: str, li
-000305d0: 6e65 5f6c 656e 6774 683a 204f 7074 696f  ne_length: Optio
-000305e0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-000305f0: 206c 6f77 6572 5f6b 6579 776f 7264 733a   lower_keywords:
-00030600: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-00030610: 3e20 7374 723a 0a20 2020 2073 716c 203d  > str:.    sql =
-00030620: 2066 6f72 6d61 745f 7371 6c5f 7465 6d70   format_sql_temp
-00030630: 6c61 7465 2873 716c 2e73 7472 6970 2829  late(sql.strip()
-00030640: 2c20 6c69 6e65 5f6c 656e 6774 683d 6c69  , line_length=li
-00030650: 6e65 5f6c 656e 6774 682c 206c 6f77 6572  ne_length, lower
-00030660: 5f6b 6579 776f 7264 733d 6c6f 7765 725f  _keywords=lower_
-00030670: 6b65 7977 6f72 6473 290a 2020 2020 7265  keywords).    re
-00030680: 7475 726e 2022 5c6e 222e 6a6f 696e 285b  turn "\n".join([
-00030690: 6622 7b44 4154 4146 494c 455f 494e 4445  f"{DATAFILE_INDE
-000306a0: 4e54 7d7b 7061 7274 7d22 2066 6f72 2070  NT}{part}" for p
-000306b0: 6172 7420 696e 2073 716c 2e73 706c 6974  art in sql.split
-000306c0: 2822 5c6e 2229 2069 6620 6c65 6e28 7061  ("\n") if len(pa
-000306d0: 7274 2e73 7472 6970 2829 295d 290a 0a0a  rt.strip())])...
-000306e0: 6173 796e 6320 6465 6620 5f67 6174 6865  async def _gathe
-000306f0: 725f 7769 7468 5f63 6f6e 6375 7272 656e  r_with_concurren
-00030700: 6379 286e 2c20 2a74 6173 6b73 293a 0a20  cy(n, *tasks):. 
-00030710: 2020 2073 656d 6170 686f 7265 203d 2053     semaphore = S
-00030720: 656d 6170 686f 7265 286e 290a 0a20 2020  emaphore(n)..   
-00030730: 2061 7379 6e63 2064 6566 2073 656d 5f74   async def sem_t
-00030740: 6173 6b28 7461 736b 293a 0a20 2020 2020  ask(task):.     
-00030750: 2020 2061 7379 6e63 2077 6974 6820 7365     async with se
-00030760: 6d61 7068 6f72 653a 0a20 2020 2020 2020  maphore:.       
-00030770: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-00030780: 7420 7461 736b 0a0a 2020 2020 7265 7475  t task..    retu
-00030790: 726e 2061 7761 6974 2067 6174 6865 7228  rn await gather(
-000307a0: 2a28 7365 6d5f 7461 736b 2874 6173 6b29  *(sem_task(task)
-000307b0: 2066 6f72 2074 6173 6b20 696e 2074 6173   for task in tas
-000307c0: 6b73 2929 0a0a 0a61 7379 6e63 2064 6566  ks))...async def
-000307d0: 2066 6f6c 6465 725f 7075 6c6c 280a 2020   folder_pull(.  
-000307e0: 2020 636c 6965 6e74 3a20 5469 6e79 422c    client: TinyB,
-000307f0: 0a20 2020 2066 6f6c 6465 723a 2073 7472  .    folder: str
-00030800: 2c0a 2020 2020 6175 746f 3a20 626f 6f6c  ,.    auto: bool
-00030810: 2c0a 2020 2020 6d61 7463 683a 204f 7074  ,.    match: Opt
-00030820: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
-00030830: 666f 7263 653a 2062 6f6f 6c2c 0a20 2020  force: bool,.   
-00030840: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
-00030850: 2054 7275 652c 0a20 2020 2070 726f 6772   True,.    progr
-00030860: 6573 735f 6261 723a 2062 6f6f 6c20 3d20  ess_bar: bool = 
-00030870: 4661 6c73 652c 0a29 3a20 2023 206e 6f71  False,.):  # noq
-00030880: 613a 2043 3930 310a 2020 2020 7061 7474  a: C901.    patt
-00030890: 6572 6e20 3d20 7265 2e63 6f6d 7069 6c65  ern = re.compile
-000308a0: 286d 6174 6368 2920 6966 206d 6174 6368  (match) if match
-000308b0: 2065 6c73 6520 4e6f 6e65 0a0a 2020 2020   else None..    
-000308c0: 6465 6620 5f67 6574 5f6c 6174 6573 745f  def _get_latest_
-000308d0: 7665 7273 696f 6e73 2872 6573 6f75 7263  versions(resourc
-000308e0: 6573 3a20 4c69 7374 5b73 7472 5d29 3a0a  es: List[str]):.
-000308f0: 2020 2020 2020 2020 7665 7273 696f 6e73          versions
-00030900: 3a20 4469 6374 5b73 7472 2c20 416e 795d  : Dict[str, Any]
-00030910: 203d 207b 7d0a 0a20 2020 2020 2020 2066   = {}..        f
-00030920: 6f72 2078 2069 6e20 7265 736f 7572 6365  or x in resource
-00030930: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-00030940: 203d 2067 6574 5f6e 616d 655f 7665 7273   = get_name_vers
-00030950: 696f 6e28 7829 0a20 2020 2020 2020 2020  ion(x).         
-00030960: 2020 2074 5b22 6f72 6967 696e 616c 5f6e     t["original_n
-00030970: 616d 6522 5d20 3d20 780a 2020 2020 2020  ame"] = x.      
-00030980: 2020 2020 2020 6966 2074 5b22 7665 7273        if t["vers
-00030990: 696f 6e22 5d20 6973 204e 6f6e 653a 0a20  ion"] is None:. 
-000309a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000309b0: 5b22 7665 7273 696f 6e22 5d20 3d20 2d31  ["version"] = -1
-000309c0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-000309d0: 6520 3d20 745b 226e 616d 6522 5d0a 0a20  e = t["name"].. 
-000309e0: 2020 2020 2020 2020 2020 2069 6620 6e61             if na
-000309f0: 6d65 206e 6f74 2069 6e20 7665 7273 696f  me not in versio
-00030a00: 6e73 206f 7220 6e61 6d65 203d 3d20 7820  ns or name == x 
-00030a10: 6f72 2076 6572 7369 6f6e 735b 6e61 6d65  or versions[name
-00030a20: 5d5b 2276 6572 7369 6f6e 225d 203c 2074  ]["version"] < t
-00030a30: 5b22 7665 7273 696f 6e22 5d3a 0a20 2020  ["version"]:.   
-00030a40: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00030a50: 7369 6f6e 735b 6e61 6d65 5d20 3d20 740a  sions[name] = t.
-00030a60: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-00030a70: 6572 7369 6f6e 730a 0a20 2020 2064 6566  ersions..    def
-00030a80: 2067 6574 5f66 696c 655f 666f 6c64 6572   get_file_folder
-00030a90: 2865 7874 656e 7369 6f6e 3a20 7374 7229  (extension: str)
-00030aa0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00030ab0: 2061 7574 6f3a 0a20 2020 2020 2020 2020   auto:.         
-00030ac0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00030ad0: 2020 2020 2020 2069 6620 6578 7465 6e73         if extens
-00030ae0: 696f 6e20 3d3d 2022 6461 7461 736f 7572  ion == "datasour
-00030af0: 6365 223a 0a20 2020 2020 2020 2020 2020  ce":.           
-00030b00: 2072 6574 7572 6e20 2264 6174 6173 6f75   return "datasou
-00030b10: 7263 6573 220a 2020 2020 2020 2020 6966  rces".        if
-00030b20: 2065 7874 656e 7369 6f6e 203d 3d20 2270   extension == "p
-00030b30: 6970 6522 3a0a 2020 2020 2020 2020 2020  ipe":.          
-00030b40: 2020 7265 7475 726e 2022 7069 7065 7322    return "pipes"
-00030b50: 0a20 2020 2020 2020 2069 6620 6578 7465  .        if exte
-00030b60: 6e73 696f 6e20 3d3d 2022 746f 6b65 6e22  nsion == "token"
-00030b70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00030b80: 7475 726e 2022 746f 6b65 6e73 220a 2020  turn "tokens".  
-00030b90: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00030ba0: 650a 0a20 2020 2061 7379 6e63 2064 6566  e..    async def
-00030bb0: 2077 7269 7465 5f66 696c 6573 280a 2020   write_files(.  
-00030bc0: 2020 2020 2020 7665 7273 696f 6e73 3a20        versions: 
-00030bd0: 4469 6374 5b73 7472 2c20 416e 795d 2c0a  Dict[str, Any],.
-00030be0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00030bf0: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
-00030c00: 2020 2020 2020 6578 7465 6e73 696f 6e3a        extension:
-00030c10: 2073 7472 2c0a 2020 2020 2020 2020 6765   str,.        ge
-00030c20: 745f 7265 736f 7572 6365 5f66 756e 6374  t_resource_funct
-00030c30: 696f 6e3a 2073 7472 2c0a 2020 2020 2020  ion: str,.      
-00030c40: 2020 7072 6f67 7265 7373 5f62 6172 3a20    progress_bar: 
-00030c50: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00030c60: 2020 293a 0a20 2020 2020 2020 2061 7379    ):.        asy
-00030c70: 6e63 2064 6566 2077 7269 7465 5f72 6573  nc def write_res
-00030c80: 6f75 7263 6528 6b3a 2044 6963 745b 7374  ource(k: Dict[st
-00030c90: 722c 2041 6e79 5d29 3a0a 2020 2020 2020  r, Any]):.      
-00030ca0: 2020 2020 2020 6e61 6d65 203d 2066 227b        name = f"{
-00030cb0: 6b5b 276e 616d 6527 5d7d 2e7b 6578 7465  k['name']}.{exte
-00030cc0: 6e73 696f 6e7d 220a 2020 2020 2020 2020  nsion}".        
-00030cd0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00030ce0: 2020 2020 2020 2020 2069 6620 7061 7474           if patt
-00030cf0: 6572 6e20 616e 6420 6e6f 7420 7061 7474  ern and not patt
-00030d00: 6572 6e2e 7365 6172 6368 286e 616d 6529  ern.search(name)
-00030d10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00030d20: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-00030d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00030d40: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-00030d50: 6563 686f 2846 6565 6462 6163 6b4d 616e  echo(FeedbackMan
-00030d60: 6167 6572 2e69 6e66 6f5f 736b 6970 7069  ager.info_skippi
-00030d70: 6e67 5f72 6573 6f75 7263 6528 7265 736f  ng_resource(reso
-00030d80: 7572 6365 3d6e 616d 6529 290a 2020 2020  urce=name)).    
-00030d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030da0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-00030db0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00030dc0: 203d 2061 7761 6974 2067 6574 6174 7472   = await getattr
-00030dd0: 2863 6c69 656e 742c 2067 6574 5f72 6573  (client, get_res
-00030de0: 6f75 7263 655f 6675 6e63 7469 6f6e 2928  ource_function)(
-00030df0: 6b5b 226f 7269 6769 6e61 6c5f 6e61 6d65  k["original_name
-00030e00: 225d 290a 0a20 2020 2020 2020 2020 2020  "])..           
-00030e10: 2020 2020 2064 6573 745f 666f 6c64 6572       dest_folder
-00030e20: 203d 2066 6f6c 6465 720a 2020 2020 2020   = folder.      
-00030e30: 2020 2020 2020 2020 2020 6966 2022 2e22            if "."
-00030e40: 2069 6e20 6b5b 226e 616d 6522 5d20 616e   in k["name"] an
-00030e50: 6420 6578 7465 6e73 696f 6e20 213d 2022  d extension != "
-00030e60: 746f 6b65 6e22 3a0a 2020 2020 2020 2020  token":.        
-00030e70: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00030e80: 5f66 6f6c 6465 7220 3d20 5061 7468 2866  _folder = Path(f
-00030e90: 6f6c 6465 7229 202f 2022 7665 6e64 6f72  older) / "vendor
-00030ea0: 2220 2f20 6b5b 226e 616d 6522 5d2e 7370  " / k["name"].sp
-00030eb0: 6c69 7428 222e 222c 2031 295b 305d 0a20  lit(".", 1)[0]. 
-00030ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ed0: 2020 206e 616d 6520 3d20 6622 7b6b 5b27     name = f"{k['
-00030ee0: 6e61 6d65 275d 2e73 706c 6974 2827 2e27  name'].split('.'
-00030ef0: 2c20 3129 5b31 5d7d 2e7b 6578 7465 6e73  , 1)[1]}.{extens
-00030f00: 696f 6e7d 220a 0a20 2020 2020 2020 2020  ion}"..         
-00030f10: 2020 2020 2020 2066 696c 655f 666f 6c64         file_fold
-00030f20: 6572 203d 2067 6574 5f66 696c 655f 666f  er = get_file_fo
-00030f30: 6c64 6572 2865 7874 656e 7369 6f6e 290a  lder(extension).
-00030f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030f50: 6620 3d20 5061 7468 2864 6573 745f 666f  f = Path(dest_fo
-00030f60: 6c64 6572 2920 2f20 6669 6c65 5f66 6f6c  lder) / file_fol
-00030f70: 6465 7220 6966 2066 696c 655f 666f 6c64  der if file_fold
-00030f80: 6572 2069 7320 6e6f 7420 4e6f 6e65 2065  er is not None e
-00030f90: 6c73 6520 5061 7468 2864 6573 745f 666f  lse Path(dest_fo
-00030fa0: 6c64 6572 290a 0a20 2020 2020 2020 2020  lder)..         
-00030fb0: 2020 2020 2020 2069 6620 6e6f 7420 662e         if not f.
-00030fc0: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-00030fd0: 2020 2020 2020 2020 2020 2020 2020 662e                f.
-00030fe0: 6d6b 6469 7228 7061 7265 6e74 733d 5472  mkdir(parents=Tr
-00030ff0: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
-00031000: 2020 2020 2066 203d 2066 202f 206e 616d       f = f / nam
-00031010: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00031020: 2020 7265 736f 7572 6365 5f6e 616d 6573    resource_names
-00031030: 203d 205b 782e 7370 6c69 7428 222e 2229   = [x.split(".")
-00031040: 5b2d 315d 2066 6f72 2078 2069 6e20 7265  [-1] for x in re
-00031050: 736f 7572 6365 735d 0a0a 2020 2020 2020  sources]..      
-00031060: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
-00031070: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
-00031080: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-00031090: 6563 686f 2846 6565 6462 6163 6b4d 616e  echo(FeedbackMan
-000310a0: 6167 6572 2e69 6e66 6f5f 7772 6974 696e  ager.info_writin
-000310b0: 675f 7265 736f 7572 6365 2872 6573 6f75  g_resource(resou
-000310c0: 7263 653d 6629 290a 2020 2020 2020 2020  rce=f)).        
-000310d0: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
-000310e0: 2e65 7869 7374 7328 2920 6f72 2066 6f72  .exists() or for
-000310f0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-00031100: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00031110: 6e28 662c 2022 7722 2920 6173 2066 643a  n(f, "w") as fd:
-00031120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00031130: 2020 2020 2020 2020 2023 2076 6572 7369           # versi
-00031140: 6f6e 7320 6172 6520 6120 636c 6965 6e74  ons are a client
-00031150: 206f 6e6c 7920 7468 696e 6720 736f 0a20   only thing so. 
-00031160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031170: 2020 2020 2020 2023 2064 6174 6166 696c         # datafil
-00031180: 6573 2066 726f 6d20 7468 6520 7365 7276  es from the serv
-00031190: 6572 2064 6f20 6e6f 7420 636f 6e74 6169  er do not contai
-000311a0: 6e73 2069 6e66 6f72 6d61 7469 6f6e 2061  ns information a
-000311b0: 626f 7574 2076 6572 7369 6f6e 730a 2020  bout versions.  
-000311c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000311d0: 2020 2020 2020 6966 206b 5b22 7665 7273        if k["vers
-000311e0: 696f 6e22 5d20 3e3d 2030 3a0a 2020 2020  ion"] >= 0:.    
-000311f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031200: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00031210: 203d 2066 2256 4552 5349 4f4e 207b 6b5b   = f"VERSION {k[
-00031220: 2776 6572 7369 6f6e 275d 7d5c 6e22 202b  'version']}\n" +
-00031230: 2072 6573 6f75 7263 650a 2020 2020 2020   resource.      
-00031240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031250: 2020 6966 2072 6573 6f75 7263 653a 0a20    if resource:. 
-00031260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031270: 2020 2020 2020 2020 2020 206d 6174 6368             match
-00031280: 6573 203d 2072 652e 6669 6e64 616c 6c28  es = re.findall(
-00031290: 7222 285b 5e5c 735c 2e5d 2a5f 5f76 5c64  r"([^\s\.]*__v\d
-000312a0: 2b29 222c 2072 6573 6f75 7263 6529 0a20  +)", resource). 
-000312b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000312c0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
-000312d0: 6174 6368 2069 6e20 7365 7428 6d61 7463  atch in set(matc
-000312e0: 6865 7329 3a0a 2020 2020 2020 2020 2020  hes):.          
+0002eaf0: 2020 2020 2020 2020 2020 666f 726d 6174            format
+0002eb00: 7465 645f 7474 6c20 3d20 7474 6c5f 7371  ted_ttl = ttl_sq
+0002eb10: 6c5b 373a 5d0a 2020 2020 2020 2020 2020  l[7:].          
+0002eb20: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0002eb30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002eb50: 666f 726d 6174 7465 645f 7474 6c20 3d20  formatted_ttl = 
+0002eb60: 656c 656d 0a20 2020 2020 2020 2020 2020  elem.           
+0002eb70: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0002eb80: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
+0002eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002eba0: 2020 2066 6f72 6d61 7474 6564 5f74 746c     formatted_ttl
+0002ebb0: 203d 2065 6c65 6d0a 2020 2020 2020 2020   = elem.        
+0002ebc0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+0002ebd0: 5f70 6172 7473 2e61 7070 656e 6428 6622  _parts.append(f"
+0002ebe0: 454e 4749 4e45 5f7b 6172 675b 305d 2e75  ENGINE_{arg[0].u
+0002ebf0: 7070 6572 2829 7d20 7b66 6f72 6d61 7474  pper()} {formatt
+0002ec00: 6564 5f74 746c 7d22 290a 2020 2020 2020  ed_ttl}").      
+0002ec10: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0002ec20: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
+0002ec30: 4441 5441 4649 4c45 5f4e 4557 5f4c 494e  DATAFILE_NEW_LIN
+0002ec40: 4529 0a20 2020 2020 2020 2020 2020 2066  E).            f
+0002ec50: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002ec60: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
+0002ec70: 4e45 290a 2020 2020 2020 2020 7265 7475  NE).        retu
+0002ec80: 726e 2066 696c 655f 7061 7274 730a 2020  rn file_parts.  
+0002ec90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002eca0: 6966 206e 6f64 652e 6765 7428 2265 6e67  if node.get("eng
+0002ecb0: 696e 6522 2c20 4e6f 6e65 293a 0a20 2020  ine", None):.   
+0002ecc0: 2020 2020 2020 2020 2065 6d70 7479 203d           empty =
+0002ecd0: 2027 2222 270a 2020 2020 2020 2020 2020   '""'.          
+0002ece0: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
+0002ecf0: 656e 6428 6627 454e 4749 4e45 207b 6e6f  end(f'ENGINE {no
+0002ed00: 6465 5b22 656e 6769 6e65 225d 5b22 7479  de["engine"]["ty
+0002ed10: 7065 225d 7d27 2069 6620 6e6f 6465 2e67  pe"]}' if node.g
+0002ed20: 6574 2822 656e 6769 6e65 222c 207b 7d29  et("engine", {})
+0002ed30: 2e67 6574 2822 7479 7065 2229 2065 6c73  .get("type") els
+0002ed40: 6520 656d 7074 7929 0a20 2020 2020 2020  e empty).       
+0002ed50: 2020 2020 2066 696c 655f 7061 7274 732e       file_parts.
+0002ed60: 6170 7065 6e64 2844 4154 4146 494c 455f  append(DATAFILE_
+0002ed70: 4e45 575f 4c49 4e45 290a 2020 2020 2020  NEW_LINE).      
+0002ed80: 2020 2020 2020 666f 7220 6172 6720 696e        for arg in
+0002ed90: 2073 6f72 7465 6428 6e6f 6465 5b22 656e   sorted(node["en
+0002eda0: 6769 6e65 225d 2e67 6574 2822 6172 6773  gine"].get("args
+0002edb0: 222c 205b 5d29 293a 0a20 2020 2020 2020  ", [])):.       
+0002edc0: 2020 2020 2020 2020 2065 6c65 6d20 3d20           elem = 
+0002edd0: 222c 2022 2e6a 6f69 6e28 5b78 2e73 7472  ", ".join([x.str
+0002ede0: 6970 2829 2066 6f72 2078 2069 6e20 6172  ip() for x in ar
+0002edf0: 675b 315d 2e73 706c 6974 2822 2c22 295d  g[1].split(",")]
+0002ee00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002ee10: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
+0002ee20: 656e 6428 6622 454e 4749 4e45 5f7b 6172  end(f"ENGINE_{ar
+0002ee30: 675b 305d 2e75 7070 6572 2829 7d20 7b65  g[0].upper()} {e
+0002ee40: 6c65 6d20 6966 2065 6c65 6d20 656c 7365  lem if elem else
+0002ee50: 2065 6d70 7479 7d22 290a 2020 2020 2020   empty}").      
+0002ee60: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
+0002ee70: 6172 7473 2e61 7070 656e 6428 4441 5441  arts.append(DATA
+0002ee80: 4649 4c45 5f4e 4557 5f4c 494e 4529 0a20  FILE_NEW_LINE). 
+0002ee90: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+0002eea0: 7061 7274 732e 6170 7065 6e64 2844 4154  parts.append(DAT
+0002eeb0: 4146 494c 455f 4e45 575f 4c49 4e45 290a  AFILE_NEW_LINE).
+0002eec0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+0002eed0: 696c 655f 7061 7274 730a 0a0a 6173 796e  ile_parts...asyn
+0002eee0: 6320 6465 6620 666f 726d 6174 5f6e 6f64  c def format_nod
+0002eef0: 655f 7479 7065 2866 696c 655f 7061 7274  e_type(file_part
+0002ef00: 733a 204c 6973 745b 7374 725d 2c20 6e6f  s: List[str], no
+0002ef10: 6465 3a20 4469 6374 5b73 7472 2c20 416e  de: Dict[str, An
+0002ef20: 795d 2920 2d3e 204c 6973 745b 7374 725d  y]) -> List[str]
+0002ef30: 3a0a 2020 2020 6e6f 6465 5f74 7970 6520  :.    node_type 
+0002ef40: 3d20 6e6f 6465 2e67 6574 2822 7479 7065  = node.get("type
+0002ef50: 222c 2022 2229 2e6c 6f77 6572 2829 0a20  ", "").lower(). 
+0002ef60: 2020 206e 6f64 655f 7479 7065 5f75 7070     node_type_upp
+0002ef70: 6572 203d 2066 2254 5950 4520 7b6e 6f64  er = f"TYPE {nod
+0002ef80: 655f 7479 7065 2e75 7070 6572 2829 7d22  e_type.upper()}"
+0002ef90: 0a0a 2020 2020 2320 4d61 7465 7269 616c  ..    # Material
+0002efa0: 697a 6564 2070 6970 650a 2020 2020 6966  ized pipe.    if
+0002efb0: 206e 6f64 655f 7479 7065 203d 3d20 5069   node_type == Pi
+0002efc0: 7065 4e6f 6465 5479 7065 732e 4d41 5445  peNodeTypes.MATE
+0002efd0: 5249 414c 495a 4544 3a0a 2020 2020 2020  RIALIZED:.      
+0002efe0: 2020 6669 6c65 5f70 6172 7473 2e61 7070    file_parts.app
+0002eff0: 656e 6428 6e6f 6465 5f74 7970 655f 7570  end(node_type_up
+0002f000: 7065 7229 0a20 2020 2020 2020 2066 696c  per).        fil
+0002f010: 655f 7061 7274 732e 6170 7065 6e64 2844  e_parts.append(D
+0002f020: 4154 4146 494c 455f 4e45 575f 4c49 4e45  ATAFILE_NEW_LINE
+0002f030: 290a 2020 2020 2020 2020 6669 6c65 5f70  ).        file_p
+0002f040: 6172 7473 2e61 7070 656e 6428 6627 4441  arts.append(f'DA
+0002f050: 5441 534f 5552 4345 207b 6e6f 6465 5b22  TASOURCE {node["
+0002f060: 6461 7461 736f 7572 6365 225d 7d27 290a  datasource"]}').
+0002f070: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
+0002f080: 7473 2e61 7070 656e 6428 4441 5441 4649  ts.append(DATAFI
+0002f090: 4c45 5f4e 4557 5f4c 494e 4529 0a20 2020  LE_NEW_LINE).   
+0002f0a0: 2020 2020 2061 7761 6974 2066 6f72 6d61       await forma
+0002f0b0: 745f 656e 6769 6e65 2866 696c 655f 7061  t_engine(file_pa
+0002f0c0: 7274 732c 206e 6f64 6529 0a0a 2020 2020  rts, node)..    
+0002f0d0: 2320 436f 7079 2070 6970 650a 2020 2020  # Copy pipe.    
+0002f0e0: 6966 206e 6f64 655f 7479 7065 203d 3d20  if node_type == 
+0002f0f0: 5069 7065 4e6f 6465 5479 7065 732e 434f  PipeNodeTypes.CO
+0002f100: 5059 3a0a 2020 2020 2020 2020 6669 6c65  PY:.        file
+0002f110: 5f70 6172 7473 2e61 7070 656e 6428 6e6f  _parts.append(no
+0002f120: 6465 5f74 7970 655f 7570 7065 7229 0a20  de_type_upper). 
+0002f130: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002f140: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
+0002f150: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
+0002f160: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
+0002f170: 7070 656e 6428 6627 5441 5247 4554 5f44  ppend(f'TARGET_D
+0002f180: 4154 4153 4f55 5243 4520 7b6e 6f64 655b  ATASOURCE {node[
+0002f190: 2274 6172 6765 745f 6461 7461 736f 7572  "target_datasour
+0002f1a0: 6365 225d 7d27 290a 2020 2020 2020 2020  ce"]}').        
+0002f1b0: 6966 2043 6f70 7950 6172 616d 6574 6572  if CopyParameter
+0002f1c0: 732e 434f 5059 5f53 4348 4544 554c 4520  s.COPY_SCHEDULE 
+0002f1d0: 696e 206e 6f64 6520 616e 6420 6e6f 6465  in node and node
+0002f1e0: 5b43 6f70 7950 6172 616d 6574 6572 732e  [CopyParameters.
+0002f1f0: 434f 5059 5f53 4348 4544 554c 455d 3a0a  COPY_SCHEDULE]:.
+0002f200: 2020 2020 2020 2020 2020 2020 6973 5f6f              is_o
+0002f210: 6e64 656d 616e 6420 3d20 6e6f 6465 5b43  ndemand = node[C
+0002f220: 6f70 7950 6172 616d 6574 6572 732e 434f  opyParameters.CO
+0002f230: 5059 5f53 4348 4544 554c 455d 2e6c 6f77  PY_SCHEDULE].low
+0002f240: 6572 2829 203d 3d20 4f4e 5f44 454d 414e  er() == ON_DEMAN
+0002f250: 440a 2020 2020 2020 2020 2020 2020 6669  D.            fi
+0002f260: 6c65 5f70 6172 7473 2e61 7070 656e 6428  le_parts.append(
+0002f270: 4441 5441 4649 4c45 5f4e 4557 5f4c 494e  DATAFILE_NEW_LIN
+0002f280: 4529 0a20 2020 2020 2020 2020 2020 2066  E).            f
+0002f290: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002f2a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0002f2b0: 2020 6622 7b43 6f70 7950 6172 616d 6574    f"{CopyParamet
+0002f2c0: 6572 732e 434f 5059 5f53 4348 4544 554c  ers.COPY_SCHEDUL
+0002f2d0: 452e 7570 7065 7228 297d 207b 4f4e 5f44  E.upper()} {ON_D
+0002f2e0: 454d 414e 4420 6966 2069 735f 6f6e 6465  EMAND if is_onde
+0002f2f0: 6d61 6e64 2065 6c73 6520 6e6f 6465 5b43  mand else node[C
+0002f300: 6f70 7950 6172 616d 6574 6572 732e 434f  opyParameters.CO
+0002f310: 5059 5f53 4348 4544 554c 455d 7d22 0a20  PY_SCHEDULE]}". 
+0002f320: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0002f330: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0002f340: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002f350: 732e 6170 7065 6e64 2844 4154 4146 494c  s.append(DATAFIL
+0002f360: 455f 4e45 575f 4c49 4e45 290a 2020 2020  E_NEW_LINE).    
+0002f370: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
+0002f380: 7473 2e61 7070 656e 6428 6622 7b43 6f70  ts.append(f"{Cop
+0002f390: 7950 6172 616d 6574 6572 732e 434f 5059  yParameters.COPY
+0002f3a0: 5f53 4348 4544 554c 452e 7570 7065 7228  _SCHEDULE.upper(
+0002f3b0: 297d 207b 4f4e 5f44 454d 414e 447d 2229  )} {ON_DEMAND}")
+0002f3c0: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
+0002f3d0: 7274 732e 6170 7065 6e64 2844 4154 4146  rts.append(DATAF
+0002f3e0: 494c 455f 4e45 575f 4c49 4e45 290a 0a20  ILE_NEW_LINE).. 
+0002f3f0: 2020 2023 2053 696e 6b20 7069 7065 0a20     # Sink pipe. 
+0002f400: 2020 2069 6620 4578 706f 7274 5265 706c     if ExportRepl
+0002f410: 6163 656d 656e 7473 2e69 735f 6578 706f  acements.is_expo
+0002f420: 7274 5f6e 6f64 6528 6e6f 6465 293a 0a20  rt_node(node):. 
+0002f430: 2020 2020 2020 2066 696c 655f 7061 7274         file_part
+0002f440: 732e 6170 7065 6e64 286e 6f64 655f 7479  s.append(node_ty
+0002f450: 7065 5f75 7070 6572 290a 2020 2020 2020  pe_upper).      
+0002f460: 2020 6578 706f 7274 5f70 6172 616d 7320    export_params 
+0002f470: 3d20 4578 706f 7274 5265 706c 6163 656d  = ExportReplacem
+0002f480: 656e 7473 2e67 6574 5f70 6172 616d 735f  ents.get_params_
+0002f490: 6672 6f6d 5f64 6174 6166 696c 6528 6e6f  from_datafile(no
+0002f4a0: 6465 290a 2020 2020 2020 2020 6669 6c65  de).        file
+0002f4b0: 5f70 6172 7473 2e61 7070 656e 6428 4441  _parts.append(DA
+0002f4c0: 5441 4649 4c45 5f4e 4557 5f4c 494e 4529  TAFILE_NEW_LINE)
+0002f4d0: 0a20 2020 2020 2020 2066 6f72 2070 6172  .        for par
+0002f4e0: 616d 2c20 7661 6c75 6520 696e 2065 7870  am, value in exp
+0002f4f0: 6f72 745f 7061 7261 6d73 2e69 7465 6d73  ort_params.items
+0002f500: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0002f510: 6966 2070 6172 616d 203d 3d20 2273 6368  if param == "sch
+0002f520: 6564 756c 655f 6372 6f6e 2220 616e 6420  edule_cron" and 
+0002f530: 6e6f 7420 7661 6c75 653a 0a20 2020 2020  not value:.     
+0002f540: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0002f550: 203d 204f 4e5f 4445 4d41 4e44 0a20 2020   = ON_DEMAND.   
+0002f560: 2020 2020 2020 2020 2064 6174 6166 696c           datafil
+0002f570: 655f 6b65 7920 3d20 4578 706f 7274 5265  e_key = ExportRe
+0002f580: 706c 6163 656d 656e 7473 2e67 6574 5f64  placements.get_d
+0002f590: 6174 6166 696c 655f 6b65 7928 7061 7261  atafile_key(para
+0002f5a0: 6d29 0a20 2020 2020 2020 2020 2020 2069  m).            i
+0002f5b0: 6620 6461 7461 6669 6c65 5f6b 6579 3a0a  f datafile_key:.
+0002f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f5d0: 6669 6c65 5f70 6172 7473 2e61 7070 656e  file_parts.appen
+0002f5e0: 6428 6622 7b64 6174 6166 696c 655f 6b65  d(f"{datafile_ke
+0002f5f0: 797d 207b 7661 6c75 657d 2229 0a20 2020  y} {value}").   
+0002f600: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0002f610: 655f 7061 7274 732e 6170 7065 6e64 2844  e_parts.append(D
+0002f620: 4154 4146 494c 455f 4e45 575f 4c49 4e45  ATAFILE_NEW_LINE
+0002f630: 290a 0a20 2020 2072 6574 7572 6e20 6669  )..    return fi
+0002f640: 6c65 5f70 6172 7473 0a0a 0a64 6566 2066  le_parts...def f
+0002f650: 6f72 6d61 745f 7069 7065 5f69 6e63 6c75  ormat_pipe_inclu
+0002f660: 6465 2866 696c 655f 7061 7274 733a 204c  de(file_parts: L
+0002f670: 6973 745b 7374 725d 2c20 6e6f 6465 3a20  ist[str], node: 
+0002f680: 4469 6374 5b73 7472 2c20 416e 795d 2c20  Dict[str, Any], 
+0002f690: 696e 636c 7564 6573 3a20 4469 6374 5b73  includes: Dict[s
+0002f6a0: 7472 2c20 416e 795d 2920 2d3e 204c 6973  tr, Any]) -> Lis
+0002f6b0: 745b 7374 725d 3a0a 2020 2020 6966 2069  t[str]:.    if i
+0002f6c0: 6e63 6c75 6465 733a 0a20 2020 2020 2020  ncludes:.       
+0002f6d0: 2066 6f72 206b 2c20 7620 696e 2069 6e63   for k, v in inc
+0002f6e0: 6c75 6465 732e 636f 7079 2829 2e69 7465  ludes.copy().ite
+0002f6f0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0002f700: 2020 6966 206e 6f64 655b 226e 616d 6522    if node["name"
+0002f710: 5d20 696e 2076 3a0a 2020 2020 2020 2020  ] in v:.        
+0002f720: 2020 2020 2020 2020 6669 6c65 5f70 6172          file_par
+0002f730: 7473 2e61 7070 656e 6428 6622 494e 434c  ts.append(f"INCL
+0002f740: 5544 4520 7b6b 7d22 290a 2020 2020 2020  UDE {k}").      
+0002f750: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
+0002f760: 6172 7473 2e61 7070 656e 6428 4441 5441  arts.append(DATA
+0002f770: 4649 4c45 5f4e 4557 5f4c 494e 4529 0a20  FILE_NEW_LINE). 
+0002f780: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002f790: 696c 655f 7061 7274 732e 6170 7065 6e64  ile_parts.append
+0002f7a0: 2844 4154 4146 494c 455f 4e45 575f 4c49  (DATAFILE_NEW_LI
+0002f7b0: 4e45 290a 2020 2020 2020 2020 2020 2020  NE).            
+0002f7c0: 2020 2020 6465 6c20 696e 636c 7564 6573      del includes
+0002f7d0: 5b6b 5d0a 2020 2020 7265 7475 726e 2066  [k].    return f
+0002f7e0: 696c 655f 7061 7274 730a 0a0a 6173 796e  ile_parts...asyn
+0002f7f0: 6320 6465 6620 666f 726d 6174 5f6e 6f64  c def format_nod
+0002f800: 6528 0a20 2020 2066 696c 655f 7061 7274  e(.    file_part
+0002f810: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
+0002f820: 2020 6e6f 6465 3a20 4469 6374 5b73 7472    node: Dict[str
+0002f830: 2c20 416e 795d 2c0a 2020 2020 696e 636c  , Any],.    incl
+0002f840: 7564 6573 3a20 4469 6374 5b73 7472 2c20  udes: Dict[str, 
+0002f850: 416e 795d 2c0a 2020 2020 6c69 6e65 5f6c  Any],.    line_l
+0002f860: 656e 6774 683a 204f 7074 696f 6e61 6c5b  ength: Optional[
+0002f870: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+0002f880: 2075 6e72 6f6c 6c5f 696e 636c 7564 6573   unroll_includes
+0002f890: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0002f8a0: 2020 2020 6c6f 7765 725f 6b65 7977 6f72      lower_keywor
+0002f8b0: 6473 3a20 626f 6f6c 203d 2046 616c 7365  ds: bool = False
+0002f8c0: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
+0002f8d0: 2069 6620 6e6f 7420 756e 726f 6c6c 5f69   if not unroll_i
+0002f8e0: 6e63 6c75 6465 733a 0a20 2020 2020 2020  ncludes:.       
+0002f8f0: 2066 6f72 6d61 745f 7069 7065 5f69 6e63   format_pipe_inc
+0002f900: 6c75 6465 2866 696c 655f 7061 7274 732c  lude(file_parts,
+0002f910: 206e 6f64 652c 2069 6e63 6c75 6465 7329   node, includes)
+0002f920: 0a20 2020 2069 7465 6d20 3d20 5b6b 2066  .    item = [k f
+0002f930: 6f72 206b 2c20 5f20 696e 2069 6e63 6c75  or k, _ in inclu
+0002f940: 6465 732e 6974 656d 7328 2920 6966 206e  des.items() if n
+0002f950: 6f64 655b 226e 616d 6522 5d2e 7374 7269  ode["name"].stri
+0002f960: 7028 2920 696e 206b 5d0a 2020 2020 6966  p() in k].    if
+0002f970: 2069 7465 6d20 616e 6420 6e6f 7420 756e   item and not un
+0002f980: 726f 6c6c 5f69 6e63 6c75 6465 733a 0a20  roll_includes:. 
+0002f990: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0002f9a0: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
+0002f9b0: 7065 6e64 2866 274e 4f44 4520 7b6e 6f64  pend(f'NODE {nod
+0002f9c0: 655b 226e 616d 6522 5d2e 7374 7269 7028  e["name"].strip(
+0002f9d0: 297d 2729 0a20 2020 2066 696c 655f 7061  )}').    file_pa
+0002f9e0: 7274 732e 6170 7065 6e64 2844 4154 4146  rts.append(DATAF
+0002f9f0: 494c 455f 4e45 575f 4c49 4e45 290a 0a20  ILE_NEW_LINE).. 
+0002fa00: 2020 2066 726f 6d20 636f 6c6c 6563 7469     from collecti
+0002fa10: 6f6e 7320 696d 706f 7274 206e 616d 6564  ons import named
+0002fa20: 7475 706c 650a 0a20 2020 2044 6f63 203d  tuple..    Doc =
+0002fa30: 206e 616d 6564 7475 706c 6528 2244 6f63   namedtuple("Doc
+0002fa40: 222c 205b 2264 6573 6372 6970 7469 6f6e  ", ["description
+0002fa50: 225d 290a 2020 2020 666f 726d 6174 5f64  "]).    format_d
+0002fa60: 6573 6372 6970 7469 6f6e 2866 696c 655f  escription(file_
+0002fa70: 7061 7274 732c 2044 6f63 286e 6f64 652e  parts, Doc(node.
+0002fa80: 6765 7428 2264 6573 6372 6970 7469 6f6e  get("description
+0002fa90: 222c 2022 2229 2929 0a20 2020 2066 6f72  ", ""))).    for
+0002faa0: 6d61 745f 6e6f 6465 5f73 716c 2866 696c  mat_node_sql(fil
+0002fab0: 655f 7061 7274 732c 206e 6f64 652c 206c  e_parts, node, l
+0002fac0: 696e 655f 6c65 6e67 7468 3d6c 696e 655f  ine_length=line_
+0002fad0: 6c65 6e67 7468 2c20 6c6f 7765 725f 6b65  length, lower_ke
+0002fae0: 7977 6f72 6473 3d6c 6f77 6572 5f6b 6579  ywords=lower_key
+0002faf0: 776f 7264 7329 0a20 2020 2061 7761 6974  words).    await
+0002fb00: 2066 6f72 6d61 745f 6e6f 6465 5f74 7970   format_node_typ
+0002fb10: 6528 6669 6c65 5f70 6172 7473 2c20 6e6f  e(file_parts, no
+0002fb20: 6465 290a 0a0a 6173 796e 6320 6465 6620  de)...async def 
+0002fb30: 666f 726d 6174 5f70 6970 6528 0a20 2020  format_pipe(.   
+0002fb40: 2066 696c 656e 616d 653a 2073 7472 2c0a   filename: str,.
+0002fb50: 2020 2020 6c69 6e65 5f6c 656e 6774 683a      line_length:
+0002fb60: 204f 7074 696f 6e61 6c5b 696e 745d 2c0a   Optional[int],.
+0002fb70: 2020 2020 756e 726f 6c6c 5f69 6e63 6c75      unroll_inclu
+0002fb80: 6465 733a 2062 6f6f 6c20 3d20 4661 6c73  des: bool = Fals
+0002fb90: 652c 0a20 2020 2072 6570 6c61 6365 5f69  e,.    replace_i
+0002fba0: 6e63 6c75 6465 733a 2062 6f6f 6c20 3d20  ncludes: bool = 
+0002fbb0: 4661 6c73 652c 0a20 2020 2064 6174 6166  False,.    dataf
+0002fbc0: 696c 653a 204f 7074 696f 6e61 6c5b 4461  ile: Optional[Da
+0002fbd0: 7461 6669 6c65 5d20 3d20 4e6f 6e65 2c0a  tafile] = None,.
+0002fbe0: 2020 2020 666f 725f 6465 706c 6f79 5f64      for_deploy_d
+0002fbf0: 6966 663a 2062 6f6f 6c20 3d20 4661 6c73  iff: bool = Fals
+0002fc00: 652c 0a20 2020 2073 6b69 705f 6576 616c  e,.    skip_eval
+0002fc10: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0002fc20: 2920 2d3e 2073 7472 3a0a 2020 2020 6966  ) -> str:.    if
+0002fc30: 2064 6174 6166 696c 653a 0a20 2020 2020   datafile:.     
+0002fc40: 2020 2064 6f63 203d 2064 6174 6166 696c     doc = datafil
+0002fc50: 650a 2020 2020 656c 7365 3a0a 2020 2020  e.    else:.    
+0002fc60: 2020 2020 646f 6320 3d20 7061 7273 655f      doc = parse_
+0002fc70: 7069 7065 2866 696c 656e 616d 652c 2072  pipe(filename, r
+0002fc80: 6570 6c61 6365 5f69 6e63 6c75 6465 733d  eplace_includes=
+0002fc90: 7265 706c 6163 655f 696e 636c 7564 6573  replace_includes
+0002fca0: 2c20 736b 6970 5f65 7661 6c3d 736b 6970  , skip_eval=skip
+0002fcb0: 5f65 7661 6c29 0a0a 2020 2020 6669 6c65  _eval)..    file
+0002fcc0: 5f70 6172 7473 3a20 4c69 7374 5b73 7472  _parts: List[str
+0002fcd0: 5d20 3d20 5b5d 0a20 2020 2066 6f72 6d61  ] = [].    forma
+0002fce0: 745f 736f 7572 6365 7328 6669 6c65 5f70  t_sources(file_p
+0002fcf0: 6172 7473 2c20 646f 6329 0a20 2020 2066  arts, doc).    f
+0002fd00: 6f72 6d61 745f 6d61 696e 7461 696e 6572  ormat_maintainer
+0002fd10: 2866 696c 655f 7061 7274 732c 2064 6f63  (file_parts, doc
+0002fd20: 290a 2020 2020 666f 726d 6174 5f76 6572  ).    format_ver
+0002fd30: 7369 6f6e 2866 696c 655f 7061 7274 732c  sion(file_parts,
+0002fd40: 2064 6f63 290a 2020 2020 666f 726d 6174   doc).    format
+0002fd50: 5f64 6573 6372 6970 7469 6f6e 2866 696c  _description(fil
+0002fd60: 655f 7061 7274 732c 2064 6f63 290a 2020  e_parts, doc).  
+0002fd70: 2020 666f 726d 6174 5f74 6f6b 656e 7328    format_tokens(
+0002fd80: 6669 6c65 5f70 6172 7473 2c20 646f 6329  file_parts, doc)
+0002fd90: 0a20 2020 2069 6620 646f 632e 696e 636c  .    if doc.incl
+0002fda0: 7564 6573 2061 6e64 206e 6f74 2075 6e72  udes and not unr
+0002fdb0: 6f6c 6c5f 696e 636c 7564 6573 3a0a 2020  oll_includes:.  
+0002fdc0: 2020 2020 2020 666f 7220 6b20 696e 2064        for k in d
+0002fdd0: 6f63 2e69 6e63 6c75 6465 733a 0a20 2020  oc.includes:.   
+0002fde0: 2020 2020 2020 2020 2023 2057 6520 6669           # We fi
+0002fdf0: 6c74 6572 206f 6e6c 7920 7468 6520 696e  lter only the in
+0002fe00: 636c 7564 6520 6669 6c65 7320 6173 2077  clude files as w
+0002fe10: 6520 6375 7272 656e 746c 7920 6861 7665  e currently have
+0002fe20: 2032 2069 7465 6d73 2066 6f72 2065 6163   2 items for eac
+0002fe30: 6820 696e 636c 7564 650a 2020 2020 2020  h include.      
+0002fe40: 2020 2020 2020 2320 7b20 2769 6e63 6c75        # { 'inclu
+0002fe50: 6465 5f66 696c 652e 696e 636c 273a 2027  de_file.incl': '
+0002fe60: 4669 7273 7420 6e6f 6465 206f 6620 7468  First node of th
+0002fe70: 6520 696e 636c 7564 6522 207d 0a20 2020  e include" }.   
+0002fe80: 2020 2020 2020 2020 2023 207b 2027 6669           # { 'fi
+0002fe90: 7273 7420 6e6f 6465 206f 6620 7468 6520  rst node of the 
+0002fea0: 7069 7065 2061 6674 6572 2074 6865 2069  pipe after the i
+0002feb0: 6e63 6c75 6465 273a 207d 0a20 2020 2020  nclude': }.     
+0002fec0: 2020 2020 2020 2069 6620 222e 696e 636c         if ".incl
+0002fed0: 2220 6e6f 7420 696e 206b 3a0a 2020 2020  " not in k:.    
+0002fee0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0002fef0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+0002ff00: 2020 2320 5765 2067 6574 2061 6c6c 2074    # We get all t
+0002ff10: 6865 206e 6f64 6573 2069 6e73 6964 6520  he nodes inside 
+0002ff20: 7468 6520 696e 636c 7564 6520 616e 6420  the include and 
+0002ff30: 7265 6d6f 7665 2074 6865 6d20 6672 6f6d  remove them from
+0002ff40: 2074 6865 2075 6e72 6f6c 6c65 6420 7069   the unrolled pi
+0002ff50: 7065 2061 7320 7765 2077 616e 7420 7468  pe as we want th
+0002ff60: 696e 6773 2075 6e72 6f6c 6c65 640a 2020  ings unrolled.  
+0002ff70: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+0002ff80: 655f 7061 7261 6d65 7465 7273 203d 205f  e_parameters = _
+0002ff90: 756e 7175 6f74 6528 6b29 0a0a 2020 2020  unquote(k)..    
+0002ffa0: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
+0002ffb0: 7920 7573 6520 616e 2069 6e63 6c75 6465  y use an include
+0002ffc0: 2077 6974 6820 7061 7261 6d65 7465 7273   with parameters
+0002ffd0: 206c 696b 6520 6049 4e43 4c55 4445 2022   like `INCLUDE "
+0002ffe0: 7878 782e 696e 636c 2220 2247 524f 5550  xxx.incl" "GROUP
+0002fff0: 5f43 4f4c 3d70 6174 6822 2022 4d41 5445  _COL=path" "MATE
+00030000: 5249 414c 495a 4544 5f56 4945 573d 7370  RIALIZED_VIEW=sp
+00030010: 6565 645f 696e 7369 6768 7473 5f70 6174  eed_insights_pat
+00030020: 685f 6461 696c 795f 6d76 2260 600a 2020  h_daily_mv"``.  
+00030030: 2020 2020 2020 2020 2020 2320 5765 206a            # We j
+00030040: 7573 7420 7761 6e74 2074 6865 2066 696c  ust want the fil
+00030050: 6520 6e61 6d65 2074 6f20 7461 6b65 206e  e name to take n
+00030060: 6f64 6573 0a20 2020 2020 2020 2020 2020  odes.           
+00030070: 2069 6e63 6c75 6465 5f66 696c 6520 3d20   include_file = 
+00030080: 696e 636c 7564 655f 7061 7261 6d65 7465  include_paramete
+00030090: 7273 2e73 706c 6974 2827 2227 295b 305d  rs.split('"')[0]
+000300a0: 0a20 2020 2020 2020 2020 2020 2069 6e63  .            inc
+000300b0: 6c75 6465 5f66 696c 6520 3d20 280a 2020  lude_file = (.  
+000300c0: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
+000300d0: 7468 286f 732e 7061 7468 2e64 6972 6e61  th(os.path.dirna
+000300e0: 6d65 2866 696c 656e 616d 6529 2920 2f20  me(filename)) / 
+000300f0: 6576 616c 5f76 6172 2869 6e63 6c75 6465  eval_var(include
+00030100: 5f66 696c 6529 0a20 2020 2020 2020 2020  _file).         
+00030110: 2020 2020 2020 2069 6620 222e 2220 696e         if "." in
+00030120: 2069 6e63 6c75 6465 5f66 696c 650a 2020   include_file.  
+00030130: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00030140: 7365 2065 7661 6c5f 7661 7228 696e 636c  se eval_var(incl
+00030150: 7564 655f 6669 6c65 290a 2020 2020 2020  ude_file).      
+00030160: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00030170: 2020 2020 696e 636c 7564 6564 5f70 6970      included_pip
+00030180: 6520 3d20 7061 7273 655f 7069 7065 2869  e = parse_pipe(i
+00030190: 6e63 6c75 6465 5f66 696c 652c 2073 6b69  nclude_file, ski
+000301a0: 705f 6576 616c 3d73 6b69 705f 6576 616c  p_eval=skip_eval
+000301b0: 290a 2020 2020 2020 2020 2020 2020 7069  ).            pi
+000301c0: 7065 5f6e 6f64 6573 203d 2064 6f63 2e6e  pe_nodes = doc.n
+000301d0: 6f64 6573 2e63 6f70 7928 290a 2020 2020  odes.copy().    
+000301e0: 2020 2020 2020 2020 666f 7220 696e 636c          for incl
+000301f0: 7564 6564 5f6e 6f64 6520 696e 2069 6e63  uded_node in inc
+00030200: 6c75 6465 645f 7069 7065 2e6e 6f64 6573  luded_pipe.nodes
+00030210: 2e63 6f70 7928 293a 0a20 2020 2020 2020  .copy():.       
+00030220: 2020 2020 2020 2020 2075 6e72 6f6c 6c65           unrolle
+00030230: 645f 696e 636c 7564 6564 5f6e 6f64 6520  d_included_node 
+00030240: 3d20 6e65 7874 280a 2020 2020 2020 2020  = next(.        
+00030250: 2020 2020 2020 2020 2020 2020 286e 6f64              (nod
+00030260: 6520 666f 7220 6e6f 6465 2069 6e20 7069  e for node in pi
+00030270: 7065 5f6e 6f64 6573 2069 6620 6e6f 6465  pe_nodes if node
+00030280: 5b22 6e61 6d65 225d 203d 3d20 696e 636c  ["name"] == incl
+00030290: 7564 6564 5f6e 6f64 655b 226e 616d 6522  uded_node["name"
+000302a0: 5d29 2c20 4e6f 6e65 0a20 2020 2020 2020  ]), None.       
+000302b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000302c0: 2020 2020 2020 2020 2020 2069 6620 756e             if un
+000302d0: 726f 6c6c 6564 5f69 6e63 6c75 6465 645f  rolled_included_
+000302e0: 6e6f 6465 3a0a 2020 2020 2020 2020 2020  node:.          
+000302f0: 2020 2020 2020 2020 2020 646f 632e 6e6f            doc.no
+00030300: 6465 732e 7265 6d6f 7665 2875 6e72 6f6c  des.remove(unrol
+00030310: 6c65 645f 696e 636c 7564 6564 5f6e 6f64  led_included_nod
+00030320: 6529 0a20 2020 2066 6f72 206e 6f64 6520  e).    for node 
+00030330: 696e 2064 6f63 2e6e 6f64 6573 3a0a 2020  in doc.nodes:.  
+00030340: 2020 2020 2020 6177 6169 7420 666f 726d        await form
+00030350: 6174 5f6e 6f64 6528 0a20 2020 2020 2020  at_node(.       
+00030360: 2020 2020 2066 696c 655f 7061 7274 732c       file_parts,
+00030370: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
+00030380: 652c 0a20 2020 2020 2020 2020 2020 2064  e,.            d
+00030390: 6f63 2e69 6e63 6c75 6465 732c 0a20 2020  oc.includes,.   
+000303a0: 2020 2020 2020 2020 206c 696e 655f 6c65           line_le
+000303b0: 6e67 7468 3d6c 696e 655f 6c65 6e67 7468  ngth=line_length
+000303c0: 2c0a 2020 2020 2020 2020 2020 2020 756e  ,.            un
+000303d0: 726f 6c6c 5f69 6e63 6c75 6465 733d 756e  roll_includes=un
+000303e0: 726f 6c6c 5f69 6e63 6c75 6465 732c 0a20  roll_includes,. 
+000303f0: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00030400: 5f6b 6579 776f 7264 733d 5472 7565 2069  _keywords=True i
+00030410: 6620 666f 725f 6465 706c 6f79 5f64 6966  f for_deploy_dif
+00030420: 6620 656c 7365 2046 616c 7365 2c0a 2020  f else False,.  
+00030430: 2020 2020 2020 290a 0a20 2020 2069 6620        )..    if 
+00030440: 6e6f 7420 756e 726f 6c6c 5f69 6e63 6c75  not unroll_inclu
+00030450: 6465 733a 0a20 2020 2020 2020 2066 6f72  des:.        for
+00030460: 206b 2c20 5f20 696e 2064 6f63 2e69 6e63   k, _ in doc.inc
+00030470: 6c75 6465 732e 6974 656d 7328 293a 0a20  ludes.items():. 
+00030480: 2020 2020 2020 2020 2020 2069 6620 222e             if ".
+00030490: 696e 636c 2220 6e6f 7420 696e 206b 3a0a  incl" not in k:.
+000304a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000304b0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+000304c0: 2020 2020 2066 696c 655f 7061 7274 732e       file_parts.
+000304d0: 6170 7065 6e64 2866 2249 4e43 4c55 4445  append(f"INCLUDE
+000304e0: 207b 6b7d 2229 0a20 2020 2020 2020 2020   {k}").         
+000304f0: 2020 2066 696c 655f 7061 7274 732e 6170     file_parts.ap
+00030500: 7065 6e64 2844 4154 4146 494c 455f 4e45  pend(DATAFILE_NE
+00030510: 575f 4c49 4e45 290a 2020 2020 2020 2020  W_LINE).        
+00030520: 2020 2020 6669 6c65 5f70 6172 7473 2e61      file_parts.a
+00030530: 7070 656e 6428 4441 5441 4649 4c45 5f4e  ppend(DATAFILE_N
+00030540: 4557 5f4c 494e 4529 0a0a 2020 2020 7265  EW_LINE)..    re
+00030550: 7375 6c74 203d 2022 222e 6a6f 696e 2866  sult = "".join(f
+00030560: 696c 655f 7061 7274 7329 0a20 2020 2072  ile_parts).    r
+00030570: 6573 756c 7420 3d20 7265 7375 6c74 2e72  esult = result.r
+00030580: 7374 7269 7028 225c 6e22 2920 2b20 225c  strip("\n") + "\
+00030590: 6e22 0a20 2020 2072 6574 7572 6e20 7265  n".    return re
+000305a0: 7375 6c74 0a0a 0a64 6566 2066 6f72 6d61  sult...def forma
+000305b0: 745f 7371 6c28 7371 6c3a 2073 7472 2c20  t_sql(sql: str, 
+000305c0: 4441 5441 4649 4c45 5f49 4e44 454e 543a  DATAFILE_INDENT:
+000305d0: 2073 7472 2c20 6c69 6e65 5f6c 656e 6774   str, line_lengt
+000305e0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
+000305f0: 203d 204e 6f6e 652c 206c 6f77 6572 5f6b   = None, lower_k
+00030600: 6579 776f 7264 733a 2062 6f6f 6c20 3d20  eywords: bool = 
+00030610: 4661 6c73 6529 202d 3e20 7374 723a 0a20  False) -> str:. 
+00030620: 2020 2073 716c 203d 2066 6f72 6d61 745f     sql = format_
+00030630: 7371 6c5f 7465 6d70 6c61 7465 2873 716c  sql_template(sql
+00030640: 2e73 7472 6970 2829 2c20 6c69 6e65 5f6c  .strip(), line_l
+00030650: 656e 6774 683d 6c69 6e65 5f6c 656e 6774  ength=line_lengt
+00030660: 682c 206c 6f77 6572 5f6b 6579 776f 7264  h, lower_keyword
+00030670: 733d 6c6f 7765 725f 6b65 7977 6f72 6473  s=lower_keywords
+00030680: 290a 2020 2020 7265 7475 726e 2022 5c6e  ).    return "\n
+00030690: 222e 6a6f 696e 285b 6622 7b44 4154 4146  ".join([f"{DATAF
+000306a0: 494c 455f 494e 4445 4e54 7d7b 7061 7274  ILE_INDENT}{part
+000306b0: 7d22 2066 6f72 2070 6172 7420 696e 2073  }" for part in s
+000306c0: 716c 2e73 706c 6974 2822 5c6e 2229 2069  ql.split("\n") i
+000306d0: 6620 6c65 6e28 7061 7274 2e73 7472 6970  f len(part.strip
+000306e0: 2829 295d 290a 0a0a 6173 796e 6320 6465  ())])...async de
+000306f0: 6620 5f67 6174 6865 725f 7769 7468 5f63  f _gather_with_c
+00030700: 6f6e 6375 7272 656e 6379 286e 2c20 2a74  oncurrency(n, *t
+00030710: 6173 6b73 293a 0a20 2020 2073 656d 6170  asks):.    semap
+00030720: 686f 7265 203d 2053 656d 6170 686f 7265  hore = Semaphore
+00030730: 286e 290a 0a20 2020 2061 7379 6e63 2064  (n)..    async d
+00030740: 6566 2073 656d 5f74 6173 6b28 7461 736b  ef sem_task(task
+00030750: 293a 0a20 2020 2020 2020 2061 7379 6e63  ):.        async
+00030760: 2077 6974 6820 7365 6d61 7068 6f72 653a   with semaphore:
+00030770: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00030780: 7572 6e20 6177 6169 7420 7461 736b 0a0a  urn await task..
+00030790: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+000307a0: 2067 6174 6865 7228 2a28 7365 6d5f 7461   gather(*(sem_ta
+000307b0: 736b 2874 6173 6b29 2066 6f72 2074 6173  sk(task) for tas
+000307c0: 6b20 696e 2074 6173 6b73 2929 0a0a 0a61  k in tasks))...a
+000307d0: 7379 6e63 2064 6566 2066 6f6c 6465 725f  sync def folder_
+000307e0: 7075 6c6c 280a 2020 2020 636c 6965 6e74  pull(.    client
+000307f0: 3a20 5469 6e79 422c 0a20 2020 2066 6f6c  : TinyB,.    fol
+00030800: 6465 723a 2073 7472 2c0a 2020 2020 6175  der: str,.    au
+00030810: 746f 3a20 626f 6f6c 2c0a 2020 2020 6d61  to: bool,.    ma
+00030820: 7463 683a 204f 7074 696f 6e61 6c5b 7374  tch: Optional[st
+00030830: 725d 2c0a 2020 2020 666f 7263 653a 2062  r],.    force: b
+00030840: 6f6f 6c2c 0a20 2020 2076 6572 626f 7365  ool,.    verbose
+00030850: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+00030860: 2020 2070 726f 6772 6573 735f 6261 723a     progress_bar:
+00030870: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a29   bool = False,.)
+00030880: 3a20 2023 206e 6f71 613a 2043 3930 310a  :  # noqa: C901.
+00030890: 2020 2020 7061 7474 6572 6e20 3d20 7265      pattern = re
+000308a0: 2e63 6f6d 7069 6c65 286d 6174 6368 2920  .compile(match) 
+000308b0: 6966 206d 6174 6368 2065 6c73 6520 4e6f  if match else No
+000308c0: 6e65 0a0a 2020 2020 6465 6620 5f67 6574  ne..    def _get
+000308d0: 5f6c 6174 6573 745f 7665 7273 696f 6e73  _latest_versions
+000308e0: 2872 6573 6f75 7263 6573 3a20 4c69 7374  (resources: List
+000308f0: 5b73 7472 5d29 3a0a 2020 2020 2020 2020  [str]):.        
+00030900: 7665 7273 696f 6e73 3a20 4469 6374 5b73  versions: Dict[s
+00030910: 7472 2c20 416e 795d 203d 207b 7d0a 0a20  tr, Any] = {}.. 
+00030920: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
+00030930: 7265 736f 7572 6365 733a 0a20 2020 2020  resources:.     
+00030940: 2020 2020 2020 2074 203d 2067 6574 5f6e         t = get_n
+00030950: 616d 655f 7665 7273 696f 6e28 7829 0a20  ame_version(x). 
+00030960: 2020 2020 2020 2020 2020 2074 5b22 6f72             t["or
+00030970: 6967 696e 616c 5f6e 616d 6522 5d20 3d20  iginal_name"] = 
+00030980: 780a 2020 2020 2020 2020 2020 2020 6966  x.            if
+00030990: 2074 5b22 7665 7273 696f 6e22 5d20 6973   t["version"] is
+000309a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000309b0: 2020 2020 2020 2074 5b22 7665 7273 696f         t["versio
+000309c0: 6e22 5d20 3d20 2d31 0a20 2020 2020 2020  n"] = -1.       
+000309d0: 2020 2020 206e 616d 6520 3d20 745b 226e       name = t["n
+000309e0: 616d 6522 5d0a 0a20 2020 2020 2020 2020  ame"]..         
+000309f0: 2020 2069 6620 6e61 6d65 206e 6f74 2069     if name not i
+00030a00: 6e20 7665 7273 696f 6e73 206f 7220 6e61  n versions or na
+00030a10: 6d65 203d 3d20 7820 6f72 2076 6572 7369  me == x or versi
+00030a20: 6f6e 735b 6e61 6d65 5d5b 2276 6572 7369  ons[name]["versi
+00030a30: 6f6e 225d 203c 2074 5b22 7665 7273 696f  on"] < t["versio
+00030a40: 6e22 5d3a 0a20 2020 2020 2020 2020 2020  n"]:.           
+00030a50: 2020 2020 2076 6572 7369 6f6e 735b 6e61       versions[na
+00030a60: 6d65 5d20 3d20 740a 2020 2020 2020 2020  me] = t.        
+00030a70: 7265 7475 726e 2076 6572 7369 6f6e 730a  return versions.
+00030a80: 0a20 2020 2064 6566 2067 6574 5f66 696c  .    def get_fil
+00030a90: 655f 666f 6c64 6572 2865 7874 656e 7369  e_folder(extensi
+00030aa0: 6f6e 3a20 7374 7229 3a0a 2020 2020 2020  on: str):.      
+00030ab0: 2020 6966 206e 6f74 2061 7574 6f3a 0a20    if not auto:. 
+00030ac0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00030ad0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2069  n None.        i
+00030ae0: 6620 6578 7465 6e73 696f 6e20 3d3d 2022  f extension == "
+00030af0: 6461 7461 736f 7572 6365 223a 0a20 2020  datasource":.   
+00030b00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00030b10: 2264 6174 6173 6f75 7263 6573 220a 2020  "datasources".  
+00030b20: 2020 2020 2020 6966 2065 7874 656e 7369        if extensi
+00030b30: 6f6e 203d 3d20 2270 6970 6522 3a0a 2020  on == "pipe":.  
+00030b40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00030b50: 2022 7069 7065 7322 0a20 2020 2020 2020   "pipes".       
+00030b60: 2069 6620 6578 7465 6e73 696f 6e20 3d3d   if extension ==
+00030b70: 2022 746f 6b65 6e22 3a0a 2020 2020 2020   "token":.      
+00030b80: 2020 2020 2020 7265 7475 726e 2022 746f        return "to
+00030b90: 6b65 6e73 220a 2020 2020 2020 2020 7265  kens".        re
+00030ba0: 7475 726e 204e 6f6e 650a 0a20 2020 2061  turn None..    a
+00030bb0: 7379 6e63 2064 6566 2077 7269 7465 5f66  sync def write_f
+00030bc0: 696c 6573 280a 2020 2020 2020 2020 7665  iles(.        ve
+00030bd0: 7273 696f 6e73 3a20 4469 6374 5b73 7472  rsions: Dict[str
+00030be0: 2c20 416e 795d 2c0a 2020 2020 2020 2020  , Any],.        
+00030bf0: 7265 736f 7572 6365 733a 204c 6973 745b  resources: List[
+00030c00: 7374 725d 2c0a 2020 2020 2020 2020 6578  str],.        ex
+00030c10: 7465 6e73 696f 6e3a 2073 7472 2c0a 2020  tension: str,.  
+00030c20: 2020 2020 2020 6765 745f 7265 736f 7572        get_resour
+00030c30: 6365 5f66 756e 6374 696f 6e3a 2073 7472  ce_function: str
+00030c40: 2c0a 2020 2020 2020 2020 7072 6f67 7265  ,.        progre
+00030c50: 7373 5f62 6172 3a20 626f 6f6c 203d 2046  ss_bar: bool = F
+00030c60: 616c 7365 2c0a 2020 2020 293a 0a20 2020  alse,.    ):.   
+00030c70: 2020 2020 2061 7379 6e63 2064 6566 2077       async def w
+00030c80: 7269 7465 5f72 6573 6f75 7263 6528 6b3a  rite_resource(k:
+00030c90: 2044 6963 745b 7374 722c 2041 6e79 5d29   Dict[str, Any])
+00030ca0: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
+00030cb0: 6d65 203d 2066 227b 6b5b 276e 616d 6527  me = f"{k['name'
+00030cc0: 5d7d 2e7b 6578 7465 6e73 696f 6e7d 220a  ]}.{extension}".
+00030cd0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00030ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030cf0: 2069 6620 7061 7474 6572 6e20 616e 6420   if pattern and 
+00030d00: 6e6f 7420 7061 7474 6572 6e2e 7365 6172  not pattern.sear
+00030d10: 6368 286e 616d 6529 3a0a 2020 2020 2020  ch(name):.      
+00030d20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00030d30: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+00030d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030d50: 2020 636c 6963 6b2e 6563 686f 2846 6565    click.echo(Fee
+00030d60: 6462 6163 6b4d 616e 6167 6572 2e69 6e66  dbackManager.inf
+00030d70: 6f5f 736b 6970 7069 6e67 5f72 6573 6f75  o_skipping_resou
+00030d80: 7263 6528 7265 736f 7572 6365 3d6e 616d  rce(resource=nam
+00030d90: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+00030da0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00030db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030dc0: 7265 736f 7572 6365 203d 2061 7761 6974  resource = await
+00030dd0: 2067 6574 6174 7472 2863 6c69 656e 742c   getattr(client,
+00030de0: 2067 6574 5f72 6573 6f75 7263 655f 6675   get_resource_fu
+00030df0: 6e63 7469 6f6e 2928 6b5b 226f 7269 6769  nction)(k["origi
+00030e00: 6e61 6c5f 6e61 6d65 225d 290a 0a20 2020  nal_name"])..   
+00030e10: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00030e20: 745f 666f 6c64 6572 203d 2066 6f6c 6465  t_folder = folde
+00030e30: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00030e40: 2020 6966 2022 2e22 2069 6e20 6b5b 226e    if "." in k["n
+00030e50: 616d 6522 5d20 616e 6420 6578 7465 6e73  ame"] and extens
+00030e60: 696f 6e20 213d 2022 746f 6b65 6e22 3a0a  ion != "token":.
+00030e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030e80: 2020 2020 6465 7374 5f66 6f6c 6465 7220      dest_folder 
+00030e90: 3d20 5061 7468 2866 6f6c 6465 7229 202f  = Path(folder) /
+00030ea0: 2022 7665 6e64 6f72 2220 2f20 6b5b 226e   "vendor" / k["n
+00030eb0: 616d 6522 5d2e 7370 6c69 7428 222e 222c  ame"].split(".",
+00030ec0: 2031 295b 305d 0a20 2020 2020 2020 2020   1)[0].         
+00030ed0: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+00030ee0: 3d20 6622 7b6b 5b27 6e61 6d65 275d 2e73  = f"{k['name'].s
+00030ef0: 706c 6974 2827 2e27 2c20 3129 5b31 5d7d  plit('.', 1)[1]}
+00030f00: 2e7b 6578 7465 6e73 696f 6e7d 220a 0a20  .{extension}".. 
+00030f10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00030f20: 696c 655f 666f 6c64 6572 203d 2067 6574  ile_folder = get
+00030f30: 5f66 696c 655f 666f 6c64 6572 2865 7874  _file_folder(ext
+00030f40: 656e 7369 6f6e 290a 2020 2020 2020 2020  ension).        
+00030f50: 2020 2020 2020 2020 6620 3d20 5061 7468          f = Path
+00030f60: 2864 6573 745f 666f 6c64 6572 2920 2f20  (dest_folder) / 
+00030f70: 6669 6c65 5f66 6f6c 6465 7220 6966 2066  file_folder if f
+00030f80: 696c 655f 666f 6c64 6572 2069 7320 6e6f  ile_folder is no
+00030f90: 7420 4e6f 6e65 2065 6c73 6520 5061 7468  t None else Path
+00030fa0: 2864 6573 745f 666f 6c64 6572 290a 0a20  (dest_folder).. 
+00030fb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00030fc0: 6620 6e6f 7420 662e 6578 6973 7473 2829  f not f.exists()
+00030fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00030fe0: 2020 2020 2020 662e 6d6b 6469 7228 7061        f.mkdir(pa
+00030ff0: 7265 6e74 733d 5472 7565 290a 0a20 2020  rents=True)..   
+00031000: 2020 2020 2020 2020 2020 2020 2066 203d               f =
+00031010: 2066 202f 206e 616d 650a 2020 2020 2020   f / name.      
+00031020: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+00031030: 6365 5f6e 616d 6573 203d 205b 782e 7370  ce_names = [x.sp
+00031040: 6c69 7428 222e 2229 5b2d 315d 2066 6f72  lit(".")[-1] for
+00031050: 2078 2069 6e20 7265 736f 7572 6365 735d   x in resources]
+00031060: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00031070: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+00031080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031090: 2020 636c 6963 6b2e 6563 686f 2846 6565    click.echo(Fee
+000310a0: 6462 6163 6b4d 616e 6167 6572 2e69 6e66  dbackManager.inf
+000310b0: 6f5f 7772 6974 696e 675f 7265 736f 7572  o_writing_resour
+000310c0: 6365 2872 6573 6f75 7263 653d 6629 290a  ce(resource=f)).
+000310d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000310e0: 6966 206e 6f74 2066 2e65 7869 7374 7328  if not f.exists(
+000310f0: 2920 6f72 2066 6f72 6365 3a0a 2020 2020  ) or force:.    
+00031100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031110: 7769 7468 206f 7065 6e28 662c 2022 7722  with open(f, "w"
+00031120: 2920 6173 2066 643a 0a20 2020 2020 2020  ) as fd:.       
+00031130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031140: 2023 2076 6572 7369 6f6e 7320 6172 6520   # versions are 
+00031150: 6120 636c 6965 6e74 206f 6e6c 7920 7468  a client only th
+00031160: 696e 6720 736f 0a20 2020 2020 2020 2020  ing so.         
+00031170: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00031180: 2064 6174 6166 696c 6573 2066 726f 6d20   datafiles from 
+00031190: 7468 6520 7365 7276 6572 2064 6f20 6e6f  the server do no
+000311a0: 7420 636f 6e74 6169 6e73 2069 6e66 6f72  t contains infor
+000311b0: 6d61 7469 6f6e 2061 626f 7574 2076 6572  mation about ver
+000311c0: 7369 6f6e 730a 2020 2020 2020 2020 2020  sions.          
+000311d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000311e0: 206b 5b22 7665 7273 696f 6e22 5d20 3e3d   k["version"] >=
+000311f0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00031200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031210: 7265 736f 7572 6365 203d 2066 2256 4552  resource = f"VER
+00031220: 5349 4f4e 207b 6b5b 2776 6572 7369 6f6e  SION {k['version
+00031230: 275d 7d5c 6e22 202b 2072 6573 6f75 7263  ']}\n" + resourc
+00031240: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00031250: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+00031260: 6f75 7263 653a 0a20 2020 2020 2020 2020  ource:.         
+00031270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031280: 2020 206d 6174 6368 6573 203d 2072 652e     matches = re.
+00031290: 6669 6e64 616c 6c28 7222 285b 5e5c 735c  findall(r"([^\s\
+000312a0: 2e5d 2a5f 5f76 5c64 2b29 222c 2072 6573  .]*__v\d+)", res
+000312b0: 6f75 7263 6529 0a20 2020 2020 2020 2020  ource).         
+000312c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000312d0: 2020 2066 6f72 206d 6174 6368 2069 6e20     for match in 
+000312e0: 7365 7428 6d61 7463 6865 7329 3a0a 2020  set(matches):.  
 000312f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031300: 2020 2020 2020 6d20 3d20 6d61 7463 682e        m = match.
-00031310: 7370 6c69 7428 225f 5f76 2229 5b30 5d0a  split("__v")[0].
-00031320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031300: 2020 2020 2020 2020 2020 2020 2020 6d20                m 
+00031310: 3d20 6d61 7463 682e 7370 6c69 7428 225f  = match.split("_
+00031320: 5f76 2229 5b30 5d0a 2020 2020 2020 2020  _v")[0].        
 00031330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031340: 6966 206d 2069 6e20 7265 736f 7572 6365  if m in resource
-00031350: 7320 6f72 206d 2069 6e20 7265 736f 7572  s or m in resour
-00031360: 6365 5f6e 616d 6573 3a0a 2020 2020 2020  ce_names:.      
-00031370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031380: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00031390: 736f 7572 6365 203d 2072 6573 6f75 7263  source = resourc
-000313a0: 652e 7265 706c 6163 6528 6d61 7463 682c  e.replace(match,
-000313b0: 206d 290a 2020 2020 2020 2020 2020 2020   m).            
+00031340: 2020 2020 2020 2020 6966 206d 2069 6e20          if m in 
+00031350: 7265 736f 7572 6365 7320 6f72 206d 2069  resources or m i
+00031360: 6e20 7265 736f 7572 6365 5f6e 616d 6573  n resource_names
+00031370: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00031380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031390: 2020 2020 2020 7265 736f 7572 6365 203d        resource =
+000313a0: 2072 6573 6f75 7263 652e 7265 706c 6163   resource.replac
+000313b0: 6528 6d61 7463 682c 206d 290a 2020 2020  e(match, m).    
 000313c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000313d0: 6664 2e77 7269 7465 2872 6573 6f75 7263  fd.write(resourc
-000313e0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-000313f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00031400: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00031410: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-00031420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031430: 2063 6c69 636b 2e65 6368 6f28 4665 6564   click.echo(Feed
-00031440: 6261 636b 4d61 6e61 6765 722e 696e 666f  backManager.info
-00031450: 5f73 6b69 705f 616c 7265 6164 795f 6578  _skip_already_ex
-00031460: 6973 7473 2829 290a 2020 2020 2020 2020  ists()).        
-00031470: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00031480: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00031490: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000314a0: 2063 6c69 636b 2e43 6c69 636b 4578 6365   click.ClickExce
-000314b0: 7074 696f 6e28 4665 6564 6261 636b 4d61  ption(FeedbackMa
-000314c0: 6e61 6765 722e 6572 726f 725f 6578 6365  nager.error_exce
-000314d0: 7074 696f 6e28 6572 726f 723d 6529 290a  ption(error=e)).
-000314e0: 0a20 2020 2020 2020 2076 616c 7565 7320  .        values 
-000314f0: 3d20 7665 7273 696f 6e73 2e76 616c 7565  = versions.value
-00031500: 7328 290a 0a20 2020 2020 2020 2069 6620  s()..        if 
-00031510: 7072 6f67 7265 7373 5f62 6172 3a0a 2020  progress_bar:.  
-00031520: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-00031530: 6c69 636b 2e70 726f 6772 6573 7362 6172  lick.progressbar
-00031540: 2876 616c 7565 732c 206c 6162 656c 3d66  (values, label=f
-00031550: 2250 756c 6c69 6e67 207b 6578 7465 6e73  "Pulling {extens
-00031560: 696f 6e7d 7322 2920 6173 2076 616c 7565  ion}s") as value
-00031570: 733a 2020 2320 7479 7065 3a20 6967 6e6f  s:  # type: igno
-00031580: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
-00031590: 2020 2066 6f72 206b 2069 6e20 7661 6c75     for k in valu
-000315a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-000315b0: 2020 2020 2020 2020 6177 6169 7420 7772          await wr
-000315c0: 6974 655f 7265 736f 7572 6365 286b 290a  ite_resource(k).
-000315d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000315e0: 2020 2020 2020 2020 2020 7461 736b 7320            tasks 
-000315f0: 3d20 5b77 7269 7465 5f72 6573 6f75 7263  = [write_resourc
-00031600: 6528 6b29 2066 6f72 206b 2069 6e20 7661  e(k) for k in va
-00031610: 6c75 6573 5d0a 2020 2020 2020 2020 2020  lues].          
-00031620: 2020 6177 6169 7420 5f67 6174 6865 725f    await _gather_
-00031630: 7769 7468 5f63 6f6e 6375 7272 656e 6379  with_concurrency
-00031640: 2835 2c20 2a74 6173 6b73 290a 0a20 2020  (5, *tasks)..   
-00031650: 2074 7279 3a0a 2020 2020 2020 2020 6461   try:.        da
-00031660: 7461 736f 7572 6365 7320 3d20 6177 6169  tasources = awai
-00031670: 7420 636c 6965 6e74 2e64 6174 6173 6f75  t client.datasou
-00031680: 7263 6573 2829 0a20 2020 2020 2020 2072  rces().        r
-00031690: 656d 6f74 655f 6461 7461 736f 7572 6365  emote_datasource
-000316a0: 7320 3d20 736f 7274 6564 285b 785b 226e  s = sorted([x["n
-000316b0: 616d 6522 5d20 666f 7220 7820 696e 2064  ame"] for x in d
-000316c0: 6174 6173 6f75 7263 6573 5d29 0a20 2020  atasources]).   
-000316d0: 2020 2020 2064 6174 6173 6f75 7263 6573       datasources
-000316e0: 5f76 6572 7369 6f6e 7320 3d20 5f67 6574  _versions = _get
-000316f0: 5f6c 6174 6573 745f 7665 7273 696f 6e73  _latest_versions
-00031700: 2872 656d 6f74 655f 6461 7461 736f 7572  (remote_datasour
-00031710: 6365 7329 0a0a 2020 2020 2020 2020 7069  ces)..        pi
-00031720: 7065 7320 3d20 6177 6169 7420 636c 6965  pes = await clie
-00031730: 6e74 2e70 6970 6573 2829 0a20 2020 2020  nt.pipes().     
-00031740: 2020 2072 656d 6f74 655f 7069 7065 7320     remote_pipes 
-00031750: 3d20 736f 7274 6564 285b 785b 226e 616d  = sorted([x["nam
-00031760: 6522 5d20 666f 7220 7820 696e 2070 6970  e"] for x in pip
-00031770: 6573 5d29 0a20 2020 2020 2020 2070 6970  es]).        pip
-00031780: 6573 5f76 6572 7369 6f6e 7320 3d20 5f67  es_versions = _g
-00031790: 6574 5f6c 6174 6573 745f 7665 7273 696f  et_latest_versio
-000317a0: 6e73 2872 656d 6f74 655f 7069 7065 7329  ns(remote_pipes)
-000317b0: 0a0a 2020 2020 2020 2020 7265 736f 7572  ..        resour
-000317c0: 6365 7320 3d20 6c69 7374 2864 6174 6173  ces = list(datas
-000317d0: 6f75 7263 6573 5f76 6572 7369 6f6e 732e  ources_versions.
-000317e0: 6b65 7973 2829 2920 2b20 6c69 7374 2870  keys()) + list(p
-000317f0: 6970 6573 5f76 6572 7369 6f6e 732e 6b65  ipes_versions.ke
-00031800: 7973 2829 290a 0a20 2020 2020 2020 2061  ys())..        a
-00031810: 7761 6974 2077 7269 7465 5f66 696c 6573  wait write_files
-00031820: 2864 6174 6173 6f75 7263 6573 5f76 6572  (datasources_ver
-00031830: 7369 6f6e 732c 2072 6573 6f75 7263 6573  sions, resources
-00031840: 2c20 2264 6174 6173 6f75 7263 6522 2c20  , "datasource", 
-00031850: 2264 6174 6173 6f75 7263 655f 6669 6c65  "datasource_file
-00031860: 222c 2070 726f 6772 6573 735f 6261 723d  ", progress_bar=
-00031870: 7072 6f67 7265 7373 5f62 6172 290a 2020  progress_bar).  
-00031880: 2020 2020 2020 6177 6169 7420 7772 6974        await writ
-00031890: 655f 6669 6c65 7328 7069 7065 735f 7665  e_files(pipes_ve
-000318a0: 7273 696f 6e73 2c20 7265 736f 7572 6365  rsions, resource
-000318b0: 732c 2022 7069 7065 222c 2022 7069 7065  s, "pipe", "pipe
-000318c0: 5f66 696c 6522 2c20 7072 6f67 7265 7373  _file", progress
-000318d0: 5f62 6172 3d70 726f 6772 6573 735f 6261  _bar=progress_ba
-000318e0: 7229 0a0a 2020 2020 2020 2020 7265 7475  r)..        retu
-000318f0: 726e 0a0a 2020 2020 6578 6365 7074 2045  rn..    except E
-00031900: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
-00031910: 2020 2020 2020 2072 6169 7365 2063 6c69         raise cli
-00031920: 636b 2e43 6c69 636b 4578 6365 7074 696f  ck.ClickExceptio
-00031930: 6e28 4665 6564 6261 636b 4d61 6e61 6765  n(FeedbackManage
-00031940: 722e 6572 726f 725f 7075 6c6c 2865 7272  r.error_pull(err
-00031950: 6f72 3d73 7472 2865 2929 290a 0a0a 6465  or=str(e)))...de
-00031960: 6620 636f 6c6f 725f 6469 6666 2864 6966  f color_diff(dif
-00031970: 663a 2049 7465 7261 626c 655b 7374 725d  f: Iterable[str]
-00031980: 2920 2d3e 2047 656e 6572 6174 6f72 5b73  ) -> Generator[s
-00031990: 7472 2c20 416e 792c 204e 6f6e 655d 3a0a  tr, Any, None]:.
-000319a0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-000319b0: 6469 6666 3a0a 2020 2020 2020 2020 6966  diff:.        if
-000319c0: 206c 696e 652e 7374 6172 7473 7769 7468   line.startswith
-000319d0: 2822 2b22 293a 0a20 2020 2020 2020 2020  ("+"):.         
-000319e0: 2020 2079 6965 6c64 2046 6f72 652e 4752     yield Fore.GR
-000319f0: 4545 4e20 2b20 6c69 6e65 202b 2046 6f72  EEN + line + For
-00031a00: 652e 5245 5345 540a 2020 2020 2020 2020  e.RESET.        
-00031a10: 656c 6966 206c 696e 652e 7374 6172 7473  elif line.starts
-00031a20: 7769 7468 2822 2d22 293a 0a20 2020 2020  with("-"):.     
-00031a30: 2020 2020 2020 2079 6965 6c64 2046 6f72         yield For
-00031a40: 652e 5245 4420 2b20 6c69 6e65 202b 2046  e.RED + line + F
-00031a50: 6f72 652e 5245 5345 540a 2020 2020 2020  ore.RESET.      
-00031a60: 2020 656c 6966 206c 696e 652e 7374 6172    elif line.star
-00031a70: 7473 7769 7468 2822 5e22 293a 0a20 2020  tswith("^"):.   
-00031a80: 2020 2020 2020 2020 2079 6965 6c64 2046           yield F
-00031a90: 6f72 652e 424c 5545 202b 206c 696e 6520  ore.BLUE + line 
-00031aa0: 2b20 466f 7265 2e52 4553 4554 0a20 2020  + Fore.RESET.   
-00031ab0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00031ac0: 2020 2020 2020 2079 6965 6c64 206c 696e         yield lin
-00031ad0: 650a 0a0a 6465 6620 7065 656b 2869 7465  e...def peek(ite
-00031ae0: 7261 626c 6529 3a0a 2020 2020 7472 793a  rable):.    try:
-00031af0: 0a20 2020 2020 2020 2066 6972 7374 203d  .        first =
-00031b00: 206e 6578 7428 6974 6572 6162 6c65 290a   next(iterable).
-00031b10: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00031b20: 7469 6f6e 3a0a 2020 2020 2020 2020 7265  tion:.        re
-00031b30: 7475 726e 204e 6f6e 652c 204e 6f6e 650a  turn None, None.
-00031b40: 2020 2020 7265 7475 726e 2066 6972 7374      return first
-00031b50: 2c20 6974 6572 746f 6f6c 732e 6368 6169  , itertools.chai
-00031b60: 6e28 5b66 6972 7374 5d2c 2069 7465 7261  n([first], itera
-00031b70: 626c 6529 0a0a 0a61 7379 6e63 2064 6566  ble)...async def
-00031b80: 2064 6966 665f 636f 6d6d 616e 6428 0a20   diff_command(. 
-00031b90: 2020 2066 696c 656e 616d 6573 3a20 4f70     filenames: Op
-00031ba0: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
-00031bb0: 5d2c 0a20 2020 2066 6d74 3a20 626f 6f6c  ],.    fmt: bool
-00031bc0: 2c0a 2020 2020 636c 6965 6e74 3a20 5469  ,.    client: Ti
-00031bd0: 6e79 422c 0a20 2020 206e 6f5f 636f 6c6f  nyB,.    no_colo
-00031be0: 723a 204f 7074 696f 6e61 6c5b 626f 6f6c  r: Optional[bool
-00031bf0: 5d20 3d20 4661 6c73 652c 0a20 2020 2077  ] = False,.    w
-00031c00: 6974 685f 7072 696e 743a 204f 7074 696f  ith_print: Optio
-00031c10: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-00031c20: 2c0a 2020 2020 7665 7262 6f73 653a 204f  ,.    verbose: O
-00031c30: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00031c40: 4e6f 6e65 2c0a 2020 2020 636c 6561 6e5f  None,.    clean_
-00031c50: 7570 3a20 4f70 7469 6f6e 616c 5b62 6f6f  up: Optional[boo
-00031c60: 6c5d 203d 2046 616c 7365 2c0a 2020 2020  l] = False,.    
-00031c70: 7072 6f67 7265 7373 5f62 6172 3a20 626f  progress_bar: bo
-00031c80: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00031c90: 666f 725f 6465 706c 6f79 3a20 626f 6f6c  for_deploy: bool
-00031ca0: 203d 2046 616c 7365 2c0a 293a 0a20 2020   = False,.):.   
-00031cb0: 2064 6566 2069 735f 7368 6172 6564 5f64   def is_shared_d
-00031cc0: 6174 6173 6f75 7263 6528 6e61 6d65 293a  atasource(name):
-00031cd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00031ce0: 222e 2220 696e 206e 616d 650a 0a20 2020  "." in name..   
-00031cf0: 2077 6974 685f 6578 706c 6963 6974 5f66   with_explicit_f
-00031d00: 696c 656e 616d 6573 203d 2066 696c 656e  ilenames = filen
-00031d10: 616d 6573 0a20 2020 2076 6572 626f 7365  ames.    verbose
-00031d20: 203d 2054 7275 6520 6966 2076 6572 626f   = True if verbo
-00031d30: 7365 2069 7320 4e6f 6e65 2065 6c73 6520  se is None else 
-00031d40: 7665 7262 6f73 650a 0a20 2020 2074 6172  verbose..    tar
-00031d50: 6765 745f 6469 7220 3d20 6765 7463 7764  get_dir = getcwd
-00031d60: 2829 202b 206f 732e 7061 7468 2e73 6570  () + os.path.sep
-00031d70: 202b 2022 2e64 6966 665f 746d 7022 0a20   + ".diff_tmp". 
-00031d80: 2020 2050 6174 6828 7461 7267 6574 5f64     Path(target_d
-00031d90: 6972 292e 6d6b 6469 7228 7061 7265 6e74  ir).mkdir(parent
-00031da0: 733d 5472 7565 2c20 6578 6973 745f 6f6b  s=True, exist_ok
-00031db0: 3d54 7275 6529 0a0a 2020 2020 6966 2066  =True)..    if f
-00031dc0: 696c 656e 616d 6573 3a0a 2020 2020 2020  ilenames:.      
-00031dd0: 2020 6966 206c 656e 2866 696c 656e 616d    if len(filenam
-00031de0: 6573 2920 3d3d 2031 3a0a 2020 2020 2020  es) == 1:.      
-00031df0: 2020 2020 2020 6669 6c65 6e61 6d65 7320        filenames 
-00031e00: 3d20 5b66 696c 656e 616d 6573 5b30 5d5d  = [filenames[0]]
-00031e10: 202b 2067 6574 5f70 726f 6a65 6374 5f66   + get_project_f
-00031e20: 696c 656e 616d 6573 2866 696c 656e 616d  ilenames(filenam
-00031e30: 6573 5b30 5d29 0a20 2020 2020 2020 2061  es[0]).        a
-00031e40: 7761 6974 2066 6f6c 6465 725f 7075 6c6c  wait folder_pull
-00031e50: 2863 6c69 656e 742c 2074 6172 6765 745f  (client, target_
-00031e60: 6469 722c 2046 616c 7365 2c20 4e6f 6e65  dir, False, None
-00031e70: 2c20 5472 7565 2c20 7665 7262 6f73 653d  , True, verbose=
-00031e80: 4661 6c73 6529 0a20 2020 2065 6c73 653a  False).    else:
-00031e90: 0a20 2020 2020 2020 2066 696c 656e 616d  .        filenam
-00031ea0: 6573 203d 2067 6574 5f70 726f 6a65 6374  es = get_project
-00031eb0: 5f66 696c 656e 616d 6573 2822 2e22 290a  _filenames(".").
-00031ec0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-00031ed0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00031ee0: 636c 6963 6b2e 6563 686f 2822 5361 7669  click.echo("Savi
-00031ef0: 6e67 2072 656d 6f74 6520 7265 736f 7572  ng remote resour
-00031f00: 6365 7320 696e 202e 6469 6666 5f74 6d70  ces in .diff_tmp
-00031f10: 2066 6f6c 6465 722e 5c6e 2229 0a20 2020   folder.\n").   
-00031f20: 2020 2020 2061 7761 6974 2066 6f6c 6465       await folde
-00031f30: 725f 7075 6c6c 2863 6c69 656e 742c 2074  r_pull(client, t
-00031f40: 6172 6765 745f 6469 722c 2046 616c 7365  arget_dir, False
-00031f50: 2c20 4e6f 6e65 2c20 5472 7565 2c20 7665  , None, True, ve
-00031f60: 7262 6f73 653d 7665 7262 6f73 652c 2070  rbose=verbose, p
-00031f70: 726f 6772 6573 735f 6261 723d 7072 6f67  rogress_bar=prog
-00031f80: 7265 7373 5f62 6172 290a 0a20 2020 2072  ress_bar)..    r
-00031f90: 656d 6f74 655f 6461 7461 736f 7572 6365  emote_datasource
-00031fa0: 733a 204c 6973 745b 4469 6374 5b73 7472  s: List[Dict[str
-00031fb0: 2c20 416e 795d 5d20 3d20 6177 6169 7420  , Any]] = await 
-00031fc0: 636c 6965 6e74 2e64 6174 6173 6f75 7263  client.datasourc
-00031fd0: 6573 2829 0a20 2020 2072 656d 6f74 655f  es().    remote_
-00031fe0: 7069 7065 733a 204c 6973 745b 4469 6374  pipes: List[Dict
-00031ff0: 5b73 7472 2c20 416e 795d 5d20 3d20 6177  [str, Any]] = aw
-00032000: 6169 7420 636c 6965 6e74 2e70 6970 6573  ait client.pipes
-00032010: 2829 0a0a 2020 2020 6c6f 6361 6c5f 7265  ()..    local_re
-00032020: 736f 7572 6365 7320 3d20 7b0a 2020 2020  sources = {.    
-00032030: 2020 2020 5061 7468 2866 696c 6529 2e72      Path(file).r
-00032040: 6573 6f6c 7665 2829 2e73 7465 6d3a 2066  esolve().stem: f
-00032050: 696c 650a 2020 2020 2020 2020 666f 7220  ile.        for 
-00032060: 6669 6c65 2069 6e20 6669 6c65 6e61 6d65  file in filename
-00032070: 730a 2020 2020 2020 2020 6966 2028 222e  s.        if (".
-00032080: 6461 7461 736f 7572 6365 2220 696e 2066  datasource" in f
-00032090: 696c 6520 6f72 2022 2e70 6970 6522 2069  ile or ".pipe" i
-000320a0: 6e20 6669 6c65 2920 616e 6420 222e 696e  n file) and ".in
-000320b0: 636c 2220 6e6f 7420 696e 2066 696c 650a  cl" not in file.
-000320c0: 2020 2020 7d0a 0a20 2020 2063 6861 6e67      }..    chang
-000320d0: 6564 203d 207b 7d0a 2020 2020 666f 7220  ed = {}.    for 
-000320e0: 7265 736f 7572 6365 2069 6e20 7265 6d6f  resource in remo
-000320f0: 7465 5f64 6174 6173 6f75 7263 6573 202b  te_datasources +
-00032100: 2072 656d 6f74 655f 7069 7065 733a 0a20   remote_pipes:. 
-00032110: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-00032120: 733a 2044 6963 745b 7374 722c 2041 6e79  s: Dict[str, Any
-00032130: 5d20 3d20 6765 745f 6e61 6d65 5f76 6572  ] = get_name_ver
-00032140: 7369 6f6e 2872 6573 6f75 7263 655b 226e  sion(resource["n
-00032150: 616d 6522 5d29 0a20 2020 2020 2020 206e  ame"]).        n
-00032160: 616d 6520 3d20 7072 6f70 6572 7469 6573  ame = properties
-00032170: 2e67 6574 2822 6e61 6d65 222c 204e 6f6e  .get("name", Non
-00032180: 6529 0a20 2020 2020 2020 2069 6620 6e61  e).        if na
-00032190: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-000321a0: 2872 6669 6c65 6e61 6d65 2c20 6669 6c65  (rfilename, file
-000321b0: 2920 3d20 6e65 7874 280a 2020 2020 2020  ) = next(.      
-000321c0: 2020 2020 2020 2020 2020 2828 7266 696c            ((rfil
-000321d0: 656e 616d 652c 2066 696c 6529 2066 6f72  ename, file) for
-000321e0: 2028 7266 696c 656e 616d 652c 2066 696c   (rfilename, fil
-000321f0: 6529 2069 6e20 6c6f 6361 6c5f 7265 736f  e) in local_reso
-00032200: 7572 6365 732e 6974 656d 7328 2920 6966  urces.items() if
-00032210: 206e 616d 6520 3d3d 2072 6669 6c65 6e61   name == rfilena
-00032220: 6d65 292c 0a20 2020 2020 2020 2020 2020  me),.           
-00032230: 2020 2020 2028 2222 2c20 4e6f 6e65 292c       ("", None),
-00032240: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00032250: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00032260: 7420 6669 6c65 3a0a 2020 2020 2020 2020  t file:.        
-00032270: 2020 2020 2020 2020 6966 206e 6f74 2077          if not w
-00032280: 6974 685f 6578 706c 6963 6974 5f66 696c  ith_explicit_fil
-00032290: 656e 616d 6573 3a0a 2020 2020 2020 2020  enames:.        
-000322a0: 2020 2020 2020 2020 2020 2020 6966 2077              if w
-000322b0: 6974 685f 7072 696e 743a 0a20 2020 2020  ith_print:.     
-000322c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000322d0: 2020 2063 6c69 636b 2e65 6368 6f28 6622     click.echo(f"
-000322e0: 7b72 6573 6f75 7263 655b 276e 616d 6527  {resource['name'
-000322f0: 5d7d 206f 6e6c 7920 6578 6973 7473 2072  ]} only exists r
-00032300: 656d 6f74 656c 795c 6e22 290a 2020 2020  emotely\n").    
-00032310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032320: 6966 2069 735f 7368 6172 6564 5f64 6174  if is_shared_dat
-00032330: 6173 6f75 7263 6528 7265 736f 7572 6365  asource(resource
-00032340: 5b22 6e61 6d65 225d 293a 0a20 2020 2020  ["name"]):.     
-00032350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032360: 2020 2063 6861 6e67 6564 5b72 6573 6f75     changed[resou
-00032370: 7263 655b 226e 616d 6522 5d5d 203d 2022  rce["name"]] = "
-00032380: 7368 6172 6564 220a 2020 2020 2020 2020  shared".        
-00032390: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000323a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000323b0: 2020 2020 2020 2020 2020 6368 616e 6765            change
-000323c0: 645b 7265 736f 7572 6365 5b22 6e61 6d65  d[resource["name
-000323d0: 225d 5d20 3d20 2272 656d 6f74 6522 0a20  "]] = "remote". 
-000323e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000323f0: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
-00032400: 2020 2020 2073 7566 6669 7820 3d20 222e       suffix = ".
-00032410: 6461 7461 736f 7572 6365 2220 6966 2022  datasource" if "
-00032420: 2e64 6174 6173 6f75 7263 6522 2069 6e20  .datasource" in 
-00032430: 6669 6c65 2065 6c73 6520 222e 7069 7065  file else ".pipe
-00032440: 220a 2020 2020 2020 2020 2020 2020 7461  ".            ta
-00032450: 7267 6574 203d 2074 6172 6765 745f 6469  rget = target_di
-00032460: 7220 2b20 6f73 2e70 6174 682e 7365 7020  r + os.path.sep 
-00032470: 2b20 7266 696c 656e 616d 6520 2b20 7375  + rfilename + su
-00032480: 6666 6978 0a0a 2020 2020 2020 2020 2020  ffix..          
-00032490: 2020 6469 6666 5f6c 696e 6573 203d 2061    diff_lines = a
-000324a0: 7761 6974 2064 6966 665f 6669 6c65 7328  wait diff_files(
-000324b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000324c0: 2074 6172 6765 742c 2066 696c 652c 2077   target, file, w
-000324d0: 6974 685f 666f 726d 6174 3d66 6d74 2c20  ith_format=fmt, 
-000324e0: 7769 7468 5f63 6f6c 6f72 3d28 6e6f 7420  with_color=(not 
-000324f0: 6e6f 5f63 6f6c 6f72 292c 2063 6c69 656e  no_color), clien
-00032500: 743d 636c 6965 6e74 2c20 666f 725f 6465  t=client, for_de
-00032510: 706c 6f79 3d66 6f72 5f64 6570 6c6f 790a  ploy=for_deploy.
-00032520: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00032530: 2020 2020 2020 2020 2020 6e6f 745f 656d            not_em
-00032540: 7074 792c 2064 6966 665f 6c69 6e65 7320  pty, diff_lines 
-00032550: 3d20 7065 656b 2864 6966 665f 6c69 6e65  = peek(diff_line
-00032560: 7329 0a20 2020 2020 2020 2020 2020 2063  s).            c
-00032570: 6861 6e67 6564 5b72 6669 6c65 6e61 6d65  hanged[rfilename
-00032580: 5d20 3d20 6e6f 745f 656d 7074 790a 2020  ] = not_empty.  
-00032590: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000325a0: 5f65 6d70 7479 2061 6e64 2077 6974 685f  _empty and with_
-000325b0: 7072 696e 743a 0a20 2020 2020 2020 2020  print:.         
-000325c0: 2020 2020 2020 2073 7973 2e73 7464 6f75         sys.stdou
-000325d0: 742e 7772 6974 656c 696e 6573 2864 6966  t.writelines(dif
-000325e0: 665f 6c69 6e65 7329 0a20 2020 2020 2020  f_lines).       
-000325f0: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-00032600: 6368 6f28 2222 290a 0a20 2020 2066 6f72  cho("")..    for
-00032610: 2072 6669 6c65 6e61 6d65 2c20 5f20 696e   rfilename, _ in
-00032620: 206c 6f63 616c 5f72 6573 6f75 7263 6573   local_resources
-00032630: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00032640: 2020 6966 2072 6669 6c65 6e61 6d65 206e    if rfilename n
-00032650: 6f74 2069 6e20 6368 616e 6765 643a 0a20  ot in changed:. 
-00032660: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-00032670: 6573 6f75 7263 6520 696e 2072 656d 6f74  esource in remot
-00032680: 655f 6461 7461 736f 7572 6365 7320 2b20  e_datasources + 
-00032690: 7265 6d6f 7465 5f70 6970 6573 3a0a 2020  remote_pipes:.  
-000326a0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000326b0: 6f70 6572 7469 6573 203d 2067 6574 5f6e  operties = get_n
-000326c0: 616d 655f 7665 7273 696f 6e28 7265 736f  ame_version(reso
-000326d0: 7572 6365 5b22 6e61 6d65 225d 290a 2020  urce["name"]).  
-000326e0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-000326f0: 6d65 203d 2070 726f 7065 7274 6965 732e  me = properties.
-00032700: 6765 7428 226e 616d 6522 2c20 4e6f 6e65  get("name", None
-00032710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00032720: 2020 6966 206e 616d 6520 616e 6420 6e61    if name and na
-00032730: 6d65 203d 3d20 7266 696c 656e 616d 653a  me == rfilename:
-00032740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00032750: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
-00032760: 2020 2020 2020 2020 2020 2020 6966 2077              if w
-00032770: 6974 685f 7072 696e 7420 616e 6420 7266  ith_print and rf
-00032780: 696c 656e 616d 6520 6e6f 7420 696e 2063  ilename not in c
-00032790: 6861 6e67 6564 3a0a 2020 2020 2020 2020  hanged:.        
-000327a0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-000327b0: 6b2e 6563 686f 2866 227b 7266 696c 656e  k.echo(f"{rfilen
-000327c0: 616d 657d 206f 6e6c 7920 6578 6973 7473  ame} only exists
-000327d0: 206c 6f63 616c 6c79 5c6e 2229 0a20 2020   locally\n").   
-000327e0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-000327f0: 6e67 6564 5b72 6669 6c65 6e61 6d65 5d20  nged[rfilename] 
-00032800: 3d20 226c 6f63 616c 220a 2020 2020 6966  = "local".    if
-00032810: 2063 6c65 616e 5f75 703a 0a20 2020 2020   clean_up:.     
-00032820: 2020 2073 6875 7469 6c2e 726d 7472 6565     shutil.rmtree
-00032830: 2874 6172 6765 745f 6469 7229 0a0a 2020  (target_dir)..  
-00032840: 2020 7265 7475 726e 2063 6861 6e67 6564    return changed
-00032850: 0a0a 0a61 7379 6e63 2064 6566 2064 6966  ...async def dif
-00032860: 665f 6669 6c65 7328 0a20 2020 2066 726f  f_files(.    fro
-00032870: 6d5f 6669 6c65 3a20 7374 722c 0a20 2020  m_file: str,.   
-00032880: 2074 6f5f 6669 6c65 3a20 7374 722c 0a20   to_file: str,. 
-00032890: 2020 2066 726f 6d5f 6669 6c65 5f73 7566     from_file_suf
-000328a0: 6669 783a 2073 7472 203d 2022 5b72 656d  fix: str = "[rem
-000328b0: 6f74 655d 222c 0a20 2020 2074 6f5f 6669  ote]",.    to_fi
-000328c0: 6c65 5f73 7566 6669 783a 2073 7472 203d  le_suffix: str =
-000328d0: 2022 5b6c 6f63 616c 5d22 2c0a 2020 2020   "[local]",.    
-000328e0: 7769 7468 5f66 6f72 6d61 743a 2062 6f6f  with_format: boo
-000328f0: 6c20 3d20 5472 7565 2c0a 2020 2020 7769  l = True,.    wi
-00032900: 7468 5f63 6f6c 6f72 3a20 626f 6f6c 203d  th_color: bool =
-00032910: 2046 616c 7365 2c0a 2020 2020 636c 6965   False,.    clie
-00032920: 6e74 3a20 4f70 7469 6f6e 616c 5b54 696e  nt: Optional[Tin
-00032930: 7942 5d20 3d20 4e6f 6e65 2c0a 2020 2020  yB] = None,.    
-00032940: 666f 725f 6465 706c 6f79 3a20 626f 6f6c  for_deploy: bool
-00032950: 203d 2046 616c 7365 2c0a 293a 0a20 2020   = False,.):.   
-00032960: 2064 6566 2066 696c 655f 6c69 6e65 7328   def file_lines(
-00032970: 6669 6c65 6e61 6d65 293a 0a20 2020 2020  filename):.     
-00032980: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
-00032990: 656e 616d 6529 2061 7320 6669 6c65 3a0a  ename) as file:.
-000329a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000329b0: 726e 2066 696c 652e 7265 6164 6c69 6e65  rn file.readline
-000329c0: 7328 290a 0a20 2020 2061 7379 6e63 2064  s()..    async d
-000329d0: 6566 2070 6172 7365 2866 696c 656e 616d  ef parse(filenam
-000329e0: 652c 2077 6974 685f 666f 726d 6174 3d54  e, with_format=T
-000329f0: 7275 652c 2075 6e72 6f6c 6c5f 696e 636c  rue, unroll_incl
-00032a00: 7564 6573 3d46 616c 7365 293a 0a20 2020  udes=False):.   
-00032a10: 2020 2020 2065 7874 656e 7369 6f6e 7320       extensions 
-00032a20: 3d20 5061 7468 2866 696c 656e 616d 6529  = Path(filename)
-00032a30: 2e73 7566 6669 7865 730a 2020 2020 2020  .suffixes.      
-00032a40: 2020 6c69 6e65 7320 3d20 4e6f 6e65 0a20    lines = None. 
-00032a50: 2020 2020 2020 2069 6620 6973 5f66 696c         if is_fil
-00032a60: 655f 615f 6461 7461 736f 7572 6365 2866  e_a_datasource(f
-00032a70: 696c 656e 616d 6529 3a0a 2020 2020 2020  ilename):.      
-00032a80: 2020 2020 2020 6c69 6e65 7320 3d20 280a        lines = (.
-00032a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032aa0: 6177 6169 7420 666f 726d 6174 5f64 6174  await format_dat
-00032ab0: 6173 6f75 7263 6528 0a20 2020 2020 2020  asource(.       
-00032ac0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00032ad0: 656e 616d 652c 0a20 2020 2020 2020 2020  ename,.         
-00032ae0: 2020 2020 2020 2020 2020 2075 6e72 6f6c             unrol
-00032af0: 6c5f 696e 636c 7564 6573 3d75 6e72 6f6c  l_includes=unrol
-00032b00: 6c5f 696e 636c 7564 6573 2c0a 2020 2020  l_includes,.    
-00032b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032b20: 666f 725f 6469 6666 3d54 7275 652c 0a20  for_diff=True,. 
-00032b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032b40: 2020 2063 6c69 656e 743d 636c 6965 6e74     client=client
-00032b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00032b60: 2020 2020 2020 7265 706c 6163 655f 696e        replace_in
-00032b70: 636c 7564 6573 3d54 7275 652c 0a20 2020  cludes=True,.   
-00032b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032b90: 2066 6f72 5f64 6570 6c6f 795f 6469 6666   for_deploy_diff
-00032ba0: 3d66 6f72 5f64 6570 6c6f 792c 0a20 2020  =for_deploy,.   
-00032bb0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00032bc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00032bd0: 6620 7769 7468 5f66 6f72 6d61 740a 2020  f with_format.  
-00032be0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00032bf0: 7365 2066 696c 655f 6c69 6e65 7328 6669  se file_lines(fi
-00032c00: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
-00032c10: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00032c20: 6966 2028 222e 7069 7065 2220 696e 2065  if (".pipe" in e
-00032c30: 7874 656e 7369 6f6e 7329 206f 7220 2822  xtensions) or ("
-00032c40: 2e69 6e63 6c22 2069 6e20 6578 7465 6e73  .incl" in extens
-00032c50: 696f 6e73 293a 0a20 2020 2020 2020 2020  ions):.         
-00032c60: 2020 206c 696e 6573 203d 2028 0a20 2020     lines = (.   
-00032c70: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00032c80: 6974 2066 6f72 6d61 745f 7069 7065 280a  it format_pipe(.
-00032c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032ca0: 2020 2020 6669 6c65 6e61 6d65 2c0a 2020      filename,.  
-00032cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032cc0: 2020 4445 4641 554c 545f 464d 545f 4c49    DEFAULT_FMT_LI
-00032cd0: 4e45 5f4c 454e 4754 482c 0a20 2020 2020  NE_LENGTH,.     
-00032ce0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00032cf0: 6e72 6f6c 6c5f 696e 636c 7564 6573 3d75  nroll_includes=u
-00032d00: 6e72 6f6c 6c5f 696e 636c 7564 6573 2c0a  nroll_includes,.
-00032d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032d20: 2020 2020 7265 706c 6163 655f 696e 636c      replace_incl
-00032d30: 7564 6573 3d54 7275 652c 0a20 2020 2020  udes=True,.     
-00032d40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00032d50: 6f72 5f64 6570 6c6f 795f 6469 6666 3d66  or_deploy_diff=f
-00032d60: 6f72 5f64 6570 6c6f 792c 0a20 2020 2020  or_deploy,.     
-00032d70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00032d80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00032d90: 7769 7468 5f66 6f72 6d61 740a 2020 2020  with_format.    
-00032da0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00032db0: 2066 696c 655f 6c69 6e65 7328 6669 6c65   file_lines(file
-00032dc0: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
-00032dd0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-00032de0: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-00032df0: 6963 6b2e 6563 686f 2866 2255 6e73 7570  ick.echo(f"Unsup
-00032e00: 706f 7274 6564 2066 696c 6520 7479 7065  ported file type
-00032e10: 3a20 7b66 696c 656e 616d 657d 2229 0a20  : {filename}"). 
-00032e20: 2020 2020 2020 2069 6620 6c69 6e65 733a         if lines:
-00032e30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00032e40: 7572 6e20 5b66 227b 6c7d 5c6e 2220 666f  urn [f"{l}\n" fo
-00032e50: 7220 6c20 696e 206c 696e 6573 2e73 706c  r l in lines.spl
-00032e60: 6974 2822 5c6e 2229 5d20 6966 2077 6974  it("\n")] if wit
-00032e70: 685f 666f 726d 6174 2065 6c73 6520 6c69  h_format else li
-00032e80: 6e65 7320 2023 206e 6f71 613a 2045 3734  nes  # noqa: E74
-00032e90: 310a 0a20 2020 2074 7279 3a0a 2020 2020  1..    try:.    
-00032ea0: 2020 2020 6c69 6e65 7331 203d 2061 7761      lines1 = awa
-00032eb0: 6974 2070 6172 7365 2866 726f 6d5f 6669  it parse(from_fi
-00032ec0: 6c65 2c20 7769 7468 5f66 6f72 6d61 7429  le, with_format)
-00032ed0: 0a20 2020 2020 2020 206c 696e 6573 3220  .        lines2 
-00032ee0: 3d20 6177 6169 7420 7061 7273 6528 746f  = await parse(to
-00032ef0: 5f66 696c 652c 2077 6974 685f 666f 726d  _file, with_form
-00032f00: 6174 2c20 756e 726f 6c6c 5f69 6e63 6c75  at, unroll_inclu
-00032f10: 6465 733d 5472 7565 290a 2020 2020 6578  des=True).    ex
-00032f20: 6365 7074 2046 696c 654e 6f74 466f 756e  cept FileNotFoun
-00032f30: 6445 7272 6f72 2061 7320 653a 0a20 2020  dError as e:.   
-00032f40: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
-00032f50: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-00032f60: 2873 7472 2865 2929 2e73 7472 6970 2822  (str(e)).strip("
-00032f70: 2722 290a 2020 2020 2020 2020 7261 6973  '").        rais
-00032f80: 6520 636c 6963 6b2e 436c 6963 6b45 7863  e click.ClickExc
-00032f90: 6570 7469 6f6e 2846 6565 6462 6163 6b4d  eption(FeedbackM
-00032fa0: 616e 6167 6572 2e65 7272 6f72 5f64 6966  anager.error_dif
-00032fb0: 665f 6669 6c65 2866 696c 656e 616d 653d  f_file(filename=
-00032fc0: 6669 6c65 6e61 6d65 2929 0a0a 2020 2020  filename))..    
-00032fd0: 6966 206e 6f74 206c 696e 6573 3120 6f72  if not lines1 or
-00032fe0: 206e 6f74 206c 696e 6573 323a 0a20 2020   not lines2:.   
-00032ff0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00033000: 2064 6966 6620 3d20 6469 6666 6c69 622e   diff = difflib.
-00033010: 756e 6966 6965 645f 6469 6666 280a 2020  unified_diff(.  
-00033020: 2020 2020 2020 6c69 6e65 7331 2c20 6c69        lines1, li
-00033030: 6e65 7332 2c20 6672 6f6d 6669 6c65 3d66  nes2, fromfile=f
-00033040: 227b 5061 7468 2866 726f 6d5f 6669 6c65  "{Path(from_file
-00033050: 292e 6e61 6d65 7d20 7b66 726f 6d5f 6669  ).name} {from_fi
-00033060: 6c65 5f73 7566 6669 787d 222c 2074 6f66  le_suffix}", tof
-00033070: 696c 653d 6622 7b74 6f5f 6669 6c65 7d20  ile=f"{to_file} 
-00033080: 7b74 6f5f 6669 6c65 5f73 7566 6669 787d  {to_file_suffix}
-00033090: 220a 2020 2020 290a 0a20 2020 2069 6620  ".    )..    if 
-000330a0: 7769 7468 5f63 6f6c 6f72 3a0a 2020 2020  with_color:.    
-000330b0: 2020 2020 6469 6666 203d 2063 6f6c 6f72      diff = color
-000330c0: 5f64 6966 6628 6469 6666 290a 0a20 2020  _diff(diff)..   
-000330d0: 2072 6574 7572 6e20 6469 6666 0a0a 0a64   return diff...d
-000330e0: 6566 2069 735f 656e 6470 6f69 6e74 2872  ef is_endpoint(r
-000330f0: 6573 6f75 7263 653a 204f 7074 696f 6e61  esource: Optiona
-00033100: 6c5b 4469 6374 5b73 7472 2c20 416e 795d  l[Dict[str, Any]
-00033110: 5d29 202d 3e20 626f 6f6c 3a0a 2020 2020  ]) -> bool:.    
-00033120: 6966 2072 6573 6f75 7263 6520 616e 6420  if resource and 
-00033130: 6c65 6e28 7265 736f 7572 6365 2e67 6574  len(resource.get
-00033140: 2822 746f 6b65 6e73 222c 205b 5d29 2920  ("tokens", [])) 
-00033150: 213d 2030 2061 6e64 2072 6573 6f75 7263  != 0 and resourc
-00033160: 652e 6765 7428 2272 6573 6f75 7263 6522  e.get("resource"
-00033170: 2920 3d3d 2022 7069 7065 7322 3a0a 2020  ) == "pipes":.  
-00033180: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00033190: 650a 2020 2020 7265 7475 726e 2046 616c  e.    return Fal
-000331a0: 7365 0a0a 0a64 6566 2069 735f 6d61 7465  se...def is_mate
-000331b0: 7269 616c 697a 6564 2872 6573 6f75 7263  rialized(resourc
-000331c0: 653a 204f 7074 696f 6e61 6c5b 4469 6374  e: Optional[Dict
-000331d0: 5b73 7472 2c20 416e 795d 5d29 202d 3e20  [str, Any]]) -> 
-000331e0: 626f 6f6c 3a0a 2020 2020 6966 206e 6f74  bool:.    if not
-000331f0: 2072 6573 6f75 7263 653a 0a20 2020 2020   resource:.     
-00033200: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00033210: 0a20 2020 2069 735f 6d61 7465 7269 616c  .    is_material
-00033220: 697a 6564 203d 2061 6e79 280a 2020 2020  ized = any(.    
-00033230: 2020 2020 5b6e 6f64 652e 6765 7428 2270      [node.get("p
-00033240: 6172 616d 7322 2c20 7b7d 292e 6765 7428  arams", {}).get(
-00033250: 2274 7970 6522 2c20 4e6f 6e65 2920 3d3d  "type", None) ==
-00033260: 2022 6d61 7465 7269 616c 697a 6564 2220   "materialized" 
-00033270: 666f 7220 6e6f 6465 2069 6e20 7265 736f  for node in reso
-00033280: 7572 6365 2e67 6574 2822 6e6f 6465 7322  urce.get("nodes"
-00033290: 2c20 5b5d 2920 6f72 205b 5d5d 0a20 2020  , []) or []].   
-000332a0: 2029 0a20 2020 2072 6574 7572 6e20 6973   ).    return is
-000332b0: 5f6d 6174 6572 6961 6c69 7a65 640a 0a0a  _materialized...
-000332c0: 6465 6620 6973 5f65 6e64 706f 696e 745f  def is_endpoint_
-000332d0: 7769 7468 5f6e 6f5f 6465 7065 6e64 656e  with_no_dependen
-000332e0: 6369 6573 280a 2020 2020 7265 736f 7572  cies(.    resour
-000332f0: 6365 3a20 4469 6374 5b73 7472 2c20 416e  ce: Dict[str, An
-00033300: 795d 2c20 6465 705f 6d61 703a 2044 6963  y], dep_map: Dic
-00033310: 745b 7374 722c 2053 6574 5b73 7472 5d5d  t[str, Set[str]]
-00033320: 2c20 746f 5f72 756e 3a20 4469 6374 5b73  , to_run: Dict[s
-00033330: 7472 2c20 4469 6374 5b73 7472 2c20 416e  tr, Dict[str, An
-00033340: 795d 5d0a 2920 2d3e 2062 6f6f 6c3a 0a20  y]].) -> bool:. 
-00033350: 2020 2069 6620 6e6f 7420 7265 736f 7572     if not resour
-00033360: 6365 206f 7220 7265 736f 7572 6365 2e67  ce or resource.g
-00033370: 6574 2822 7265 736f 7572 6365 2229 203d  et("resource") =
-00033380: 3d20 2264 6174 6173 6f75 7263 6573 223a  = "datasources":
-00033390: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000333a0: 4661 6c73 650a 0a20 2020 2066 6f72 206e  False..    for n
-000333b0: 6f64 6520 696e 2072 6573 6f75 7263 652e  ode in resource.
-000333c0: 6765 7428 226e 6f64 6573 222c 205b 5d29  get("nodes", [])
-000333d0: 3a0a 2020 2020 2020 2020 2320 4649 584d  :.        # FIXM
-000333e0: 453a 2068 7474 7073 3a2f 2f67 6974 6c61  E: https://gitla
-000333f0: 622e 636f 6d2f 7469 6e79 6269 7264 2f61  b.com/tinybird/a
-00033400: 6e61 6c79 7469 6373 2f2d 2f69 7373 7565  nalytics/-/issue
-00033410: 732f 3233 3931 0a20 2020 2020 2020 2069  s/2391.        i
-00033420: 6620 6e6f 6465 2e67 6574 2822 7061 7261  f node.get("para
-00033430: 6d73 222c 207b 7d29 2e67 6574 2822 7479  ms", {}).get("ty
-00033440: 7065 222c 2022 2229 2e6c 6f77 6572 2829  pe", "").lower()
-00033450: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-00033460: 2020 5069 7065 4e6f 6465 5479 7065 732e    PipeNodeTypes.
-00033470: 4d41 5445 5249 414c 495a 4544 2c0a 2020  MATERIALIZED,.  
-00033480: 2020 2020 2020 2020 2020 5069 7065 4e6f            PipeNo
-00033490: 6465 5479 7065 732e 434f 5059 2c0a 2020  deTypes.COPY,.  
-000334a0: 2020 2020 2020 2020 2020 5069 7065 4e6f            PipeNo
-000334b0: 6465 5479 7065 732e 4441 5441 5f53 494e  deTypes.DATA_SIN
-000334c0: 4b2c 0a20 2020 2020 2020 205d 3a0a 2020  K,.        ]:.  
-000334d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000334e0: 2046 616c 7365 0a0a 2020 2020 666f 7220   False..    for 
-000334f0: 6b65 792c 2076 616c 7565 7320 696e 2064  key, values in d
-00033500: 6570 5f6d 6170 2e69 7465 6d73 2829 3a0a  ep_map.items():.
-00033510: 2020 2020 2020 2020 6966 2072 6573 6f75          if resou
-00033520: 7263 655b 2272 6573 6f75 7263 655f 6e61  rce["resource_na
-00033530: 6d65 225d 2069 6e20 7661 6c75 6573 3a0a  me"] in values:.
-00033540: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
-00033550: 746f 5f72 756e 2e67 6574 286b 6579 2c20  to_run.get(key, 
-00033560: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
-00033570: 2020 6966 206e 6f74 2072 3a0a 2020 2020    if not r:.    
-00033580: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00033590: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-000335a0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-000335b0: 2020 2064 6570 7320 3d20 6465 705f 6d61     deps = dep_ma
-000335c0: 702e 6765 7428 7265 736f 7572 6365 5b22  p.get(resource["
-000335d0: 7265 736f 7572 6365 5f6e 616d 6522 5d29  resource_name"])
-000335e0: 0a20 2020 2069 6620 6e6f 7420 6465 7073  .    if not deps
-000335f0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00033600: 2054 7275 650a 0a20 2020 2066 6f72 2064   True..    for d
-00033610: 6570 2069 6e20 6465 7073 3a0a 2020 2020  ep in deps:.    
-00033620: 2020 2020 7220 3d20 746f 5f72 756e 2e67      r = to_run.g
-00033630: 6574 2864 6570 2c20 4e6f 6e65 290a 2020  et(dep, None).  
-00033640: 2020 2020 2020 6966 2069 735f 656e 6470        if is_endp
-00033650: 6f69 6e74 2872 2920 6f72 2069 735f 6d61  oint(r) or is_ma
-00033660: 7465 7269 616c 697a 6564 2872 293a 0a20  terialized(r):. 
-00033670: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00033680: 6e20 4661 6c73 650a 0a20 2020 2072 6574  n False..    ret
-00033690: 7572 6e20 5472 7565 0a0a 0a64 6566 2067  urn True...def g
-000336a0: 6574 5f74 6172 6765 745f 6d61 7465 7269  et_target_materi
-000336b0: 616c 697a 6564 5f64 6174 615f 736f 7572  alized_data_sour
-000336c0: 6365 5f6e 616d 6528 7265 736f 7572 6365  ce_name(resource
-000336d0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-000336e0: 7374 722c 2041 6e79 5d5d 2920 2d3e 204f  str, Any]]) -> O
-000336f0: 7074 696f 6e61 6c5b 7374 725d 3a0a 2020  ptional[str]:.  
-00033700: 2020 6966 206e 6f74 2072 6573 6f75 7263    if not resourc
-00033710: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00033720: 6e20 4e6f 6e65 0a0a 2020 2020 666f 7220  n None..    for 
-00033730: 6e6f 6465 2069 6e20 7265 736f 7572 6365  node in resource
-00033740: 2e67 6574 2822 6e6f 6465 7322 2c20 5b5d  .get("nodes", []
-00033750: 293a 0a20 2020 2020 2020 2023 2046 4958  ):.        # FIX
-00033760: 4d45 3a20 6874 7470 733a 2f2f 6769 746c  ME: https://gitl
-00033770: 6162 2e63 6f6d 2f74 696e 7962 6972 642f  ab.com/tinybird/
-00033780: 616e 616c 7974 6963 732f 2d2f 6973 7375  analytics/-/issu
-00033790: 6573 2f32 3339 310a 2020 2020 2020 2020  es/2391.        
-000337a0: 6966 206e 6f64 652e 6765 7428 2270 6172  if node.get("par
-000337b0: 616d 7322 2c20 7b7d 292e 6765 7428 2274  ams", {}).get("t
-000337c0: 7970 6522 2c20 2222 292e 6c6f 7765 7228  ype", "").lower(
-000337d0: 2920 3d3d 2050 6970 654e 6f64 6554 7970  ) == PipeNodeTyp
-000337e0: 6573 2e4d 4154 4552 4941 4c49 5a45 443a  es.MATERIALIZED:
-000337f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00033800: 7572 6e20 6e6f 6465 2e67 6574 2822 7061  urn node.get("pa
-00033810: 7261 6d73 2229 5b22 6461 7461 736f 7572  rams")["datasour
-00033820: 6365 225d 2e73 706c 6974 2822 5f5f 7622  ce"].split("__v"
-00033830: 295b 305d 0a0a 2020 2020 7265 7475 726e  )[0]..    return
-00033840: 204e 6f6e 650a 0a0a 6465 6620 6973 5f64   None...def is_d
-00033850: 6174 6173 6f75 7263 6528 7265 736f 7572  atasource(resour
-00033860: 6365 3a20 4f70 7469 6f6e 616c 5b44 6963  ce: Optional[Dic
-00033870: 745b 7374 722c 2041 6e79 5d5d 2920 2d3e  t[str, Any]]) ->
-00033880: 2062 6f6f 6c3a 0a20 2020 2069 6620 7265   bool:.    if re
-00033890: 736f 7572 6365 2061 6e64 2072 6573 6f75  source and resou
-000338a0: 7263 652e 6765 7428 2272 6573 6f75 7263  rce.get("resourc
-000338b0: 6522 2920 3d3d 2022 6461 7461 736f 7572  e") == "datasour
-000338c0: 6365 7322 3a0a 2020 2020 2020 2020 7265  ces":.        re
-000338d0: 7475 726e 2054 7275 650a 2020 2020 7265  turn True.    re
-000338e0: 7475 726e 2046 616c 7365 0a0a 0a61 7379  turn False...asy
-000338f0: 6e63 2064 6566 2063 7265 6174 655f 7265  nc def create_re
-00033900: 6c65 6173 6528 0a20 2020 2063 6c69 656e  lease(.    clien
-00033910: 743a 2054 696e 7942 2c20 636f 6e66 6967  t: TinyB, config
-00033920: 3a20 556e 696f 6e5b 4469 6374 5b73 7472  : Union[Dict[str
-00033930: 2c20 416e 795d 2c20 434c 4943 6f6e 6669  , Any], CLIConfi
-00033940: 675d 2c20 7365 6d76 6572 3a20 7374 722c  g], semver: str,
-00033950: 2066 6f6c 6465 723a 204f 7074 696f 6e61   folder: Optiona
-00033960: 6c5b 7374 725d 203d 204e 6f6e 650a 2920  l[str] = None.) 
-00033970: 2d3e 204e 6f6e 653a 0a20 2020 2069 6620  -> None:.    if 
-00033980: 6e6f 7420 666f 6c64 6572 3a0a 2020 2020  not folder:.    
-00033990: 2020 2020 666f 6c64 6572 203d 2067 6574      folder = get
-000339a0: 6377 6428 290a 2020 2020 636c 695f 6769  cwd().    cli_gi
-000339b0: 745f 7265 6c65 6173 6520 3d20 4e6f 6e65  t_release = None
-000339c0: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-000339d0: 2020 636c 695f 6769 745f 7265 6c65 6173    cli_git_releas
-000339e0: 6520 3d20 434c 4947 6974 5265 6c65 6173  e = CLIGitReleas
-000339f0: 6528 7061 7468 3d66 6f6c 6465 7229 0a20  e(path=folder). 
-00033a00: 2020 2020 2020 2063 6f6d 6d69 7420 3d20         commit = 
-00033a10: 636c 695f 6769 745f 7265 6c65 6173 652e  cli_git_release.
-00033a20: 6865 6164 5f63 6f6d 6d69 7428 290a 2020  head_commit().  
-00033a30: 2020 6578 6365 7074 2043 4c49 4769 7452    except CLIGitR
-00033a40: 656c 6561 7365 4578 6365 7074 696f 6e3a  eleaseException:
-00033a50: 0a20 2020 2020 2020 2072 6169 7365 2043  .        raise C
-00033a60: 4c49 4769 7452 656c 6561 7365 4578 6365  LIGitReleaseExce
-00033a70: 7074 696f 6e28 4665 6564 6261 636b 4d61  ption(FeedbackMa
-00033a80: 6e61 6765 722e 6572 726f 725f 6e6f 5f67  nager.error_no_g
-00033a90: 6974 5f72 6570 6f5f 666f 725f 696e 6974  it_repo_for_init
-00033aa0: 2872 6570 6f5f 7061 7468 3d66 6f6c 6465  (repo_path=folde
-00033ab0: 7229 290a 0a20 2020 2061 7761 6974 2063  r))..    await c
-00033ac0: 6c69 656e 742e 7265 6c65 6173 655f 6e65  lient.release_ne
-00033ad0: 7728 636f 6e66 6967 5b22 6964 225d 2c20  w(config["id"], 
-00033ae0: 7365 6d76 6572 2c20 636f 6d6d 6974 290a  semver, commit).
-00033af0: 2020 2020 636c 6963 6b2e 6563 686f 2846      click.echo(F
-00033b00: 6565 6462 6163 6b4d 616e 6167 6572 2e73  eedbackManager.s
-00033b10: 7563 6365 7373 5f64 6570 6c6f 796d 656e  uccess_deploymen
-00033b20: 745f 7265 6c65 6173 6528 7365 6d76 6572  t_release(semver
-00033b30: 3d73 656d 7665 7229 290a 0a0a 6465 6620  =semver))...def 
-00033b40: 6861 735f 696e 7465 726e 616c 5f64 6174  has_internal_dat
-00033b50: 6166 696c 6573 2866 6f6c 6465 723a 2073  afiles(folder: s
-00033b60: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
-00033b70: 2066 6f6c 6465 7220 3d20 666f 6c64 6572   folder = folder
-00033b80: 206f 7220 222e 220a 2020 2020 6669 6c65   or ".".    file
-00033b90: 6e61 6d65 7320 3d20 6765 745f 7072 6f6a  names = get_proj
-00033ba0: 6563 745f 6669 6c65 6e61 6d65 7328 666f  ect_filenames(fo
-00033bb0: 6c64 6572 290a 2020 2020 7265 7475 726e  lder).    return
-00033bc0: 2061 6e79 285b 6620 666f 7220 6620 696e   any([f for f in
-00033bd0: 2066 696c 656e 616d 6573 2069 6620 2273   filenames if "s
-00033be0: 7061 6e73 2220 696e 2073 7472 2866 2920  pans" in str(f) 
-00033bf0: 616e 6420 2276 656e 646f 7222 206e 6f74  and "vendor" not
-00033c00: 2069 6e20 7374 7228 6629 5d29 0a0a 0a64   in str(f)])...d
-00033c10: 6566 2069 735f 6669 6c65 5f61 5f64 6174  ef is_file_a_dat
-00033c20: 6173 6f75 7263 6528 6669 6c65 6e61 6d65  asource(filename
-00033c30: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
-00033c40: 2020 2020 6578 7465 6e73 696f 6e73 203d      extensions =
-00033c50: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
-00033c60: 7375 6666 6978 6573 0a20 2020 2069 6620  suffixes.    if 
-00033c70: 222e 6461 7461 736f 7572 6365 2220 696e  ".datasource" in
-00033c80: 2065 7874 656e 7369 6f6e 733a 2020 2320   extensions:  # 
-00033c90: 4163 6365 7074 7320 272e 6461 7461 736f  Accepts '.dataso
-00033ca0: 7572 6365 2720 616e 6420 272e 6461 7461  urce' and '.data
-00033cb0: 736f 7572 6365 2e69 6e63 6c27 0a20 2020  source.incl'.   
-00033cc0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00033cd0: 0a0a 2020 2020 6966 2022 2e69 6e63 6c22  ..    if ".incl"
-00033ce0: 2069 6e20 6578 7465 6e73 696f 6e73 3a0a   in extensions:.
-00033cf0: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-00033d00: 5b5d 0a20 2020 2020 2020 2077 6974 6820  [].        with 
-00033d10: 6f70 656e 2866 696c 656e 616d 6529 2061  open(filename) a
-00033d20: 7320 6669 6c65 3a0a 2020 2020 2020 2020  s file:.        
-00033d30: 2020 2020 6c69 6e65 7320 3d20 6669 6c65      lines = file
-00033d40: 2e72 6561 646c 696e 6573 2829 0a0a 2020  .readlines()..  
-00033d50: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-00033d60: 6e20 6c69 6e65 733a 0a20 2020 2020 2020  n lines:.       
-00033d70: 2020 2020 2074 7269 6d6d 6564 5f6c 696e       trimmed_lin
-00033d80: 6520 3d20 6c69 6e65 2e73 7472 6970 2829  e = line.strip()
-00033d90: 2e6c 6f77 6572 2829 0a20 2020 2020 2020  .lower().       
-00033da0: 2020 2020 2069 6620 7472 696d 6d65 645f       if trimmed_
-00033db0: 6c69 6e65 2e73 7461 7274 7377 6974 6828  line.startswith(
-00033dc0: 2273 6368 656d 6122 2920 6f72 2074 7269  "schema") or tri
-00033dd0: 6d6d 6564 5f6c 696e 652e 7374 6172 7473  mmed_line.starts
-00033de0: 7769 7468 2822 656e 6769 6e65 2229 3a0a  with("engine"):.
-00033df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033e00: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
-00033e10: 2072 6574 7572 6e20 4661 6c73 650a        return False.
+000313d0: 2020 2020 2020 2020 6664 2e77 7269 7465          fd.write
+000313e0: 2872 6573 6f75 7263 6529 0a20 2020 2020  (resource).     
+000313f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00031400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00031410: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
+00031420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00031430: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
+00031440: 6368 6f28 4665 6564 6261 636b 4d61 6e61  cho(FeedbackMana
+00031450: 6765 722e 696e 666f 5f73 6b69 705f 616c  ger.info_skip_al
+00031460: 7265 6164 795f 6578 6973 7473 2829 290a  ready_exists()).
+00031470: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00031480: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00031490: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000314a0: 2020 2072 6169 7365 2063 6c69 636b 2e43     raise click.C
+000314b0: 6c69 636b 4578 6365 7074 696f 6e28 4665  lickException(Fe
+000314c0: 6564 6261 636b 4d61 6e61 6765 722e 6572  edbackManager.er
+000314d0: 726f 725f 6578 6365 7074 696f 6e28 6572  ror_exception(er
+000314e0: 726f 723d 6529 290a 0a20 2020 2020 2020  ror=e))..       
+000314f0: 2076 616c 7565 7320 3d20 7665 7273 696f   values = versio
+00031500: 6e73 2e76 616c 7565 7328 290a 0a20 2020  ns.values()..   
+00031510: 2020 2020 2069 6620 7072 6f67 7265 7373       if progress
+00031520: 5f62 6172 3a0a 2020 2020 2020 2020 2020  _bar:.          
+00031530: 2020 7769 7468 2063 6c69 636b 2e70 726f    with click.pro
+00031540: 6772 6573 7362 6172 2876 616c 7565 732c  gressbar(values,
+00031550: 206c 6162 656c 3d66 2250 756c 6c69 6e67   label=f"Pulling
+00031560: 207b 6578 7465 6e73 696f 6e7d 7322 2920   {extension}s") 
+00031570: 6173 2076 616c 7565 733a 2020 2320 7479  as values:  # ty
+00031580: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
+00031590: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+000315a0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+000315b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000315c0: 6177 6169 7420 7772 6974 655f 7265 736f  await write_reso
+000315d0: 7572 6365 286b 290a 2020 2020 2020 2020  urce(k).        
+000315e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000315f0: 2020 7461 736b 7320 3d20 5b77 7269 7465    tasks = [write
+00031600: 5f72 6573 6f75 7263 6528 6b29 2066 6f72  _resource(k) for
+00031610: 206b 2069 6e20 7661 6c75 6573 5d0a 2020   k in values].  
+00031620: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00031630: 5f67 6174 6865 725f 7769 7468 5f63 6f6e  _gather_with_con
+00031640: 6375 7272 656e 6379 2835 2c20 2a74 6173  currency(5, *tas
+00031650: 6b73 290a 0a20 2020 2074 7279 3a0a 2020  ks)..    try:.  
+00031660: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
+00031670: 7320 3d20 6177 6169 7420 636c 6965 6e74  s = await client
+00031680: 2e64 6174 6173 6f75 7263 6573 2829 0a20  .datasources(). 
+00031690: 2020 2020 2020 2072 656d 6f74 655f 6461         remote_da
+000316a0: 7461 736f 7572 6365 7320 3d20 736f 7274  tasources = sort
+000316b0: 6564 285b 785b 226e 616d 6522 5d20 666f  ed([x["name"] fo
+000316c0: 7220 7820 696e 2064 6174 6173 6f75 7263  r x in datasourc
+000316d0: 6573 5d29 0a20 2020 2020 2020 2064 6174  es]).        dat
+000316e0: 6173 6f75 7263 6573 5f76 6572 7369 6f6e  asources_version
+000316f0: 7320 3d20 5f67 6574 5f6c 6174 6573 745f  s = _get_latest_
+00031700: 7665 7273 696f 6e73 2872 656d 6f74 655f  versions(remote_
+00031710: 6461 7461 736f 7572 6365 7329 0a0a 2020  datasources)..  
+00031720: 2020 2020 2020 7069 7065 7320 3d20 6177        pipes = aw
+00031730: 6169 7420 636c 6965 6e74 2e70 6970 6573  ait client.pipes
+00031740: 2829 0a20 2020 2020 2020 2072 656d 6f74  ().        remot
+00031750: 655f 7069 7065 7320 3d20 736f 7274 6564  e_pipes = sorted
+00031760: 285b 785b 226e 616d 6522 5d20 666f 7220  ([x["name"] for 
+00031770: 7820 696e 2070 6970 6573 5d29 0a20 2020  x in pipes]).   
+00031780: 2020 2020 2070 6970 6573 5f76 6572 7369       pipes_versi
+00031790: 6f6e 7320 3d20 5f67 6574 5f6c 6174 6573  ons = _get_lates
+000317a0: 745f 7665 7273 696f 6e73 2872 656d 6f74  t_versions(remot
+000317b0: 655f 7069 7065 7329 0a0a 2020 2020 2020  e_pipes)..      
+000317c0: 2020 7265 736f 7572 6365 7320 3d20 6c69    resources = li
+000317d0: 7374 2864 6174 6173 6f75 7263 6573 5f76  st(datasources_v
+000317e0: 6572 7369 6f6e 732e 6b65 7973 2829 2920  ersions.keys()) 
+000317f0: 2b20 6c69 7374 2870 6970 6573 5f76 6572  + list(pipes_ver
+00031800: 7369 6f6e 732e 6b65 7973 2829 290a 0a20  sions.keys()).. 
+00031810: 2020 2020 2020 2061 7761 6974 2077 7269         await wri
+00031820: 7465 5f66 696c 6573 2864 6174 6173 6f75  te_files(datasou
+00031830: 7263 6573 5f76 6572 7369 6f6e 732c 2072  rces_versions, r
+00031840: 6573 6f75 7263 6573 2c20 2264 6174 6173  esources, "datas
+00031850: 6f75 7263 6522 2c20 2264 6174 6173 6f75  ource", "datasou
+00031860: 7263 655f 6669 6c65 222c 2070 726f 6772  rce_file", progr
+00031870: 6573 735f 6261 723d 7072 6f67 7265 7373  ess_bar=progress
+00031880: 5f62 6172 290a 2020 2020 2020 2020 6177  _bar).        aw
+00031890: 6169 7420 7772 6974 655f 6669 6c65 7328  ait write_files(
+000318a0: 7069 7065 735f 7665 7273 696f 6e73 2c20  pipes_versions, 
+000318b0: 7265 736f 7572 6365 732c 2022 7069 7065  resources, "pipe
+000318c0: 222c 2022 7069 7065 5f66 696c 6522 2c20  ", "pipe_file", 
+000318d0: 7072 6f67 7265 7373 5f62 6172 3d70 726f  progress_bar=pro
+000318e0: 6772 6573 735f 6261 7229 0a0a 2020 2020  gress_bar)..    
+000318f0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00031900: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00031910: 2061 7320 653a 0a20 2020 2020 2020 2072   as e:.        r
+00031920: 6169 7365 2063 6c69 636b 2e43 6c69 636b  aise click.Click
+00031930: 4578 6365 7074 696f 6e28 4665 6564 6261  Exception(Feedba
+00031940: 636b 4d61 6e61 6765 722e 6572 726f 725f  ckManager.error_
+00031950: 7075 6c6c 2865 7272 6f72 3d73 7472 2865  pull(error=str(e
+00031960: 2929 290a 0a0a 6465 6620 636f 6c6f 725f  )))...def color_
+00031970: 6469 6666 2864 6966 663a 2049 7465 7261  diff(diff: Itera
+00031980: 626c 655b 7374 725d 2920 2d3e 2047 656e  ble[str]) -> Gen
+00031990: 6572 6174 6f72 5b73 7472 2c20 416e 792c  erator[str, Any,
+000319a0: 204e 6f6e 655d 3a0a 2020 2020 666f 7220   None]:.    for 
+000319b0: 6c69 6e65 2069 6e20 6469 6666 3a0a 2020  line in diff:.  
+000319c0: 2020 2020 2020 6966 206c 696e 652e 7374        if line.st
+000319d0: 6172 7473 7769 7468 2822 2b22 293a 0a20  artswith("+"):. 
+000319e0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+000319f0: 2046 6f72 652e 4752 4545 4e20 2b20 6c69   Fore.GREEN + li
+00031a00: 6e65 202b 2046 6f72 652e 5245 5345 540a  ne + Fore.RESET.
+00031a10: 2020 2020 2020 2020 656c 6966 206c 696e          elif lin
+00031a20: 652e 7374 6172 7473 7769 7468 2822 2d22  e.startswith("-"
+00031a30: 293a 0a20 2020 2020 2020 2020 2020 2079  ):.            y
+00031a40: 6965 6c64 2046 6f72 652e 5245 4420 2b20  ield Fore.RED + 
+00031a50: 6c69 6e65 202b 2046 6f72 652e 5245 5345  line + Fore.RESE
+00031a60: 540a 2020 2020 2020 2020 656c 6966 206c  T.        elif l
+00031a70: 696e 652e 7374 6172 7473 7769 7468 2822  ine.startswith("
+00031a80: 5e22 293a 0a20 2020 2020 2020 2020 2020  ^"):.           
+00031a90: 2079 6965 6c64 2046 6f72 652e 424c 5545   yield Fore.BLUE
+00031aa0: 202b 206c 696e 6520 2b20 466f 7265 2e52   + line + Fore.R
+00031ab0: 4553 4554 0a20 2020 2020 2020 2065 6c73  ESET.        els
+00031ac0: 653a 0a20 2020 2020 2020 2020 2020 2079  e:.            y
+00031ad0: 6965 6c64 206c 696e 650a 0a0a 6465 6620  ield line...def 
+00031ae0: 7065 656b 2869 7465 7261 626c 6529 3a0a  peek(iterable):.
+00031af0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00031b00: 2066 6972 7374 203d 206e 6578 7428 6974   first = next(it
+00031b10: 6572 6162 6c65 290a 2020 2020 6578 6365  erable).    exce
+00031b20: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
+00031b30: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00031b40: 652c 204e 6f6e 650a 2020 2020 7265 7475  e, None.    retu
+00031b50: 726e 2066 6972 7374 2c20 6974 6572 746f  rn first, iterto
+00031b60: 6f6c 732e 6368 6169 6e28 5b66 6972 7374  ols.chain([first
+00031b70: 5d2c 2069 7465 7261 626c 6529 0a0a 0a61  ], iterable)...a
+00031b80: 7379 6e63 2064 6566 2064 6966 665f 636f  sync def diff_co
+00031b90: 6d6d 616e 6428 0a20 2020 2066 696c 656e  mmand(.    filen
+00031ba0: 616d 6573 3a20 4f70 7469 6f6e 616c 5b4c  ames: Optional[L
+00031bb0: 6973 745b 7374 725d 5d2c 0a20 2020 2066  ist[str]],.    f
+00031bc0: 6d74 3a20 626f 6f6c 2c0a 2020 2020 636c  mt: bool,.    cl
+00031bd0: 6965 6e74 3a20 5469 6e79 422c 0a20 2020  ient: TinyB,.   
+00031be0: 206e 6f5f 636f 6c6f 723a 204f 7074 696f   no_color: Optio
+00031bf0: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
+00031c00: 652c 0a20 2020 2077 6974 685f 7072 696e  e,.    with_prin
+00031c10: 743a 204f 7074 696f 6e61 6c5b 626f 6f6c  t: Optional[bool
+00031c20: 5d20 3d20 5472 7565 2c0a 2020 2020 7665  ] = True,.    ve
+00031c30: 7262 6f73 653a 204f 7074 696f 6e61 6c5b  rbose: Optional[
+00031c40: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020  bool] = None,.  
+00031c50: 2020 636c 6561 6e5f 7570 3a20 4f70 7469    clean_up: Opti
+00031c60: 6f6e 616c 5b62 6f6f 6c5d 203d 2046 616c  onal[bool] = Fal
+00031c70: 7365 2c0a 2020 2020 7072 6f67 7265 7373  se,.    progress
+00031c80: 5f62 6172 3a20 626f 6f6c 203d 2046 616c  _bar: bool = Fal
+00031c90: 7365 2c0a 2020 2020 666f 725f 6465 706c  se,.    for_depl
+00031ca0: 6f79 3a20 626f 6f6c 203d 2046 616c 7365  oy: bool = False
+00031cb0: 2c0a 293a 0a20 2020 2064 6566 2069 735f  ,.):.    def is_
+00031cc0: 7368 6172 6564 5f64 6174 6173 6f75 7263  shared_datasourc
+00031cd0: 6528 6e61 6d65 293a 0a20 2020 2020 2020  e(name):.       
+00031ce0: 2072 6574 7572 6e20 222e 2220 696e 206e   return "." in n
+00031cf0: 616d 650a 0a20 2020 2077 6974 685f 6578  ame..    with_ex
+00031d00: 706c 6963 6974 5f66 696c 656e 616d 6573  plicit_filenames
+00031d10: 203d 2066 696c 656e 616d 6573 0a20 2020   = filenames.   
+00031d20: 2076 6572 626f 7365 203d 2054 7275 6520   verbose = True 
+00031d30: 6966 2076 6572 626f 7365 2069 7320 4e6f  if verbose is No
+00031d40: 6e65 2065 6c73 6520 7665 7262 6f73 650a  ne else verbose.
+00031d50: 0a20 2020 2074 6172 6765 745f 6469 7220  .    target_dir 
+00031d60: 3d20 6765 7463 7764 2829 202b 206f 732e  = getcwd() + os.
+00031d70: 7061 7468 2e73 6570 202b 2022 2e64 6966  path.sep + ".dif
+00031d80: 665f 746d 7022 0a20 2020 2050 6174 6828  f_tmp".    Path(
+00031d90: 7461 7267 6574 5f64 6972 292e 6d6b 6469  target_dir).mkdi
+00031da0: 7228 7061 7265 6e74 733d 5472 7565 2c20  r(parents=True, 
+00031db0: 6578 6973 745f 6f6b 3d54 7275 6529 0a0a  exist_ok=True)..
+00031dc0: 2020 2020 6966 2066 696c 656e 616d 6573      if filenames
+00031dd0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
+00031de0: 2866 696c 656e 616d 6573 2920 3d3d 2031  (filenames) == 1
+00031df0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00031e00: 6c65 6e61 6d65 7320 3d20 5b66 696c 656e  lenames = [filen
+00031e10: 616d 6573 5b30 5d5d 202b 2067 6574 5f70  ames[0]] + get_p
+00031e20: 726f 6a65 6374 5f66 696c 656e 616d 6573  roject_filenames
+00031e30: 2866 696c 656e 616d 6573 5b30 5d29 0a20  (filenames[0]). 
+00031e40: 2020 2020 2020 2061 7761 6974 2066 6f6c         await fol
+00031e50: 6465 725f 7075 6c6c 2863 6c69 656e 742c  der_pull(client,
+00031e60: 2074 6172 6765 745f 6469 722c 2046 616c   target_dir, Fal
+00031e70: 7365 2c20 4e6f 6e65 2c20 5472 7565 2c20  se, None, True, 
+00031e80: 7665 7262 6f73 653d 4661 6c73 6529 0a20  verbose=False). 
+00031e90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00031ea0: 2066 696c 656e 616d 6573 203d 2067 6574   filenames = get
+00031eb0: 5f70 726f 6a65 6374 5f66 696c 656e 616d  _project_filenam
+00031ec0: 6573 2822 2e22 290a 2020 2020 2020 2020  es(".").        
+00031ed0: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+00031ee0: 2020 2020 2020 2020 636c 6963 6b2e 6563          click.ec
+00031ef0: 686f 2822 5361 7669 6e67 2072 656d 6f74  ho("Saving remot
+00031f00: 6520 7265 736f 7572 6365 7320 696e 202e  e resources in .
+00031f10: 6469 6666 5f74 6d70 2066 6f6c 6465 722e  diff_tmp folder.
+00031f20: 5c6e 2229 0a20 2020 2020 2020 2061 7761  \n").        awa
+00031f30: 6974 2066 6f6c 6465 725f 7075 6c6c 2863  it folder_pull(c
+00031f40: 6c69 656e 742c 2074 6172 6765 745f 6469  lient, target_di
+00031f50: 722c 2046 616c 7365 2c20 4e6f 6e65 2c20  r, False, None, 
+00031f60: 5472 7565 2c20 7665 7262 6f73 653d 7665  True, verbose=ve
+00031f70: 7262 6f73 652c 2070 726f 6772 6573 735f  rbose, progress_
+00031f80: 6261 723d 7072 6f67 7265 7373 5f62 6172  bar=progress_bar
+00031f90: 290a 0a20 2020 2072 656d 6f74 655f 6461  )..    remote_da
+00031fa0: 7461 736f 7572 6365 733a 204c 6973 745b  tasources: List[
+00031fb0: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
+00031fc0: 3d20 6177 6169 7420 636c 6965 6e74 2e64  = await client.d
+00031fd0: 6174 6173 6f75 7263 6573 2829 0a20 2020  atasources().   
+00031fe0: 2072 656d 6f74 655f 7069 7065 733a 204c   remote_pipes: L
+00031ff0: 6973 745b 4469 6374 5b73 7472 2c20 416e  ist[Dict[str, An
+00032000: 795d 5d20 3d20 6177 6169 7420 636c 6965  y]] = await clie
+00032010: 6e74 2e70 6970 6573 2829 0a0a 2020 2020  nt.pipes()..    
+00032020: 6c6f 6361 6c5f 7265 736f 7572 6365 7320  local_resources 
+00032030: 3d20 7b0a 2020 2020 2020 2020 5061 7468  = {.        Path
+00032040: 2866 696c 6529 2e72 6573 6f6c 7665 2829  (file).resolve()
+00032050: 2e73 7465 6d3a 2066 696c 650a 2020 2020  .stem: file.    
+00032060: 2020 2020 666f 7220 6669 6c65 2069 6e20      for file in 
+00032070: 6669 6c65 6e61 6d65 730a 2020 2020 2020  filenames.      
+00032080: 2020 6966 2028 222e 6461 7461 736f 7572    if (".datasour
+00032090: 6365 2220 696e 2066 696c 6520 6f72 2022  ce" in file or "
+000320a0: 2e70 6970 6522 2069 6e20 6669 6c65 2920  .pipe" in file) 
+000320b0: 616e 6420 222e 696e 636c 2220 6e6f 7420  and ".incl" not 
+000320c0: 696e 2066 696c 650a 2020 2020 7d0a 0a20  in file.    }.. 
+000320d0: 2020 2063 6861 6e67 6564 203d 207b 7d0a     changed = {}.
+000320e0: 2020 2020 666f 7220 7265 736f 7572 6365      for resource
+000320f0: 2069 6e20 7265 6d6f 7465 5f64 6174 6173   in remote_datas
+00032100: 6f75 7263 6573 202b 2072 656d 6f74 655f  ources + remote_
+00032110: 7069 7065 733a 0a20 2020 2020 2020 2070  pipes:.        p
+00032120: 726f 7065 7274 6965 733a 2044 6963 745b  roperties: Dict[
+00032130: 7374 722c 2041 6e79 5d20 3d20 6765 745f  str, Any] = get_
+00032140: 6e61 6d65 5f76 6572 7369 6f6e 2872 6573  name_version(res
+00032150: 6f75 7263 655b 226e 616d 6522 5d29 0a20  ource["name"]). 
+00032160: 2020 2020 2020 206e 616d 6520 3d20 7072         name = pr
+00032170: 6f70 6572 7469 6573 2e67 6574 2822 6e61  operties.get("na
+00032180: 6d65 222c 204e 6f6e 6529 0a20 2020 2020  me", None).     
+00032190: 2020 2069 6620 6e61 6d65 3a0a 2020 2020     if name:.    
+000321a0: 2020 2020 2020 2020 2872 6669 6c65 6e61          (rfilena
+000321b0: 6d65 2c20 6669 6c65 2920 3d20 6e65 7874  me, file) = next
+000321c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000321d0: 2020 2828 7266 696c 656e 616d 652c 2066    ((rfilename, f
+000321e0: 696c 6529 2066 6f72 2028 7266 696c 656e  ile) for (rfilen
+000321f0: 616d 652c 2066 696c 6529 2069 6e20 6c6f  ame, file) in lo
+00032200: 6361 6c5f 7265 736f 7572 6365 732e 6974  cal_resources.it
+00032210: 656d 7328 2920 6966 206e 616d 6520 3d3d  ems() if name ==
+00032220: 2072 6669 6c65 6e61 6d65 292c 0a20 2020   rfilename),.   
+00032230: 2020 2020 2020 2020 2020 2020 2028 2222               (""
+00032240: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
+00032250: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00032260: 2020 2069 6620 6e6f 7420 6669 6c65 3a0a     if not file:.
+00032270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032280: 6966 206e 6f74 2077 6974 685f 6578 706c  if not with_expl
+00032290: 6963 6974 5f66 696c 656e 616d 6573 3a0a  icit_filenames:.
+000322a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000322b0: 2020 2020 6966 2077 6974 685f 7072 696e      if with_prin
+000322c0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+000322d0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+000322e0: 2e65 6368 6f28 6622 7b72 6573 6f75 7263  .echo(f"{resourc
+000322f0: 655b 276e 616d 6527 5d7d 206f 6e6c 7920  e['name']} only 
+00032300: 6578 6973 7473 2072 656d 6f74 656c 795c  exists remotely\
+00032310: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00032320: 2020 2020 2020 2020 6966 2069 735f 7368          if is_sh
+00032330: 6172 6564 5f64 6174 6173 6f75 7263 6528  ared_datasource(
+00032340: 7265 736f 7572 6365 5b22 6e61 6d65 225d  resource["name"]
+00032350: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00032360: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
+00032370: 6564 5b72 6573 6f75 7263 655b 226e 616d  ed[resource["nam
+00032380: 6522 5d5d 203d 2022 7368 6172 6564 220a  e"]] = "shared".
+00032390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000323a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000323b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000323c0: 2020 6368 616e 6765 645b 7265 736f 7572    changed[resour
+000323d0: 6365 5b22 6e61 6d65 225d 5d20 3d20 2272  ce["name"]] = "r
+000323e0: 656d 6f74 6522 0a20 2020 2020 2020 2020  emote".         
+000323f0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00032400: 0a20 2020 2020 2020 2020 2020 2073 7566  .            suf
+00032410: 6669 7820 3d20 222e 6461 7461 736f 7572  fix = ".datasour
+00032420: 6365 2220 6966 2022 2e64 6174 6173 6f75  ce" if ".datasou
+00032430: 7263 6522 2069 6e20 6669 6c65 2065 6c73  rce" in file els
+00032440: 6520 222e 7069 7065 220a 2020 2020 2020  e ".pipe".      
+00032450: 2020 2020 2020 7461 7267 6574 203d 2074        target = t
+00032460: 6172 6765 745f 6469 7220 2b20 6f73 2e70  arget_dir + os.p
+00032470: 6174 682e 7365 7020 2b20 7266 696c 656e  ath.sep + rfilen
+00032480: 616d 6520 2b20 7375 6666 6978 0a0a 2020  ame + suffix..  
+00032490: 2020 2020 2020 2020 2020 6469 6666 5f6c            diff_l
+000324a0: 696e 6573 203d 2061 7761 6974 2064 6966  ines = await dif
+000324b0: 665f 6669 6c65 7328 0a20 2020 2020 2020  f_files(.       
+000324c0: 2020 2020 2020 2020 2074 6172 6765 742c           target,
+000324d0: 2066 696c 652c 2077 6974 685f 666f 726d   file, with_form
+000324e0: 6174 3d66 6d74 2c20 7769 7468 5f63 6f6c  at=fmt, with_col
+000324f0: 6f72 3d28 6e6f 7420 6e6f 5f63 6f6c 6f72  or=(not no_color
+00032500: 292c 2063 6c69 656e 743d 636c 6965 6e74  ), client=client
+00032510: 2c20 666f 725f 6465 706c 6f79 3d66 6f72  , for_deploy=for
+00032520: 5f64 6570 6c6f 790a 2020 2020 2020 2020  _deploy.        
+00032530: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00032540: 2020 6e6f 745f 656d 7074 792c 2064 6966    not_empty, dif
+00032550: 665f 6c69 6e65 7320 3d20 7065 656b 2864  f_lines = peek(d
+00032560: 6966 665f 6c69 6e65 7329 0a20 2020 2020  iff_lines).     
+00032570: 2020 2020 2020 2063 6861 6e67 6564 5b72         changed[r
+00032580: 6669 6c65 6e61 6d65 5d20 3d20 6e6f 745f  filename] = not_
+00032590: 656d 7074 790a 2020 2020 2020 2020 2020  empty.          
+000325a0: 2020 6966 206e 6f74 5f65 6d70 7479 2061    if not_empty a
+000325b0: 6e64 2077 6974 685f 7072 696e 743a 0a20  nd with_print:. 
+000325c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000325d0: 7973 2e73 7464 6f75 742e 7772 6974 656c  ys.stdout.writel
+000325e0: 696e 6573 2864 6966 665f 6c69 6e65 7329  ines(diff_lines)
+000325f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00032600: 2063 6c69 636b 2e65 6368 6f28 2222 290a   click.echo("").
+00032610: 0a20 2020 2066 6f72 2072 6669 6c65 6e61  .    for rfilena
+00032620: 6d65 2c20 5f20 696e 206c 6f63 616c 5f72  me, _ in local_r
+00032630: 6573 6f75 7263 6573 2e69 7465 6d73 2829  esources.items()
+00032640: 3a0a 2020 2020 2020 2020 6966 2072 6669  :.        if rfi
+00032650: 6c65 6e61 6d65 206e 6f74 2069 6e20 6368  lename not in ch
+00032660: 616e 6765 643a 0a20 2020 2020 2020 2020  anged:.         
+00032670: 2020 2066 6f72 2072 6573 6f75 7263 6520     for resource 
+00032680: 696e 2072 656d 6f74 655f 6461 7461 736f  in remote_dataso
+00032690: 7572 6365 7320 2b20 7265 6d6f 7465 5f70  urces + remote_p
+000326a0: 6970 6573 3a0a 2020 2020 2020 2020 2020  ipes:.          
+000326b0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+000326c0: 203d 2067 6574 5f6e 616d 655f 7665 7273   = get_name_vers
+000326d0: 696f 6e28 7265 736f 7572 6365 5b22 6e61  ion(resource["na
+000326e0: 6d65 225d 290a 2020 2020 2020 2020 2020  me"]).          
+000326f0: 2020 2020 2020 6e61 6d65 203d 2070 726f        name = pro
+00032700: 7065 7274 6965 732e 6765 7428 226e 616d  perties.get("nam
+00032710: 6522 2c20 4e6f 6e65 290a 2020 2020 2020  e", None).      
+00032720: 2020 2020 2020 2020 2020 6966 206e 616d            if nam
+00032730: 6520 616e 6420 6e61 6d65 203d 3d20 7266  e and name == rf
+00032740: 696c 656e 616d 653a 0a20 2020 2020 2020  ilename:.       
+00032750: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00032760: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
+00032770: 2020 2020 6966 2077 6974 685f 7072 696e      if with_prin
+00032780: 7420 616e 6420 7266 696c 656e 616d 6520  t and rfilename 
+00032790: 6e6f 7420 696e 2063 6861 6e67 6564 3a0a  not in changed:.
+000327a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000327b0: 2020 2020 636c 6963 6b2e 6563 686f 2866      click.echo(f
+000327c0: 227b 7266 696c 656e 616d 657d 206f 6e6c  "{rfilename} onl
+000327d0: 7920 6578 6973 7473 206c 6f63 616c 6c79  y exists locally
+000327e0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+000327f0: 2020 2020 2063 6861 6e67 6564 5b72 6669       changed[rfi
+00032800: 6c65 6e61 6d65 5d20 3d20 226c 6f63 616c  lename] = "local
+00032810: 220a 2020 2020 6966 2063 6c65 616e 5f75  ".    if clean_u
+00032820: 703a 0a20 2020 2020 2020 2073 6875 7469  p:.        shuti
+00032830: 6c2e 726d 7472 6565 2874 6172 6765 745f  l.rmtree(target_
+00032840: 6469 7229 0a0a 2020 2020 7265 7475 726e  dir)..    return
+00032850: 2063 6861 6e67 6564 0a0a 0a61 7379 6e63   changed...async
+00032860: 2064 6566 2064 6966 665f 6669 6c65 7328   def diff_files(
+00032870: 0a20 2020 2066 726f 6d5f 6669 6c65 3a20  .    from_file: 
+00032880: 7374 722c 0a20 2020 2074 6f5f 6669 6c65  str,.    to_file
+00032890: 3a20 7374 722c 0a20 2020 2066 726f 6d5f  : str,.    from_
+000328a0: 6669 6c65 5f73 7566 6669 783a 2073 7472  file_suffix: str
+000328b0: 203d 2022 5b72 656d 6f74 655d 222c 0a20   = "[remote]",. 
+000328c0: 2020 2074 6f5f 6669 6c65 5f73 7566 6669     to_file_suffi
+000328d0: 783a 2073 7472 203d 2022 5b6c 6f63 616c  x: str = "[local
+000328e0: 5d22 2c0a 2020 2020 7769 7468 5f66 6f72  ]",.    with_for
+000328f0: 6d61 743a 2062 6f6f 6c20 3d20 5472 7565  mat: bool = True
+00032900: 2c0a 2020 2020 7769 7468 5f63 6f6c 6f72  ,.    with_color
+00032910: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00032920: 2020 2020 636c 6965 6e74 3a20 4f70 7469      client: Opti
+00032930: 6f6e 616c 5b54 696e 7942 5d20 3d20 4e6f  onal[TinyB] = No
+00032940: 6e65 2c0a 2020 2020 666f 725f 6465 706c  ne,.    for_depl
+00032950: 6f79 3a20 626f 6f6c 203d 2046 616c 7365  oy: bool = False
+00032960: 2c0a 293a 0a20 2020 2064 6566 2066 696c  ,.):.    def fil
+00032970: 655f 6c69 6e65 7328 6669 6c65 6e61 6d65  e_lines(filename
+00032980: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+00032990: 6f70 656e 2866 696c 656e 616d 6529 2061  open(filename) a
+000329a0: 7320 6669 6c65 3a0a 2020 2020 2020 2020  s file:.        
+000329b0: 2020 2020 7265 7475 726e 2066 696c 652e      return file.
+000329c0: 7265 6164 6c69 6e65 7328 290a 0a20 2020  readlines()..   
+000329d0: 2061 7379 6e63 2064 6566 2070 6172 7365   async def parse
+000329e0: 2866 696c 656e 616d 652c 2077 6974 685f  (filename, with_
+000329f0: 666f 726d 6174 3d54 7275 652c 2075 6e72  format=True, unr
+00032a00: 6f6c 6c5f 696e 636c 7564 6573 3d46 616c  oll_includes=Fal
+00032a10: 7365 293a 0a20 2020 2020 2020 2065 7874  se):.        ext
+00032a20: 656e 7369 6f6e 7320 3d20 5061 7468 2866  ensions = Path(f
+00032a30: 696c 656e 616d 6529 2e73 7566 6669 7865  ilename).suffixe
+00032a40: 730a 2020 2020 2020 2020 6c69 6e65 7320  s.        lines 
+00032a50: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+00032a60: 6620 6973 5f66 696c 655f 615f 6461 7461  f is_file_a_data
+00032a70: 736f 7572 6365 2866 696c 656e 616d 6529  source(filename)
+00032a80: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00032a90: 6e65 7320 3d20 280a 2020 2020 2020 2020  nes = (.        
+00032aa0: 2020 2020 2020 2020 6177 6169 7420 666f          await fo
+00032ab0: 726d 6174 5f64 6174 6173 6f75 7263 6528  rmat_datasource(
+00032ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00032ad0: 2020 2020 2066 696c 656e 616d 652c 0a20       filename,. 
+00032ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032af0: 2020 2075 6e72 6f6c 6c5f 696e 636c 7564     unroll_includ
+00032b00: 6573 3d75 6e72 6f6c 6c5f 696e 636c 7564  es=unroll_includ
+00032b10: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00032b20: 2020 2020 2020 2020 666f 725f 6469 6666          for_diff
+00032b30: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00032b40: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00032b50: 743d 636c 6965 6e74 2c0a 2020 2020 2020  t=client,.      
+00032b60: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00032b70: 706c 6163 655f 696e 636c 7564 6573 3d54  place_includes=T
+00032b80: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00032b90: 2020 2020 2020 2020 2066 6f72 5f64 6570           for_dep
+00032ba0: 6c6f 795f 6469 6666 3d66 6f72 5f64 6570  loy_diff=for_dep
+00032bb0: 6c6f 792c 0a20 2020 2020 2020 2020 2020  loy,.           
+00032bc0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00032bd0: 2020 2020 2020 2069 6620 7769 7468 5f66         if with_f
+00032be0: 6f72 6d61 740a 2020 2020 2020 2020 2020  ormat.          
+00032bf0: 2020 2020 2020 656c 7365 2066 696c 655f        else file_
+00032c00: 6c69 6e65 7328 6669 6c65 6e61 6d65 290a  lines(filename).
+00032c10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00032c20: 2020 2020 2020 656c 6966 2028 222e 7069        elif (".pi
+00032c30: 7065 2220 696e 2065 7874 656e 7369 6f6e  pe" in extension
+00032c40: 7329 206f 7220 2822 2e69 6e63 6c22 2069  s) or (".incl" i
+00032c50: 6e20 6578 7465 6e73 696f 6e73 293a 0a20  n extensions):. 
+00032c60: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+00032c70: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00032c80: 2020 2020 2061 7761 6974 2066 6f72 6d61       await forma
+00032c90: 745f 7069 7065 280a 2020 2020 2020 2020  t_pipe(.        
+00032ca0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00032cb0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00032cc0: 2020 2020 2020 2020 2020 4445 4641 554c            DEFAUL
+00032cd0: 545f 464d 545f 4c49 4e45 5f4c 454e 4754  T_FMT_LINE_LENGT
+00032ce0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+00032cf0: 2020 2020 2020 2075 6e72 6f6c 6c5f 696e         unroll_in
+00032d00: 636c 7564 6573 3d75 6e72 6f6c 6c5f 696e  cludes=unroll_in
+00032d10: 636c 7564 6573 2c0a 2020 2020 2020 2020  cludes,.        
+00032d20: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00032d30: 6163 655f 696e 636c 7564 6573 3d54 7275  ace_includes=Tru
+00032d40: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00032d50: 2020 2020 2020 2066 6f72 5f64 6570 6c6f         for_deplo
+00032d60: 795f 6469 6666 3d66 6f72 5f64 6570 6c6f  y_diff=for_deplo
+00032d70: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+00032d80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00032d90: 2020 2020 2069 6620 7769 7468 5f66 6f72       if with_for
+00032da0: 6d61 740a 2020 2020 2020 2020 2020 2020  mat.            
+00032db0: 2020 2020 656c 7365 2066 696c 655f 6c69      else file_li
+00032dc0: 6e65 7328 6669 6c65 6e61 6d65 290a 2020  nes(filename).  
+00032dd0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00032de0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00032df0: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
+00032e00: 2866 2255 6e73 7570 706f 7274 6564 2066  (f"Unsupported f
+00032e10: 696c 6520 7479 7065 3a20 7b66 696c 656e  ile type: {filen
+00032e20: 616d 657d 2229 0a20 2020 2020 2020 2069  ame}").        i
+00032e30: 6620 6c69 6e65 733a 0a20 2020 2020 2020  f lines:.       
+00032e40: 2020 2020 2072 6574 7572 6e20 5b66 227b       return [f"{
+00032e50: 6c7d 5c6e 2220 666f 7220 6c20 696e 206c  l}\n" for l in l
+00032e60: 696e 6573 2e73 706c 6974 2822 5c6e 2229  ines.split("\n")
+00032e70: 5d20 6966 2077 6974 685f 666f 726d 6174  ] if with_format
+00032e80: 2065 6c73 6520 6c69 6e65 7320 2023 206e   else lines  # n
+00032e90: 6f71 613a 2045 3734 310a 0a20 2020 2074  oqa: E741..    t
+00032ea0: 7279 3a0a 2020 2020 2020 2020 6c69 6e65  ry:.        line
+00032eb0: 7331 203d 2061 7761 6974 2070 6172 7365  s1 = await parse
+00032ec0: 2866 726f 6d5f 6669 6c65 2c20 7769 7468  (from_file, with
+00032ed0: 5f66 6f72 6d61 7429 0a20 2020 2020 2020  _format).       
+00032ee0: 206c 696e 6573 3220 3d20 6177 6169 7420   lines2 = await 
+00032ef0: 7061 7273 6528 746f 5f66 696c 652c 2077  parse(to_file, w
+00032f00: 6974 685f 666f 726d 6174 2c20 756e 726f  ith_format, unro
+00032f10: 6c6c 5f69 6e63 6c75 6465 733d 5472 7565  ll_includes=True
+00032f20: 290a 2020 2020 6578 6365 7074 2046 696c  ).    except Fil
+00032f30: 654e 6f74 466f 756e 6445 7272 6f72 2061  eNotFoundError a
+00032f40: 7320 653a 0a20 2020 2020 2020 2066 696c  s e:.        fil
+00032f50: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
+00032f60: 6261 7365 6e61 6d65 2873 7472 2865 2929  basename(str(e))
+00032f70: 2e73 7472 6970 2822 2722 290a 2020 2020  .strip("'").    
+00032f80: 2020 2020 7261 6973 6520 636c 6963 6b2e      raise click.
+00032f90: 436c 6963 6b45 7863 6570 7469 6f6e 2846  ClickException(F
+00032fa0: 6565 6462 6163 6b4d 616e 6167 6572 2e65  eedbackManager.e
+00032fb0: 7272 6f72 5f64 6966 665f 6669 6c65 2866  rror_diff_file(f
+00032fc0: 696c 656e 616d 653d 6669 6c65 6e61 6d65  ilename=filename
+00032fd0: 2929 0a0a 2020 2020 6966 206e 6f74 206c  ))..    if not l
+00032fe0: 696e 6573 3120 6f72 206e 6f74 206c 696e  ines1 or not lin
+00032ff0: 6573 323a 0a20 2020 2020 2020 2072 6574  es2:.        ret
+00033000: 7572 6e0a 0a20 2020 2064 6966 6620 3d20  urn..    diff = 
+00033010: 6469 6666 6c69 622e 756e 6966 6965 645f  difflib.unified_
+00033020: 6469 6666 280a 2020 2020 2020 2020 6c69  diff(.        li
+00033030: 6e65 7331 2c20 6c69 6e65 7332 2c20 6672  nes1, lines2, fr
+00033040: 6f6d 6669 6c65 3d66 227b 5061 7468 2866  omfile=f"{Path(f
+00033050: 726f 6d5f 6669 6c65 292e 6e61 6d65 7d20  rom_file).name} 
+00033060: 7b66 726f 6d5f 6669 6c65 5f73 7566 6669  {from_file_suffi
+00033070: 787d 222c 2074 6f66 696c 653d 6622 7b74  x}", tofile=f"{t
+00033080: 6f5f 6669 6c65 7d20 7b74 6f5f 6669 6c65  o_file} {to_file
+00033090: 5f73 7566 6669 787d 220a 2020 2020 290a  _suffix}".    ).
+000330a0: 0a20 2020 2069 6620 7769 7468 5f63 6f6c  .    if with_col
+000330b0: 6f72 3a0a 2020 2020 2020 2020 6469 6666  or:.        diff
+000330c0: 203d 2063 6f6c 6f72 5f64 6966 6628 6469   = color_diff(di
+000330d0: 6666 290a 0a20 2020 2072 6574 7572 6e20  ff)..    return 
+000330e0: 6469 6666 0a0a 0a64 6566 2069 735f 656e  diff...def is_en
+000330f0: 6470 6f69 6e74 2872 6573 6f75 7263 653a  dpoint(resource:
+00033100: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00033110: 7472 2c20 416e 795d 5d29 202d 3e20 626f  tr, Any]]) -> bo
+00033120: 6f6c 3a0a 2020 2020 6966 2072 6573 6f75  ol:.    if resou
+00033130: 7263 6520 616e 6420 6c65 6e28 7265 736f  rce and len(reso
+00033140: 7572 6365 2e67 6574 2822 746f 6b65 6e73  urce.get("tokens
+00033150: 222c 205b 5d29 2920 213d 2030 2061 6e64  ", [])) != 0 and
+00033160: 2072 6573 6f75 7263 652e 6765 7428 2272   resource.get("r
+00033170: 6573 6f75 7263 6522 2920 3d3d 2022 7069  esource") == "pi
+00033180: 7065 7322 3a0a 2020 2020 2020 2020 7265  pes":.        re
+00033190: 7475 726e 2054 7275 650a 2020 2020 7265  turn True.    re
+000331a0: 7475 726e 2046 616c 7365 0a0a 0a64 6566  turn False...def
+000331b0: 2069 735f 6d61 7465 7269 616c 697a 6564   is_materialized
+000331c0: 2872 6573 6f75 7263 653a 204f 7074 696f  (resource: Optio
+000331d0: 6e61 6c5b 4469 6374 5b73 7472 2c20 416e  nal[Dict[str, An
+000331e0: 795d 5d29 202d 3e20 626f 6f6c 3a0a 2020  y]]) -> bool:.  
+000331f0: 2020 6966 206e 6f74 2072 6573 6f75 7263    if not resourc
+00033200: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+00033210: 6e20 4661 6c73 650a 0a20 2020 2069 735f  n False..    is_
+00033220: 6d61 7465 7269 616c 697a 6564 203d 2061  materialized = a
+00033230: 6e79 280a 2020 2020 2020 2020 5b6e 6f64  ny(.        [nod
+00033240: 652e 6765 7428 2270 6172 616d 7322 2c20  e.get("params", 
+00033250: 7b7d 292e 6765 7428 2274 7970 6522 2c20  {}).get("type", 
+00033260: 4e6f 6e65 2920 3d3d 2022 6d61 7465 7269  None) == "materi
+00033270: 616c 697a 6564 2220 666f 7220 6e6f 6465  alized" for node
+00033280: 2069 6e20 7265 736f 7572 6365 2e67 6574   in resource.get
+00033290: 2822 6e6f 6465 7322 2c20 5b5d 2920 6f72  ("nodes", []) or
+000332a0: 205b 5d5d 0a20 2020 2029 0a20 2020 2072   []].    ).    r
+000332b0: 6574 7572 6e20 6973 5f6d 6174 6572 6961  eturn is_materia
+000332c0: 6c69 7a65 640a 0a0a 6465 6620 6973 5f65  lized...def is_e
+000332d0: 6e64 706f 696e 745f 7769 7468 5f6e 6f5f  ndpoint_with_no_
+000332e0: 6465 7065 6e64 656e 6369 6573 280a 2020  dependencies(.  
+000332f0: 2020 7265 736f 7572 6365 3a20 4469 6374    resource: Dict
+00033300: 5b73 7472 2c20 416e 795d 2c20 6465 705f  [str, Any], dep_
+00033310: 6d61 703a 2044 6963 745b 7374 722c 2053  map: Dict[str, S
+00033320: 6574 5b73 7472 5d5d 2c20 746f 5f72 756e  et[str]], to_run
+00033330: 3a20 4469 6374 5b73 7472 2c20 4469 6374  : Dict[str, Dict
+00033340: 5b73 7472 2c20 416e 795d 5d0a 2920 2d3e  [str, Any]].) ->
+00033350: 2062 6f6f 6c3a 0a20 2020 2069 6620 6e6f   bool:.    if no
+00033360: 7420 7265 736f 7572 6365 206f 7220 7265  t resource or re
+00033370: 736f 7572 6365 2e67 6574 2822 7265 736f  source.get("reso
+00033380: 7572 6365 2229 203d 3d20 2264 6174 6173  urce") == "datas
+00033390: 6f75 7263 6573 223a 0a20 2020 2020 2020  ources":.       
+000333a0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+000333b0: 2020 2066 6f72 206e 6f64 6520 696e 2072     for node in r
+000333c0: 6573 6f75 7263 652e 6765 7428 226e 6f64  esource.get("nod
+000333d0: 6573 222c 205b 5d29 3a0a 2020 2020 2020  es", []):.      
+000333e0: 2020 2320 4649 584d 453a 2068 7474 7073    # FIXME: https
+000333f0: 3a2f 2f67 6974 6c61 622e 636f 6d2f 7469  ://gitlab.com/ti
+00033400: 6e79 6269 7264 2f61 6e61 6c79 7469 6373  nybird/analytics
+00033410: 2f2d 2f69 7373 7565 732f 3233 3931 0a20  /-/issues/2391. 
+00033420: 2020 2020 2020 2069 6620 6e6f 6465 2e67         if node.g
+00033430: 6574 2822 7061 7261 6d73 222c 207b 7d29  et("params", {})
+00033440: 2e67 6574 2822 7479 7065 222c 2022 2229  .get("type", "")
+00033450: 2e6c 6f77 6572 2829 2069 6e20 5b0a 2020  .lower() in [.  
+00033460: 2020 2020 2020 2020 2020 5069 7065 4e6f            PipeNo
+00033470: 6465 5479 7065 732e 4d41 5445 5249 414c  deTypes.MATERIAL
+00033480: 495a 4544 2c0a 2020 2020 2020 2020 2020  IZED,.          
+00033490: 2020 5069 7065 4e6f 6465 5479 7065 732e    PipeNodeTypes.
+000334a0: 434f 5059 2c0a 2020 2020 2020 2020 2020  COPY,.          
+000334b0: 2020 5069 7065 4e6f 6465 5479 7065 732e    PipeNodeTypes.
+000334c0: 4441 5441 5f53 494e 4b2c 0a20 2020 2020  DATA_SINK,.     
+000334d0: 2020 205d 3a0a 2020 2020 2020 2020 2020     ]:.          
+000334e0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+000334f0: 2020 2020 666f 7220 6b65 792c 2076 616c      for key, val
+00033500: 7565 7320 696e 2064 6570 5f6d 6170 2e69  ues in dep_map.i
+00033510: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00033520: 6966 2072 6573 6f75 7263 655b 2272 6573  if resource["res
+00033530: 6f75 7263 655f 6e61 6d65 225d 2069 6e20  ource_name"] in 
+00033540: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+00033550: 2020 2020 7220 3d20 746f 5f72 756e 2e67      r = to_run.g
+00033560: 6574 286b 6579 2c20 4e6f 6e65 290a 2020  et(key, None).  
+00033570: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00033580: 2072 3a0a 2020 2020 2020 2020 2020 2020   r:.            
+00033590: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+000335a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000335b0: 4661 6c73 650a 0a20 2020 2064 6570 7320  False..    deps 
+000335c0: 3d20 6465 705f 6d61 702e 6765 7428 7265  = dep_map.get(re
+000335d0: 736f 7572 6365 5b22 7265 736f 7572 6365  source["resource
+000335e0: 5f6e 616d 6522 5d29 0a20 2020 2069 6620  _name"]).    if 
+000335f0: 6e6f 7420 6465 7073 3a0a 2020 2020 2020  not deps:.      
+00033600: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00033610: 2020 2066 6f72 2064 6570 2069 6e20 6465     for dep in de
+00033620: 7073 3a0a 2020 2020 2020 2020 7220 3d20  ps:.        r = 
+00033630: 746f 5f72 756e 2e67 6574 2864 6570 2c20  to_run.get(dep, 
+00033640: 4e6f 6e65 290a 2020 2020 2020 2020 6966  None).        if
+00033650: 2069 735f 656e 6470 6f69 6e74 2872 2920   is_endpoint(r) 
+00033660: 6f72 2069 735f 6d61 7465 7269 616c 697a  or is_materializ
+00033670: 6564 2872 293a 0a20 2020 2020 2020 2020  ed(r):.         
+00033680: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00033690: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
+000336a0: 0a0a 0a64 6566 2067 6574 5f74 6172 6765  ...def get_targe
+000336b0: 745f 6d61 7465 7269 616c 697a 6564 5f64  t_materialized_d
+000336c0: 6174 615f 736f 7572 6365 5f6e 616d 6528  ata_source_name(
+000336d0: 7265 736f 7572 6365 3a20 4f70 7469 6f6e  resource: Option
+000336e0: 616c 5b44 6963 745b 7374 722c 2041 6e79  al[Dict[str, Any
+000336f0: 5d5d 2920 2d3e 204f 7074 696f 6e61 6c5b  ]]) -> Optional[
+00033700: 7374 725d 3a0a 2020 2020 6966 206e 6f74  str]:.    if not
+00033710: 2072 6573 6f75 7263 653a 0a20 2020 2020   resource:.     
+00033720: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00033730: 2020 2020 666f 7220 6e6f 6465 2069 6e20      for node in 
+00033740: 7265 736f 7572 6365 2e67 6574 2822 6e6f  resource.get("no
+00033750: 6465 7322 2c20 5b5d 293a 0a20 2020 2020  des", []):.     
+00033760: 2020 2023 2046 4958 4d45 3a20 6874 7470     # FIXME: http
+00033770: 733a 2f2f 6769 746c 6162 2e63 6f6d 2f74  s://gitlab.com/t
+00033780: 696e 7962 6972 642f 616e 616c 7974 6963  inybird/analytic
+00033790: 732f 2d2f 6973 7375 6573 2f32 3339 310a  s/-/issues/2391.
+000337a0: 2020 2020 2020 2020 6966 206e 6f64 652e          if node.
+000337b0: 6765 7428 2270 6172 616d 7322 2c20 7b7d  get("params", {}
+000337c0: 292e 6765 7428 2274 7970 6522 2c20 2222  ).get("type", ""
+000337d0: 292e 6c6f 7765 7228 2920 3d3d 2050 6970  ).lower() == Pip
+000337e0: 654e 6f64 6554 7970 6573 2e4d 4154 4552  eNodeTypes.MATER
+000337f0: 4941 4c49 5a45 443a 0a20 2020 2020 2020  IALIZED:.       
+00033800: 2020 2020 2072 6574 7572 6e20 6e6f 6465       return node
+00033810: 2e67 6574 2822 7061 7261 6d73 2229 5b22  .get("params")["
+00033820: 6461 7461 736f 7572 6365 225d 2e73 706c  datasource"].spl
+00033830: 6974 2822 5f5f 7622 295b 305d 0a0a 2020  it("__v")[0]..  
+00033840: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
+00033850: 6465 6620 6973 5f64 6174 6173 6f75 7263  def is_datasourc
+00033860: 6528 7265 736f 7572 6365 3a20 4f70 7469  e(resource: Opti
+00033870: 6f6e 616c 5b44 6963 745b 7374 722c 2041  onal[Dict[str, A
+00033880: 6e79 5d5d 2920 2d3e 2062 6f6f 6c3a 0a20  ny]]) -> bool:. 
+00033890: 2020 2069 6620 7265 736f 7572 6365 2061     if resource a
+000338a0: 6e64 2072 6573 6f75 7263 652e 6765 7428  nd resource.get(
+000338b0: 2272 6573 6f75 7263 6522 2920 3d3d 2022  "resource") == "
+000338c0: 6461 7461 736f 7572 6365 7322 3a0a 2020  datasources":.  
+000338d0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000338e0: 650a 2020 2020 7265 7475 726e 2046 616c  e.    return Fal
+000338f0: 7365 0a0a 0a61 7379 6e63 2064 6566 2063  se...async def c
+00033900: 7265 6174 655f 7265 6c65 6173 6528 0a20  reate_release(. 
+00033910: 2020 2063 6c69 656e 743a 2054 696e 7942     client: TinyB
+00033920: 2c20 636f 6e66 6967 3a20 556e 696f 6e5b  , config: Union[
+00033930: 4469 6374 5b73 7472 2c20 416e 795d 2c20  Dict[str, Any], 
+00033940: 434c 4943 6f6e 6669 675d 2c20 7365 6d76  CLIConfig], semv
+00033950: 6572 3a20 7374 722c 2066 6f6c 6465 723a  er: str, folder:
+00033960: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00033970: 204e 6f6e 650a 2920 2d3e 204e 6f6e 653a   None.) -> None:
+00033980: 0a20 2020 2069 6620 6e6f 7420 666f 6c64  .    if not fold
+00033990: 6572 3a0a 2020 2020 2020 2020 666f 6c64  er:.        fold
+000339a0: 6572 203d 2067 6574 6377 6428 290a 2020  er = getcwd().  
+000339b0: 2020 636c 695f 6769 745f 7265 6c65 6173    cli_git_releas
+000339c0: 6520 3d20 4e6f 6e65 0a20 2020 2074 7279  e = None.    try
+000339d0: 3a0a 2020 2020 2020 2020 636c 695f 6769  :.        cli_gi
+000339e0: 745f 7265 6c65 6173 6520 3d20 434c 4947  t_release = CLIG
+000339f0: 6974 5265 6c65 6173 6528 7061 7468 3d66  itRelease(path=f
+00033a00: 6f6c 6465 7229 0a20 2020 2020 2020 2063  older).        c
+00033a10: 6f6d 6d69 7420 3d20 636c 695f 6769 745f  ommit = cli_git_
+00033a20: 7265 6c65 6173 652e 6865 6164 5f63 6f6d  release.head_com
+00033a30: 6d69 7428 290a 2020 2020 6578 6365 7074  mit().    except
+00033a40: 2043 4c49 4769 7452 656c 6561 7365 4578   CLIGitReleaseEx
+00033a50: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+00033a60: 2072 6169 7365 2043 4c49 4769 7452 656c   raise CLIGitRel
+00033a70: 6561 7365 4578 6365 7074 696f 6e28 4665  easeException(Fe
+00033a80: 6564 6261 636b 4d61 6e61 6765 722e 6572  edbackManager.er
+00033a90: 726f 725f 6e6f 5f67 6974 5f72 6570 6f5f  ror_no_git_repo_
+00033aa0: 666f 725f 696e 6974 2872 6570 6f5f 7061  for_init(repo_pa
+00033ab0: 7468 3d66 6f6c 6465 7229 290a 0a20 2020  th=folder))..   
+00033ac0: 2061 7761 6974 2063 6c69 656e 742e 7265   await client.re
+00033ad0: 6c65 6173 655f 6e65 7728 636f 6e66 6967  lease_new(config
+00033ae0: 5b22 6964 225d 2c20 7365 6d76 6572 2c20  ["id"], semver, 
+00033af0: 636f 6d6d 6974 290a 2020 2020 636c 6963  commit).    clic
+00033b00: 6b2e 6563 686f 2846 6565 6462 6163 6b4d  k.echo(FeedbackM
+00033b10: 616e 6167 6572 2e73 7563 6365 7373 5f64  anager.success_d
+00033b20: 6570 6c6f 796d 656e 745f 7265 6c65 6173  eployment_releas
+00033b30: 6528 7365 6d76 6572 3d73 656d 7665 7229  e(semver=semver)
+00033b40: 290a 0a0a 6465 6620 6861 735f 696e 7465  )...def has_inte
+00033b50: 726e 616c 5f64 6174 6166 696c 6573 2866  rnal_datafiles(f
+00033b60: 6f6c 6465 723a 2073 7472 2920 2d3e 2062  older: str) -> b
+00033b70: 6f6f 6c3a 0a20 2020 2066 6f6c 6465 7220  ool:.    folder 
+00033b80: 3d20 666f 6c64 6572 206f 7220 222e 220a  = folder or ".".
+00033b90: 2020 2020 6669 6c65 6e61 6d65 7320 3d20      filenames = 
+00033ba0: 6765 745f 7072 6f6a 6563 745f 6669 6c65  get_project_file
+00033bb0: 6e61 6d65 7328 666f 6c64 6572 290a 2020  names(folder).  
+00033bc0: 2020 7265 7475 726e 2061 6e79 285b 6620    return any([f 
+00033bd0: 666f 7220 6620 696e 2066 696c 656e 616d  for f in filenam
+00033be0: 6573 2069 6620 2273 7061 6e73 2220 696e  es if "spans" in
+00033bf0: 2073 7472 2866 2920 616e 6420 2276 656e   str(f) and "ven
+00033c00: 646f 7222 206e 6f74 2069 6e20 7374 7228  dor" not in str(
+00033c10: 6629 5d29 0a0a 0a64 6566 2069 735f 6669  f)])...def is_fi
+00033c20: 6c65 5f61 5f64 6174 6173 6f75 7263 6528  le_a_datasource(
+00033c30: 6669 6c65 6e61 6d65 3a20 7374 7229 202d  filename: str) -
+00033c40: 3e20 626f 6f6c 3a0a 2020 2020 6578 7465  > bool:.    exte
+00033c50: 6e73 696f 6e73 203d 2050 6174 6828 6669  nsions = Path(fi
+00033c60: 6c65 6e61 6d65 292e 7375 6666 6978 6573  lename).suffixes
+00033c70: 0a20 2020 2069 6620 222e 6461 7461 736f  .    if ".dataso
+00033c80: 7572 6365 2220 696e 2065 7874 656e 7369  urce" in extensi
+00033c90: 6f6e 733a 2020 2320 4163 6365 7074 7320  ons:  # Accepts 
+00033ca0: 272e 6461 7461 736f 7572 6365 2720 616e  '.datasource' an
+00033cb0: 6420 272e 6461 7461 736f 7572 6365 2e69  d '.datasource.i
+00033cc0: 6e63 6c27 0a20 2020 2020 2020 2072 6574  ncl'.        ret
+00033cd0: 7572 6e20 5472 7565 0a0a 2020 2020 6966  urn True..    if
+00033ce0: 2022 2e69 6e63 6c22 2069 6e20 6578 7465   ".incl" in exte
+00033cf0: 6e73 696f 6e73 3a0a 2020 2020 2020 2020  nsions:.        
+00033d00: 6c69 6e65 7320 3d20 5b5d 0a20 2020 2020  lines = [].     
+00033d10: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
+00033d20: 656e 616d 6529 2061 7320 6669 6c65 3a0a  ename) as file:.
+00033d30: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00033d40: 7320 3d20 6669 6c65 2e72 6561 646c 696e  s = file.readlin
+00033d50: 6573 2829 0a0a 2020 2020 2020 2020 666f  es()..        fo
+00033d60: 7220 6c69 6e65 2069 6e20 6c69 6e65 733a  r line in lines:
+00033d70: 0a20 2020 2020 2020 2020 2020 2074 7269  .            tri
+00033d80: 6d6d 6564 5f6c 696e 6520 3d20 6c69 6e65  mmed_line = line
+00033d90: 2e73 7472 6970 2829 2e6c 6f77 6572 2829  .strip().lower()
+00033da0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00033db0: 7472 696d 6d65 645f 6c69 6e65 2e73 7461  trimmed_line.sta
+00033dc0: 7274 7377 6974 6828 2273 6368 656d 6122  rtswith("schema"
+00033dd0: 2920 6f72 2074 7269 6d6d 6564 5f6c 696e  ) or trimmed_lin
+00033de0: 652e 7374 6172 7473 7769 7468 2822 656e  e.startswith("en
+00033df0: 6769 6e65 2229 3a0a 2020 2020 2020 2020  gine"):.        
+00033e00: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00033e10: 7275 650a 0a20 2020 2072 6574 7572 6e20  rue..    return 
+00033e20: 4661 6c73 650a                           False.
```

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/datatypes.py` & `tinybird-cli-3.9.1.dev5/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/feedback_manager.py` & `tinybird-cli-3.9.1.dev5/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/git_settings.py` & `tinybird-cli-3.9.1.dev5/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/sql.py` & `tinybird-cli-3.9.1.dev5/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/sql_template.py` & `tinybird-cli-3.9.1.dev5/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/sql_template_fmt.py` & `tinybird-cli-3.9.1.dev5/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/sql_toolset.py` & `tinybird-cli-3.9.1.dev5/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/syncasync.py` & `tinybird-cli-3.9.1.dev5/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird/tornado_template.py` & `tinybird-cli-3.9.1.dev5/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev4
+Version: 3.9.1.dev5
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,14 +14,19 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ----------
 
+3.9.1.dev5
+************
+
+- `Added` support for adding multiple tokens when pushing a `.datasource` file
+
 
 3.9.1.dev4
 ************
 
 - `Fixed` s3 iamrole connection creation will not fail when `pbcopy` dependency is not available
 
 3.9.1.dev3
```

### Comparing `tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

