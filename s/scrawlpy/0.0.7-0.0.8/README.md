# Comparing `tmp/scrawlpy-0.0.7.tar.gz` & `tmp/scrawlpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrawlpy-0.0.7.tar", last modified: Tue Apr 30 18:09:58 2024, max compression
+gzip compressed data, was "scrawlpy-0.0.8.tar", last modified: Tue Apr 30 18:28:30 2024, max compression
```

## Comparing `scrawlpy-0.0.7.tar` & `scrawlpy-0.0.8.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.717884 scrawlpy-0.0.7/
--rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/LICENSE
--rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.7/MANIFEST.in
--rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:09:58.717580 scrawlpy-0.0.7/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.7/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.693325 scrawlpy-0.0.7/scrawlpy/
--rw-r--r--   0 wu         (501) staff       (20)        5 2024-04-30 18:09:55.000000 scrawlpy-0.0.7/scrawlpy/VERSION
--rw-r--r--   0 wu         (501) staff       (20)      179 2024-04-30 09:29:03.000000 scrawlpy-0.0.7/scrawlpy/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.696875 scrawlpy-0.0.7/scrawlpy/commands/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/cmdline.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.702430 scrawlpy-0.0.7/scrawlpy/commands/create/
--rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_cookies.py
--rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_init.py
--rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_item.py
--rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_json.py
--rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_params.py
--rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_project.py
--rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_setting.py
--rw-r--r--   0 wu         (501) staff       (20)     3649 2024-04-30 17:38:40.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_spider.py
--rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_table.py
--rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.7/scrawlpy/commands/create_builder.py
--rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.7/scrawlpy/commands/retry.py
--rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/shell.py
--rw-r--r--   0 wu         (501) staff       (20)     1141 2024-04-30 17:45:58.000000 scrawlpy-0.0.7/scrawlpy/commands/spider.py
--rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/zip.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.703042 scrawlpy-0.0.7/scrawlpy/core/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.7/scrawlpy/core/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1328 2024-04-30 17:55:11.000000 scrawlpy-0.0.7/scrawlpy/core/base_spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.703974 scrawlpy-0.0.7/scrawlpy/core/spiders/
--rw-r--r--   0 wu         (501) staff       (20)      190 2024-04-30 16:37:30.000000 scrawlpy-0.0.7/scrawlpy/core/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3036 2024-04-30 17:53:46.000000 scrawlpy-0.0.7/scrawlpy/core/spiders/airspider.py
--rw-r--r--   0 wu         (501) staff       (20)      269 2024-04-30 08:49:30.000000 scrawlpy-0.0.7/scrawlpy/core/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.704739 scrawlpy-0.0.7/scrawlpy/http/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:13.000000 scrawlpy-0.0.7/scrawlpy/http/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.7/scrawlpy/http/request.py
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.7/scrawlpy/requirements.txt
--rw-r--r--   0 wu         (501) staff       (20)    12212 2024-04-30 17:25:57.000000 scrawlpy-0.0.7/scrawlpy/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.705419 scrawlpy-0.0.7/scrawlpy/storage/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:03:26.000000 scrawlpy-0.0.7/scrawlpy/storage/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1774 2024-04-30 10:13:18.000000 scrawlpy-0.0.7/scrawlpy/storage/memorydb.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.707946 scrawlpy-0.0.7/scrawlpy/templates/
--rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/air_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/batch_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/item_template.tmpl
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.709264 scrawlpy-0.0.7/scrawlpy/templates/project_template/
--rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.710014 scrawlpy-0.0.7/scrawlpy/templates/project_template/items/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/items/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/main.py
--rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.710198 scrawlpy-0.0.7/scrawlpy/templates/project_template/spiders/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.7/scrawlpy/templates/spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/task_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/update_item_template.tmpl
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.712079 scrawlpy-0.0.7/scrawlpy/utils/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 09:29:03.000000 scrawlpy-0.0.7/scrawlpy/utils/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1439 2024-04-30 10:51:36.000000 scrawlpy-0.0.7/scrawlpy/utils/concurrent_util.py
--rw-r--r--   0 wu         (501) staff       (20)      827 2024-04-30 17:04:03.000000 scrawlpy-0.0.7/scrawlpy/utils/logger_util.py
--rw-r--r--   0 wu         (501) staff       (20)      727 2024-04-30 17:22:41.000000 scrawlpy-0.0.7/scrawlpy/utils/obj_util.py
--rw-r--r--   0 wu         (501) staff       (20)      726 2024-04-30 09:29:03.000000 scrawlpy-0.0.7/scrawlpy/utils/tail_thread.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.694523 scrawlpy-0.0.7/scrawlpy.egg-info/
--rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)     2291 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/SOURCES.txt
--rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/dependency_links.txt
--rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/entry_points.txt
--rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/requires.txt
--rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/top_level.txt
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.712357 scrawlpy-0.0.7/scripts/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.7/scripts/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 18:09:58.718063 scrawlpy-0.0.7/setup.cfg
--rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.7/setup.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.713147 scrawlpy-0.0.7/test/
--rw-r--r--   0 wu         (501) staff       (20)       68 2024-04-30 18:04:25.000000 scrawlpy-0.0.7/test/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      419 2024-04-30 10:53:23.000000 scrawlpy-0.0.7/test/func_demo.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.714462 scrawlpy-0.0.7/test/func_timeout_demo/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:34.000000 scrawlpy-0.0.7/test/func_timeout_demo/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     2123 2024-04-30 11:04:37.000000 scrawlpy-0.0.7/test/func_timeout_demo/demo.py
--rw-r--r--   0 wu         (501) staff       (20)     1521 2024-04-30 11:01:42.000000 scrawlpy-0.0.7/test/func_timeout_demo/test2.py
--rw-r--r--   0 wu         (501) staff       (20)     1470 2024-04-30 16:41:53.000000 scrawlpy-0.0.7/test/func_timeout_demo/test3.py
--rw-r--r--   0 wu         (501) staff       (20)     2934 2024-04-30 18:09:06.000000 scrawlpy-0.0.7/test/main.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.715011 scrawlpy-0.0.7/test/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.7/test/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      728 2024-04-30 17:49:57.000000 scrawlpy-0.0.7/test/spiders/airspider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.715649 scrawlpy-0.0.7/test/spiders/settings/
--rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.7/test/spiders/settings/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.7/test/spiders/settings/airspider_settings.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.716380 scrawlpy-0.0.7/test/spiders/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:50:00.000000 scrawlpy-0.0.7/test/spiders/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     1037 2024-04-30 17:56:49.000000 scrawlpy-0.0.7/test/spiders/spiders/airspider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.322928 scrawlpy-0.0.8/
+-rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/LICENSE
+-rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.8/MANIFEST.in
+-rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:28:30.322664 scrawlpy-0.0.8/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.8/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.302977 scrawlpy-0.0.8/scrawlpy/
+-rw-r--r--   0 wu         (501) staff       (20)        5 2024-04-30 18:28:29.000000 scrawlpy-0.0.8/scrawlpy/VERSION
+-rw-r--r--   0 wu         (501) staff       (20)      179 2024-04-30 09:29:03.000000 scrawlpy-0.0.8/scrawlpy/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.305817 scrawlpy-0.0.8/scrawlpy/commands/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/cmdline.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.308488 scrawlpy-0.0.8/scrawlpy/commands/create/
+-rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_cookies.py
+-rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_init.py
+-rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_item.py
+-rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_json.py
+-rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_params.py
+-rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_project.py
+-rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_setting.py
+-rw-r--r--   0 wu         (501) staff       (20)     3649 2024-04-30 17:38:40.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/create/create_table.py
+-rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.8/scrawlpy/commands/create_builder.py
+-rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.8/scrawlpy/commands/retry.py
+-rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/shell.py
+-rw-r--r--   0 wu         (501) staff       (20)     1177 2024-04-30 18:28:22.000000 scrawlpy-0.0.8/scrawlpy/commands/spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/commands/zip.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.309034 scrawlpy-0.0.8/scrawlpy/core/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.8/scrawlpy/core/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1328 2024-04-30 17:55:11.000000 scrawlpy-0.0.8/scrawlpy/core/base_spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.309822 scrawlpy-0.0.8/scrawlpy/core/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)      190 2024-04-30 16:37:30.000000 scrawlpy-0.0.8/scrawlpy/core/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3036 2024-04-30 17:53:46.000000 scrawlpy-0.0.8/scrawlpy/core/spiders/airspider.py
+-rw-r--r--   0 wu         (501) staff       (20)      269 2024-04-30 08:49:30.000000 scrawlpy-0.0.8/scrawlpy/core/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.310455 scrawlpy-0.0.8/scrawlpy/http/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:13.000000 scrawlpy-0.0.8/scrawlpy/http/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.8/scrawlpy/http/request.py
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.8/scrawlpy/requirements.txt
+-rw-r--r--   0 wu         (501) staff       (20)    12212 2024-04-30 17:25:57.000000 scrawlpy-0.0.8/scrawlpy/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.311094 scrawlpy-0.0.8/scrawlpy/storage/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:03:26.000000 scrawlpy-0.0.8/scrawlpy/storage/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1774 2024-04-30 10:13:18.000000 scrawlpy-0.0.8/scrawlpy/storage/memorydb.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.314140 scrawlpy-0.0.8/scrawlpy/templates/
+-rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/air_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/batch_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.315024 scrawlpy-0.0.8/scrawlpy/templates/project_template/
+-rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/project_template/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.315586 scrawlpy-0.0.8/scrawlpy/templates/project_template/items/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/project_template/items/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/project_template/main.py
+-rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/project_template/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.315713 scrawlpy-0.0.8/scrawlpy/templates/project_template/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.8/scrawlpy/templates/spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/task_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.8/scrawlpy/templates/update_item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.317274 scrawlpy-0.0.8/scrawlpy/utils/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 09:29:03.000000 scrawlpy-0.0.8/scrawlpy/utils/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1439 2024-04-30 10:51:36.000000 scrawlpy-0.0.8/scrawlpy/utils/concurrent_util.py
+-rw-r--r--   0 wu         (501) staff       (20)     5490 2024-04-30 18:18:53.000000 scrawlpy-0.0.8/scrawlpy/utils/loader_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      827 2024-04-30 17:04:03.000000 scrawlpy-0.0.8/scrawlpy/utils/logger_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      727 2024-04-30 17:22:41.000000 scrawlpy-0.0.8/scrawlpy/utils/obj_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      726 2024-04-30 09:29:03.000000 scrawlpy-0.0.8/scrawlpy/utils/tail_thread.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.304080 scrawlpy-0.0.8/scrawlpy.egg-info/
+-rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:28:30.000000 scrawlpy-0.0.8/scrawlpy.egg-info/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)     2321 2024-04-30 18:28:30.000000 scrawlpy-0.0.8/scrawlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 18:28:30.000000 scrawlpy-0.0.8/scrawlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 18:28:30.000000 scrawlpy-0.0.8/scrawlpy.egg-info/entry_points.txt
+-rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 18:28:30.000000 scrawlpy-0.0.8/scrawlpy.egg-info/requires.txt
+-rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 18:28:30.000000 scrawlpy-0.0.8/scrawlpy.egg-info/top_level.txt
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.317509 scrawlpy-0.0.8/scripts/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.8/scripts/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 18:28:30.322994 scrawlpy-0.0.8/setup.cfg
+-rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.8/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.318249 scrawlpy-0.0.8/test/
+-rw-r--r--   0 wu         (501) staff       (20)       68 2024-04-30 18:04:25.000000 scrawlpy-0.0.8/test/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      419 2024-04-30 10:53:23.000000 scrawlpy-0.0.8/test/func_demo.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.319483 scrawlpy-0.0.8/test/func_timeout_demo/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:34.000000 scrawlpy-0.0.8/test/func_timeout_demo/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2123 2024-04-30 11:04:37.000000 scrawlpy-0.0.8/test/func_timeout_demo/demo.py
+-rw-r--r--   0 wu         (501) staff       (20)     1521 2024-04-30 11:01:42.000000 scrawlpy-0.0.8/test/func_timeout_demo/test2.py
+-rw-r--r--   0 wu         (501) staff       (20)     1470 2024-04-30 16:41:53.000000 scrawlpy-0.0.8/test/func_timeout_demo/test3.py
+-rw-r--r--   0 wu         (501) staff       (20)     2934 2024-04-30 18:09:06.000000 scrawlpy-0.0.8/test/main.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.320266 scrawlpy-0.0.8/test/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.8/test/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      728 2024-04-30 17:49:57.000000 scrawlpy-0.0.8/test/spiders/airspider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.320984 scrawlpy-0.0.8/test/spiders/settings/
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.8/test/spiders/settings/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.8/test/spiders/settings/airspider_settings.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:28:30.321715 scrawlpy-0.0.8/test/spiders/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:50:00.000000 scrawlpy-0.0.8/test/spiders/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1037 2024-04-30 17:56:49.000000 scrawlpy-0.0.8/test/spiders/spiders/airspider.py
```

### Comparing `scrawlpy-0.0.7/LICENSE` & `scrawlpy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/PKG-INFO` & `scrawlpy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/cmdline.py` & `scrawlpy-0.0.8/scrawlpy/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/__init__.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_cookies.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_init.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_item.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_json.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_params.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_project.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_setting.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_spider.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create/create_table.py` & `scrawlpy-0.0.8/scrawlpy/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/create_builder.py` & `scrawlpy-0.0.8/scrawlpy/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/retry.py` & `scrawlpy-0.0.8/scrawlpy/commands/retry.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/shell.py` & `scrawlpy-0.0.8/scrawlpy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/spider.py` & `scrawlpy-0.0.8/scrawlpy/commands/spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Time   : 2024/5/1 01:38
 import argparse
 from scrawlpy.setting import Settings
 
 
-def main():
-    params = argparse.ArgumentParser(description="sql执行参数")
-    params.add_argument("-a", "--append", action="append", help="环境", metavar="")
-    params.add_argument("-e", "--env", help="环境", metavar="")
-    params.add_argument("-d", "--day", help="日期", metavar="")
-    params.add_argument("--hour", type=int, help="小时", metavar="")
-    params.add_argument("-j", "--job_id", type=str, help="任务id", metavar="")
-    params.add_argument("-k", "--url_kind", type=int, help="结果类型", metavar="", default=0)
-    # params.add_argument("-t", "--query_type", type=str, help=f"查询类型 {', '.join(query_type_list)}", metavar="")
-    params.add_argument("-l", "--limit", type=int, help="查询限制数", metavar="", default=10)
-    params.add_argument("-b", "--bot", type=int, help="是否告警", metavar="", default=1)
-    args = params.parse_args()
-    if args.append:
-        print("哈哈哈哈哈")
-        setattr(Settings, "Append", args.append)
-
-
-if __name__ == '__main__':
-    main()
+# def main():
+#     params = argparse.ArgumentParser(description="sql执行参数")
+#     params.add_argument("-a", "--append", action="append", help="环境", metavar="")
+#     params.add_argument("-e", "--env", help="环境", metavar="")
+#     params.add_argument("-d", "--day", help="日期", metavar="")
+#     params.add_argument("--hour", type=int, help="小时", metavar="")
+#     params.add_argument("-j", "--job_id", type=str, help="任务id", metavar="")
+#     params.add_argument("-k", "--url_kind", type=int, help="结果类型", metavar="", default=0)
+#     # params.add_argument("-t", "--query_type", type=str, help=f"查询类型 {', '.join(query_type_list)}", metavar="")
+#     params.add_argument("-l", "--limit", type=int, help="查询限制数", metavar="", default=10)
+#     params.add_argument("-b", "--bot", type=int, help="是否告警", metavar="", default=1)
+#     args = params.parse_args()
+#     if args.append:
+#         print("哈哈哈哈哈")
+#         setattr(Settings, "Append", args.append)
+#
+#
+# if __name__ == '__main__':
+#     main()
```

### Comparing `scrawlpy-0.0.7/scrawlpy/commands/zip.py` & `scrawlpy-0.0.8/scrawlpy/commands/zip.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/core/base_spider.py` & `scrawlpy-0.0.8/scrawlpy/core/base_spider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/core/spiders/airspider.py` & `scrawlpy-0.0.8/scrawlpy/core/spiders/airspider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/http/request.py` & `scrawlpy-0.0.8/scrawlpy/http/request.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/setting.py` & `scrawlpy-0.0.8/scrawlpy/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/storage/memorydb.py` & `scrawlpy-0.0.8/scrawlpy/storage/memorydb.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/air_spider_template.tmpl` & `scrawlpy-0.0.8/scrawlpy/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/batch_spider_template.tmpl` & `scrawlpy-0.0.8/scrawlpy/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/project_template/CHECK_DATA.md` & `scrawlpy-0.0.8/scrawlpy/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/project_template/main.py` & `scrawlpy-0.0.8/scrawlpy/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/project_template/setting.py` & `scrawlpy-0.0.8/scrawlpy/templates/project_template/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/spider_template.tmpl` & `scrawlpy-0.0.8/scrawlpy/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/templates/task_spider_template.tmpl` & `scrawlpy-0.0.8/scrawlpy/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/utils/concurrent_util.py` & `scrawlpy-0.0.8/scrawlpy/utils/concurrent_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/utils/logger_util.py` & `scrawlpy-0.0.8/scrawlpy/utils/logger_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/utils/obj_util.py` & `scrawlpy-0.0.8/scrawlpy/utils/obj_util.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy/utils/tail_thread.py` & `scrawlpy-0.0.8/scrawlpy/utils/tail_thread.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/scrawlpy.egg-info/PKG-INFO` & `scrawlpy-0.0.8/scrawlpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.7/scrawlpy.egg-info/SOURCES.txt` & `scrawlpy-0.0.8/scrawlpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 scrawlpy/templates/project_template/README.md
 scrawlpy/templates/project_template/main.py
 scrawlpy/templates/project_template/setting.py
 scrawlpy/templates/project_template/items/__init__.py
 scrawlpy/templates/project_template/spiders/__init__.py
 scrawlpy/utils/__init__.py
 scrawlpy/utils/concurrent_util.py
+scrawlpy/utils/loader_util.py
 scrawlpy/utils/logger_util.py
 scrawlpy/utils/obj_util.py
 scrawlpy/utils/tail_thread.py
 scripts/__init__.py
 test/__init__.py
 test/func_demo.py
 test/main.py
```

### Comparing `scrawlpy-0.0.7/setup.py` & `scrawlpy-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/test/func_timeout_demo/demo.py` & `scrawlpy-0.0.8/test/func_timeout_demo/demo.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/test/func_timeout_demo/test2.py` & `scrawlpy-0.0.8/test/func_timeout_demo/test2.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/test/func_timeout_demo/test3.py` & `scrawlpy-0.0.8/test/func_timeout_demo/test3.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/test/main.py` & `scrawlpy-0.0.8/test/main.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/test/spiders/airspider.py` & `scrawlpy-0.0.8/test/spiders/airspider.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.7/test/spiders/spiders/airspider.py` & `scrawlpy-0.0.8/test/spiders/spiders/airspider.py`

 * *Files identical despite different names*

