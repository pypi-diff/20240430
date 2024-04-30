# Comparing `tmp/scs_analysis-3.8.3.tar.gz` & `tmp/scs_analysis-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs_analysis-3.8.3.tar", last modified: Sun Apr 14 07:54:53 2024, max compression
+gzip compressed data, was "scs_analysis-3.8.6.tar", last modified: Tue Apr 30 09:03:10 2024, max compression
```

## Comparing `scs_analysis-3.8.3.tar` & `scs_analysis-3.8.6.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.501544 scs_analysis-3.8.3/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.3/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-14 07:54:53.501334 scs_analysis-3.8.3/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-14 07:54:47.000000 scs_analysis-3.8.3/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-14 07:54:53.501579 scs_analysis-3.8.3/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-09 15:18:11.000000 scs_analysis-3.8.3/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.473330 scs_analysis-3.8.3/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.488049 scs_analysis-3.8.3/src/scs_analysis/
--rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-14 07:54:47.000000 scs_analysis-3.8.3/src/scs_analysis/__init__.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.3/src/scs_analysis/alert.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.3/src/scs_analysis/alert_status.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/aws_byline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.3/src/scs_analysis/aws_client_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/aws_mqtt_client.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/aws_topic_history.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4190 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/aws_topic_origin.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/aws_topic_publisher.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/aws_upload_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/baseline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.3/src/scs_analysis/baseline_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.489376 scs_analysis-3.8.3/src/scs_analysis/chart/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/chart/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/chart/chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/chart/histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/chart/multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/chart/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6514 2024-03-13 09:22:10.000000 scs_analysis-3.8.3/src/scs_analysis/client_traffic.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.499316 scs_analysis-3.8.3/src/scs_analysis/cmd/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_alert.py
--rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_alert_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_topic_origin.py
--rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     4868 2024-03-13 09:22:10.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_client_traffic.py
--rw-r--r--   0 bruno      (502) admin       (80)     4739 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_email.py
--rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-r--r--   0 bruno      (502) admin       (80)     4798 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     4518 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     2372 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_join.py
--rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_device_controller.py
--rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_device_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_device_monitor_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3123 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_node.py
--rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisations.py
--rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_error.py
--rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
--rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_gas_density.py
--rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_localize.py
--rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_median.py
--rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_record.py
--rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_single_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_uds.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5450 2024-04-03 10:23:16.000000 scs_analysis-3.8.3/src/scs_analysis/cognito_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6576 2023-12-05 08:54:35.000000 scs_analysis-3.8.3/src/scs_analysis/cognito_email.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.3/src/scs_analysis/cognito_user_credentials.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8085 2024-01-08 13:19:59.000000 scs_analysis-3.8.3/src/scs_analysis/cognito_user_identity.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs_analysis-3.8.3/src/scs_analysis/cognito_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7628 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/configuration_csv.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3546 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/configuration_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3947 2023-12-05 08:54:35.000000 scs_analysis-3.8.3/src/scs_analysis/configuration_monitor_check.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4001 2023-12-01 15:39:55.000000 scs_analysis-3.8.3/src/scs_analysis/configuration_report.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/csv_collation_summary.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/csv_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/csv_join.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/csv_reader.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/csv_segmentor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.3/src/scs_analysis/csv_writer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs_analysis-3.8.3/src/scs_analysis/device_controller.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs_analysis-3.8.3/src/scs_analysis/device_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.3/src/scs_analysis/device_monitor_status.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.500782 scs_analysis-3.8.3/src/scs_analysis/handler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/handler/batch_download_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/configuration_csv_generator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5893 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/mqtt_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/sample_midpoint.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/handler/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/histo_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2127 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/localised_datetime.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/monitor_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/multi_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.3/src/scs_analysis/node.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs_analysis-3.8.3/src/scs_analysis/organisation_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs_analysis-3.8.3/src/scs_analysis/organisation_path_roots.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs_analysis-3.8.3/src/scs_analysis/organisation_user_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs_analysis-3.8.3/src/scs_analysis/organisation_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs_analysis-3.8.3/src/scs_analysis/organisations.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.3/src/scs_analysis/sample_aggregate.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_average.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_distance.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_duplicates.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_error.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_gas_concentration.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.3/src/scs_analysis/sample_gas_density.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/sample_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.3/src/scs_analysis/sample_iso_8601.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_localize.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_low_pass.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_max.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_median.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_midpoint.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_min.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/sample_noise.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_nullify.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/sample_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.3/src/scs_analysis/sample_slope.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_sort.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_stats.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.3/src/scs_analysis/sample_subset.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/sample_time_shift.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.3/src/scs_analysis/socket_receiver.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.3/src/scs_analysis/timer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.3/src/scs_analysis/uds_receiver.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:54:53.500978 scs_analysis-3.8.3/src/scs_analysis.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-14 07:54:53.000000 scs_analysis-3.8.3/src/scs_analysis.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-04-14 07:54:53.000000 scs_analysis-3.8.3/src/scs_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-14 07:54:53.000000 scs_analysis-3.8.3/src/scs_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-14 07:54:53.000000 scs_analysis-3.8.3/src/scs_analysis.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-14 07:54:53.000000 scs_analysis-3.8.3/src/scs_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.421790 scs_analysis-3.8.6/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.6/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-30 09:03:10.421579 scs_analysis-3.8.6/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-30 09:03:10.421827 scs_analysis-3.8.6/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.393802 scs_analysis-3.8.6/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.408030 scs_analysis-3.8.6/src/scs_analysis/
+-rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/__init__.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.6/src/scs_analysis/alert.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.6/src/scs_analysis/alert_status.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/aws_byline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.6/src/scs_analysis/aws_client_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/aws_mqtt_client.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/aws_topic_history.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4140 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/aws_topic_origin.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/aws_topic_publisher.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/aws_upload_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/baseline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.6/src/scs_analysis/baseline_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.409463 scs_analysis-3.8.6/src/scs_analysis/chart/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/chart/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6609 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/client_traffic.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.419559 scs_analysis-3.8.6/src/scs_analysis/cmd/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_origin.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4821 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_client_traffic.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4805 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4539 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2373 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3454 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisations.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_density.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_localize.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_uds.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5844 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6685 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_email.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_user_credentials.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8095 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_user_identity.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs_analysis-3.8.6/src/scs_analysis/cognito_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7640 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_csv.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3591 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4000 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_monitor_check.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4110 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/configuration_report.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_collation_summary.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_join.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_reader.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/csv_segmentor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.6/src/scs_analysis/csv_writer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs_analysis-3.8.6/src/scs_analysis/device_controller.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs_analysis-3.8.6/src/scs_analysis/device_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.6/src/scs_analysis/device_monitor_status.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.421068 scs_analysis-3.8.6/src/scs_analysis/handler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/handler/batch_download_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5567 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/handler/csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5903 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/handler/csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/mqtt_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/sample_midpoint.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/handler/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/histo_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2175 2024-04-30 09:02:59.000000 scs_analysis-3.8.6/src/scs_analysis/localised_datetime.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/monitor_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/multi_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.6/src/scs_analysis/node.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_path_roots.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_user_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/organisation_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs_analysis-3.8.6/src/scs_analysis/organisations.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.6/src/scs_analysis/sample_aggregate.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_average.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_distance.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_duplicates.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_error.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_gas_concentration.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.6/src/scs_analysis/sample_gas_density.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/sample_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.6/src/scs_analysis/sample_iso_8601.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_localize.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_low_pass.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_max.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_median.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_midpoint.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_min.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/sample_noise.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_nullify.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/sample_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.6/src/scs_analysis/sample_slope.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_sort.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_stats.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.6/src/scs_analysis/sample_subset.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/sample_time_shift.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.6/src/scs_analysis/socket_receiver.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.6/src/scs_analysis/timer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.6/src/scs_analysis/uds_receiver.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:03:10.421270 scs_analysis-3.8.6/src/scs_analysis.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-30 09:03:10.000000 scs_analysis-3.8.6/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs_analysis-3.8.3/LICENSE` & `scs_analysis-3.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/PKG-INFO` & `scs_analysis-3.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.3
+Version: 3.8.6
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -23,16 +23,16 @@
 Requires-Dist: pypandoc~=1.5
 Requires-Dist: pysftp~=0.2.9
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: scipy~=1.5
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.13.0
-Requires-Dist: scs-host-posix~=3.3.0
+Requires-Dist: scs-core~=3.13.4
+Requires-Dist: scs-host-posix~=3.3.1
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_analysis
 _Information management and analysis utilities for South Coast Science data consumers_
 
 Detailed information at the [scs_analysis wiki](https://github.com/south-coast-science/scs_analysis/wiki).
```

### Comparing `scs_analysis-3.8.3/README.md` & `scs_analysis-3.8.6/README.md`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/setup.py` & `scs_analysis-3.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import os
 import setuptools
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(str(os.path.join(here, rel_path))) as fp:
+    here = str(os.path.abspath(os.path.dirname(__file__)))
+    with codecs.open(os.path.join(here, rel_path)) as fp:
         return fp.read()
 
 
 def get_version(rel_path):
     for line in read(rel_path).splitlines():
         if line.startswith('__version__'):
             return line.split("'")[1]
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/alert.py` & `scs_analysis-3.8.6/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/alert_status.py` & `scs_analysis-3.8.6/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_byline.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_client_auth.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_mqtt_client.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_topic_history.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_topic_origin.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_topic_origin.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 DOCUMENT EXAMPLE
 {"topic": "ricardo/gatwick/loc/1/gases", "device": "scs-bgx-507", "rec": "2019-05-10T09:17:39Z",
 "expiry": "2019-05-17T09:17:46Z"}
 
 SEE ALSO
 scs_analysis/aws_byline
 scs_analysis/aws_topic_history
+scs_analysis/cognito_user_credentials
 
 scs_lambda/aws_message_delete
 """
 
 import sys
 
 from scs_analysis.cmd.cmd_aws_topic_origin import CmdAWSTopicOrigin
@@ -46,15 +47,14 @@
 from scs_core.data.json import JSONify
 
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
-# TODO: optionally exclude control topics - they are not in DynamoDB (or shouldn't be!)
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     # ----------------------------------------------------------------------------------------------------------------
     # cmd...
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_topic_publisher.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/aws_upload_interval.py` & `scs_analysis-3.8.6/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/baseline.py` & `scs_analysis-3.8.6/src/scs_analysis/baseline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/baseline_conf.py` & `scs_analysis-3.8.6/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/chart/chart.py` & `scs_analysis-3.8.6/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/chart/histo_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/chart/multi_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/chart/single_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/client_traffic.py` & `scs_analysis-3.8.6/src/scs_analysis/client_traffic.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,33 @@
 * --aggregate - (only relevant when specifying a year or month period) statistics are aggregated to totals for the
 period
 
 Statistics are available only for the clients(s) that are visible to the user. Only organisation admins may view
 statistics for whole organisations. Only superusers can view the statistics for all users.
 
 SYNOPSIS
-client_traffic.py [-c CREDENTIALS] [-e ENDPOINT] { -u | -o [-s] } -p PERIOD [-a] [-i INDENT] [-v]  [CLIENT_1..CLIENT_N]
+client_traffic.py [-c CREDENTIALS] -e ENDPOINT { -u | -o [-s] } -p PERIOD [-a] [-i INDENT] [-v]  [CLIENT_1..CLIENT_N]
 
 EXAMPLES
-client_traffic.py -c super -o Ricardo -e test1 -p 2023-08-22
+client_traffic.py -c super -e test1 -o Ricardo -p 2023-08-22
 
-client_traffic.py -v -c super -p 2024 -e TopicHistory -u production@southcoastscience.com | node.py -s | \
+client_traffic.py -v -c super -e TopicHistory -p 2024 -u production@southcoastscience.com | node.py -s | \
 csv_writer.py -v traffic.csv
 
 DOCUMENT EXAMPLE
-[{"endpoint": "test1", "client": "MyOrg", "period": "2023-08-22", "queries": 99, "invocations": 99, "documents": 495}]
+[
+    {
+        "endpoint": "TopicHistory",
+        "client": "production@southcoastscience.com",
+        "period": "2024",
+        "queries": 855,
+        "invocations": 855,
+        "characters": 266633895
+    }
+]
 
 SEE ALSO
 scs_analysis/cognito_user_credentials
 """
 
 import sys
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_alert.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_alert_status.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_topic_origin.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_origin.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_baseline.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_client_traffic.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_client_traffic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 
     # --------------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-e ENDPOINT] "
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -e ENDPOINT "
                                                     "{ -u | -o [-s] } -p PERIOD [-a] "
                                                     "[-i INDENT] [-v] [CLIENT_1..CLIENT_N]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # filters...
         self.__parser.add_option("--endpoint", "-e", type="string", action="store", dest="endpoint",
-                                 help="a specific endpoint (required if no clients)")
+                                 help="a specific endpoint")
 
         self.__parser.add_option("--users", "-u", action="store_true", dest="user", default=False,
                                  help="a specific user")
 
         self.__parser.add_option("--organisations", "-o", action="store_true", dest="organisation", default=False,
                                  help="a specific organisation")
 
@@ -56,29 +56,29 @@
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
+        if not self.endpoint:
+            return False
+
         if self.user and self.organisation:
             return False
 
         if self.period is None:
             return False
 
         if self.separate and not self.organisation:
             return False
 
         if self.separate and len(self.clients) > 1:
             return False
 
-        if not self.endpoint and not self.__args:
-            return False
-
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # properties: identity...
 
     @property
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] "
-                                                    "{ -F [{ -t TAG | -n INVOICE }] [-m] "
-                                                    "| -U TAG INVOICE "
-                                                    "| -D TAG } "
+                                                    "{ -F [{ -t DEVICE_TAG | -n INVOICE }] [-m] "
+                                                    "| -U DEVICE_TAG INVOICE "
+                                                    "| -D DEVICE_TAG } "
                                                     "[-i INDENT] [-v]",
                                               version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_email.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class CmdConfigurationMonitor(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t TAG [-x]] { -l | -f | -d | -o } "
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t DEVICE_TAG [-x]] { -l | -f | -d | -o } "
                                                     "[-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # filters...
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
     def __init__(self):
         """
         Constructor
         """
         codes = ' | '.join(ConfigurationCheck.result_codes())
 
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [{ -f TAG | -t TAG [-x] [-o] | -r CODE }] "
-                                                    "[-i INDENT] [-v]", version=version())
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [{ -f DEVICE_TAG | -t DEVICE_TAG [-x] [-o] "
+                                                    "| -r CODE }] [-i INDENT] [-v]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--force", "-f", type="string", action="store", dest="force",
-                                 help="force check the device with TAG now")
+                                 help="force check the device with DEVICE_TAG now")
 
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
                                  help="the (partial) tag of the device(s)")
 
         self.__parser.add_option("--exactly", "-x", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_configuration_report.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_configuration_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # --------------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-v] DEVICE_TAG_1 [..DEVICE_TAG_N]",
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-v] DEVICE_TAG_1 [...DEVICE_TAG_N]",
                                               version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_join.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_device_controller.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_device_monitor.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_device_monitor_status.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,97 @@
 """
-Created on 20 Feb 2017
+Created on 4 Sep 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdLocalizedDatetime(object):
+class CmdSampleNullify(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { [-o HOURS] [-m MINUTES] [-s SECONDS] [-t TIMEZONE_NAME] | "
-                                                    "-z }", version=version())
+        self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
+                                                    " [-v]", version=version())
 
-        # fields...
-        self.__parser.add_option("--hours", "-o", type="int", default=0, action="store", dest="hours",
-                                 help="offset from now in hours")
+        # input...
+        self.__parser.add_option("--target", "-t", type="string", action="store", dest="target",
+                                 help="field to be nullified")
+
+        self.__parser.add_option("--source", "-s", type="string", action="store", dest="source",
+                                 help="field providing the test value")
+
+        # operation...
+        self.__parser.add_option("--lower", "-l", type="float", action="store", dest="lower",
+                                 help="lower bound")
 
-        self.__parser.add_option("--minutes", "-m", type="int", default=0, action="store", dest="minutes",
-                                 help="offset from now in minutes")
-
-        self.__parser.add_option("--seconds", "-s", type="int", default=0, action="store", dest="seconds",
-                                 help="offset from now in seconds")
-
-        self.__parser.add_option("--timezone", "-t", type="string", action="store", dest="zone",
-                                 help="present the time in the given zone")
-
-        # helper...
-        self.__parser.add_option("--zones", "-z", action="store_true", dest="list", default=False,
-                                 help="list the available timezone names to stderr")
+        self.__parser.add_option("--upper", "-u", type="float", action="store", dest="upper",
+                                 help="upper bound")
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.list and (self.hours or self.minutes or self.seconds or self.zone):
+        if self.target is None or self.source is None:
+            return False
+
+        if self.lower is not None and self.upper is not None and self.upper <= self.lower:
             return False
 
         if self.__args:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def hours(self):
-        return self.__opts.hours
-
-
-    @property
-    def minutes(self):
-        return self.__opts.minutes
+    def target(self):
+        return self.__opts.target
 
 
     @property
-    def seconds(self):
-        return self.__opts.seconds
+    def source(self):
+        return self.__opts.source
 
 
     @property
-    def zone(self):
-        return self.__opts.zone
+    def lower(self):
+        return self.__opts.lower
 
 
     @property
-    def list(self):
-        return self.__opts.list
+    def upper(self):
+        return self.__opts.upper
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdLocalizedDatetime:{hours:%s, minutes:%s, seconds:%s, seconds:%s, seconds:%s, verbose:%s}" % \
-               (self.hours, self.minutes, self.seconds, self.zone, self.list, self.verbose)
+        return "CmdSampleNullify:{target:%s, source:%s, lower:%s, upper:%s, verbose:%s}" % \
+               (self.target, self.source, self.lower, self.upper, self.verbose)
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_node.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_organisations.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_error.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_gas_concentration.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_gas_density.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_localize.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_median.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,81 @@
 """
-Created on 4 Sep 2019
+Created on 22 Aug 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleNullify(object):
+class CmdSampleTally(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
-                                                    " [-v]", version=version())
+        self.__parser = optparse.OptionParser(usage="%prog [-t TALLY] [-p PRECISION] [-v] [PATH]", version=version())
 
-        # input...
-        self.__parser.add_option("--target", "-t", type="string", action="store", dest="target",
-                                 help="field to be nullified")
-
-        self.__parser.add_option("--source", "-s", type="string", action="store", dest="source",
-                                 help="field providing the test value")
-
-        # operation...
-        self.__parser.add_option("--lower", "-l", type="float", action="store", dest="lower",
-                                 help="lower bound")
-
-        self.__parser.add_option("--upper", "-u", type="float", action="store", dest="upper",
-                                 help="upper bound")
+        # mode...
+        self.__parser.add_option("--tally", "-t", type="int", action="store", dest="tally",
+                                 help="generate a rolling aggregate for TALLY number of data points (default all)")
 
         # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
+                                 help="precision (default 0 decimal places)")
+
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.target is None or self.source is None:
-            return False
-
-        if self.lower is not None and self.upper is not None and self.upper <= self.lower:
+        if self.tally is not None and self.tally < 1:
             return False
 
-        if self.__args:
+        if self.__args and len(self.__args) != 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def target(self):
-        return self.__opts.target
+    def tally(self):
+        return self.__opts.tally
 
 
     @property
-    def source(self):
-        return self.__opts.source
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def lower(self):
-        return self.__opts.lower
-
-
-    @property
-    def upper(self):
-        return self.__opts.upper
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleNullify:{target:%s, source:%s, lower:%s, upper:%s, verbose:%s}" % \
-               (self.target, self.source, self.lower, self.upper, self.verbose)
+        return "CmdSampleTally:{tally:%s, precision:%s, verbose:%s, path:%s}" % \
+                    (self.tally, self.precision, self.verbose, self.path)
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_record.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,64 @@
 """
-Created on 22 Aug 2017
+Created on 13 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleTally(object):
+class CmdSocketReceiver(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-t TALLY] [-p PRECISION] [-v] [PATH]", version=version())
+        self.__parser = optparse.OptionParser(usage="%prog [-p PORT] [-v]", version=version())
 
-        # mode...
-        self.__parser.add_option("--tally", "-t", type="int", action="store", dest="tally",
-                                 help="generate a rolling aggregate for TALLY number of data points (default all)")
+        # input...
+        self.__parser.add_option("--port", "-p", type="int", action="store", default=2000, dest="port",
+                                 help="socket port (default 2000)")
 
         # output...
-        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
-                                 help="precision (default 0 decimal places)")
-
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.tally is not None and self.tally < 1:
-            return False
-
-        if self.__args and len(self.__args) != 1:
+        if self.__args:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def tally(self):
-        return self.__opts.tally
-
-
-    @property
-    def precision(self):
-        return self.__opts.precision
+    def port(self):
+        return self.__opts.port
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleTally:{tally:%s, precision:%s, verbose:%s, path:%s}" % \
-                    (self.tally, self.precision, self.verbose, self.path)
+        return "CmdSocketReceiver:{port:%d, verbose:%s}" % (self.port, self.verbose)
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_single_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cmd/cmd_uds.py` & `scs_analysis-3.8.6/src/scs_analysis/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cognito_devices.py` & `scs_analysis-3.8.6/src/scs_analysis/cognito_devices.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,55 @@
 Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_devices utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
-by customer organisation administrators, SCS administrators and superusers.
-
-If the --Create function is used, an email is sent to the new user. The verification link in the email must be
-excercised using the cognito_email utility in order for the account to gain a CONFIRMED status.
+The cognito_devices utility is used to
 
 SYNOPSIS
-cognito_devices.py  [-c CREDENTIALS] { -F [{ -t TAG | -n INVOICE }] [-m] | -U TAG INVOICE | -D TAG } [-i INDENT] [-v]
+cognito_devices.py  [-c CREDENTIALS] { -F [{ -t DEVICE_TAG | -n INVOICE }] [-m] | -U DEVICE_TAG INVOICE |
+-D DEVICE_TAG } [-i INDENT] [-v]
 
 EXAMPLES
 cognito_devices.py -vi4 -c super -F -m
 
 DOCUMENT EXAMPLE
-{"username": "scs-bgx-401", "invoice": "INV-000123",
-"created": "2023-06-23T10:32:52+01:00", "last-updated": "2023-06-23T10:32:52+01:00"}
+[
+    {
+        "username": "scs-ph1-8",
+        "invoice": "INV-0000",
+        "created": "2023-04-20T12:25:47Z",
+        "last-updated": "2024-01-29T15:37:21Z"
+    }
+]
+
+DOCUMENT EXAMPLE - WITH MEMBERSHIPS
+[
+    {
+        "account": {
+            "username": "scs-ph1-8",
+            "invoice": "INV-0000",
+            "created": "2023-04-20T12:25:47Z",
+            "last-updated": "2024-01-29T15:37:21Z"
+        },
+        "memberships": [
+            {
+                "DeviceTag": "scs-ph1-8",
+                "OrgID": 69,
+                "DeploymentLabel": "SCS Dev / Mobile 8",
+                "DevicePath": "south-coast-science-dev/mobile/device/praxis-handheld-000008/",
+                "LocationPath": "south-coast-science-dev/mobile/loc/8/",
+                "StartDatetime": "1970-01-01T00:00:00Z",
+                "EndDatetime": null
+            }
+        ]
+    }
+]
 
 SEE ALSO
 scs_analysis/cognito_users
 scs_analysis/cognito_user_credentials
 scs_analysis/organisation_devices
 
 RESOURCES
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cognito_email.py` & `scs_analysis-3.8.6/src/scs_analysis/cognito_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     HTTPNotFoundException, HTTPNotAllowedException, HTTPUnauthorizedException
 
 from scs_core.data.datum import Datum
 
 from scs_core.sys.logging import Logging
 
 from scs_host.comms.stdio import StdIO
+from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 def do_password(do_set):
     new_password = StdIO.prompt("Enter new password")
 
@@ -90,15 +91,14 @@
 
         logger.error(repr(ex))
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
-
     logger = None
     credentials = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
@@ -108,15 +108,15 @@
             cmd.print_help(sys.stderr)
             exit(2)
 
         Logging.config('cognito_email', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
-
+        logger.debug(Host)              # initialise API endpoint reporting
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         password_manager = CognitoPasswordManager()
         user_manager = CognitoUserCreator()
         gatekeeper = CognitoLoginManager()
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cognito_user_credentials.py` & `scs_analysis-3.8.6/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cognito_user_identity.py` & `scs_analysis-3.8.6/src/scs_analysis/cognito_user_identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 if __name__ == '__main__':
 
     logger = None
     gatekeeper = None
     credentials = None
     auth = None
+    email = None
     finder = None
     report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
@@ -205,15 +206,15 @@
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPConflictException as ex:
-        logger.error("the email address '%s' is already in use." % report.email)
+        logger.error("the email address '%s' is already in use." % email)
         exit(1)
 
     except HTTPException as ex:
         logger.error(ex.error_report)
         exit(1)
 
     except Exception as ex:
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/cognito_users.py` & `scs_analysis-3.8.6/src/scs_analysis/cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/configuration_csv.py` & `scs_analysis-3.8.6/src/scs_analysis/configuration_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 EXAMPLES
 configuration_csv.py -vs configs.csv
 configuration_csv.py -vdo afe_ids afe-id
 configuration_csv.py -vft scs-bgx-431
 
 SEE ALSO
+scs_analysis/cognito_user_credentials
 scs_analysis/configuration_monitor
 scs_analysis/configuration_monitor_check
-scs_analysis/monitor_auth
 
 scs_mfr/configuration
 """
 
 import os
 import sys
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/configuration_monitor.py` & `scs_analysis-3.8.6/src/scs_analysis/configuration_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 DESCRIPTION
 The configuration_monitor utility is used to retrieve configuration information relating to one or more devices.
 Flags enable the selection of either the latest recorded configuration for the device(s), or a history of
 configuration changes. In the case of historical reports, either all the field values can be returned, or
 only those that changed from the previous recording.
 
 SYNOPSIS
-configuration_monitor.py [-c CREDENTIALS] [-t TAG [-x]] { -l | -f | -d | -o } [-i INDENT] [-v]
+configuration_monitor.py [-c CREDENTIALS] [-t DEVICE_TAG [-x]] { -l | -f | -d | -o } [-i INDENT] [-v]
 
 EXAMPLES
 configuration_monitor.py -t scs-bgx-401 -d | node.py -s | csv_writer.py -s
 
 SEE ALSO
+scs_analysis/cognito_user_credentials
 scs_analysis/configuration_csv
 scs_analysis/configuration_monitor_check
 scs_analysis/monitor_auth
 
 scs_mfr/configuration
 """
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/configuration_monitor_check.py` & `scs_analysis-3.8.6/src/scs_analysis/configuration_monitor_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 * NSP - NOT SUPPORTED
 * R - RECEIVED:
 * RNW - RECEIVED:NEW
 * RUN - RECEIVED:UNCHANGED
 * RUP - RECEIVED:UPDATED
 
 SYNOPSIS
-configuration_monitor_check.py [-c CREDENTIALS] [{ -f TAG | -t TAG [-x] [-o] | -r CODE }] [-i INDENT] [-v]
+configuration_monitor_check.py [-c CREDENTIALS] [{ -f DEVICE_TAG | -t DEVICE_TAG [-x] [-o] | -r CODE }] [-i INDENT] [-v]
 
 EXAMPLES
 configuration_monitor_check.py -r ERR | node.py -s | csv_writer.py
 
 DOCUMENT EXAMPLE
 {"tag": "scs-ph1-26", "rec": "2021-05-18T14:36:00Z", "result": "ERROR",
 "context": ["TimeoutExpired(['./configuration'], 30)"]}
 
 SEE ALSO
+scs_analysis/cognito_user_credentials
 scs_analysis/configuration_csv
 scs_analysis/configuration_monitor
 scs_analysis/monitor_auth
 
 scs_mfr/configuration
 
 BUGS
@@ -110,14 +111,15 @@
 
         if cmd.force:
             response = requester.request(auth.id_token, cmd.force)
             print(response.result, file=sys.stderr)
             exit(0 if response.result == 'OK' else 1)
 
         response = finder.find(auth.id_token, cmd.tag_filter, cmd.exact_match, cmd.response_mode())
+
         print(JSONify.dumps(sorted(response.items), indent=cmd.indent))
         logger.info('retrieved: %s' % len(response.items))
 
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/configuration_report.py` & `scs_analysis-3.8.6/src/scs_analysis/configuration_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 """
 Created on 12 Sep 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 DESCRIPTION
 The configuration_report utility is used to generate a configuration CSV file by remotely interrogating the specified
-device. The utility should be run in the directory that is scanned for raw report CSVs, such as
+device. The result is written to a CSV file named conf-scs-TYPE-NUMBER.csv
+
+The utility is normally run in the directory that is scanned for raw report CSVs, such as
 /Users/bruno/gbb/Production/ConfigurationGenerator/RawConfigs
 
 SYNOPSIS
-configuration_report.py [-c CREDENTIALS] [-v] DEVICE_TAG_1 [..DEVICE_TAG_N]
+configuration_report.py [-c CREDENTIALS] [-v] DEVICE_TAG_1 [...DEVICE_TAG_N]
 
 EXAMPLES
 configuration_report.py -v -c super scs-opc-245
 
 SEE ALSO
+scs_analysis/cognito_user_credentials
 scs_analysis/device_controller
 
 scs_mfr/configuration
 """
 
 import sys
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/csv_collation_summary.py` & `scs_analysis-3.8.6/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/csv_collator.py` & `scs_analysis-3.8.6/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/csv_join.py` & `scs_analysis-3.8.6/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/csv_reader.py` & `scs_analysis-3.8.6/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/csv_segmentor.py` & `scs_analysis-3.8.6/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/csv_writer.py` & `scs_analysis-3.8.6/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/device_controller.py` & `scs_analysis-3.8.6/src/scs_analysis/device_controller.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/device_monitor.py` & `scs_analysis-3.8.6/src/scs_analysis/device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/device_monitor_status.py` & `scs_analysis-3.8.6/src/scs_analysis/device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/batch_download_reporter.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/configuration_csv_generator.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/csv_collator.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/csv_collator.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     def close(self):
         if self.__writer:
             self.__writer.close()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, **kwargs):
         jdict = OrderedDict()
 
         jdict['lower'] = self.lower
         jdict['upper'] = self.upper
         jdict['count'] = self.count
 
         return jdict
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/csv_segmentor.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/csv_segmentor.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def close(self):
         if self.__writer:
             self.__writer.close()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, **kwargs):
         jdict = OrderedDict()
 
         jdict['start'] = self.start.as_json()
         jdict['end'] = self.end.as_json()
 
         jdict['prev-interval'] = None if self.prev_interval is None else \
             Timedelta.construct(self.prev_interval).as_json()
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/mqtt_reporter.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/sample_midpoint.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/handler/sample_regression.py` & `scs_analysis-3.8.6/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/histo_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/localised_datetime.py` & `scs_analysis-3.8.6/src/scs_analysis/localised_datetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,18 +59,20 @@
 
     if cmd.list:
         for zone in Timezone.zones():
             print(zone, file=sys.stderr)
         exit(0)
 
     now = LocalizedDatetime.now()
-    offset = now.timedelta(hours=cmd.hours, minutes=cmd.minutes, seconds=cmd.seconds)
+    ldt = now.timedelta(hours=cmd.hours, minutes=cmd.minutes, seconds=cmd.seconds)
 
     if cmd.zone is not None:
         if not Timezone.is_valid(cmd.zone):
             print("localised_datetime: invalid timezone: %s" % cmd.zone, file=sys.stderr)
             exit(1)
 
         timezone = Timezone(cmd.zone)
-        offset = offset.localize(timezone.zone)
+        ldt = ldt.localize(timezone.zone)
 
-    print(offset.as_iso8601())
+    report = ldt.as_readable() if cmd.readable else ldt.as_iso8601()
+
+    print(report)
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis/monitor_auth.py` & `scs_analysis-3.8.6/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/multi_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/node.py` & `scs_analysis-3.8.6/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/organisation_devices.py` & `scs_analysis-3.8.6/src/scs_analysis/organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/organisation_path_roots.py` & `scs_analysis-3.8.6/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/organisation_user_paths.py` & `scs_analysis-3.8.6/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/organisation_users.py` & `scs_analysis-3.8.6/src/scs_analysis/organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/organisations.py` & `scs_analysis-3.8.6/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_aggregate.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_average.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_collator.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_distance.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_duplicates.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_error.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_gas_concentration.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_gas_density.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_interval.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_iso_8601.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_localize.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_low_pass.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_max.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_median.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_midpoint.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_min.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_noise.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_nullify.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_paths.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_regression.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_slope.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_sort.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_stats.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_subset.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/sample_time_shift.py` & `scs_analysis-3.8.6/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/single_chart.py` & `scs_analysis-3.8.6/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/socket_receiver.py` & `scs_analysis-3.8.6/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/timer.py` & `scs_analysis-3.8.6/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis/uds_receiver.py` & `scs_analysis-3.8.6/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.3/src/scs_analysis.egg-info/PKG-INFO` & `scs_analysis-3.8.6/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.3
+Version: 3.8.6
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -23,16 +23,16 @@
 Requires-Dist: pypandoc~=1.5
 Requires-Dist: pysftp~=0.2.9
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: scipy~=1.5
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.13.0
-Requires-Dist: scs-host-posix~=3.3.0
+Requires-Dist: scs-core~=3.13.4
+Requires-Dist: scs-host-posix~=3.3.1
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_analysis
 _Information management and analysis utilities for South Coast Science data consumers_
 
 Detailed information at the [scs_analysis wiki](https://github.com/south-coast-science/scs_analysis/wiki).
```

### Comparing `scs_analysis-3.8.3/src/scs_analysis.egg-info/SOURCES.txt` & `scs_analysis-3.8.6/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

