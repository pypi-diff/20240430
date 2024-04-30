# Comparing `tmp/scrawlpy-0.0.9.tar.gz` & `tmp/scrawlpy-0.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrawlpy-0.0.9.tar", last modified: Tue Apr 30 18:29:45 2024, max compression
+gzip compressed data, was "scrawlpy-0.0.9b0.tar", last modified: Tue Apr 30 18:30:32 2024, max compression
```

## Comparing `scrawlpy-0.0.9.tar` & `scrawlpy-0.0.9b0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.344597 scrawlpy-0.0.9/
--rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/LICENSE
--rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.9/MANIFEST.in
--rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:29:45.344178 scrawlpy-0.0.9/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.9/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.324811 scrawlpy-0.0.9/scrawlpy/
--rw-r--r--   0 wu         (501) staff       (20)        5 2024-04-30 18:29:44.000000 scrawlpy-0.0.9/scrawlpy/VERSION
--rw-r--r--   0 wu         (501) staff       (20)      179 2024-04-30 09:29:03.000000 scrawlpy-0.0.9/scrawlpy/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.327747 scrawlpy-0.0.9/scrawlpy/commands/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/cmdline.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.330414 scrawlpy-0.0.9/scrawlpy/commands/create/
--rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_cookies.py
--rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_init.py
--rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_item.py
--rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_json.py
--rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_params.py
--rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_project.py
--rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_setting.py
--rw-r--r--   0 wu         (501) staff       (20)     3649 2024-04-30 17:38:40.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_spider.py
--rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/create/create_table.py
--rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.9/scrawlpy/commands/create_builder.py
--rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.9/scrawlpy/commands/retry.py
--rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/shell.py
--rw-r--r--   0 wu         (501) staff       (20)     1177 2024-04-30 18:28:22.000000 scrawlpy-0.0.9/scrawlpy/commands/spider.py
--rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/commands/zip.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.330917 scrawlpy-0.0.9/scrawlpy/core/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.9/scrawlpy/core/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1328 2024-04-30 17:55:11.000000 scrawlpy-0.0.9/scrawlpy/core/base_spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.331654 scrawlpy-0.0.9/scrawlpy/core/spiders/
--rw-r--r--   0 wu         (501) staff       (20)      190 2024-04-30 16:37:30.000000 scrawlpy-0.0.9/scrawlpy/core/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3038 2024-04-30 18:29:12.000000 scrawlpy-0.0.9/scrawlpy/core/spiders/airspider.py
--rw-r--r--   0 wu         (501) staff       (20)      269 2024-04-30 08:49:30.000000 scrawlpy-0.0.9/scrawlpy/core/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.332153 scrawlpy-0.0.9/scrawlpy/http/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:13.000000 scrawlpy-0.0.9/scrawlpy/http/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.9/scrawlpy/http/request.py
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.9/scrawlpy/requirements.txt
--rw-r--r--   0 wu         (501) staff       (20)    12212 2024-04-30 17:25:57.000000 scrawlpy-0.0.9/scrawlpy/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.332837 scrawlpy-0.0.9/scrawlpy/storage/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:03:26.000000 scrawlpy-0.0.9/scrawlpy/storage/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1774 2024-04-30 10:13:18.000000 scrawlpy-0.0.9/scrawlpy/storage/memorydb.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.334531 scrawlpy-0.0.9/scrawlpy/templates/
--rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/air_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/batch_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/item_template.tmpl
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.335169 scrawlpy-0.0.9/scrawlpy/templates/project_template/
--rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/project_template/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.335551 scrawlpy-0.0.9/scrawlpy/templates/project_template/items/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/project_template/items/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/project_template/main.py
--rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/project_template/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.335670 scrawlpy-0.0.9/scrawlpy/templates/project_template/spiders/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/project_template/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.9/scrawlpy/templates/spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/task_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.9/scrawlpy/templates/update_item_template.tmpl
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.337127 scrawlpy-0.0.9/scrawlpy/utils/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 09:29:03.000000 scrawlpy-0.0.9/scrawlpy/utils/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1439 2024-04-30 10:51:36.000000 scrawlpy-0.0.9/scrawlpy/utils/concurrent_util.py
--rw-r--r--   0 wu         (501) staff       (20)     5490 2024-04-30 18:18:53.000000 scrawlpy-0.0.9/scrawlpy/utils/loader_util.py
--rw-r--r--   0 wu         (501) staff       (20)      827 2024-04-30 17:04:03.000000 scrawlpy-0.0.9/scrawlpy/utils/logger_util.py
--rw-r--r--   0 wu         (501) staff       (20)      727 2024-04-30 17:22:41.000000 scrawlpy-0.0.9/scrawlpy/utils/obj_util.py
--rw-r--r--   0 wu         (501) staff       (20)      726 2024-04-30 09:29:03.000000 scrawlpy-0.0.9/scrawlpy/utils/tail_thread.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.326007 scrawlpy-0.0.9/scrawlpy.egg-info/
--rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:29:45.000000 scrawlpy-0.0.9/scrawlpy.egg-info/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)     2321 2024-04-30 18:29:45.000000 scrawlpy-0.0.9/scrawlpy.egg-info/SOURCES.txt
--rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 18:29:45.000000 scrawlpy-0.0.9/scrawlpy.egg-info/dependency_links.txt
--rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 18:29:45.000000 scrawlpy-0.0.9/scrawlpy.egg-info/entry_points.txt
--rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 18:29:45.000000 scrawlpy-0.0.9/scrawlpy.egg-info/requires.txt
--rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 18:29:45.000000 scrawlpy-0.0.9/scrawlpy.egg-info/top_level.txt
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.337393 scrawlpy-0.0.9/scripts/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.9/scripts/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 18:29:45.344688 scrawlpy-0.0.9/setup.cfg
--rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.9/setup.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.338117 scrawlpy-0.0.9/test/
--rw-r--r--   0 wu         (501) staff       (20)       68 2024-04-30 18:04:25.000000 scrawlpy-0.0.9/test/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      419 2024-04-30 10:53:23.000000 scrawlpy-0.0.9/test/func_demo.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.339595 scrawlpy-0.0.9/test/func_timeout_demo/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:34.000000 scrawlpy-0.0.9/test/func_timeout_demo/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     2123 2024-04-30 11:04:37.000000 scrawlpy-0.0.9/test/func_timeout_demo/demo.py
--rw-r--r--   0 wu         (501) staff       (20)     1521 2024-04-30 11:01:42.000000 scrawlpy-0.0.9/test/func_timeout_demo/test2.py
--rw-r--r--   0 wu         (501) staff       (20)     1470 2024-04-30 16:41:53.000000 scrawlpy-0.0.9/test/func_timeout_demo/test3.py
--rw-r--r--   0 wu         (501) staff       (20)     2934 2024-04-30 18:09:06.000000 scrawlpy-0.0.9/test/main.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.340223 scrawlpy-0.0.9/test/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.9/test/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      728 2024-04-30 17:49:57.000000 scrawlpy-0.0.9/test/spiders/airspider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.340855 scrawlpy-0.0.9/test/spiders/settings/
--rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.9/test/spiders/settings/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.9/test/spiders/settings/airspider_settings.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:29:45.341801 scrawlpy-0.0.9/test/spiders/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:50:00.000000 scrawlpy-0.0.9/test/spiders/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1037 2024-04-30 17:56:49.000000 scrawlpy-0.0.9/test/spiders/spiders/airspider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.323652 scrawlpy-0.0.9b0/
+-rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/LICENSE
+-rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.9b0/MANIFEST.in
+-rw-r--r--   0 wu         (501) staff       (20)      930 2024-04-30 18:30:32.323404 scrawlpy-0.0.9b0/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.9b0/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.307086 scrawlpy-0.0.9b0/scrawlpy/
+-rw-r--r--   0 wu         (501) staff       (20)        9 2024-04-30 18:30:31.000000 scrawlpy-0.0.9b0/scrawlpy/VERSION
+-rw-r--r--   0 wu         (501) staff       (20)      179 2024-04-30 09:29:03.000000 scrawlpy-0.0.9b0/scrawlpy/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.309846 scrawlpy-0.0.9b0/scrawlpy/commands/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/cmdline.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.312310 scrawlpy-0.0.9b0/scrawlpy/commands/create/
+-rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_cookies.py
+-rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_init.py
+-rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_item.py
+-rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_json.py
+-rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_params.py
+-rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_project.py
+-rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_setting.py
+-rw-r--r--   0 wu         (501) staff       (20)     3649 2024-04-30 17:38:40.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create/create_table.py
+-rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.9b0/scrawlpy/commands/create_builder.py
+-rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.9b0/scrawlpy/commands/retry.py
+-rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/shell.py
+-rw-r--r--   0 wu         (501) staff       (20)     1177 2024-04-30 18:28:22.000000 scrawlpy-0.0.9b0/scrawlpy/commands/spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/commands/zip.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.312870 scrawlpy-0.0.9b0/scrawlpy/core/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.9b0/scrawlpy/core/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1328 2024-04-30 17:55:11.000000 scrawlpy-0.0.9b0/scrawlpy/core/base_spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.313697 scrawlpy-0.0.9b0/scrawlpy/core/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)      190 2024-04-30 16:37:30.000000 scrawlpy-0.0.9b0/scrawlpy/core/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3040 2024-04-30 18:30:11.000000 scrawlpy-0.0.9b0/scrawlpy/core/spiders/airspider.py
+-rw-r--r--   0 wu         (501) staff       (20)      269 2024-04-30 08:49:30.000000 scrawlpy-0.0.9b0/scrawlpy/core/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.314256 scrawlpy-0.0.9b0/scrawlpy/http/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:13.000000 scrawlpy-0.0.9b0/scrawlpy/http/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.9b0/scrawlpy/http/request.py
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.9b0/scrawlpy/requirements.txt
+-rw-r--r--   0 wu         (501) staff       (20)    12212 2024-04-30 17:25:57.000000 scrawlpy-0.0.9b0/scrawlpy/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.314808 scrawlpy-0.0.9b0/scrawlpy/storage/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:03:26.000000 scrawlpy-0.0.9b0/scrawlpy/storage/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1774 2024-04-30 10:13:18.000000 scrawlpy-0.0.9b0/scrawlpy/storage/memorydb.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.316245 scrawlpy-0.0.9b0/scrawlpy/templates/
+-rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/air_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/batch_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.316853 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/
+-rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.317291 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/items/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/items/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/main.py
+-rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.317410 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.9b0/scrawlpy/templates/spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/task_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.9b0/scrawlpy/templates/update_item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.318917 scrawlpy-0.0.9b0/scrawlpy/utils/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 09:29:03.000000 scrawlpy-0.0.9b0/scrawlpy/utils/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1439 2024-04-30 10:51:36.000000 scrawlpy-0.0.9b0/scrawlpy/utils/concurrent_util.py
+-rw-r--r--   0 wu         (501) staff       (20)     5490 2024-04-30 18:18:53.000000 scrawlpy-0.0.9b0/scrawlpy/utils/loader_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      827 2024-04-30 17:04:03.000000 scrawlpy-0.0.9b0/scrawlpy/utils/logger_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      727 2024-04-30 17:22:41.000000 scrawlpy-0.0.9b0/scrawlpy/utils/obj_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      726 2024-04-30 09:29:03.000000 scrawlpy-0.0.9b0/scrawlpy/utils/tail_thread.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.308126 scrawlpy-0.0.9b0/scrawlpy.egg-info/
+-rw-r--r--   0 wu         (501) staff       (20)      930 2024-04-30 18:30:32.000000 scrawlpy-0.0.9b0/scrawlpy.egg-info/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)     2321 2024-04-30 18:30:32.000000 scrawlpy-0.0.9b0/scrawlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 18:30:32.000000 scrawlpy-0.0.9b0/scrawlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 18:30:32.000000 scrawlpy-0.0.9b0/scrawlpy.egg-info/entry_points.txt
+-rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 18:30:32.000000 scrawlpy-0.0.9b0/scrawlpy.egg-info/requires.txt
+-rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 18:30:32.000000 scrawlpy-0.0.9b0/scrawlpy.egg-info/top_level.txt
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.319137 scrawlpy-0.0.9b0/scripts/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.9b0/scripts/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 18:30:32.323761 scrawlpy-0.0.9b0/setup.cfg
+-rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.9b0/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.319805 scrawlpy-0.0.9b0/test/
+-rw-r--r--   0 wu         (501) staff       (20)       68 2024-04-30 18:04:25.000000 scrawlpy-0.0.9b0/test/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      419 2024-04-30 10:53:23.000000 scrawlpy-0.0.9b0/test/func_demo.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.321017 scrawlpy-0.0.9b0/test/func_timeout_demo/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:34.000000 scrawlpy-0.0.9b0/test/func_timeout_demo/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2123 2024-04-30 11:04:37.000000 scrawlpy-0.0.9b0/test/func_timeout_demo/demo.py
+-rw-r--r--   0 wu         (501) staff       (20)     1521 2024-04-30 11:01:42.000000 scrawlpy-0.0.9b0/test/func_timeout_demo/test2.py
+-rw-r--r--   0 wu         (501) staff       (20)     1470 2024-04-30 16:41:53.000000 scrawlpy-0.0.9b0/test/func_timeout_demo/test3.py
+-rw-r--r--   0 wu         (501) staff       (20)     2934 2024-04-30 18:09:06.000000 scrawlpy-0.0.9b0/test/main.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.321538 scrawlpy-0.0.9b0/test/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.9b0/test/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      728 2024-04-30 17:49:57.000000 scrawlpy-0.0.9b0/test/spiders/airspider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.322013 scrawlpy-0.0.9b0/test/spiders/settings/
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.9b0/test/spiders/settings/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.9b0/test/spiders/settings/airspider_settings.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:30:32.322446 scrawlpy-0.0.9b0/test/spiders/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:50:00.000000 scrawlpy-0.0.9b0/test/spiders/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1037 2024-04-30 17:56:49.000000 scrawlpy-0.0.9b0/test/spiders/spiders/airspider.py
```

### Comparing `scrawlpy-0.0.9/LICENSE` & `scrawlpy-0.0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/PKG-INFO` & `scrawlpy-0.0.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.9
+Version: 0.0.9b0
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/cmdline.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/__init__.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_cookies.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_init.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_item.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_json.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_params.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_project.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_setting.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_spider.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create/create_table.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/create_builder.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/retry.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/retry.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/shell.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/spider.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/commands/zip.py` & `scrawlpy-0.0.9b0/scrawlpy/commands/zip.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/core/base_spider.py` & `scrawlpy-0.0.9b0/scrawlpy/core/base_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/core/spiders/airspider.py` & `scrawlpy-0.0.9b0/scrawlpy/core/spiders/airspider.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class AirSpider(AbstractSpider, TailThread):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.kwargs = kwargs
         self.thread_num = self.kwargs.get("thread_num", 1)
         self.crawler_threads = []
         self.request_queue = MemoryDB()
-        main()
+        # main()
 
     def start_task_distribute(self) -> None:
         """
         分发任务
         Returns:
 
         """
```

### Comparing `scrawlpy-0.0.9/scrawlpy/http/request.py` & `scrawlpy-0.0.9b0/scrawlpy/http/request.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/setting.py` & `scrawlpy-0.0.9b0/scrawlpy/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/storage/memorydb.py` & `scrawlpy-0.0.9b0/scrawlpy/storage/memorydb.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/air_spider_template.tmpl` & `scrawlpy-0.0.9b0/scrawlpy/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/batch_spider_template.tmpl` & `scrawlpy-0.0.9b0/scrawlpy/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/project_template/CHECK_DATA.md` & `scrawlpy-0.0.9b0/scrawlpy/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/project_template/main.py` & `scrawlpy-0.0.9b0/scrawlpy/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/project_template/setting.py` & `scrawlpy-0.0.9b0/scrawlpy/templates/project_template/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/spider_template.tmpl` & `scrawlpy-0.0.9b0/scrawlpy/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/templates/task_spider_template.tmpl` & `scrawlpy-0.0.9b0/scrawlpy/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/utils/concurrent_util.py` & `scrawlpy-0.0.9b0/scrawlpy/utils/concurrent_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/utils/loader_util.py` & `scrawlpy-0.0.9b0/scrawlpy/utils/loader_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/utils/logger_util.py` & `scrawlpy-0.0.9b0/scrawlpy/utils/logger_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/utils/obj_util.py` & `scrawlpy-0.0.9b0/scrawlpy/utils/obj_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy/utils/tail_thread.py` & `scrawlpy-0.0.9b0/scrawlpy/utils/tail_thread.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/scrawlpy.egg-info/PKG-INFO` & `scrawlpy-0.0.9b0/scrawlpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.9
+Version: 0.0.9b0
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.9/scrawlpy.egg-info/SOURCES.txt` & `scrawlpy-0.0.9b0/scrawlpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/setup.py` & `scrawlpy-0.0.9b0/setup.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/test/func_timeout_demo/demo.py` & `scrawlpy-0.0.9b0/test/func_timeout_demo/demo.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/test/func_timeout_demo/test2.py` & `scrawlpy-0.0.9b0/test/func_timeout_demo/test2.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/test/func_timeout_demo/test3.py` & `scrawlpy-0.0.9b0/test/func_timeout_demo/test3.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/test/main.py` & `scrawlpy-0.0.9b0/test/main.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/test/spiders/airspider.py` & `scrawlpy-0.0.9b0/test/spiders/airspider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.9/test/spiders/spiders/airspider.py` & `scrawlpy-0.0.9b0/test/spiders/spiders/airspider.py`

 * *Files identical despite different names*

