# Comparing `tmp/migration_db-1.0.3.tar.gz` & `tmp/migration_db-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migration_db-1.0.3.tar", last modified: Tue Apr 30 08:11:39 2024, max compression
+gzip compressed data, was "migration_db-1.0.4.tar", last modified: Tue Apr 30 08:59:18 2024, max compression
```

## Comparing `migration_db-1.0.3.tar` & `migration_db-1.0.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:39.066475 migration_db-1.0.3/
--rw-rw-rw-   0        0        0     1091 2023-02-14 02:04:04.000000 migration_db-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       42 2024-04-30 06:49:17.000000 migration_db-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      330 2024-04-30 08:11:39.064477 migration_db-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-04-30 07:55:39.000000 migration_db-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.723386 migration_db-1.0.3/migration_db/
--rw-rw-rw-   0        0        0      172 2024-04-30 08:11:32.000000 migration_db-1.0.3/migration_db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.757298 migration_db-1.0.3/migration_db/common/
--rw-rw-rw-   0        0        0      564 2023-07-14 03:27:20.000000 migration_db-1.0.3/migration_db/common/calc_time.py
--rw-rw-rw-   0        0        0     2375 2023-07-31 07:46:04.000000 migration_db-1.0.3/migration_db/common/compare_two_dict.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.765278 migration_db-1.0.3/migration_db/common/conf/
--rw-rw-rw-   0        0        0     1212 2023-02-23 08:16:11.000000 migration_db-1.0.3/migration_db/common/conf/config.py
--rw-rw-rw-   0        0        0      490 2023-11-20 10:13:23.000000 migration_db-1.0.3/migration_db/common/conf/constant.py
--rw-rw-rw-   0        0        0     1782 2023-07-17 03:00:20.000000 migration_db-1.0.3/migration_db/common/conf/data_source_route.py
--rw-rw-rw-   0        0        0     1942 2023-07-31 03:14:53.000000 migration_db-1.0.3/migration_db/common/conf/datasource.json
--rw-rw-rw-   0        0        0     1242 2023-02-23 08:15:20.000000 migration_db-1.0.3/migration_db/common/conf/study_info_route.py
--rw-rw-rw-   0        0        0     1368 2024-01-17 08:08:39.000000 migration_db-1.0.3/migration_db/common/constant.py
--rw-rw-rw-   0        0        0     1176 2024-02-19 06:49:07.000000 migration_db-1.0.3/migration_db/common/create_folder.py
--rw-rw-rw-   0        0        0      875 2024-04-11 10:28:33.000000 migration_db-1.0.3/migration_db/common/database.py
--rw-rw-rw-   0        0        0     1179 2023-05-31 08:12:05.000000 migration_db-1.0.3/migration_db/common/file.py
--rw-rw-rw-   0        0        0      581 2023-12-14 10:16:04.000000 migration_db-1.0.3/migration_db/common/format_time.py
--rw-rw-rw-   0        0        0     2162 2024-02-05 10:15:53.000000 migration_db-1.0.3/migration_db/common/handle_git.py
--rw-rw-rw-   0        0        0      477 2020-12-24 07:05:06.000000 migration_db-1.0.3/migration_db/common/handle_remove_read_only.py
--rw-rw-rw-   0        0        0     4705 2024-01-17 08:26:53.000000 migration_db-1.0.3/migration_db/common/handle_str.py
--rw-rw-rw-   0        0        0     1503 2023-11-07 08:02:22.000000 migration_db-1.0.3/migration_db/common/lib.py
--rw-rw-rw-   0        0        0     2713 2024-02-19 06:06:43.000000 migration_db-1.0.3/migration_db/common/log.py
--rw-rw-rw-   0        0        0     7702 2023-12-15 09:02:25.000000 migration_db-1.0.3/migration_db/common/my_db.py
--rw-rw-rw-   0        0        0     2055 2024-04-08 03:43:19.000000 migration_db-1.0.3/migration_db/common/path.py
--rw-rw-rw-   0        0        0     2047 2023-07-31 09:19:01.000000 migration_db-1.0.3/migration_db/common/read_file.py
--rw-rw-rw-   0        0        0      408 2021-08-03 02:42:25.000000 migration_db-1.0.3/migration_db/common/template_parse.py
--rw-rw-rw-   0        0        0      951 2024-02-19 06:42:00.000000 migration_db-1.0.3/migration_db/common/write_file.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.710421 migration_db-1.0.3/migration_db/migration/
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.857067 migration_db-1.0.3/migration_db/migration/core/
--rw-rw-rw-   0        0        0    12633 2024-02-27 02:57:11.000000 migration_db-1.0.3/migration_db/migration/core/_migration.py
--rw-rw-rw-   0        0        0     1990 2024-01-15 08:02:29.000000 migration_db-1.0.3/migration_db/migration/core/base.py
--rw-rw-rw-   0        0        0    16811 2024-02-19 07:29:21.000000 migration_db-1.0.3/migration_db/migration/core/build_update_sql.py
--rw-rw-rw-   0        0        0     5672 2024-04-30 07:52:21.000000 migration_db-1.0.3/migration_db/migration/core/execute_script.py
--rw-rw-rw-   0        0        0      754 2023-05-06 06:41:30.000000 migration_db-1.0.3/migration_db/migration/core/handle_external_condition_mapping_data.py
--rw-rw-rw-   0        0        0     1339 2023-03-24 13:30:58.000000 migration_db-1.0.3/migration_db/migration/core/handle_procedures.py
--rw-rw-rw-   0        0        0     1840 2023-03-28 07:10:57.000000 migration_db-1.0.3/migration_db/migration/core/handle_special_field.py
--rw-rw-rw-   0        0        0     1711 2022-08-30 02:56:27.000000 migration_db-1.0.3/migration_db/migration/core/handle_table_action.py
--rw-rw-rw-   0        0        0    10110 2024-04-23 08:01:53.000000 migration_db-1.0.3/migration_db/migration/core/incremental_sql.py
--rw-rw-rw-   0        0        0     5211 2023-09-21 04:39:01.000000 migration_db-1.0.3/migration_db/migration/core/match_ids.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.877013 migration_db-1.0.3/migration_db/migration/core/models/
--rw-rw-rw-   0        0        0     1115 2021-03-16 05:40:58.000000 migration_db-1.0.3/migration_db/migration/core/models/config.py
--rw-rw-rw-   0        0        0      709 2023-09-08 02:39:23.000000 migration_db-1.0.3/migration_db/migration/core/models/file_detail.py
--rw-rw-rw-   0        0        0     2436 2023-03-24 13:00:15.000000 migration_db-1.0.3/migration_db/migration/core/models/table_detail.py
--rw-rw-rw-   0        0        0     1574 2024-02-19 07:27:11.000000 migration_db-1.0.3/migration_db/migration/core/redis_biz.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.881966 migration_db-1.0.3/migration_db/migration/core/split_sql/
--rw-rw-rw-   0        0        0     5463 2023-09-25 08:55:57.000000 migration_db-1.0.3/migration_db/migration/core/split_sql/split_sql.py
--rw-rw-rw-   0        0        0     2048 2024-01-09 08:39:16.000000 migration_db-1.0.3/migration_db/migration/core/switch_data_source.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.899980 migration_db-1.0.3/migration_db/migration/db/
--rw-rw-rw-   0        0        0     8020 2024-01-15 07:44:36.000000 migration_db-1.0.3/migration_db/migration/db/admin_db.py
--rw-rw-rw-   0        0        0     2373 2024-02-27 06:56:06.000000 migration_db-1.0.3/migration_db/migration/db/base_db.py
--rw-rw-rw-   0        0        0      460 2023-03-02 01:37:13.000000 migration_db-1.0.3/migration_db/migration/db/design_db.py
--rw-rw-rw-   0        0        0     1260 2023-03-14 09:20:46.000000 migration_db-1.0.3/migration_db/migration/db/edc_db.py
--rw-rw-rw-   0        0        0      693 2023-09-21 01:31:22.000000 migration_db-1.0.3/migration_db/migration/db/iwrs_db.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.904902 migration_db-1.0.3/migration_db/migration/docs/
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.915881 migration_db-1.0.3/migration_db/migration/docs/common_sql/
--rw-rw-rw-   0        0        0     2370 2023-03-27 01:40:59.000000 migration_db-1.0.3/migration_db/migration/docs/common_sql/create_procedure.sql
--rw-rw-rw-   0        0        0      128 2023-03-30 06:10:59.000000 migration_db-1.0.3/migration_db/migration/docs/common_sql/drop_procedure.sql
--rw-rw-rw-   0        0        0      871 2022-05-30 09:06:22.000000 migration_db-1.0.3/migration_db/migration/docs/common_sql/eclinical_schema_history.sql
--rw-rw-rw-   0        0        0    29341 2024-04-30 08:08:27.000000 migration_db-1.0.3/migration_db/migration/docs/config_info.json
--rw-rw-rw-   0        0        0      982 2023-07-31 03:14:53.000000 migration_db-1.0.3/migration_db/migration/docs/redis_detail.json
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.934823 migration_db-1.0.3/migration_db/migration/docs/template/
--rw-rw-rw-   0        0        0      213 2023-06-07 10:37:29.000000 migration_db-1.0.3/migration_db/migration/docs/template/mysql-shell-dump.j2
--rw-rw-rw-   0        0        0      219 2023-06-07 10:37:27.000000 migration_db-1.0.3/migration_db/migration/docs/template/mysql-shell-load-dump.j2
--rw-rw-rw-   0        0        0      429 2022-06-26 13:22:39.000000 migration_db-1.0.3/migration_db/migration/docs/template/parse.py
--rw-rw-rw-   0        0        0     1146 2023-03-24 13:00:15.000000 migration_db-1.0.3/migration_db/migration/docs/template/update_id_template.j2
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:38.962759 migration_db-1.0.3/migration_db/migration/helper/
--rw-rw-rw-   0        0        0     2388 2024-04-30 07:52:21.000000 migration_db-1.0.3/migration_db/migration/helper/run_edc.py
--rw-rw-rw-   0        0        0     2661 2024-04-30 07:52:21.000000 migration_db-1.0.3/migration_db/migration/helper/run_pv.py
--rw-rw-rw-   0        0        0    11665 2024-04-30 07:52:21.000000 migration_db-1.0.3/migration_db/migration/helper/run_split_sql.py
--rw-rw-rw-   0        0        0     1407 2024-04-30 07:52:21.000000 migration_db-1.0.3/migration_db/migration/helper/run_table_action.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:39.007629 migration_db-1.0.3/migration_db/migration/lib/
--rw-rw-rw-   0        0        0     2282 2020-12-23 14:18:08.000000 migration_db-1.0.3/migration_db/migration/lib/compareTwoDict.py
--rw-rw-rw-   0        0        0     2422 2024-01-18 08:52:06.000000 migration_db-1.0.3/migration_db/migration/lib/constant.py
--rw-rw-rw-   0        0        0     2282 2024-02-19 07:26:01.000000 migration_db-1.0.3/migration_db/migration/lib/handle_redis.py
--rw-rw-rw-   0        0        0      602 2023-08-07 06:38:30.000000 migration_db-1.0.3/migration_db/migration/lib/handle_str.py
--rw-rw-rw-   0        0        0     5757 2024-02-19 07:24:41.000000 migration_db-1.0.3/migration_db/migration/lib/my_db.py
--rw-rw-rw-   0        0        0     2384 2021-08-07 06:57:33.000000 migration_db-1.0.3/migration_db/migration/lib/my_excel.py
--rw-rw-rw-   0        0        0     5867 2024-02-05 12:03:52.000000 migration_db-1.0.3/migration_db/migration/lib/mysql_connector.py
--rw-rw-rw-   0        0        0     3277 2024-02-19 07:29:21.000000 migration_db-1.0.3/migration_db/migration/lib/mysql_shell.py
--rw-rw-rw-   0        0        0     1531 2023-10-29 07:05:46.000000 migration_db-1.0.3/migration_db/migration/lib/mysql_task.py
--rw-rw-rw-   0        0        0     1506 2024-04-30 08:10:52.000000 migration_db-1.0.3/migration_db/migration/lib/path.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:11:39.042535 migration_db-1.0.3/migration_db.egg-info/
--rw-rw-rw-   0        0        0      330 2024-04-30 08:11:38.000000 migration_db-1.0.3/migration_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5546 2024-04-30 08:11:38.000000 migration_db-1.0.3/migration_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:11:38.000000 migration_db-1.0.3/migration_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-30 08:11:38.000000 migration_db-1.0.3/migration_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 08:11:38.000000 migration_db-1.0.3/migration_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 08:11:39.067468 migration_db-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      850 2024-04-30 07:55:10.000000 migration_db-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.494130 migration_db-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-14 02:04:04.000000 migration_db-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:49:17.000000 migration_db-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      330 2024-04-30 08:59:18.493133 migration_db-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-30 07:55:39.000000 migration_db-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.285096 migration_db-1.0.4/migration_db/
+-rw-rw-rw-   0        0        0      172 2024-04-30 08:59:08.000000 migration_db-1.0.4/migration_db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.328974 migration_db-1.0.4/migration_db/common/
+-rw-rw-rw-   0        0        0      564 2023-07-14 03:27:20.000000 migration_db-1.0.4/migration_db/common/calc_time.py
+-rw-rw-rw-   0        0        0     2375 2023-07-31 07:46:04.000000 migration_db-1.0.4/migration_db/common/compare_two_dict.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.343938 migration_db-1.0.4/migration_db/common/conf/
+-rw-rw-rw-   0        0        0     1212 2023-02-23 08:16:11.000000 migration_db-1.0.4/migration_db/common/conf/config.py
+-rw-rw-rw-   0        0        0      490 2023-11-20 10:13:23.000000 migration_db-1.0.4/migration_db/common/conf/constant.py
+-rw-rw-rw-   0        0        0     1782 2023-07-17 03:00:20.000000 migration_db-1.0.4/migration_db/common/conf/data_source_route.py
+-rw-rw-rw-   0        0        0     1942 2023-07-31 03:14:53.000000 migration_db-1.0.4/migration_db/common/conf/datasource.json
+-rw-rw-rw-   0        0        0     1242 2023-02-23 08:15:20.000000 migration_db-1.0.4/migration_db/common/conf/study_info_route.py
+-rw-rw-rw-   0        0        0     1368 2024-01-17 08:08:39.000000 migration_db-1.0.4/migration_db/common/constant.py
+-rw-rw-rw-   0        0        0     1176 2024-02-19 06:49:07.000000 migration_db-1.0.4/migration_db/common/create_folder.py
+-rw-rw-rw-   0        0        0      875 2024-04-11 10:28:33.000000 migration_db-1.0.4/migration_db/common/database.py
+-rw-rw-rw-   0        0        0     1179 2023-05-31 08:12:05.000000 migration_db-1.0.4/migration_db/common/file.py
+-rw-rw-rw-   0        0        0      581 2023-12-14 10:16:04.000000 migration_db-1.0.4/migration_db/common/format_time.py
+-rw-rw-rw-   0        0        0     2162 2024-02-05 10:15:53.000000 migration_db-1.0.4/migration_db/common/handle_git.py
+-rw-rw-rw-   0        0        0      477 2020-12-24 07:05:06.000000 migration_db-1.0.4/migration_db/common/handle_remove_read_only.py
+-rw-rw-rw-   0        0        0     4705 2024-01-17 08:26:53.000000 migration_db-1.0.4/migration_db/common/handle_str.py
+-rw-rw-rw-   0        0        0     1503 2023-11-07 08:02:22.000000 migration_db-1.0.4/migration_db/common/lib.py
+-rw-rw-rw-   0        0        0     2713 2024-02-19 06:06:43.000000 migration_db-1.0.4/migration_db/common/log.py
+-rw-rw-rw-   0        0        0     7702 2023-12-15 09:02:25.000000 migration_db-1.0.4/migration_db/common/my_db.py
+-rw-rw-rw-   0        0        0     2055 2024-04-08 03:43:19.000000 migration_db-1.0.4/migration_db/common/path.py
+-rw-rw-rw-   0        0        0     2047 2023-07-31 09:19:01.000000 migration_db-1.0.4/migration_db/common/read_file.py
+-rw-rw-rw-   0        0        0      408 2021-08-03 02:42:25.000000 migration_db-1.0.4/migration_db/common/template_parse.py
+-rw-rw-rw-   0        0        0      951 2024-02-19 06:42:00.000000 migration_db-1.0.4/migration_db/common/write_file.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.277112 migration_db-1.0.4/migration_db/migration/
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.372855 migration_db-1.0.4/migration_db/migration/core/
+-rw-rw-rw-   0        0        0    12633 2024-02-27 02:57:11.000000 migration_db-1.0.4/migration_db/migration/core/_migration.py
+-rw-rw-rw-   0        0        0     1990 2024-01-15 08:02:29.000000 migration_db-1.0.4/migration_db/migration/core/base.py
+-rw-rw-rw-   0        0        0    16811 2024-02-19 07:29:21.000000 migration_db-1.0.4/migration_db/migration/core/build_update_sql.py
+-rw-rw-rw-   0        0        0     5672 2024-04-30 07:52:21.000000 migration_db-1.0.4/migration_db/migration/core/execute_script.py
+-rw-rw-rw-   0        0        0      754 2023-05-06 06:41:30.000000 migration_db-1.0.4/migration_db/migration/core/handle_external_condition_mapping_data.py
+-rw-rw-rw-   0        0        0     1339 2023-03-24 13:30:58.000000 migration_db-1.0.4/migration_db/migration/core/handle_procedures.py
+-rw-rw-rw-   0        0        0     1840 2023-03-28 07:10:57.000000 migration_db-1.0.4/migration_db/migration/core/handle_special_field.py
+-rw-rw-rw-   0        0        0     1711 2022-08-30 02:56:27.000000 migration_db-1.0.4/migration_db/migration/core/handle_table_action.py
+-rw-rw-rw-   0        0        0    10110 2024-04-23 08:01:53.000000 migration_db-1.0.4/migration_db/migration/core/incremental_sql.py
+-rw-rw-rw-   0        0        0     5211 2023-09-21 04:39:01.000000 migration_db-1.0.4/migration_db/migration/core/match_ids.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.377843 migration_db-1.0.4/migration_db/migration/core/models/
+-rw-rw-rw-   0        0        0     1115 2021-03-16 05:40:58.000000 migration_db-1.0.4/migration_db/migration/core/models/config.py
+-rw-rw-rw-   0        0        0      709 2023-09-08 02:39:23.000000 migration_db-1.0.4/migration_db/migration/core/models/file_detail.py
+-rw-rw-rw-   0        0        0     2436 2023-03-24 13:00:15.000000 migration_db-1.0.4/migration_db/migration/core/models/table_detail.py
+-rw-rw-rw-   0        0        0     1574 2024-02-19 07:27:11.000000 migration_db-1.0.4/migration_db/migration/core/redis_biz.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.378841 migration_db-1.0.4/migration_db/migration/core/split_sql/
+-rw-rw-rw-   0        0        0     5463 2023-09-25 08:55:57.000000 migration_db-1.0.4/migration_db/migration/core/split_sql/split_sql.py
+-rw-rw-rw-   0        0        0     2048 2024-01-09 08:39:16.000000 migration_db-1.0.4/migration_db/migration/core/switch_data_source.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.394798 migration_db-1.0.4/migration_db/migration/db/
+-rw-rw-rw-   0        0        0     8020 2024-01-15 07:44:36.000000 migration_db-1.0.4/migration_db/migration/db/admin_db.py
+-rw-rw-rw-   0        0        0     2373 2024-02-27 06:56:06.000000 migration_db-1.0.4/migration_db/migration/db/base_db.py
+-rw-rw-rw-   0        0        0      460 2023-03-02 01:37:13.000000 migration_db-1.0.4/migration_db/migration/db/design_db.py
+-rw-rw-rw-   0        0        0     1260 2023-03-14 09:20:46.000000 migration_db-1.0.4/migration_db/migration/db/edc_db.py
+-rw-rw-rw-   0        0        0      693 2023-09-21 01:31:22.000000 migration_db-1.0.4/migration_db/migration/db/iwrs_db.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.399783 migration_db-1.0.4/migration_db/migration/docs/
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.408759 migration_db-1.0.4/migration_db/migration/docs/common_sql/
+-rw-rw-rw-   0        0        0     2370 2023-03-27 01:40:59.000000 migration_db-1.0.4/migration_db/migration/docs/common_sql/create_procedure.sql
+-rw-rw-rw-   0        0        0      128 2023-03-30 06:10:59.000000 migration_db-1.0.4/migration_db/migration/docs/common_sql/drop_procedure.sql
+-rw-rw-rw-   0        0        0      871 2022-05-30 09:06:22.000000 migration_db-1.0.4/migration_db/migration/docs/common_sql/eclinical_schema_history.sql
+-rw-rw-rw-   0        0        0    29341 2024-04-30 08:08:27.000000 migration_db-1.0.4/migration_db/migration/docs/config_info.json
+-rw-rw-rw-   0        0        0      982 2023-07-31 03:14:53.000000 migration_db-1.0.4/migration_db/migration/docs/redis_detail.json
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.417336 migration_db-1.0.4/migration_db/migration/docs/template/
+-rw-rw-rw-   0        0        0      213 2023-06-07 10:37:29.000000 migration_db-1.0.4/migration_db/migration/docs/template/mysql-shell-dump.j2
+-rw-rw-rw-   0        0        0      219 2023-06-07 10:37:27.000000 migration_db-1.0.4/migration_db/migration/docs/template/mysql-shell-load-dump.j2
+-rw-rw-rw-   0        0        0      429 2022-06-26 13:22:39.000000 migration_db-1.0.4/migration_db/migration/docs/template/parse.py
+-rw-rw-rw-   0        0        0     1146 2023-03-24 13:00:15.000000 migration_db-1.0.4/migration_db/migration/docs/template/update_id_template.j2
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.426312 migration_db-1.0.4/migration_db/migration/helper/
+-rw-rw-rw-   0        0        0     2388 2024-04-30 07:52:21.000000 migration_db-1.0.4/migration_db/migration/helper/run_edc.py
+-rw-rw-rw-   0        0        0     2661 2024-04-30 07:52:21.000000 migration_db-1.0.4/migration_db/migration/helper/run_pv.py
+-rw-rw-rw-   0        0        0    11665 2024-04-30 07:52:21.000000 migration_db-1.0.4/migration_db/migration/helper/run_split_sql.py
+-rw-rw-rw-   0        0        0     1407 2024-04-30 07:52:21.000000 migration_db-1.0.4/migration_db/migration/helper/run_table_action.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.447255 migration_db-1.0.4/migration_db/migration/lib/
+-rw-rw-rw-   0        0        0     2282 2020-12-23 14:18:08.000000 migration_db-1.0.4/migration_db/migration/lib/compareTwoDict.py
+-rw-rw-rw-   0        0        0     2422 2024-01-18 08:52:06.000000 migration_db-1.0.4/migration_db/migration/lib/constant.py
+-rw-rw-rw-   0        0        0     2282 2024-02-19 07:26:01.000000 migration_db-1.0.4/migration_db/migration/lib/handle_redis.py
+-rw-rw-rw-   0        0        0      602 2023-08-07 06:38:30.000000 migration_db-1.0.4/migration_db/migration/lib/handle_str.py
+-rw-rw-rw-   0        0        0     5757 2024-02-19 07:24:41.000000 migration_db-1.0.4/migration_db/migration/lib/my_db.py
+-rw-rw-rw-   0        0        0     2384 2021-08-07 06:57:33.000000 migration_db-1.0.4/migration_db/migration/lib/my_excel.py
+-rw-rw-rw-   0        0        0     5867 2024-02-05 12:03:52.000000 migration_db-1.0.4/migration_db/migration/lib/mysql_connector.py
+-rw-rw-rw-   0        0        0     3277 2024-02-19 07:29:21.000000 migration_db-1.0.4/migration_db/migration/lib/mysql_shell.py
+-rw-rw-rw-   0        0        0     1531 2023-10-29 07:05:46.000000 migration_db-1.0.4/migration_db/migration/lib/mysql_task.py
+-rw-rw-rw-   0        0        0     1506 2024-04-30 08:10:52.000000 migration_db-1.0.4/migration_db/migration/lib/path.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:59:18.469197 migration_db-1.0.4/migration_db.egg-info/
+-rw-rw-rw-   0        0        0      330 2024-04-30 08:59:18.000000 migration_db-1.0.4/migration_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6042 2024-04-30 08:59:18.000000 migration_db-1.0.4/migration_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 08:59:18.000000 migration_db-1.0.4/migration_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-04-30 08:59:18.000000 migration_db-1.0.4/migration_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 08:59:18.000000 migration_db-1.0.4/migration_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 08:59:18.494130 migration_db-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      979 2024-04-30 08:58:50.000000 migration_db-1.0.4/setup.py
```

### Comparing `migration_db-1.0.3/LICENSE` & `migration_db-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/calc_time.py` & `migration_db-1.0.4/migration_db/common/calc_time.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/compare_two_dict.py` & `migration_db-1.0.4/migration_db/common/compare_two_dict.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/conf/config.py` & `migration_db-1.0.4/migration_db/common/conf/config.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/conf/data_source_route.py` & `migration_db-1.0.4/migration_db/common/conf/data_source_route.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/conf/datasource.json` & `migration_db-1.0.4/migration_db/common/conf/datasource.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/conf/study_info_route.py` & `migration_db-1.0.4/migration_db/common/conf/study_info_route.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/constant.py` & `migration_db-1.0.4/migration_db/common/constant.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/create_folder.py` & `migration_db-1.0.4/migration_db/common/create_folder.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/database.py` & `migration_db-1.0.4/migration_db/common/database.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/file.py` & `migration_db-1.0.4/migration_db/common/file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/format_time.py` & `migration_db-1.0.4/migration_db/common/format_time.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/handle_git.py` & `migration_db-1.0.4/migration_db/common/handle_git.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/handle_str.py` & `migration_db-1.0.4/migration_db/common/handle_str.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/lib.py` & `migration_db-1.0.4/migration_db/common/lib.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/log.py` & `migration_db-1.0.4/migration_db/common/log.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/my_db.py` & `migration_db-1.0.4/migration_db/common/my_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/path.py` & `migration_db-1.0.4/migration_db/common/path.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/read_file.py` & `migration_db-1.0.4/migration_db/common/read_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/common/write_file.py` & `migration_db-1.0.4/migration_db/common/write_file.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/_migration.py` & `migration_db-1.0.4/migration_db/migration/core/_migration.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/base.py` & `migration_db-1.0.4/migration_db/migration/core/base.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/build_update_sql.py` & `migration_db-1.0.4/migration_db/migration/core/build_update_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/execute_script.py` & `migration_db-1.0.4/migration_db/migration/core/execute_script.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/handle_external_condition_mapping_data.py` & `migration_db-1.0.4/migration_db/migration/core/handle_external_condition_mapping_data.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/handle_procedures.py` & `migration_db-1.0.4/migration_db/migration/core/handle_procedures.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/handle_special_field.py` & `migration_db-1.0.4/migration_db/migration/core/handle_special_field.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/handle_table_action.py` & `migration_db-1.0.4/migration_db/migration/core/handle_table_action.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/incremental_sql.py` & `migration_db-1.0.4/migration_db/migration/core/incremental_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/match_ids.py` & `migration_db-1.0.4/migration_db/migration/core/match_ids.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/models/config.py` & `migration_db-1.0.4/migration_db/migration/core/models/config.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/models/file_detail.py` & `migration_db-1.0.4/migration_db/migration/core/models/file_detail.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/models/table_detail.py` & `migration_db-1.0.4/migration_db/migration/core/models/table_detail.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/redis_biz.py` & `migration_db-1.0.4/migration_db/migration/core/redis_biz.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/split_sql/split_sql.py` & `migration_db-1.0.4/migration_db/migration/core/split_sql/split_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/core/switch_data_source.py` & `migration_db-1.0.4/migration_db/migration/core/switch_data_source.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/db/admin_db.py` & `migration_db-1.0.4/migration_db/migration/db/admin_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/db/base_db.py` & `migration_db-1.0.4/migration_db/migration/db/base_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/db/edc_db.py` & `migration_db-1.0.4/migration_db/migration/db/edc_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/db/iwrs_db.py` & `migration_db-1.0.4/migration_db/migration/db/iwrs_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/docs/common_sql/create_procedure.sql` & `migration_db-1.0.4/migration_db/migration/docs/common_sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/docs/common_sql/eclinical_schema_history.sql` & `migration_db-1.0.4/migration_db/migration/docs/common_sql/eclinical_schema_history.sql`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/docs/config_info.json` & `migration_db-1.0.4/migration_db/migration/docs/config_info.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/docs/redis_detail.json` & `migration_db-1.0.4/migration_db/migration/docs/redis_detail.json`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/docs/template/update_id_template.j2` & `migration_db-1.0.4/migration_db/migration/docs/template/update_id_template.j2`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/helper/run_edc.py` & `migration_db-1.0.4/migration_db/migration/helper/run_edc.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/helper/run_pv.py` & `migration_db-1.0.4/migration_db/migration/helper/run_pv.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/helper/run_split_sql.py` & `migration_db-1.0.4/migration_db/migration/helper/run_split_sql.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/helper/run_table_action.py` & `migration_db-1.0.4/migration_db/migration/helper/run_table_action.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/compareTwoDict.py` & `migration_db-1.0.4/migration_db/migration/lib/compareTwoDict.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/constant.py` & `migration_db-1.0.4/migration_db/migration/lib/constant.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/handle_redis.py` & `migration_db-1.0.4/migration_db/migration/lib/handle_redis.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/handle_str.py` & `migration_db-1.0.4/migration_db/migration/lib/handle_str.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/my_db.py` & `migration_db-1.0.4/migration_db/migration/lib/my_db.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/my_excel.py` & `migration_db-1.0.4/migration_db/migration/lib/my_excel.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/mysql_connector.py` & `migration_db-1.0.4/migration_db/migration/lib/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/mysql_shell.py` & `migration_db-1.0.4/migration_db/migration/lib/mysql_shell.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/mysql_task.py` & `migration_db-1.0.4/migration_db/migration/lib/mysql_task.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db/migration/lib/path.py` & `migration_db-1.0.4/migration_db/migration/lib/path.py`

 * *Files identical despite different names*

### Comparing `migration_db-1.0.3/migration_db.egg-info/SOURCES.txt` & `migration_db-1.0.4/migration_db.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 migration_db/common/path.py
 migration_db/common/read_file.py
 migration_db/common/template_parse.py
 migration_db/common/write_file.py
 migration_db/common/conf/config.py
 migration_db/common/conf/constant.py
 migration_db/common/conf/data_source_route.py
+migration_db/common/conf/datasource.json
 migration_db/common/conf/study_info_route.py
 migration_db/migration/core/_migration.py
 migration_db/migration/core/base.py
 migration_db/migration/core/build_update_sql.py
 migration_db/migration/core/execute_script.py
 migration_db/migration/core/handle_external_condition_mapping_data.py
 migration_db/migration/core/handle_procedures.py
@@ -114,15 +115,23 @@
 migration_db/migration/core/models/table_detail.py
 migration_db/migration/core/split_sql/split_sql.py
 migration_db/migration/db/admin_db.py
 migration_db/migration/db/base_db.py
 migration_db/migration/db/design_db.py
 migration_db/migration/db/edc_db.py
 migration_db/migration/db/iwrs_db.py
+migration_db/migration/docs/config_info.json
+migration_db/migration/docs/redis_detail.json
+migration_db/migration/docs/common_sql/create_procedure.sql
+migration_db/migration/docs/common_sql/drop_procedure.sql
+migration_db/migration/docs/common_sql/eclinical_schema_history.sql
+migration_db/migration/docs/template/mysql-shell-dump.j2
+migration_db/migration/docs/template/mysql-shell-load-dump.j2
 migration_db/migration/docs/template/parse.py
+migration_db/migration/docs/template/update_id_template.j2
 migration_db/migration/helper/run_edc.py
 migration_db/migration/helper/run_pv.py
 migration_db/migration/helper/run_split_sql.py
 migration_db/migration/helper/run_table_action.py
 migration_db/migration/lib/compareTwoDict.py
 migration_db/migration/lib/constant.py
 migration_db/migration/lib/handle_redis.py
```

### Comparing `migration_db-1.0.3/setup.py` & `migration_db-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     description="Migrate database files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://example.com",
     install_requires=[
         'lxml>=4.8.0',
         'redis>=4.3.1',
-        'jinja2',
+        'jinja2>=3.1.2',
+        'mysql-connector-python>=8.3.0',
+        'slicing>=1.0.6',
     ],
     packages=setuptools.find_namespace_packages(exclude=("test")),
     classifiers=(
         "Programming Language :: Python :: 3.9",
-    )
+    ),
+    package_data={'': ['*.sql', '*.json', "*.j2"]}
 )
```

