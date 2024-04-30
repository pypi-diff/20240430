# Comparing `tmp/mns-scheduler-1.0.3.6.tar.gz` & `tmp/mns-scheduler-1.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.3.6.tar", last modified: Sun Apr 28 09:00:05 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.3.7.tar", last modified: Tue Apr 30 08:28:34 2024, max compression
```

## Comparing `mns-scheduler-1.0.3.6.tar` & `mns-scheduler-1.0.3.7.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.751563 mns-scheduler-1.0.3.6/
--rw-rw-rw-   0        0        0       62 2024-04-28 09:00:05.751563 mns-scheduler-1.0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.718597 mns-scheduler-1.0.3.6/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.720591 mns-scheduler-1.0.3.6/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.721588 mns-scheduler-1.0.3.6/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.723583 mns-scheduler-1.0.3.6/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.724615 mns-scheduler-1.0.3.6/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.725128 mns-scheduler-1.0.3.6/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.726630 mns-scheduler-1.0.3.6/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.727627 mns-scheduler-1.0.3.6/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.728625 mns-scheduler-1.0.3.6/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2459 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.728625 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.729622 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6542 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4305 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.731617 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.732614 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.734609 mns-scheduler-1.0.3.6/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.734609 mns-scheduler-1.0.3.6/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.735606 mns-scheduler-1.0.3.6/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.736603 mns-scheduler-1.0.3.6/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.737600 mns-scheduler-1.0.3.6/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.738598 mns-scheduler-1.0.3.6/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.738598 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.740593 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4503 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.740593 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.741590 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.743585 mns-scheduler-1.0.3.6/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9149 2024-04-28 08:57:27.000000 mns-scheduler-1.0.3.6/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.745579 mns-scheduler-1.0.3.6/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.3.6/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.3.6/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.3.6/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.745579 mns-scheduler-1.0.3.6/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.749569 mns-scheduler-1.0.3.6/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.750566 mns-scheduler-1.0.3.6/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    15337 2024-04-28 07:33:30.000000 mns-scheduler-1.0.3.6/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:00:05.750566 mns-scheduler-1.0.3.6/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-28 09:00:05.000000 mns-scheduler-1.0.3.6/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3247 2024-04-28 09:00:05.000000 mns-scheduler-1.0.3.6/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 09:00:05.000000 mns-scheduler-1.0.3.6/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-28 09:00:05.000000 mns-scheduler-1.0.3.6/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 09:00:05.751563 mns-scheduler-1.0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-28 08:59:30.000000 mns-scheduler-1.0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.501277 mns-scheduler-1.0.3.7/
+-rw-rw-rw-   0        0        0       62 2024-04-30 08:28:34.500280 mns-scheduler-1.0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.465373 mns-scheduler-1.0.3.7/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.467368 mns-scheduler-1.0.3.7/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.468365 mns-scheduler-1.0.3.7/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.470360 mns-scheduler-1.0.3.7/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.471357 mns-scheduler-1.0.3.7/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.472355 mns-scheduler-1.0.3.7/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.474349 mns-scheduler-1.0.3.7/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.474349 mns-scheduler-1.0.3.7/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.475347 mns-scheduler-1.0.3.7/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2459 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.476343 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.477341 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6542 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4305 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.479335 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.480333 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.482328 mns-scheduler-1.0.3.7/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.3.7/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.483325 mns-scheduler-1.0.3.7/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.483325 mns-scheduler-1.0.3.7/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.484323 mns-scheduler-1.0.3.7/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.485320 mns-scheduler-1.0.3.7/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.486317 mns-scheduler-1.0.3.7/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.486317 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.488312 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4503 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.489309 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.490307 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.492302 mns-scheduler-1.0.3.7/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9141 2024-04-29 02:30:52.000000 mns-scheduler-1.0.3.7/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.494296 mns-scheduler-1.0.3.7/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.3.7/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.3.7/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.3.7/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.495293 mns-scheduler-1.0.3.7/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.498285 mns-scheduler-1.0.3.7/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.499283 mns-scheduler-1.0.3.7/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    15385 2024-04-29 16:55:10.000000 mns-scheduler-1.0.3.7/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:28:34.500280 mns-scheduler-1.0.3.7/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-30 08:28:34.000000 mns-scheduler-1.0.3.7/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3247 2024-04-30 08:28:34.000000 mns-scheduler-1.0.3.7/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 08:28:34.000000 mns-scheduler-1.0.3.7/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-30 08:28:34.000000 mns-scheduler-1.0.3.7/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 08:28:34.501277 mns-scheduler-1.0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-30 08:28:18.000000 mns-scheduler-1.0.3.7/setup.py
```

### Comparing `mns-scheduler-1.0.3.6/README.md` & `mns-scheduler-1.0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.3.7/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.3.7/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.3.7/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.3.7/mns_scheduler/db/col_move_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,8 +105,8 @@
     os.system(cmd)
 
     logger.info("import finished:{}", col)
 
 
 # -u "username" -p "password"
 if __name__ == '__main__':
-    sync_col_move('2024-01-03')
+    sync_col_move('2024-04-30')
```

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.3.7/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.3.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.3.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.3.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         db_name_constant.REAL_TIME_QUOTES_NOW + '_' + str_day_init, 'number')
     number = number + 1
     realtime_quotes_now_create_db_index_api.create_db_index(str_day_init)
     while True:
         now_date = datetime.datetime.now()
 
         str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
-        if True or bool(date_util.is_trade_time(now_date)):
+        if bool(date_util.is_trade_time(now_date)):
             try:
                 real_time_quotes_now = east_money_stock_api.get_real_time_quotes_all_stocks()
                 real_time_quotes_now = handle_init_real_time_quotes_data(real_time_quotes_now.copy(),
                                                                          str_now_date, number)
                 save_real_time_quotes(real_time_quotes_now.copy(), now_date, db_name_constant.REAL_TIME_QUOTES_NOW,
                                       number)
                 try:
```

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,15 @@
 
 # 同步持仓
 def sync_position():
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     # 同步持仓
     if trade_date_common_service_api.is_trade_day(str_day):
+        logger.info('同步持仓任务完成')
         sync_position_api.sync_position()
 
 
 # 同步开盘啦当日精选指数行情数据
 
 def sync_kpl_best_his_quotes():
     now_date = datetime.now()
@@ -373,14 +374,14 @@
 # 更新开盘啦指数关系
 blockingScheduler.add_job(update_best_choose_plate_relation, 'cron', hour='09,18', minute='25')
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='18,22', minute='25')
 
 # 更新开盘啦指数关系
-blockingScheduler.add_job(sync_position, 'cron', hour='00,08', minute='10')
+blockingScheduler.add_job(sync_position, 'cron', hour='0,08', minute='10')
 
 print('定时任务启动成功')
 blockingScheduler.start()
 
 # if __name__ == '__main__':
 #     sync_daily_data_info()
```

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.3.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.6/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.3.7/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

