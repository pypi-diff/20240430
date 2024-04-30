# Comparing `tmp/scrawlpy-0.0.6.tar.gz` & `tmp/scrawlpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrawlpy-0.0.6.tar", last modified: Tue Apr 30 08:41:14 2024, max compression
+gzip compressed data, was "scrawlpy-0.0.7.tar", last modified: Tue Apr 30 18:09:58 2024, max compression
```

## Comparing `scrawlpy-0.0.6.tar` & `scrawlpy-0.0.7.tar`

### file list

```diff
@@ -1,69 +1,93 @@
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.249121 scrawlpy-0.0.6/
--rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/LICENSE
--rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.6/MANIFEST.in
--rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 08:41:14.248839 scrawlpy-0.0.6/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.6/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.237231 scrawlpy-0.0.6/scrawlpy/
--rw-r--r--   0 wu         (501) staff       (20)        5 2024-04-30 08:41:12.000000 scrawlpy-0.0.6/scrawlpy/VERSION
--rw-r--r--   0 wu         (501) staff       (20)      135 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.239877 scrawlpy-0.0.6/scrawlpy/commands/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/cmdline.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.242538 scrawlpy-0.0.6/scrawlpy/commands/create/
--rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_cookies.py
--rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_init.py
--rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_item.py
--rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_json.py
--rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_params.py
--rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_project.py
--rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_setting.py
--rw-r--r--   0 wu         (501) staff       (20)     3648 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_spider.py
--rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/create/create_table.py
--rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/commands/create_builder.py
--rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/commands/retry.py
--rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/shell.py
--rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/commands/zip.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.243084 scrawlpy-0.0.6/scrawlpy/core/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.6/scrawlpy/core/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      705 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/core/base_spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.243420 scrawlpy-0.0.6/scrawlpy/core/spiders/
--rw-r--r--   0 wu         (501) staff       (20)      125 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/core/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      306 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/scrawlpy/core/spiders/spider.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.243839 scrawlpy-0.0.6/scrawlpy/http/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-29 15:39:00.000000 scrawlpy-0.0.6/scrawlpy/http/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.6/scrawlpy/http/request.py
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.6/scrawlpy/requirements.txt
--rw-r--r--   0 wu         (501) staff       (20)    11219 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.245542 scrawlpy-0.0.6/scrawlpy/templates/
--rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/air_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/batch_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/item_template.tmpl
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246206 scrawlpy-0.0.6/scrawlpy/templates/project_template/
--rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/CHECK_DATA.md
--rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/README.md
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246513 scrawlpy-0.0.6/scrawlpy/templates/project_template/items/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/items/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/main.py
--rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/setting.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246613 scrawlpy-0.0.6/scrawlpy/templates/project_template/spiders/
--rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/project_template/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.6/scrawlpy/templates/spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/task_spider_template.tmpl
--rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.6/scrawlpy/templates/update_item_template.tmpl
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.238393 scrawlpy-0.0.6/scrawlpy.egg-info/
--rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/PKG-INFO
--rw-r--r--   0 wu         (501) staff       (20)     1713 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/SOURCES.txt
--rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/dependency_links.txt
--rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/entry_points.txt
--rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/requires.txt
--rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 08:41:14.000000 scrawlpy-0.0.6/scrawlpy.egg-info/top_level.txt
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.246709 scrawlpy-0.0.6/scripts/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.6/scripts/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 08:41:14.249173 scrawlpy-0.0.6/setup.cfg
--rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.6/setup.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.247082 scrawlpy-0.0.6/test/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.6/test/__init__.py
-drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 08:41:14.247658 scrawlpy-0.0.6/test/spiders/
--rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.6/test/spiders/__init__.py
--rw-r--r--   0 wu         (501) staff       (20)      326 2024-04-30 03:46:59.000000 scrawlpy-0.0.6/test/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.717884 scrawlpy-0.0.7/
+-rw-r--r--   0 wu         (501) staff       (20)     1102 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/LICENSE
+-rw-r--r--   0 wu         (501) staff       (20)      235 2024-04-30 08:40:25.000000 scrawlpy-0.0.7/MANIFEST.in
+-rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:09:58.717580 scrawlpy-0.0.7/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)       66 2024-04-30 03:52:44.000000 scrawlpy-0.0.7/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.693325 scrawlpy-0.0.7/scrawlpy/
+-rw-r--r--   0 wu         (501) staff       (20)        5 2024-04-30 18:09:55.000000 scrawlpy-0.0.7/scrawlpy/VERSION
+-rw-r--r--   0 wu         (501) staff       (20)      179 2024-04-30 09:29:03.000000 scrawlpy-0.0.7/scrawlpy/__init__.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.696875 scrawlpy-0.0.7/scrawlpy/commands/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3824 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/cmdline.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.702430 scrawlpy-0.0.7/scrawlpy/commands/create/
+-rw-r--r--   0 wu         (501) staff       (20)      543 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      975 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_cookies.py
+-rw-r--r--   0 wu         (501) staff       (20)      670 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_init.py
+-rw-r--r--   0 wu         (501) staff       (20)     6004 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_item.py
+-rw-r--r--   0 wu         (501) staff       (20)     1366 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_json.py
+-rw-r--r--   0 wu         (501) staff       (20)     1106 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_params.py
+-rw-r--r--   0 wu         (501) staff       (20)     1360 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_project.py
+-rw-r--r--   0 wu         (501) staff       (20)      693 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_setting.py
+-rw-r--r--   0 wu         (501) staff       (20)     3649 2024-04-30 17:38:40.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     4288 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/create/create_table.py
+-rw-r--r--   0 wu         (501) staff       (20)     3986 2024-04-30 03:46:59.000000 scrawlpy-0.0.7/scrawlpy/commands/create_builder.py
+-rw-r--r--   0 wu         (501) staff       (20)     1356 2024-04-30 03:46:59.000000 scrawlpy-0.0.7/scrawlpy/commands/retry.py
+-rw-r--r--   0 wu         (501) staff       (20)     5514 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/shell.py
+-rw-r--r--   0 wu         (501) staff       (20)     1141 2024-04-30 17:45:58.000000 scrawlpy-0.0.7/scrawlpy/commands/spider.py
+-rw-r--r--   0 wu         (501) staff       (20)     2572 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/commands/zip.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.703042 scrawlpy-0.0.7/scrawlpy/core/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:29:09.000000 scrawlpy-0.0.7/scrawlpy/core/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1328 2024-04-30 17:55:11.000000 scrawlpy-0.0.7/scrawlpy/core/base_spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.703974 scrawlpy-0.0.7/scrawlpy/core/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)      190 2024-04-30 16:37:30.000000 scrawlpy-0.0.7/scrawlpy/core/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     3036 2024-04-30 17:53:46.000000 scrawlpy-0.0.7/scrawlpy/core/spiders/airspider.py
+-rw-r--r--   0 wu         (501) staff       (20)      269 2024-04-30 08:49:30.000000 scrawlpy-0.0.7/scrawlpy/core/spiders/spider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.704739 scrawlpy-0.0.7/scrawlpy/http/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:13.000000 scrawlpy-0.0.7/scrawlpy/http/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     7206 2024-04-28 08:57:54.000000 scrawlpy-0.0.7/scrawlpy/http/request.py
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-30 08:37:28.000000 scrawlpy-0.0.7/scrawlpy/requirements.txt
+-rw-r--r--   0 wu         (501) staff       (20)    12212 2024-04-30 17:25:57.000000 scrawlpy-0.0.7/scrawlpy/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.705419 scrawlpy-0.0.7/scrawlpy/storage/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:03:26.000000 scrawlpy-0.0.7/scrawlpy/storage/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1774 2024-04-30 10:13:18.000000 scrawlpy-0.0.7/scrawlpy/storage/memorydb.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.707946 scrawlpy-0.0.7/scrawlpy/templates/
+-rw-r--r--   0 wu         (501) staff       (20)      592 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/air_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2083 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/batch_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      353 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.709264 scrawlpy-0.0.7/scrawlpy/templates/project_template/
+-rw-r--r--   0 wu         (501) staff       (20)     1574 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/CHECK_DATA.md
+-rw-r--r--   0 wu         (501) staff       (20)       81 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/README.md
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.710014 scrawlpy-0.0.7/scrawlpy/templates/project_template/items/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/items/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2089 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/main.py
+-rw-r--r--   0 wu         (501) staff       (20)     9207 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/setting.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.710198 scrawlpy-0.0.7/scrawlpy/templates/project_template/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)        0 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/project_template/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      805 2024-04-28 08:40:08.000000 scrawlpy-0.0.7/scrawlpy/templates/spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)     2336 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/task_spider_template.tmpl
+-rw-r--r--   0 wu         (501) staff       (20)      365 2024-04-28 08:11:46.000000 scrawlpy-0.0.7/scrawlpy/templates/update_item_template.tmpl
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.712079 scrawlpy-0.0.7/scrawlpy/utils/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 09:29:03.000000 scrawlpy-0.0.7/scrawlpy/utils/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1439 2024-04-30 10:51:36.000000 scrawlpy-0.0.7/scrawlpy/utils/concurrent_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      827 2024-04-30 17:04:03.000000 scrawlpy-0.0.7/scrawlpy/utils/logger_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      727 2024-04-30 17:22:41.000000 scrawlpy-0.0.7/scrawlpy/utils/obj_util.py
+-rw-r--r--   0 wu         (501) staff       (20)      726 2024-04-30 09:29:03.000000 scrawlpy-0.0.7/scrawlpy/utils/tail_thread.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.694523 scrawlpy-0.0.7/scrawlpy.egg-info/
+-rw-r--r--   0 wu         (501) staff       (20)      928 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/PKG-INFO
+-rw-r--r--   0 wu         (501) staff       (20)     2291 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wu         (501) staff       (20)        1 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wu         (501) staff       (20)       63 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/entry_points.txt
+-rw-r--r--   0 wu         (501) staff       (20)      214 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/requires.txt
+-rw-r--r--   0 wu         (501) staff       (20)       22 2024-04-30 18:09:58.000000 scrawlpy-0.0.7/scrawlpy.egg-info/top_level.txt
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.712357 scrawlpy-0.0.7/scripts/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:23:17.000000 scrawlpy-0.0.7/scripts/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       38 2024-04-30 18:09:58.718063 scrawlpy-0.0.7/setup.cfg
+-rw-r--r--   0 wu         (501) staff       (20)     1732 2024-04-30 08:41:12.000000 scrawlpy-0.0.7/setup.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.713147 scrawlpy-0.0.7/test/
+-rw-r--r--   0 wu         (501) staff       (20)       68 2024-04-30 18:04:25.000000 scrawlpy-0.0.7/test/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      419 2024-04-30 10:53:23.000000 scrawlpy-0.0.7/test/func_demo.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.714462 scrawlpy-0.0.7/test/func_timeout_demo/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-30 10:52:34.000000 scrawlpy-0.0.7/test/func_timeout_demo/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     2123 2024-04-30 11:04:37.000000 scrawlpy-0.0.7/test/func_timeout_demo/demo.py
+-rw-r--r--   0 wu         (501) staff       (20)     1521 2024-04-30 11:01:42.000000 scrawlpy-0.0.7/test/func_timeout_demo/test2.py
+-rw-r--r--   0 wu         (501) staff       (20)     1470 2024-04-30 16:41:53.000000 scrawlpy-0.0.7/test/func_timeout_demo/test3.py
+-rw-r--r--   0 wu         (501) staff       (20)     2934 2024-04-30 18:09:06.000000 scrawlpy-0.0.7/test/main.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.715011 scrawlpy-0.0.7/test/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       52 2024-04-28 08:55:20.000000 scrawlpy-0.0.7/test/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)      728 2024-04-30 17:49:57.000000 scrawlpy-0.0.7/test/spiders/airspider.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.715649 scrawlpy-0.0.7/test/spiders/settings/
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.7/test/spiders/settings/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:28:02.000000 scrawlpy-0.0.7/test/spiders/settings/airspider_settings.py
+drwxr-xr-x   0 wu         (501) staff       (20)        0 2024-04-30 18:09:58.716380 scrawlpy-0.0.7/test/spiders/spiders/
+-rw-r--r--   0 wu         (501) staff       (20)       51 2024-04-30 17:50:00.000000 scrawlpy-0.0.7/test/spiders/spiders/__init__.py
+-rw-r--r--   0 wu         (501) staff       (20)     1037 2024-04-30 17:56:49.000000 scrawlpy-0.0.7/test/spiders/spiders/airspider.py
```

### Comparing `scrawlpy-0.0.6/LICENSE` & `scrawlpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/PKG-INFO` & `scrawlpy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/cmdline.py` & `scrawlpy-0.0.7/scrawlpy/commands/cmdline.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/__init__.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/__init__.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_cookies.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_cookies.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_init.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_init.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_item.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_item.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_json.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_json.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_params.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_params.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_project.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_project.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_setting.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_spider.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @email:  boris_liu@foxmail.com
 """
 
 import getpass
 import os
 import re
 
-import feapder.utils.tools as tools
+import scrawlpy.utils.tools as tools
 from .create_init import CreateInit
 
 
 def deal_file_info(file):
     file = file.replace("{DATE}", tools.get_current_date())
     file = file.replace("{USER}", os.getenv("FEAPDER_USER") or getpass.getuser())
```

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create/create_table.py` & `scrawlpy-0.0.7/scrawlpy/commands/create/create_table.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/create_builder.py` & `scrawlpy-0.0.7/scrawlpy/commands/create_builder.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/retry.py` & `scrawlpy-0.0.7/scrawlpy/commands/retry.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/shell.py` & `scrawlpy-0.0.7/scrawlpy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/commands/zip.py` & `scrawlpy-0.0.7/scrawlpy/commands/zip.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/http/request.py` & `scrawlpy-0.0.7/scrawlpy/http/request.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/setting.py` & `scrawlpy-0.0.7/scrawlpy/setting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,235 +1,243 @@
 # -*- coding: utf-8 -*-
 """爬虫配置文件"""
+import json
 import os
 
-# redis 表名
-# 任务表模版
-TAB_REQUESTS = "{redis_key}:z_requests"
-# 任务失败模板
-TAB_FAILED_REQUESTS = "{redis_key}:z_failed_requests"
-# 数据保存失败模板
-TAB_FAILED_ITEMS = "{redis_key}:s_failed_items"
-# 爬虫状态表模版
-TAB_SPIDER_STATUS = "{redis_key}:h_spider_status"
-# 用户池
-TAB_USER_POOL = "{redis_key}:h_{user_type}_pool"
-
-# MYSQL
-MYSQL_IP = os.getenv("MYSQL_IP")
-MYSQL_PORT = int(os.getenv("MYSQL_PORT", 3306))
-MYSQL_DB = os.getenv("MYSQL_DB")
-MYSQL_USER_NAME = os.getenv("MYSQL_USER_NAME")
-MYSQL_USER_PASS = os.getenv("MYSQL_USER_PASS")
-
-# MONGODB
-MONGO_IP = os.getenv("MONGO_IP", "localhost")
-MONGO_PORT = int(os.getenv("MONGO_PORT", 27017))
-MONGO_DB = os.getenv("MONGO_DB")
-MONGO_USER_NAME = os.getenv("MONGO_USER_NAME")
-MONGO_USER_PASS = os.getenv("MONGO_USER_PASS")
-MONGO_URL = os.getenv("MONGO_URL")
-
-# REDIS
-# ip:port 多个可写为列表或者逗号隔开 如 ip1:port1,ip2:port2 或 ["ip1:port1", "ip2:port2"]
-REDISDB_IP_PORTS = os.getenv("REDISDB_IP_PORTS")
-REDISDB_USER_PASS = os.getenv("REDISDB_USER_PASS")
-REDISDB_DB = int(os.getenv("REDISDB_DB", 0))
-# 连接redis时携带的其他参数，如ssl=True
-REDISDB_KWARGS = dict()
-# 适用于redis哨兵模式
-REDISDB_SERVICE_NAME = os.getenv("REDISDB_SERVICE_NAME")
-
-# 数据入库的pipeline，可自定义，默认MysqlPipeline
-ITEM_PIPELINES = [
-    "feapder.pipelines.mysql_pipeline.MysqlPipeline",
-    # "feapder.pipelines.mongo_pipeline.MongoPipeline",
-    # "feapder.pipelines.console_pipeline.ConsolePipeline",
-]
-EXPORT_DATA_MAX_FAILED_TIMES = 10  # 导出数据时最大的失败次数，包括保存和更新，超过这个次数报警
-EXPORT_DATA_MAX_RETRY_TIMES = 10  # 导出数据时最大的重试次数，包括保存和更新，超过这个次数则放弃重试
-
-# 爬虫相关
-# COLLECTOR
-COLLECTOR_TASK_COUNT = 32  # 每次获取任务数量，追求速度推荐32
-
-# SPIDER
-SPIDER_THREAD_COUNT = 1  # 爬虫并发数，追求速度推荐32
-# 下载时间间隔 单位秒。 支持随机 如 SPIDER_SLEEP_TIME = [2, 5] 则间隔为 2~5秒之间的随机数，包含2和5
-SPIDER_SLEEP_TIME = 0
-SPIDER_MAX_RETRY_TIMES = 10  # 每个请求最大重试次数
-# 是否主动执行添加 设置为False 需要手动调用start_monitor_task，适用于多进程情况下
-SPIDER_AUTO_START_REQUESTS = True
-KEEP_ALIVE = False  # 爬虫是否常驻
-
-# 浏览器渲染
-WEBDRIVER = dict(
-    pool_size=1,  # 浏览器的数量
-    load_images=True,  # 是否加载图片
-    user_agent=None,  # 字符串 或 无参函数，返回值为user_agent
-    proxy=None,  # xxx.xxx.xxx.xxx:xxxx 或 无参函数，返回值为代理地址
-    headless=False,  # 是否为无头浏览器
-    driver_type="CHROME",  # CHROME、EDGE、PHANTOMJS、FIREFOX
-    timeout=30,  # 请求超时时间
-    window_size=(1024, 800),  # 窗口大小
-    executable_path=None,  # 浏览器路径，默认为默认路径
-    render_time=0,  # 渲染时长，即打开网页等待指定时间后再获取源码
-    custom_argument=[
-        "--ignore-certificate-errors",
-        "--disable-blink-features=AutomationControlled",
-    ],  # 自定义浏览器渲染参数
-    xhr_url_regexes=None,  # 拦截xhr接口，支持正则，数组类型
-    auto_install_driver=True,  # 自动下载浏览器驱动 支持chrome 和 firefox
-    download_path=None,  # 下载文件的路径
-    use_stealth_js=False,  # 使用stealth.min.js隐藏浏览器特征
-)
-
-PLAYWRIGHT = dict(
-    user_agent=None,  # 字符串 或 无参函数，返回值为user_agent
-    proxy=None,  # xxx.xxx.xxx.xxx:xxxx 或 无参函数，返回值为代理地址
-    headless=False,  # 是否为无头浏览器
-    driver_type="chromium",  # chromium、firefox、webkit
-    timeout=30,  # 请求超时时间
-    window_size=(1024, 800),  # 窗口大小
-    executable_path=None,  # 浏览器路径，默认为默认路径
-    download_path=None,  # 下载文件的路径
-    render_time=0,  # 渲染时长，即打开网页等待指定时间后再获取源码
-    wait_until="networkidle",  # 等待页面加载完成的事件,可选值："commit", "domcontentloaded", "load", "networkidle"
-    use_stealth_js=False,  # 使用stealth.min.js隐藏浏览器特征
-    page_on_event_callback=None,  # page.on() 事件的回调 如 page_on_event_callback={"dialog": lambda dialog: dialog.accept()}
-    storage_state_path=None,  # 保存浏览器状态的路径
-    url_regexes=None,  # 拦截接口，支持正则，数组类型
-    save_all=False,  # 是否保存所有拦截的接口, 配合url_regexes使用，为False时只保存最后一次拦截的接口
-)
-
-# 爬虫启动时，重新抓取失败的requests
-RETRY_FAILED_REQUESTS = False
-# 爬虫启动时，重新入库失败的item
-RETRY_FAILED_ITEMS = False
-# 保存失败的request
-SAVE_FAILED_REQUEST = True
-# request防丢机制。（指定的REQUEST_LOST_TIMEOUT时间内request还没做完，会重新下发 重做）
-REQUEST_LOST_TIMEOUT = 600  # 10分钟
-# request网络请求超时时间
-REQUEST_TIMEOUT = 22  # 等待服务器响应的超时时间，浮点数，或(connect timeout, read timeout)元组
-# item在内存队列中最大缓存数量
-ITEM_MAX_CACHED_COUNT = 5000
-# item每批入库的最大数量
-ITEM_UPLOAD_BATCH_MAX_SIZE = 1000
-# item入库时间间隔
-ITEM_UPLOAD_INTERVAL = 1
-# 内存任务队列最大缓存的任务数，默认不限制；仅对AirSpider有效。
-TASK_MAX_CACHED_SIZE = 0
-
-# 下载缓存 利用redis缓存，但由于内存大小限制，所以建议仅供开发调试代码时使用，防止每次debug都需要网络请求
-RESPONSE_CACHED_ENABLE = False  # 是否启用下载缓存 成本高的数据或容易变需求的数据，建议设置为True
-RESPONSE_CACHED_EXPIRE_TIME = 3600  # 缓存时间 秒
-RESPONSE_CACHED_USED = False  # 是否使用缓存 补采数据时可设置为True
-
-# redis 存放item与request的根目录
-REDIS_KEY = ""
-# 爬虫启动时删除的key，类型: 元组/bool/string。 支持正则; 常用于清空任务队列，否则重启时会断点续爬
-DELETE_KEYS = []
-
-# 设置代理
-PROXY_EXTRACT_API = None  # 代理提取API ，返回的代理分割符为\r\n
-PROXY_ENABLE = True
-PROXY_MAX_FAILED_TIMES = 5  # 代理最大失败次数，超过则不使用，自动删除
-PROXY_POOL = "feapder.network.proxy_pool.ProxyPool"  # 代理池
-
-# 随机headers
-RANDOM_HEADERS = True
-# UserAgent类型 支持 'chrome', 'opera', 'firefox', 'internetexplorer', 'safari'，'mobile' 若不指定则随机类型
-USER_AGENT_TYPE = "chrome"
-# 默认使用的浏览器头
-DEFAULT_USERAGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.103 Safari/537.36"
-# requests 使用session
-USE_SESSION = False
-
-# 下载
-DOWNLOADER = "feapder.network.downloader.RequestsDownloader"  # 请求下载器
-SESSION_DOWNLOADER = "feapder.network.downloader.RequestsSessionDownloader"
-RENDER_DOWNLOADER = "feapder.network.downloader.SeleniumDownloader"  # 渲染下载器
-# RENDER_DOWNLOADER="feapder.network.downloader.PlaywrightDownloader"
-MAKE_ABSOLUTE_LINKS = True  # 自动转成绝对连接
-
-# 去重
-ITEM_FILTER_ENABLE = False  # item 去重
-ITEM_FILTER_SETTING = dict(
-    filter_type=1  # 永久去重（BloomFilter） = 1 、内存去重（MemoryFilter） = 2、 临时去重（ExpireFilter）= 3、轻量去重（LiteFilter）= 4
-)
-REQUEST_FILTER_ENABLE = False  # request 去重
-REQUEST_FILTER_SETTING = dict(
-    filter_type=3,  # 永久去重（BloomFilter） = 1 、内存去重（MemoryFilter） = 2、 临时去重（ExpireFilter）= 3、 轻量去重（LiteFilter）= 4
-    expire_time=2592000,  # 过期时间1个月
-)
-
-# 报警 支持钉钉、飞书、企业微信、邮件
-# 钉钉报警
-DINGDING_WARNING_URL = ""  # 钉钉机器人api
-DINGDING_WARNING_PHONE = ""  # 被@的群成员手机号，支持列表，可指定多个。
-DINGDING_WARNING_USER_ID = ""  # 被@的群成员userId，支持列表，可指定多个
-DINGDING_WARNING_ALL = False  # 是否提示所有人， 默认为False
-DINGDING_WARNING_SECRET = None  # 加签密钥
-# 飞书报警
-# https://open.feishu.cn/document/ukTMukTMukTM/ucTM5YjL3ETO24yNxkjN#e1cdee9f
-FEISHU_WARNING_URL = ""  # 飞书机器人api
-FEISHU_WARNING_USER = None  # 报警人 {"open_id":"ou_xxxxx", "name":"xxxx"} 或 [{"open_id":"ou_xxxxx", "name":"xxxx"}]
-FEISHU_WARNING_ALL = False  # 是否提示所有人， 默认为False
-# 邮件报警
-EMAIL_SENDER = ""  # 发件人
-EMAIL_PASSWORD = ""  # 授权码
-EMAIL_RECEIVER = ""  # 收件人 支持列表，可指定多个
-EMAIL_SMTPSERVER = "smtp.163.com"  # 邮件服务器 默认为163邮箱
-# 企业微信报警
-WECHAT_WARNING_URL = ""  # 企业微信机器人api
-WECHAT_WARNING_PHONE = ""  # 报警人 将会在群内@此人, 支持列表，可指定多人
-WECHAT_WARNING_ALL = False  # 是否提示所有人， 默认为False
-# 时间间隔
-WARNING_INTERVAL = 3600  # 相同报警的报警时间间隔，防止刷屏; 0表示不去重
-WARNING_LEVEL = "DEBUG"  # 报警级别， DEBUG / INFO / ERROR
-WARNING_FAILED_COUNT = 1000  # 任务失败数 超过WARNING_FAILED_COUNT则报警
-WARNING_CHECK_TASK_COUNT_INTERVAL = 1200  # 检查已做任务数量的时间间隔，若两次时间间隔之间，任务数无变化则报警
-
-# 日志
-LOG_NAME = os.path.basename(os.getcwd())
-LOG_PATH = "log/%s.log" % LOG_NAME  # log存储路径
-LOG_LEVEL = os.getenv("LOG_LEVEL", "DEBUG")  # 日志级别
-LOG_COLOR = True  # 是否带有颜色
-LOG_IS_WRITE_TO_CONSOLE = True  # 是否打印到控制台
-LOG_IS_WRITE_TO_FILE = False  # 是否写文件
-LOG_MODE = "w"  # 写文件的模式
-LOG_MAX_BYTES = 10 * 1024 * 1024  # 每个日志文件的最大字节数
-LOG_BACKUP_COUNT = 20  # 日志文件保留数量
-LOG_ENCODING = "utf8"  # 日志文件编码
-# 是否详细的打印异常
-PRINT_EXCEPTION_DETAILS = True
-# 设置不带颜色的日志格式
-LOG_FORMAT = "%(threadName)s|%(asctime)s|%(filename)s|%(funcName)s|line:%(lineno)d|%(levelname)s| %(message)s"
-# 设置带有颜色的日志格式
-os.environ["LOGURU_FORMAT"] = (
-    "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
-    "<level>{level: <8}</level> | "
-    "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>line:{line}</cyan> | <level>{message}</level>"
-)
-OTHERS_LOG_LEVAL = "ERROR"  # 第三方库的log等级
-
-# 打点监控 influxdb 配置
-INFLUXDB_HOST = os.getenv("INFLUXDB_HOST", "localhost")
-INFLUXDB_PORT = int(os.getenv("INFLUXDB_PORT", 8086))
-INFLUXDB_UDP_PORT = int(os.getenv("INFLUXDB_UDP_PORT", 8089))
-INFLUXDB_USER = os.getenv("INFLUXDB_USER")
-INFLUXDB_PASSWORD = os.getenv("INFLUXDB_PASSWORD")
-INFLUXDB_DATABASE = os.getenv("INFLUXDB_DB")
-# 监控数据存储的表名，爬虫管理系统上会以task_id命名
-INFLUXDB_MEASUREMENT = "task_" + os.getenv("TASK_ID") if os.getenv("TASK_ID") else None
-# 打点监控其他参数，若这里也配置了influxdb的参数, 则会覆盖外面的配置
-METRICS_OTHER_ARGS = dict(retention_policy_duration="180d", emit_interval=60)
-
-############# 导入用户自定义的setting #############
-try:
-    from setting import *
-
-    # 兼容老版本的配置
-    KEEP_ALIVE = not AUTO_STOP_WHEN_SPIDER_DONE
-except:
-    pass
+from scrawlpy.utils.obj_util import inspect_all_attr
+
+
+class Settings:
+    Timeout = os.environ.get("Timeout", 3)
+
+    # redis 表名
+    # 任务表模版
+    TAB_REQUESTS = "{redis_key}:z_requests"
+    # 任务失败模板
+    TAB_FAILED_REQUESTS = "{redis_key}:z_failed_requests"
+    # 数据保存失败模板
+    TAB_FAILED_ITEMS = "{redis_key}:s_failed_items"
+    # 爬虫状态表模版
+    TAB_SPIDER_STATUS = "{redis_key}:h_spider_status"
+    # 用户池
+    TAB_USER_POOL = "{redis_key}:h_{user_type}_pool"
+
+    # MYSQL
+    MYSQL_IP = os.getenv("MYSQL_IP")
+    MYSQL_PORT = int(os.getenv("MYSQL_PORT", 3306))
+    MYSQL_DB = os.getenv("MYSQL_DB")
+    MYSQL_USER_NAME = os.getenv("MYSQL_USER_NAME")
+    MYSQL_USER_PASS = os.getenv("MYSQL_USER_PASS")
+
+    # MONGODB
+    MONGO_IP = os.getenv("MONGO_IP", "localhost")
+    MONGO_PORT = int(os.getenv("MONGO_PORT", 27017))
+    MONGO_DB = os.getenv("MONGO_DB")
+    MONGO_USER_NAME = os.getenv("MONGO_USER_NAME")
+    MONGO_USER_PASS = os.getenv("MONGO_USER_PASS")
+    MONGO_URL = os.getenv("MONGO_URL")
+
+    # REDIS
+    # ip:port 多个可写为列表或者逗号隔开 如 ip1:port1,ip2:port2 或 ["ip1:port1", "ip2:port2"]
+    REDISDB_IP_PORTS = os.getenv("REDISDB_IP_PORTS")
+    REDISDB_USER_PASS = os.getenv("REDISDB_USER_PASS")
+    REDISDB_DB = int(os.getenv("REDISDB_DB", 0))
+    # 连接redis时携带的其他参数，如ssl=True
+    REDISDB_KWARGS = dict()
+    # 适用于redis哨兵模式
+    REDISDB_SERVICE_NAME = os.getenv("REDISDB_SERVICE_NAME")
+
+    # 数据入库的pipeline，可自定义，默认MysqlPipeline
+    ITEM_PIPELINES = [
+        "feapder.pipelines.mysql_pipeline.MysqlPipeline",
+        # "feapder.pipelines.mongo_pipeline.MongoPipeline",
+        # "feapder.pipelines.console_pipeline.ConsolePipeline",
+    ]
+    EXPORT_DATA_MAX_FAILED_TIMES = 10  # 导出数据时最大的失败次数，包括保存和更新，超过这个次数报警
+    EXPORT_DATA_MAX_RETRY_TIMES = 10  # 导出数据时最大的重试次数，包括保存和更新，超过这个次数则放弃重试
+
+    # 爬虫相关
+    # COLLECTOR
+    COLLECTOR_TASK_COUNT = 32  # 每次获取任务数量，追求速度推荐32
+
+    # SPIDER
+    SPIDER_THREAD_COUNT = 1  # 爬虫并发数，追求速度推荐32
+    # 下载时间间隔 单位秒。 支持随机 如 SPIDER_SLEEP_TIME = [2, 5] 则间隔为 2~5秒之间的随机数，包含2和5
+    SPIDER_SLEEP_TIME = 0
+    SPIDER_MAX_RETRY_TIMES = 10  # 每个请求最大重试次数
+    # 是否主动执行添加 设置为False 需要手动调用start_monitor_task，适用于多进程情况下
+    SPIDER_AUTO_START_REQUESTS = True
+    KEEP_ALIVE = False  # 爬虫是否常驻
+
+    # 浏览器渲染
+    WEBDRIVER = dict(
+        pool_size=1,  # 浏览器的数量
+        load_images=True,  # 是否加载图片
+        user_agent=None,  # 字符串 或 无参函数，返回值为user_agent
+        proxy=None,  # xxx.xxx.xxx.xxx:xxxx 或 无参函数，返回值为代理地址
+        headless=False,  # 是否为无头浏览器
+        driver_type="CHROME",  # CHROME、EDGE、PHANTOMJS、FIREFOX
+        timeout=30,  # 请求超时时间
+        window_size=(1024, 800),  # 窗口大小
+        executable_path=None,  # 浏览器路径，默认为默认路径
+        render_time=0,  # 渲染时长，即打开网页等待指定时间后再获取源码
+        custom_argument=[
+            "--ignore-certificate-errors",
+            "--disable-blink-features=AutomationControlled",
+        ],  # 自定义浏览器渲染参数
+        xhr_url_regexes=None,  # 拦截xhr接口，支持正则，数组类型
+        auto_install_driver=True,  # 自动下载浏览器驱动 支持chrome 和 firefox
+        download_path=None,  # 下载文件的路径
+        use_stealth_js=False,  # 使用stealth.min.js隐藏浏览器特征
+    )
+
+    PLAYWRIGHT = dict(
+        user_agent=None,  # 字符串 或 无参函数，返回值为user_agent
+        proxy=None,  # xxx.xxx.xxx.xxx:xxxx 或 无参函数，返回值为代理地址
+        headless=False,  # 是否为无头浏览器
+        driver_type="chromium",  # chromium、firefox、webkit
+        timeout=30,  # 请求超时时间
+        window_size=(1024, 800),  # 窗口大小
+        executable_path=None,  # 浏览器路径，默认为默认路径
+        download_path=None,  # 下载文件的路径
+        render_time=0,  # 渲染时长，即打开网页等待指定时间后再获取源码
+        wait_until="networkidle",  # 等待页面加载完成的事件,可选值："commit", "domcontentloaded", "load", "networkidle"
+        use_stealth_js=False,  # 使用stealth.min.js隐藏浏览器特征
+        page_on_event_callback=None,
+        # page.on() 事件的回调 如 page_on_event_callback={"dialog": lambda dialog: dialog.accept()}
+        storage_state_path=None,  # 保存浏览器状态的路径
+        url_regexes=None,  # 拦截接口，支持正则，数组类型
+        save_all=False,  # 是否保存所有拦截的接口, 配合url_regexes使用，为False时只保存最后一次拦截的接口
+    )
+
+    # 爬虫启动时，重新抓取失败的requests
+    RETRY_FAILED_REQUESTS = False
+    # 爬虫启动时，重新入库失败的item
+    RETRY_FAILED_ITEMS = False
+    # 保存失败的request
+    SAVE_FAILED_REQUEST = True
+    # request防丢机制。（指定的REQUEST_LOST_TIMEOUT时间内request还没做完，会重新下发 重做）
+    REQUEST_LOST_TIMEOUT = 600  # 10分钟
+    # request网络请求超时时间
+    REQUEST_TIMEOUT = 22  # 等待服务器响应的超时时间，浮点数，或(connect timeout, read timeout)元组
+    # item在内存队列中最大缓存数量
+    ITEM_MAX_CACHED_COUNT = 5000
+    # item每批入库的最大数量
+    ITEM_UPLOAD_BATCH_MAX_SIZE = 1000
+    # item入库时间间隔
+    ITEM_UPLOAD_INTERVAL = 1
+    # 内存任务队列最大缓存的任务数，默认不限制；仅对AirSpider有效。
+    TASK_MAX_CACHED_SIZE = 0
+
+    # 下载缓存 利用redis缓存，但由于内存大小限制，所以建议仅供开发调试代码时使用，防止每次debug都需要网络请求
+    RESPONSE_CACHED_ENABLE = False  # 是否启用下载缓存 成本高的数据或容易变需求的数据，建议设置为True
+    RESPONSE_CACHED_EXPIRE_TIME = 3600  # 缓存时间 秒
+    RESPONSE_CACHED_USED = False  # 是否使用缓存 补采数据时可设置为True
+
+    # redis 存放item与request的根目录
+    REDIS_KEY = ""
+    # 爬虫启动时删除的key，类型: 元组/bool/string。 支持正则; 常用于清空任务队列，否则重启时会断点续爬
+    DELETE_KEYS = []
+
+    # 设置代理
+    PROXY_EXTRACT_API = None  # 代理提取API ，返回的代理分割符为\r\n
+    PROXY_ENABLE = True
+    PROXY_MAX_FAILED_TIMES = 5  # 代理最大失败次数，超过则不使用，自动删除
+    PROXY_POOL = "feapder.network.proxy_pool.ProxyPool"  # 代理池
+
+    # 随机headers
+    RANDOM_HEADERS = True
+    # UserAgent类型 支持 'chrome', 'opera', 'firefox', 'internetexplorer', 'safari'，'mobile' 若不指定则随机类型
+    USER_AGENT_TYPE = "chrome"
+    # 默认使用的浏览器头
+    DEFAULT_USERAGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.103 Safari/537.36"
+    # requests 使用session
+    USE_SESSION = False
+
+    # 下载
+    DOWNLOADER = "feapder.network.downloader.RequestsDownloader"  # 请求下载器
+    SESSION_DOWNLOADER = "feapder.network.downloader.RequestsSessionDownloader"
+    RENDER_DOWNLOADER = "feapder.network.downloader.SeleniumDownloader"  # 渲染下载器
+    # RENDER_DOWNLOADER="feapder.network.downloader.PlaywrightDownloader"
+    MAKE_ABSOLUTE_LINKS = True  # 自动转成绝对连接
+
+    # 去重
+    ITEM_FILTER_ENABLE = False  # item 去重
+    ITEM_FILTER_SETTING = dict(
+        filter_type=1  # 永久去重（BloomFilter） = 1 、内存去重（MemoryFilter） = 2、 临时去重（ExpireFilter）= 3、轻量去重（LiteFilter）= 4
+    )
+    REQUEST_FILTER_ENABLE = False  # request 去重
+    REQUEST_FILTER_SETTING = dict(
+        filter_type=3,  # 永久去重（BloomFilter） = 1 、内存去重（MemoryFilter） = 2、 临时去重（ExpireFilter）= 3、 轻量去重（LiteFilter）= 4
+        expire_time=2592000,  # 过期时间1个月
+    )
+
+    # 报警 支持钉钉、飞书、企业微信、邮件
+    # 钉钉报警
+    DINGDING_WARNING_URL = ""  # 钉钉机器人api
+    DINGDING_WARNING_PHONE = ""  # 被@的群成员手机号，支持列表，可指定多个。
+    DINGDING_WARNING_USER_ID = ""  # 被@的群成员userId，支持列表，可指定多个
+    DINGDING_WARNING_ALL = False  # 是否提示所有人， 默认为False
+    DINGDING_WARNING_SECRET = None  # 加签密钥
+    # 飞书报警
+    # https://open.feishu.cn/document/ukTMukTMukTM/ucTM5YjL3ETO24yNxkjN#e1cdee9f
+    FEISHU_WARNING_URL = ""  # 飞书机器人api
+    FEISHU_WARNING_USER = None  # 报警人 {"open_id":"ou_xxxxx", "name":"xxxx"} 或 [{"open_id":"ou_xxxxx", "name":"xxxx"}]
+    FEISHU_WARNING_ALL = False  # 是否提示所有人， 默认为False
+    # 邮件报警
+    EMAIL_SENDER = ""  # 发件人
+    EMAIL_PASSWORD = ""  # 授权码
+    EMAIL_RECEIVER = ""  # 收件人 支持列表，可指定多个
+    EMAIL_SMTPSERVER = "smtp.163.com"  # 邮件服务器 默认为163邮箱
+    # 企业微信报警
+    WECHAT_WARNING_URL = ""  # 企业微信机器人api
+    WECHAT_WARNING_PHONE = ""  # 报警人 将会在群内@此人, 支持列表，可指定多人
+    WECHAT_WARNING_ALL = False  # 是否提示所有人， 默认为False
+    # 时间间隔
+    WARNING_INTERVAL = 3600  # 相同报警的报警时间间隔，防止刷屏; 0表示不去重
+    WARNING_LEVEL = "DEBUG"  # 报警级别， DEBUG / INFO / ERROR
+    WARNING_FAILED_COUNT = 1000  # 任务失败数 超过WARNING_FAILED_COUNT则报警
+    WARNING_CHECK_TASK_COUNT_INTERVAL = 1200  # 检查已做任务数量的时间间隔，若两次时间间隔之间，任务数无变化则报警
+
+    # 日志
+    LOG_NAME = os.path.basename(os.getcwd())
+    LOG_PATH = "log/%s.log" % LOG_NAME  # log存储路径
+    LOG_LEVEL = os.getenv("LOG_LEVEL", "DEBUG")  # 日志级别
+    LOG_COLOR = True  # 是否带有颜色
+    LOG_IS_WRITE_TO_CONSOLE = True  # 是否打印到控制台
+    LOG_IS_WRITE_TO_FILE = False  # 是否写文件
+    LOG_MODE = "w"  # 写文件的模式
+    LOG_MAX_BYTES = 10 * 1024 * 1024  # 每个日志文件的最大字节数
+    LOG_BACKUP_COUNT = 20  # 日志文件保留数量
+    LOG_ENCODING = "utf8"  # 日志文件编码
+    # 是否详细的打印异常
+    PRINT_EXCEPTION_DETAILS = True
+    # 设置不带颜色的日志格式
+    LOG_FORMAT = "%(threadName)s|%(asctime)s|%(filename)s|%(funcName)s|line:%(lineno)d|%(levelname)s| %(message)s"
+    # 设置带有颜色的日志格式
+    os.environ["LOGURU_FORMAT"] = (
+        "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
+        "<level>{level: <8}</level> | "
+        "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>line:{line}</cyan> | <level>{message}</level>"
+    )
+    OTHERS_LOG_LEVAL = "ERROR"  # 第三方库的log等级
+
+    # 打点监控 influxdb 配置
+    INFLUXDB_HOST = os.getenv("INFLUXDB_HOST", "localhost")
+    INFLUXDB_PORT = int(os.getenv("INFLUXDB_PORT", 8086))
+    INFLUXDB_UDP_PORT = int(os.getenv("INFLUXDB_UDP_PORT", 8089))
+    INFLUXDB_USER = os.getenv("INFLUXDB_USER")
+    INFLUXDB_PASSWORD = os.getenv("INFLUXDB_PASSWORD")
+    INFLUXDB_DATABASE = os.getenv("INFLUXDB_DB")
+    # 监控数据存储的表名，爬虫管理系统上会以task_id命名
+    INFLUXDB_MEASUREMENT = "task_" + os.getenv("TASK_ID") if os.getenv("TASK_ID") else None
+    # 打点监控其他参数，若这里也配置了influxdb的参数, 则会覆盖外面的配置
+    METRICS_OTHER_ARGS = dict(retention_policy_duration="180d", emit_interval=60)
+
+    def __str__(self):
+        return f"{self.__class__.__name__} {json.dumps(inspect_all_attr(self), indent=4)}"
+
+    def __repr__(self):
+        return self.__str__()
+
+    def to_dict(self):
+        return inspect_all_attr(self)
```

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/air_spider_template.tmpl` & `scrawlpy-0.0.7/scrawlpy/templates/air_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/batch_spider_template.tmpl` & `scrawlpy-0.0.7/scrawlpy/templates/batch_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/project_template/CHECK_DATA.md` & `scrawlpy-0.0.7/scrawlpy/templates/project_template/CHECK_DATA.md`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/project_template/main.py` & `scrawlpy-0.0.7/scrawlpy/templates/project_template/main.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/project_template/setting.py` & `scrawlpy-0.0.7/scrawlpy/templates/project_template/setting.py`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/spider_template.tmpl` & `scrawlpy-0.0.7/scrawlpy/templates/spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy/templates/task_spider_template.tmpl` & `scrawlpy-0.0.7/scrawlpy/templates/task_spider_template.tmpl`

 * *Files identical despite different names*

### Comparing `scrawlpy-0.0.6/scrawlpy.egg-info/PKG-INFO` & `scrawlpy-0.0.7/scrawlpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrawlpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: scrawlpy是一款python爬虫框架
 Author: Jayden
 Author-email: jayden@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrawlpy-0.0.6/scrawlpy.egg-info/SOURCES.txt` & `scrawlpy-0.0.7/scrawlpy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,40 +13,59 @@
 scrawlpy.egg-info/requires.txt
 scrawlpy.egg-info/top_level.txt
 scrawlpy/commands/__init__.py
 scrawlpy/commands/cmdline.py
 scrawlpy/commands/create_builder.py
 scrawlpy/commands/retry.py
 scrawlpy/commands/shell.py
+scrawlpy/commands/spider.py
 scrawlpy/commands/zip.py
 scrawlpy/commands/create/__init__.py
 scrawlpy/commands/create/create_cookies.py
 scrawlpy/commands/create/create_init.py
 scrawlpy/commands/create/create_item.py
 scrawlpy/commands/create/create_json.py
 scrawlpy/commands/create/create_params.py
 scrawlpy/commands/create/create_project.py
 scrawlpy/commands/create/create_setting.py
 scrawlpy/commands/create/create_spider.py
 scrawlpy/commands/create/create_table.py
 scrawlpy/core/__init__.py
 scrawlpy/core/base_spider.py
 scrawlpy/core/spiders/__init__.py
+scrawlpy/core/spiders/airspider.py
 scrawlpy/core/spiders/spider.py
 scrawlpy/http/__init__.py
 scrawlpy/http/request.py
+scrawlpy/storage/__init__.py
+scrawlpy/storage/memorydb.py
 scrawlpy/templates/air_spider_template.tmpl
 scrawlpy/templates/batch_spider_template.tmpl
 scrawlpy/templates/item_template.tmpl
 scrawlpy/templates/spider_template.tmpl
 scrawlpy/templates/task_spider_template.tmpl
 scrawlpy/templates/update_item_template.tmpl
 scrawlpy/templates/project_template/CHECK_DATA.md
 scrawlpy/templates/project_template/README.md
 scrawlpy/templates/project_template/main.py
 scrawlpy/templates/project_template/setting.py
 scrawlpy/templates/project_template/items/__init__.py
 scrawlpy/templates/project_template/spiders/__init__.py
+scrawlpy/utils/__init__.py
+scrawlpy/utils/concurrent_util.py
+scrawlpy/utils/logger_util.py
+scrawlpy/utils/obj_util.py
+scrawlpy/utils/tail_thread.py
 scripts/__init__.py
 test/__init__.py
+test/func_demo.py
+test/main.py
+test/func_timeout_demo/__init__.py
+test/func_timeout_demo/demo.py
+test/func_timeout_demo/test2.py
+test/func_timeout_demo/test3.py
 test/spiders/__init__.py
-test/spiders/spider.py
+test/spiders/airspider.py
+test/spiders/settings/__init__.py
+test/spiders/settings/airspider_settings.py
+test/spiders/spiders/__init__.py
+test/spiders/spiders/airspider.py
```

### Comparing `scrawlpy-0.0.6/setup.py` & `scrawlpy-0.0.7/setup.py`

 * *Files identical despite different names*

