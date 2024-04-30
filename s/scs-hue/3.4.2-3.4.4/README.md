# Comparing `tmp/scs-hue-3.4.2.tar.gz` & `tmp/scs_hue-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-hue-3.4.2.tar", last modified: Wed Jan 31 08:48:50 2024, max compression
+gzip compressed data, was "scs_hue-3.4.4.tar", last modified: Tue Apr 30 09:04:51 2024, max compression
```

## Comparing `scs-hue-3.4.2.tar` & `scs_hue-3.4.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.652929 scs-hue-3.4.2/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-11-09 16:14:15.000000 scs-hue-3.4.2/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       84 2023-11-22 14:23:52.000000 scs-hue-3.4.2/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1315 2024-01-31 08:48:50.652731 scs-hue-3.4.2/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      347 2023-12-01 15:41:17.000000 scs-hue-3.4.2/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-11-09 16:14:15.000000 scs-hue-3.4.2/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      118 2024-01-08 13:21:12.000000 scs-hue-3.4.2/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-01-31 08:48:50.652967 scs-hue-3.4.2/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     3140 2024-01-31 08:48:42.000000 scs-hue-3.4.2/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.636357 scs-hue-3.4.2/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.652476 scs-hue-3.4.2/src/scs_hue.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1315 2024-01-31 08:48:50.000000 scs-hue-3.4.2/src/scs_hue.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     3847 2024-01-31 08:48:50.000000 scs-hue-3.4.2/src/scs_hue.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-01-31 08:48:50.000000 scs-hue-3.4.2/src/scs_hue.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      133 2024-01-31 08:48:50.000000 scs-hue-3.4.2/src/scs_hue.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)       16 2024-01-31 08:48:50.000000 scs-hue-3.4.2/src/scs_hue.egg-info/top_level.txt
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.642245 scs-hue-3.4.2/src/scs_philips_hue/
--rwxr-xr-x   0 bruno      (502) admin       (80)      244 2024-01-31 08:48:42.000000 scs-hue-3.4.2/src/scs_philips_hue/__init__.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2536 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/aws_client_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4816 2023-11-23 09:22:24.000000 scs-hue-3.4.2/src/scs_philips_hue/aws_mqtt_subscriber.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4681 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/bridge.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1927 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/bridge_address.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3288 2023-12-01 15:41:17.000000 scs-hue-3.4.2/src/scs_philips_hue/channel_test.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3901 2023-11-23 09:22:24.000000 scs-hue-3.4.2/src/scs_philips_hue/chroma.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3849 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/chroma_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.642727 scs-hue-3.4.2/src/scs_philips_hue/client/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/client/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1849 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/client/client_exception.py
--rw-r--r--   0 bruno      (502) admin       (80)     4292 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/client/rest_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     2061 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/client/upnp_client.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.645464 scs-hue-3.4.2/src/scs_philips_hue/cmd/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3111 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_aws_client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     3952 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_bridge.py
--rw-r--r--   0 bruno      (502) admin       (80)     2029 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_bridge_address.py
--rw-r--r--   0 bruno      (502) admin       (80)     2412 2023-12-01 15:41:17.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_channel_test.py
--rw-r--r--   0 bruno      (502) admin       (80)     1148 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_chroma.py
--rw-r--r--   0 bruno      (502) admin       (80)     5136 2023-12-01 15:41:17.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_chroma_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     1760 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_desk.py
--rw-r--r--   0 bruno      (502) admin       (80)     3343 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_desk_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     3086 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_domain_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2027 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_join.py
--rw-r--r--   0 bruno      (502) admin       (80)     5258 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_light.py
--rw-r--r--   0 bruno      (502) admin       (80)     2613 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_mqtt_subscriber.py
--rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_node.py
--rw-r--r--   0 bruno      (502) admin       (80)     1148 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_simple.py
--rw-r--r--   0 bruno      (502) admin       (80)     1546 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_uds.py
--rw-r--r--   0 bruno      (502) admin       (80)     2256 2023-11-22 11:45:32.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_upnp_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2620 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_user.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.646486 scs-hue-3.4.2/src/scs_philips_hue/config/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4577 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/bridge_address.py
--rw-r--r--   0 bruno      (502) admin       (80)     5083 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/bridge_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     4903 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/chroma_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     3155 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/chroma_path.py
--rw-r--r--   0 bruno      (502) admin       (80)     1950 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/conf_set.py
--rw-r--r--   0 bruno      (502) admin       (80)     3384 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/desk_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     4031 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/domain_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.646779 scs-hue-3.4.2/src/scs_philips_hue/config/paths/
--rw-r--r--   0 bruno      (502) admin       (80)       83 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/paths/green_to_red.json
--rw-r--r--   0 bruno      (502) admin       (80)      216 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/config/paths/risk_level.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.646929 scs-hue-3.4.2/src/scs_philips_hue/data/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.648409 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1869 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/backup.py
--rw-r--r--   0 bruno      (502) admin       (80)    19189 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/bridge_config.py
--rw-r--r--   0 bruno      (502) admin       (80)     1909 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/bridge_summary.py
--rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/internet_services.py
--rw-r--r--   0 bruno      (502) admin       (80)     2564 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/portal_state.py
--rw-r--r--   0 bruno      (502) admin       (80)     6091 2023-11-21 12:16:58.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/response.py
--rw-r--r--   0 bruno      (502) admin       (80)     5706 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/sw_update.py
--rw-r--r--   0 bruno      (502) admin       (80)     6460 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/sw_update_2.py
--rw-r--r--   0 bruno      (502) admin       (80)     4494 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/bridge/whitelist.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.648787 scs-hue-3.4.2/src/scs_philips_hue/data/client/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/client/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1886 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/client/client_description.py
--rw-r--r--   0 bruno      (502) admin       (80)     1805 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/client/device_description.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.649991 scs-hue-3.4.2/src/scs_philips_hue/data/light/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     7127 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/chroma.py
--rw-r--r--   0 bruno      (502) admin       (80)     6753 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/light.py
--rw-r--r--   0 bruno      (502) admin       (80)     4415 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/light_catalogue.py
--rw-r--r--   0 bruno      (502) admin       (80)     1567 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/light_device.py
--rw-r--r--   0 bruno      (502) admin       (80)     1597 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/light_name.py
--rw-r--r--   0 bruno      (502) admin       (80)     4037 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/light_scan.py
--rw-r--r--   0 bruno      (502) admin       (80)     7803 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/light_state.py
--rw-r--r--   0 bruno      (502) admin       (80)     1896 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/data/light/sw_update.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6460 2023-12-01 15:41:17.000000 scs-hue-3.4.2/src/scs_philips_hue/desk.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2239 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/desk_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.650835 scs-hue-3.4.2/src/scs_philips_hue/discovery/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/discovery/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2139 2023-11-24 15:41:31.000000 scs-hue-3.4.2/src/scs_philips_hue/discovery/discovery.py
--rw-r--r--   0 bruno      (502) admin       (80)     2758 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/discovery/ip_discovery.py
--rw-r--r--   0 bruno      (502) admin       (80)     1859 2023-11-22 11:45:32.000000 scs-hue-3.4.2/src/scs_philips_hue/discovery/upnp_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     1670 2023-11-24 15:41:31.000000 scs-hue-3.4.2/src/scs_philips_hue/discovery/upnp_discovery.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2468 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/domain_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.651157 scs-hue-3.4.2/src/scs_philips_hue/handler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/handler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1684 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/handler/aws_mqtt_subscription_handler.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6353 2023-11-24 15:41:31.000000 scs-hue-3.4.2/src/scs_philips_hue/join.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6136 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/light.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:50.652281 scs-hue-3.4.2/src/scs_philips_hue/manager/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3755 2023-11-22 11:45:32.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/bridge_builder.py
--rw-r--r--   0 bruno      (502) admin       (80)     5062 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/bridge_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     2686 2023-11-21 12:16:58.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/bridge_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     5346 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/light_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1915 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1988 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/manager/user_manager.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3066 2023-11-23 09:22:24.000000 scs-hue-3.4.2/src/scs_philips_hue/node.py
--rwxr-xr-x   0 bruno      (502) admin       (80)      121 2023-11-21 12:46:30.000000 scs-hue-3.4.2/src/scs_philips_hue/run_chroma.sh
--rwxr-xr-x   0 bruno      (502) admin       (80)     1993 2023-11-23 09:22:24.000000 scs-hue-3.4.2/src/scs_philips_hue/uds_receiver.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2069 2023-11-22 11:45:32.000000 scs-hue-3.4.2/src/scs_philips_hue/upnp_conf.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3544 2023-11-09 16:14:15.000000 scs-hue-3.4.2/src/scs_philips_hue/user.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.763051 scs_hue-3.4.4/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-11-09 16:14:15.000000 scs_hue-3.4.4/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       84 2023-11-22 14:23:52.000000 scs_hue-3.4.4/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1316 2024-04-30 09:04:51.762887 scs_hue-3.4.4/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      347 2023-12-01 15:41:17.000000 scs_hue-3.4.4/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-11-09 16:14:15.000000 scs_hue-3.4.4/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      119 2024-04-30 09:04:42.000000 scs_hue-3.4.4/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-30 09:04:51.763084 scs_hue-3.4.4/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3192 2024-04-30 09:04:42.000000 scs_hue-3.4.4/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.748015 scs_hue-3.4.4/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.762633 scs_hue-3.4.4/src/scs_hue.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1316 2024-04-30 09:04:51.000000 scs_hue-3.4.4/src/scs_hue.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     3847 2024-04-30 09:04:51.000000 scs_hue-3.4.4/src/scs_hue.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-30 09:04:51.000000 scs_hue-3.4.4/src/scs_hue.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      134 2024-04-30 09:04:51.000000 scs_hue-3.4.4/src/scs_hue.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       16 2024-04-30 09:04:51.000000 scs_hue-3.4.4/src/scs_hue.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.754279 scs_hue-3.4.4/src/scs_philips_hue/
+-rwxr-xr-x   0 bruno      (502) admin       (80)      244 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/__init__.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2536 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/aws_client_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4816 2023-11-23 09:22:24.000000 scs_hue-3.4.4/src/scs_philips_hue/aws_mqtt_subscriber.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4681 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/bridge.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1927 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/bridge_address.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3288 2023-12-01 15:41:17.000000 scs_hue-3.4.4/src/scs_philips_hue/channel_test.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3901 2023-11-23 09:22:24.000000 scs_hue-3.4.4/src/scs_philips_hue/chroma.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3849 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/chroma_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.754767 scs_hue-3.4.4/src/scs_philips_hue/client/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/client/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1866 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/client/client_exception.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4292 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/client/rest_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2061 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/client/upnp_client.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.757226 scs_hue-3.4.4/src/scs_philips_hue/cmd/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3111 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_aws_client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3952 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_bridge.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2029 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_bridge_address.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2412 2023-12-01 15:41:17.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_channel_test.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1148 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_chroma.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5136 2023-12-01 15:41:17.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_chroma_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1760 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_desk.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3343 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_desk_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3086 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_domain_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2027 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_join.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5258 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_light.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2613 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_mqtt_subscriber.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1148 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_simple.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1546 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_uds.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2256 2023-11-22 11:45:32.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_upnp_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2620 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_user.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.758042 scs_hue-3.4.4/src/scs_philips_hue/config/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/config/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4611 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/bridge_address.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5117 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/bridge_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4920 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/chroma_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3172 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/chroma_path.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1967 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/conf_set.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3401 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/desk_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4048 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/config/domain_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.758274 scs_hue-3.4.4/src/scs_philips_hue/config/paths/
+-rw-r--r--   0 bruno      (502) admin       (80)       83 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/config/paths/green_to_red.json
+-rw-r--r--   0 bruno      (502) admin       (80)      216 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/config/paths/risk_level.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.758396 scs_hue-3.4.4/src/scs_philips_hue/data/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/data/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.759412 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1886 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/backup.py
+-rw-r--r--   0 bruno      (502) admin       (80)    19223 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/bridge_config.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1926 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/bridge_summary.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2553 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/internet_services.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2581 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/portal_state.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6142 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/response.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5740 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/sw_update.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6511 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/sw_update_2.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4528 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/bridge/whitelist.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.759705 scs_hue-3.4.4/src/scs_philips_hue/data/client/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/data/client/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1903 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/client/client_description.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1822 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/client/device_description.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.760611 scs_hue-3.4.4/src/scs_philips_hue/data/light/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7144 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/chroma.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6787 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/light.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4449 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/light_catalogue.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1584 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/light_device.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1614 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/light_name.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4071 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/light_scan.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7837 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/light_state.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1913 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/data/light/sw_update.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6460 2023-12-01 15:41:17.000000 scs_hue-3.4.4/src/scs_philips_hue/desk.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2239 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/desk_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.761238 scs_hue-3.4.4/src/scs_philips_hue/discovery/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/discovery/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2139 2023-11-24 15:41:31.000000 scs_hue-3.4.4/src/scs_philips_hue/discovery/discovery.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2758 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/discovery/ip_discovery.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1876 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/discovery/upnp_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1670 2023-11-24 15:41:31.000000 scs_hue-3.4.4/src/scs_philips_hue/discovery/upnp_discovery.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2468 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/domain_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.761541 scs_hue-3.4.4/src/scs_philips_hue/handler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/handler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1684 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/handler/aws_mqtt_subscription_handler.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6353 2023-11-24 15:41:31.000000 scs_hue-3.4.4/src/scs_philips_hue/join.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6136 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/light.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-30 09:04:51.762461 scs_hue-3.4.4/src/scs_philips_hue/manager/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3755 2023-11-22 11:45:32.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/bridge_builder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5079 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/bridge_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2686 2023-11-21 12:16:58.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/bridge_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5346 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/light_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1932 2024-04-30 09:04:42.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1988 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/manager/user_manager.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3066 2023-11-23 09:22:24.000000 scs_hue-3.4.4/src/scs_philips_hue/node.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)      121 2023-11-21 12:46:30.000000 scs_hue-3.4.4/src/scs_philips_hue/run_chroma.sh
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1993 2023-11-23 09:22:24.000000 scs_hue-3.4.4/src/scs_philips_hue/uds_receiver.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2069 2023-11-22 11:45:32.000000 scs_hue-3.4.4/src/scs_philips_hue/upnp_conf.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3544 2023-11-09 16:14:15.000000 scs_hue-3.4.4/src/scs_philips_hue/user.py
```

### Comparing `scs-hue-3.4.2/LICENSE` & `scs_hue-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/PKG-INFO` & `scs_hue-3.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-hue
-Version: 3.4.2
+Version: 3.4.4
 Summary: Connecting Philips Hue light bulbs to South Coast Science environmental data sources
 Home-page: https://github.com/south-coast-science/scs_philips_hue
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -16,16 +16,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: paho-mqtt~=1.5.0
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.6.0
-Requires-Dist: scs-host-posix~=3.2.1
+Requires-Dist: scs-core~=3.13.3
+Requires-Dist: scs-host-posix~=3.3.0
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_philips_hue
 _A light bulb moment... connecting Philips Hue light bulbs to South Coast Science environmental data sources_
 
 Detailed information at the [scs_philips_hue wiki](https://github.com/south-coast-science/scs_philips_hue/wiki).
```

### Comparing `scs-hue-3.4.2/setup.py` & `scs_hue-3.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import setuptools
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
+    here = str(os.path.abspath(os.path.dirname(__file__)))
     with codecs.open(os.path.join(here, rel_path)) as fp:
         return fp.read()
 
 
 def get_version(rel_path):
     for line in read(rel_path).splitlines():
         if line.startswith('__version__'):
@@ -63,14 +63,15 @@
         "Operating System :: POSIX",
     ],
     scripts=[
         'src/scs_philips_hue/aws_client_auth.py',
         'src/scs_philips_hue/aws_mqtt_subscriber.py',
         'src/scs_philips_hue/bridge.py',
         'src/scs_philips_hue/bridge_address.py',
+        'src/scs_philips_hue/channel_test.py',
         'src/scs_philips_hue/chroma.py',
         'src/scs_philips_hue/chroma_conf.py',
         'src/scs_philips_hue/desk.py',
         'src/scs_philips_hue/desk_conf.py',
         'src/scs_philips_hue/domain_conf.py',
         'src/scs_philips_hue/join.py',
         'src/scs_philips_hue/light.py',
```

### Comparing `scs-hue-3.4.2/src/scs_hue.egg-info/PKG-INFO` & `scs_hue-3.4.4/src/scs_hue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-hue
-Version: 3.4.2
+Version: 3.4.4
 Summary: Connecting Philips Hue light bulbs to South Coast Science environmental data sources
 Home-page: https://github.com/south-coast-science/scs_philips_hue
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -16,16 +16,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: paho-mqtt~=1.5.0
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.6.0
-Requires-Dist: scs-host-posix~=3.2.1
+Requires-Dist: scs-core~=3.13.3
+Requires-Dist: scs-host-posix~=3.3.0
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_philips_hue
 _A light bulb moment... connecting Philips Hue light bulbs to South Coast Science environmental data sources_
 
 Detailed information at the [scs_philips_hue wiki](https://github.com/south-coast-science/scs_philips_hue/wiki).
```

### Comparing `scs-hue-3.4.2/src/scs_hue.egg-info/SOURCES.txt` & `scs_hue-3.4.4/src/scs_hue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/aws_client_auth.py` & `scs_hue-3.4.4/src/scs_philips_hue/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/aws_mqtt_subscriber.py` & `scs_hue-3.4.4/src/scs_philips_hue/aws_mqtt_subscriber.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/bridge.py` & `scs_hue-3.4.4/src/scs_philips_hue/bridge.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/bridge_address.py` & `scs_hue-3.4.4/src/scs_philips_hue/bridge_address.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/channel_test.py` & `scs_hue-3.4.4/src/scs_philips_hue/channel_test.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/chroma.py` & `scs_hue-3.4.4/src/scs_philips_hue/chroma.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/chroma_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/chroma_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/client/client_exception.py` & `scs_hue-3.4.4/src/scs_philips_hue/client/client_exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Constructor
         """
         self.__error = error
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['error'] = self.error
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/client/rest_client.py` & `scs_hue-3.4.4/src/scs_philips_hue/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/client/upnp_client.py` & `scs_hue-3.4.4/src/scs_philips_hue/client/upnp_client.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_aws_client_auth.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_bridge.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_bridge.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_bridge_address.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_bridge_address.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_channel_test.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_channel_test.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_chroma.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_chroma.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_chroma_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_chroma_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_desk.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_desk.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_desk_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_desk_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_domain_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_domain_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_join.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_join.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_light.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_light.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_mqtt_subscriber.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_mqtt_subscriber.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_node.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_simple.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_simple.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_uds.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_upnp_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_upnp_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/cmd/cmd_user.py` & `scs_hue-3.4.4/src/scs_philips_hue/cmd/cmd_user.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/bridge_address.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/bridge_address.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         self.__name = name                                  # string
         self.__ipv4 = ipv4                                  # IPv4Address
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['ipv4'] = None if self.ipv4 is None else self.ipv4.dot_decimal()
 
         return jdict
 
 
@@ -150,15 +150,15 @@
 
     def address(self, name):
         return self.__addresses[name]                           # may raise KeyError
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.sorted_addresses
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def sorted_addresses(self):
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/bridge_credentials.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/bridge_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.__bridge_name = bridge_name                        # string
         self.__bridge_id = bridge_id                            # string
         self.__username = username                              # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['bridge-id'] = self.bridge_id
         jdict['username'] = self.username
 
         return jdict
 
@@ -154,15 +154,15 @@
 
     def credentials(self, bridge_name):
         return self.__credentials[bridge_name]                          # may raise KeyError
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.sorted_credentials
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def sorted_credentials(self):
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/chroma_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/chroma_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     def mapping(self, path):
         return ChromaMapping.construct(self, path)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['path-name'] = self.path_name
 
         jdict['domain-min'] = self.domain_min
         jdict['domain-max'] = self.domain_max
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/chroma_path.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/chroma_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def remove_point(self, index):
         self.__points.pop(index)                    # may raise IndexError
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['name'] = self.name
         jdict['points'] = self.points
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/conf_set.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/conf_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             del self._confs[name]
         except KeyError:
             pass
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.confs
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def conf(self, name):
         try:
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/desk_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/desk_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             return
 
         self.__lamp_names.remove(lamp_name)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.lamp_names
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def lamp_names(self):
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/config/domain_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/config/domain_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             return False
 
         return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['topic-path'] = self.topic_path
         jdict['document-node'] = self.document_node
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/backup.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
         self.__status = status                          # string
         self.__error_code = int(error_code)             # int
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['status'] = self.status
         jdict['errorcode'] = self.error_code
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/bridge_config.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/bridge_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
         self.__link_button = Datum.bool(link_button)                        # bool
         self.__portal_services = Datum.bool(portal_services)                # bool
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         if self.name is not None:
             jdict['name'] = self.name
 
         if self.zigbee_channel is not None:
             jdict['zigbeechannel'] = self.zigbee_channel
@@ -425,15 +425,15 @@
         self.__starterkit_id = starterkit_id                                # string
 
         self.__whitelist = whitelist                                        # WhitelistGroup
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['name'] = self.name
         jdict['zigbeechannel'] = self.zigbee_channel
         jdict['bridgeid'] = self.bridge_id
         jdict['mac'] = self.mac
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/bridge_summary.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/bridge_summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
         self.__id = id                                  # string
         self.__ip_address = ip_address                  # string (IPv4 address)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['id'] = self.id
         jdict['internalipaddress'] = self.ip_address
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/internet_services.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/internet_services.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.__remote_access = remote_access            # string
         self.__time = time                              # string
         self.__sw_update = sw_update                    # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['internet'] = self.internet
         jdict['remoteaccess'] = self.remote_access
         jdict['time'] = self.time
         jdict['swupdate'] = self.sw_update
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/portal_state.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/portal_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.__outgoing = bool(outgoing)                    # bool
 
         self.__communication = communication                # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['signedon'] = self.signed_on
         jdict['incoming'] = self.incoming
         jdict['outgoing'] = self.outgoing
 
         jdict['communication'] = self.communication
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/response.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     def has_errors(self):
         return len(self.errors) > 0
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = []
 
         for error in self.errors:
             jdict.append(error)
 
         for success in self.successes:
             jdict.append(success)
@@ -126,15 +126,15 @@
         """
         self.__cmd = cmd                            # string
         self.__value = value                        # *
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return {'success': {self.cmd: self.value}}
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def cmd(self):
@@ -183,15 +183,15 @@
         self.__code = code                          # int
         self.__address = address                    # string
         self.__description = description            # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['type'] = self.code
         jdict['address'] = self.address
         jdict['description'] = self.description
 
         return {'error': jdict}
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/sw_update.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/sw_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         self.__text = text                                              # string
         self.__notify = Datum.bool(notify)                              # bool
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         if self.update_state is not None:
             jdict['updatestate'] = self.update_state
 
         if self.check_for_update is not None:
             jdict['checkforupdate'] = self.check_for_update
@@ -162,15 +162,15 @@
         self.__bridge = bool(bridge)                # bool
         self.__lights = lights                      # array
         self.__sensors = sensors                    # array
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['bridge'] = self.bridge
         jdict['lights'] = self.lights
         jdict['sensors'] = self.sensors
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/sw_update_2.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/sw_update_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         self.__bridge = bridge                                      # Bridge
         self.__auto_install = auto_install                          # AutoInstall
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['checkforupdate'] = self.check_for_update
         jdict['lastchange'] = self.last_change
         jdict['bridge'] = self.bridge
         jdict['state'] = self.state
         jdict['autoinstall'] = self.auto_install
@@ -132,15 +132,15 @@
         """
         self.__state = state                                # string
         self.__last_install = last_install                  # string (date / time)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['state'] = self.state
         jdict['lastinstall'] = self.last_install
 
         return jdict
 
@@ -191,15 +191,15 @@
         """
         self.__update_time = update_time                    # string (time)
         self.__on = bool(on)                                # bool
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['updatetime'] = self.update_time
         jdict['on'] = self.on
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/bridge/whitelist.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/bridge/whitelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Constructor
         """
         self.__entries = entries                    # array of WhitelistEntry
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         for entry in self.entries:
             jdict[entry.username] = entry
 
         return jdict
 
@@ -105,15 +105,15 @@
         self.__create_datetime = create_datetime                    # string (date / time)
 
         self.__description = description                            # ClientDescription
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['username'] = self.username
         jdict['last use date'] = self.last_use_datetime
         jdict['create date'] = self.create_datetime
 
         jdict['description'] = self.description
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/client/client_description.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/client/client_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         self.__app = app                    # string
         self.__user = user                  # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.app + self.__SEPARATOR + self.user
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def app(self):
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/client/device_description.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/client/device_description.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Constructor
         """
         self.__device_type = device_type                # ClientDescription
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['devicetype'] = self.device_type
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/chroma.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/chroma.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         """
         self.__x = round(float(x), 4)                   # float
         self.__y = round(float(y), 4)                   # float
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.x, self.y
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def x(self):
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/light.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         self.__sw_version = sw_version                          # string
         self.__sw_config_id = sw_config_id                      # string
         self.__product_id = product_id                          # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['state'] = self.state
         jdict['swupdate'] = self.swupdate
 
         jdict['type'] = self.light_type
         jdict['name'] = self.name
@@ -205,15 +205,15 @@
         """
         self.__index = index                            # index
         self.__light = light                            # Light
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict[self.index] = self.light
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/light_catalogue.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/light_catalogue.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def light(self, name):
         return self.__entries[name]                 # may raise KeyError
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.sorted_entries
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def sorted_entries(self):
@@ -126,15 +126,15 @@
         """
         self.__bridge_name = bridge_name                # string
         self.__index = int(index)                       # int
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['bridge-name'] = self.bridge_name
         jdict['index'] = self.index
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/light_device.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/light_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         Constructor
         """
         self.__ids = ids                        # list of string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['deviceid'] = self.ids
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/light_name.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/light_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         Constructor
         """
         self.__name = name                          # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['name'] = self.name
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/light_scan.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/light_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def is_active(self):
         return self.last_scan == 'active'
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['lastscan'] = self.last_scan
 
         for index, light in self.entries.items():
             jdict[index] = light
 
@@ -115,15 +115,15 @@
         """
         self.__index = index                            # index
         self.__name = name                              # LightName
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict[self.index] = self.name
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/light_state.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/light_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         self.__ct = ct                                  # uint16
         self.__alert = alert                            # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         if self.on is not None:
             jdict['on'] = self.on
 
         if self.bri is not None:
             jdict['bri'] = self.bri
@@ -225,15 +225,15 @@
 
         self.__color_mode = color_mode              # string
         self.__reachable = reachable                # bool
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['on'] = self.on
         jdict['bri'] = self.bri
         jdict['hue'] = self.hue
         jdict['sat'] = self.sat
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/data/light/sw_update.py` & `scs_hue-3.4.4/src/scs_philips_hue/data/light/sw_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
         self.__state = state                            # string
         self.__lastinstall = lastinstall                # string (date / time)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['state'] = self.state
         jdict['lastinstall'] = self.lastinstall
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/desk.py` & `scs_hue-3.4.4/src/scs_philips_hue/desk.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/desk_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/desk_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/discovery/discovery.py` & `scs_hue-3.4.4/src/scs_philips_hue/discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/discovery/ip_discovery.py` & `scs_hue-3.4.4/src/scs_philips_hue/discovery/ip_discovery.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/discovery/upnp_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/discovery/upnp_conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         super().__init__()
 
         self.__upnp_enabled = bool(upnp_enabled)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['upnp-enabled'] = self.upnp_enabled
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/discovery/upnp_discovery.py` & `scs_hue-3.4.4/src/scs_philips_hue/discovery/upnp_discovery.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/domain_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/domain_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/handler/aws_mqtt_subscription_handler.py` & `scs_hue-3.4.4/src/scs_philips_hue/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/join.py` & `scs_hue-3.4.4/src/scs_philips_hue/join.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/light.py` & `scs_hue-3.4.4/src/scs_philips_hue/light.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/manager/bridge_builder.py` & `scs_hue-3.4.4/src/scs_philips_hue/manager/bridge_builder.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/manager/bridge_manager.py` & `scs_hue-3.4.4/src/scs_philips_hue/manager/bridge_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         return self.__bridge_managers
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def items(self):
         return dict(sorted(self.__bridge_managers.items())).items()
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/manager/bridge_monitor.py` & `scs_hue-3.4.4/src/scs_philips_hue/manager/bridge_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/manager/light_manager.py` & `scs_hue-3.4.4/src/scs_philips_hue/manager/light_manager.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/manager/manager.py` & `scs_hue-3.4.4/src/scs_philips_hue/manager/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         self._host = host
         self._username = username
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
+    def as_json(self, *args, **kwargs):
         jdict = OrderedDict()
 
         jdict['host'] = self.host
         jdict['username'] = self.username
 
         return jdict
```

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/manager/user_manager.py` & `scs_hue-3.4.4/src/scs_philips_hue/manager/user_manager.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/node.py` & `scs_hue-3.4.4/src/scs_philips_hue/node.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/uds_receiver.py` & `scs_hue-3.4.4/src/scs_philips_hue/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/upnp_conf.py` & `scs_hue-3.4.4/src/scs_philips_hue/upnp_conf.py`

 * *Files identical despite different names*

### Comparing `scs-hue-3.4.2/src/scs_philips_hue/user.py` & `scs_hue-3.4.4/src/scs_philips_hue/user.py`

 * *Files identical despite different names*

