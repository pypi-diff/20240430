# Comparing `tmp/wedeliver_core_plus-0.1.7.tar.gz` & `tmp/wedeliver_core_plus-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-5882q60l/wedeliver_core_plus-0.1.7.tar", last modified: Tue Sep 26 13:10:47 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-yl3jaho9/wedeliver_core_plus-0.1.8.tar", last modified: Tue Apr 30 09:25:13 2024, max compression
```

## Comparing `wedeliver_core_plus-0.1.7.tar` & `wedeliver_core_plus-0.1.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/send_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-09-26 13:10:39.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-26 13:10:47.000000 wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/send_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-30 09:25:07.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 09:25:13.000000 wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/top_level.txt
```

### Comparing `wedeliver_core_plus-0.1.7/PKG-INFO` & `wedeliver_core_plus-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver_core_plus
-Version: 0.1.7
+Version: 0.1.8
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.1.7/setup.py` & `wedeliver_core_plus-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="wedeliver_core_plus",
-    version="0.1.7",
+    version="0.1.8",
     description="wedeliver_core_plus package",
     long_description="""# Markdown supported!\n\n* wedeliver core plus\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/__init__.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/app_entry.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/handle_auth.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/handle_exceptions.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/handle_response.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/app_decorators/serializer.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/base.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/base.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/acl_enum.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/get_file_url.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/get_s3_client.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/amazon/upload_file.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/atomic_transactions.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/atomic_transactions_v2.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/auth.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/config.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/database/base_model.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/database/log_model.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/enums.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/exceptions.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/fetch_relational_data.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/filters.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/format_exception.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_embedded_function.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/get_obj_value.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/get_obj_value.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_listener.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producer.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/kafka_producers/notification_center.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/kafka_producers/notification_center.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/log_config.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/micro_fetcher.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/search_function.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/security.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/security.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/service_config.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/sql.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/time.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/time.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/topics.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/topics.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/validate_mobile_number.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/validate_mobile_number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 from wedeliver_core_plus.helpers.get_country_code import get_country_code
 
 
 def validate_mobile_number(mobile, force_only=None):
+    if not mobile.isdigit():
+        return False
     mobile = mobile.replace("+", "").replace(" ", "").lstrip("0")
     if len(mobile) < 12:
         country_code = get_country_code()
         if country_code == "sa":
             dial = "966"
         elif country_code == "ps":
             dial = "970"
```

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus/helpers/validate_parameters.py` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/PKG-INFO` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver-core-plus
-Version: 0.1.7
+Version: 0.1.8
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.1.7/wedeliver_core_plus.egg-info/SOURCES.txt` & `wedeliver_core_plus-0.1.8/wedeliver_core_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

