# Comparing `tmp/mktxp-1.2.3.tar.gz` & `tmp/mktxp-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktxp-1.2.3.tar", last modified: Sun Mar 10 14:26:26 2024, max compression
+gzip compressed data, was "mktxp-1.2.4.tar", last modified: Tue Apr 30 06:06:33 2024, max compression
```

## Comparing `mktxp-1.2.3.tar` & `mktxp-1.2.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.430431 mktxp-1.2.3/
--rw-r--r--   0 akpower    (501) staff       (20)      543 2024-01-10 19:35:46.000000 mktxp-1.2.3/LICENSE
--rw-r--r--   0 akpower    (501) staff       (20)    22162 2024-03-10 14:26:26.430192 mktxp-1.2.3/PKG-INFO
--rw-r--r--   0 akpower    (501) staff       (20)    20869 2024-03-10 12:47:25.000000 mktxp-1.2.3/README.md
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.411367 mktxp-1.2.3/mktxp/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/__init__.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.412857 mktxp-1.2.3/mktxp/cli/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/__init__.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.413261 mktxp-1.2.3/mktxp/cli/checks/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/checks/__init__.py
--rwxr-xr-x   0 akpower    (501) staff       (20)     1358 2024-03-09 15:42:11.000000 mktxp-1.2.3/mktxp/cli/checks/chk_pv.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.414211 mktxp-1.2.3/mktxp/cli/config/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/config/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     1551 2024-03-10 13:20:55.000000 mktxp-1.2.3/mktxp/cli/config/_mktxp.conf
--rwxr-xr-x   0 akpower    (501) staff       (20)    18437 2024-03-10 13:15:27.000000 mktxp-1.2.3/mktxp/cli/config/config.py
--rw-r--r--   0 akpower    (501) staff       (20)     2809 2024-03-02 17:03:35.000000 mktxp-1.2.3/mktxp/cli/config/mktxp.conf
--rwxr-xr-x   0 akpower    (501) staff       (20)     3777 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/dispatch.py
--rwxr-xr-x   0 akpower    (501) staff       (20)    11095 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/options.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.415423 mktxp-1.2.3/mktxp/cli/output/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/output/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2583 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/output/capsman_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2011 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/output/conn_stats_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2547 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/output/dhcp_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2908 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/cli/output/wifi_out.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.421358 mktxp-1.2.3/mktxp/collector/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     3100 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/bandwidth_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2804 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/base_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3732 2024-03-10 14:00:30.000000 mktxp-1.2.3/mktxp/collector/bgp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4931 2024-03-02 17:02:01.000000 mktxp-1.2.3/mktxp/collector/capsman_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2039 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/connection_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3122 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/dhcp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4122 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/firewall_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3741 2024-01-22 16:34:51.000000 mktxp-1.2.3/mktxp/collector/health_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1194 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/identity_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3554 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/interface_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1348 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/ipv6_neighbor_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3417 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/kid_control_device_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1144 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/mktxp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3828 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/monitor_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1461 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/netwatch_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1272 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/package_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1310 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/poe_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2326 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/pool_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1448 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/public_ip_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4067 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/queue_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4686 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/resource_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2888 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/route_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1216 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/user_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4734 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/collector/wlan_collector.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.427272 mktxp-1.2.3/mktxp/datasource/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2109 2024-03-03 13:13:09.000000 mktxp-1.2.3/mktxp/datasource/base_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1361 2024-03-03 12:18:07.000000 mktxp-1.2.3/mktxp/datasource/bgp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     4754 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/capsman_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3863 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/connection_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2670 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/dhcp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3508 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/firewall_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1880 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/health_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1321 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/identity_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3805 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/interface_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)      962 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/ipv6_neighbor_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1469 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/kid_control_device_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1169 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/mktxp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2102 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/netwatch_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1980 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/package_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3150 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/poe_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1987 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/pool_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1211 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/public_ip_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2120 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/queue_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1306 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/route_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2462 2024-01-22 16:34:51.000000 mktxp-1.2.3/mktxp/datasource/routerboard_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2210 2024-01-22 16:34:51.000000 mktxp-1.2.3/mktxp/datasource/system_resource_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1330 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/user_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2457 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/datasource/wireless_ds.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.428625 mktxp-1.2.3/mktxp/flow/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/flow/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     6060 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/flow/collector_handler.py
--rw-r--r--   0 akpower    (501) staff       (20)     4497 2024-03-02 17:07:07.000000 mktxp-1.2.3/mktxp/flow/collector_registry.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.429261 mktxp-1.2.3/mktxp/flow/processor/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/flow/processor/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2523 2024-03-10 10:35:43.000000 mktxp-1.2.3/mktxp/flow/processor/base_proc.py
--rw-r--r--   0 akpower    (501) staff       (20)     7939 2024-03-03 06:44:29.000000 mktxp-1.2.3/mktxp/flow/processor/output.py
--rw-r--r--   0 akpower    (501) staff       (20)     5478 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/flow/router_connection.py
--rw-r--r--   0 akpower    (501) staff       (20)     2392 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/flow/router_entries_handler.py
--rw-r--r--   0 akpower    (501) staff       (20)     6359 2024-03-02 17:07:56.000000 mktxp-1.2.3/mktxp/flow/router_entry.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.429657 mktxp-1.2.3/mktxp/utils/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.3/mktxp/utils/__init__.py
--rwxr-xr-x   0 akpower    (501) staff       (20)    12425 2024-01-22 16:34:51.000000 mktxp-1.2.3/mktxp/utils/utils.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-03-10 14:26:26.412269 mktxp-1.2.3/mktxp.egg-info/
--rw-r--r--   0 akpower    (501) staff       (20)    22162 2024-03-10 14:26:26.000000 mktxp-1.2.3/mktxp.egg-info/PKG-INFO
--rw-r--r--   0 akpower    (501) staff       (20)     2630 2024-03-10 14:26:26.000000 mktxp-1.2.3/mktxp.egg-info/SOURCES.txt
--rw-r--r--   0 akpower    (501) staff       (20)        1 2024-03-10 14:26:26.000000 mktxp-1.2.3/mktxp.egg-info/dependency_links.txt
--rw-r--r--   0 akpower    (501) staff       (20)       50 2024-03-10 14:26:26.000000 mktxp-1.2.3/mktxp.egg-info/entry_points.txt
--rw-r--r--   0 akpower    (501) staff       (20)      133 2024-03-10 14:26:26.000000 mktxp-1.2.3/mktxp.egg-info/requires.txt
--rw-r--r--   0 akpower    (501) staff       (20)        6 2024-03-10 14:26:26.000000 mktxp-1.2.3/mktxp.egg-info/top_level.txt
--rw-r--r--   0 akpower    (501) staff       (20)        1 2024-02-18 09:03:50.000000 mktxp-1.2.3/mktxp.egg-info/zip-safe
--rw-r--r--   0 akpower    (501) staff       (20)       38 2024-03-10 14:26:26.430487 mktxp-1.2.3/setup.cfg
--rwxr-xr-x   0 akpower    (501) staff       (20)     2581 2024-03-09 15:40:55.000000 mktxp-1.2.3/setup.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.946256 mktxp-1.2.4/
+-rw-r--r--   0 akpower    (501) staff       (20)      543 2024-01-10 19:35:46.000000 mktxp-1.2.4/LICENSE
+-rw-r--r--   0 akpower    (501) staff       (20)    23185 2024-04-30 06:06:33.945996 mktxp-1.2.4/PKG-INFO
+-rw-r--r--   0 akpower    (501) staff       (20)    21861 2024-04-23 08:51:14.000000 mktxp-1.2.4/README.md
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.924987 mktxp-1.2.4/mktxp/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/__init__.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.926734 mktxp-1.2.4/mktxp/cli/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/__init__.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.927159 mktxp-1.2.4/mktxp/cli/checks/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/checks/__init__.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)     1358 2024-03-09 15:42:11.000000 mktxp-1.2.4/mktxp/cli/checks/chk_pv.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.928130 mktxp-1.2.4/mktxp/cli/config/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/config/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1681 2024-03-30 06:02:31.000000 mktxp-1.2.4/mktxp/cli/config/_mktxp.conf
+-rwxr-xr-x   0 akpower    (501) staff       (20)    22620 2024-04-23 06:58:43.000000 mktxp-1.2.4/mktxp/cli/config/config.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3294 2024-04-23 08:50:01.000000 mktxp-1.2.4/mktxp/cli/config/mktxp.conf
+-rwxr-xr-x   0 akpower    (501) staff       (20)     3777 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/dispatch.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)    11096 2024-03-17 12:50:04.000000 mktxp-1.2.4/mktxp/cli/options.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.929119 mktxp-1.2.4/mktxp/cli/output/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2583 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/capsman_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2011 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/conn_stats_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2547 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/dhcp_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2908 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/wifi_out.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.935779 mktxp-1.2.4/mktxp/collector/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3096 2024-03-17 08:13:42.000000 mktxp-1.2.4/mktxp/collector/bandwidth_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2804 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/base_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3241 2024-04-01 13:52:18.000000 mktxp-1.2.4/mktxp/collector/bgp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4931 2024-03-02 17:02:01.000000 mktxp-1.2.4/mktxp/collector/capsman_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2039 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/connection_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3134 2024-03-31 06:18:54.000000 mktxp-1.2.4/mktxp/collector/dhcp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4122 2024-04-02 05:59:40.000000 mktxp-1.2.4/mktxp/collector/firewall_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3741 2024-01-22 16:34:51.000000 mktxp-1.2.4/mktxp/collector/health_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1194 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/identity_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3554 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/interface_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1348 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/ipv6_neighbor_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3130 2024-04-13 14:04:55.000000 mktxp-1.2.4/mktxp/collector/kid_control_device_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1144 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/mktxp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3528 2024-04-01 15:58:46.000000 mktxp-1.2.4/mktxp/collector/monitor_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     5308 2024-04-14 15:37:01.000000 mktxp-1.2.4/mktxp/collector/netwatch_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1272 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/package_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1310 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/poe_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2326 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/pool_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1448 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/public_ip_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4067 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/queue_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4090 2024-04-02 05:43:49.000000 mktxp-1.2.4/mktxp/collector/resource_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2888 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/route_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1216 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/user_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4734 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/wlan_collector.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.942610 mktxp-1.2.4/mktxp/datasource/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2109 2024-04-01 18:08:30.000000 mktxp-1.2.4/mktxp/datasource/base_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1373 2024-04-01 13:40:34.000000 mktxp-1.2.4/mktxp/datasource/bgp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4754 2024-03-31 15:33:27.000000 mktxp-1.2.4/mktxp/datasource/capsman_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3863 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/connection_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2639 2024-03-31 06:18:54.000000 mktxp-1.2.4/mktxp/datasource/dhcp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3508 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/firewall_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1880 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/health_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1321 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/identity_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3868 2024-04-01 15:55:46.000000 mktxp-1.2.4/mktxp/datasource/interface_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)      962 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/ipv6_neighbor_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1579 2024-04-13 14:02:36.000000 mktxp-1.2.4/mktxp/datasource/kid_control_device_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1169 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/mktxp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1873 2024-04-14 15:36:43.000000 mktxp-1.2.4/mktxp/datasource/netwatch_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1980 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/package_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3150 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/poe_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1987 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/pool_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1211 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/public_ip_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2120 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/queue_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1306 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/route_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2462 2024-01-22 16:34:51.000000 mktxp-1.2.4/mktxp/datasource/routerboard_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2271 2024-04-02 05:45:09.000000 mktxp-1.2.4/mktxp/datasource/system_resource_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1330 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/user_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2457 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/wireless_ds.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.944219 mktxp-1.2.4/mktxp/flow/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/flow/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     6046 2024-03-17 08:13:29.000000 mktxp-1.2.4/mktxp/flow/collector_handler.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4497 2024-03-02 17:07:07.000000 mktxp-1.2.4/mktxp/flow/collector_registry.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.944987 mktxp-1.2.4/mktxp/flow/processor/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/flow/processor/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2519 2024-03-17 08:14:01.000000 mktxp-1.2.4/mktxp/flow/processor/base_proc.py
+-rw-r--r--   0 akpower    (501) staff       (20)     8303 2024-04-14 09:33:28.000000 mktxp-1.2.4/mktxp/flow/processor/output.py
+-rw-r--r--   0 akpower    (501) staff       (20)     5550 2024-04-23 07:00:42.000000 mktxp-1.2.4/mktxp/flow/router_connection.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2392 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/flow/router_entries_handler.py
+-rw-r--r--   0 akpower    (501) staff       (20)     6359 2024-03-02 17:07:56.000000 mktxp-1.2.4/mktxp/flow/router_entry.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.945404 mktxp-1.2.4/mktxp/utils/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/utils/__init__.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)    12368 2024-03-28 14:56:49.000000 mktxp-1.2.4/mktxp/utils/utils.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.926108 mktxp-1.2.4/mktxp.egg-info/
+-rw-r--r--   0 akpower    (501) staff       (20)    23185 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/PKG-INFO
+-rw-r--r--   0 akpower    (501) staff       (20)     2630 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/SOURCES.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        1 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/dependency_links.txt
+-rw-r--r--   0 akpower    (501) staff       (20)       50 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/entry_points.txt
+-rw-r--r--   0 akpower    (501) staff       (20)      149 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/requires.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        6 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/top_level.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        1 2024-02-18 09:03:50.000000 mktxp-1.2.4/mktxp.egg-info/zip-safe
+-rw-r--r--   0 akpower    (501) staff       (20)       38 2024-04-30 06:06:33.946330 mktxp-1.2.4/setup.cfg
+-rwxr-xr-x   0 akpower    (501) staff       (20)     2623 2024-03-18 14:33:03.000000 mktxp-1.2.4/setup.py
```

### Comparing `mktxp-1.2.3/LICENSE` & `mktxp-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/PKG-INFO` & `mktxp-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktxp
-Version: 1.2.3
+Version: 1.2.4
 Summary: Prometheus Exporter for Mikrotik RouterOS devices
 Home-page: https://github.com/akpw/mktxp
 Author: Arseniy Kuznetsov
 Author-email: k.arseniy@gmail.com
 License: GNU General Public License v2 (GPLv2)
 Keywords: Mikrotik RouterOS Prometheus Exporter
 Classifier: Development Status :: 4 - Beta
@@ -26,27 +26,28 @@
 Requires-Dist: prometheus-client>=0.9.0
 Requires-Dist: RouterOS-api>=0.17.0
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: humanize>=3.2.0
 Requires-Dist: texttable>=1.6.3
 Requires-Dist: speedtest-cli>=2.1.2
 Requires-Dist: waitress>=3.0.0
+Requires-Dist: packaging>=24.0
 
 
 ![License](https://img.shields.io/badge/License-GNU%20GPL-blue.svg)
-![Language](https://img.shields.io/badge/python-v3.6-blue)
+![Language](https://img.shields.io/badge/python-v3.8-blue)
 ![License](https://img.shields.io/badge/mikrotik-routeros-orange)
 ![License](https://img.shields.io/badge/prometheus-exporter-blueviolet)
 
 
 ## Description
 MKTXP is a Prometheus Exporter for Mikrotik RouterOS devices.\
 It gathers and exports a rich set of metrics across multiple routers, all easily configurable via built-in CLI interface. 
 
-While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, etc.
+While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, optional bandwidth testing, etc.
 
 Apart from exporting to Prometheus, MKTXP can print selected metrics directly on the command line (see examples below). 
 
 For effortless visualization of the RouterOS metrics exported to Prometheus, MKTXP comes with a dedicated [Grafana dashboard](https://grafana.com/grafana/dashboards/13679):
 
 <img width="32%" alt="1" src="https://user-images.githubusercontent.com/5028474/217029083-3c2f561e-853f-45a7-b9f1-d818a830daf5.png"> <img width="32%" alt="2" src="https://user-images.githubusercontent.com/5028474/217029092-2b86b41b-1f89-4383-ac48-16652e820f7e.png"> <img width="32%" alt="3" src="https://user-images.githubusercontent.com/5028474/217029096-dbf6b46c-3ed7-4c76-a57b-8cebfb3b671c.png">
 
@@ -79,26 +80,36 @@
 
 
 ## Getting started
 To get started with MKTXP, you need to edit its main configuration file. This essentially involves filling in your Mikrotik devices IP addresses & authentication info, optionally modifying various settings to specific needs. 
 
 The default configuration file comes with a sample configuration, making it easy to copy / edit parameters for your RouterOS devices as needed:
 ```
-[Sample-Router]
-    enabled = False         # turns metrics collection for this RouterOS device on / off
-    
+[Sample-Router-1]
+    # for specific configuration on the router level, overload the defaults here
+    hostname = 192.168.88.1
+
+[Sample-Router-2]
+    # for specific configuration on the router level, overload the defaults here
+    hostname = 192.168.88.2
+
+[default]
+    # this affects configuration of all routers, unless overloaded on their specific levels
+    enabled = True          # turns metrics collection for this RouterOS device on / off
+
     hostname = localhost    # RouterOS IP address
-    port = 8728             # RouterOS API / API-SSL service port
+    port = 8728             # RouterOS IP Port
     
     username = username     # RouterOS user, needs to have 'read' and 'api' permissions
     password = password
     
     use_ssl = False                 # enables connection via API-SSL servis
     no_ssl_certificate = False      # enables API_SSL connect without router SSL certificate
     ssl_certificate_verify = False  # turns SSL certificate verification on / off   
+    plaintext_login = True          # for legacy RouterOS versions below 6.43 use False
 
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
@@ -116,15 +127,16 @@
     public_ip = True                # Public IP metrics
     route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
-    kid_control_devices = False     # Kid Control metrics 
+    kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
+    kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
 
     bgp = False                     # BGP sessions metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
@@ -132,14 +144,15 @@
     use_comments_over_names = True  # when available, forces using comments over the interfaces names
 
     check_for_updates = False       # check for available ROS updates
 ```
 
 Most options are easy to understand at first glance, and some are described in more details [later](https://github.com/akpw/mktxp#advanced-features).
 
+<sup>💡</sup> To automatically migrate from the older `mktxp.conf` format in the existing installs, just set `compact_default_conf_values = True` in [the mktxp system config](https://github.com/akpw/mktxp#mktxp-system-configuration)
 
 #### Local install
 If you have a local MKTXP installation, you can edit the configuration file with your default system editor directly from mktxp:
 ```bash
 ❯ mktxp edit
 ```
 In case you prefer a different editor, run the ```edit``` command with its optional `-ed` parameter:
@@ -162,15 +175,15 @@
 ```
 docker run -v "$(pwd)/mktxp:/home/mktxp/mktxp/" -p 49090:49090 -it --rm ghcr.io/akpw/mktxp:latest
 ```
 
 #### MKTXP stack install
 [MKTXP Stack Getting Started](https://github.com/akpw/mktxp-stack#install--getting-started) provides similar instructions around editing the mktxp.conf file and, if needed, adding a dedicated API user to your Mikrotik RouterOS devices as mentioned below.
 
-💡 *In the case of usage within a [Docker Swarm](https://docs.docker.com/engine/swarm/), please do make sure to have all settings explicitly set in both the `mktxp.conf` and `_mktxp.conf` files.  Not doing this may cause [issues](https://github.com/akpw/mktxp/issues/55#issuecomment-1346693843) regarding a `read-only` filesystem.*
+<sup>💡</sup> *In the case of usage within a [Docker Swarm](https://docs.docker.com/engine/swarm/), please do make sure to have all settings explicitly set in both the `mktxp.conf` and `_mktxp.conf` files.  Not doing this may cause [issues](https://github.com/akpw/mktxp/issues/55#issuecomment-1346693843) regarding a `read-only` filesystem.*
 
 ## Mikrotik Device Config
 For the purpose of RouterOS device monitoring, it's best to create a dedicated user with minimal required permissions. \
 MKTXP only needs ```API``` and ```Read```, so at that point you can go to your router's terminal and type:
 ```
 /user group add name=mktxp_group policy=api,read
 /user add name=mktxp_user group=mktxp_group password=mktxp_user_password
@@ -255,18 +268,20 @@
 
     bandwidth = False               # Turns metrics bandwidth metrics collection on / off    
     bandwidth_test_interval = 600   # Interval for colllecting bandwidth metrics
     minimal_collect_interval = 5    # Minimal metric collection interval
 
     verbose_mode = False            # Set it on for troubleshooting
 
-    fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
+    fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers in parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
     total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
+
+    compact_default_conf_values = False # Compact mktxp.conf, so only specific values are kept on the individual routers' level    
 ```    
 <sup>💡</sup> *When changing the default mktxp port for [docker image installs](https://github.com/akpw/mktxp#docker-image-install), you'll need to adjust the `docker run ... -p 49090:49090 ...` command to reflect the new port*
 
 ## Grafana dashboard
 Now with your RouterOS metrics being exported to Prometheus, it's easy to visualize them with this [Grafana dashboard](https://grafana.com/grafana/dashboards/13679)
 
 
@@ -352,15 +367,15 @@
 max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
 max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
 total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
 ```
 To keeps things within expected boundaries, the last two parameters allows for controlling both individual and overall scrape durations
 
 
-### mktxp listening socket addresses
+### mktxp endpoint listen addresses
 By default, mktxp runs it's HTTP metrics endpoint on any IPv4 address on port 49090. However, it is also able to listen on multiple socket addresses, both IPv4 and IPv6. 
 You can configure this behaviour via the following [system option](https://github.com/akpw/mktxp/blob/main/README.md#mktxp-system-configuration), setting ```listen``` to a space-separated list of sockets to listen to, e.g.:
 ```
 listen = '0.0.0.0:49090 [::1]:49090'
 ```
 A wildcard for the hostname is supported as well, and binding to both IPv4/IPv6 as available.
```

### Comparing `mktxp-1.2.3/README.md` & `mktxp-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 ![License](https://img.shields.io/badge/License-GNU%20GPL-blue.svg)
-![Language](https://img.shields.io/badge/python-v3.6-blue)
+![Language](https://img.shields.io/badge/python-v3.8-blue)
 ![License](https://img.shields.io/badge/mikrotik-routeros-orange)
 ![License](https://img.shields.io/badge/prometheus-exporter-blueviolet)
 
 
 ## Description
 MKTXP is a Prometheus Exporter for Mikrotik RouterOS devices.\
 It gathers and exports a rich set of metrics across multiple routers, all easily configurable via built-in CLI interface. 
 
-While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, etc.
+While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, optional bandwidth testing, etc.
 
 Apart from exporting to Prometheus, MKTXP can print selected metrics directly on the command line (see examples below). 
 
 For effortless visualization of the RouterOS metrics exported to Prometheus, MKTXP comes with a dedicated [Grafana dashboard](https://grafana.com/grafana/dashboards/13679):
 
 <img width="32%" alt="1" src="https://user-images.githubusercontent.com/5028474/217029083-3c2f561e-853f-45a7-b9f1-d818a830daf5.png"> <img width="32%" alt="2" src="https://user-images.githubusercontent.com/5028474/217029092-2b86b41b-1f89-4383-ac48-16652e820f7e.png"> <img width="32%" alt="3" src="https://user-images.githubusercontent.com/5028474/217029096-dbf6b46c-3ed7-4c76-a57b-8cebfb3b671c.png">
 
@@ -46,26 +46,36 @@
 
 
 ## Getting started
 To get started with MKTXP, you need to edit its main configuration file. This essentially involves filling in your Mikrotik devices IP addresses & authentication info, optionally modifying various settings to specific needs. 
 
 The default configuration file comes with a sample configuration, making it easy to copy / edit parameters for your RouterOS devices as needed:
 ```
-[Sample-Router]
-    enabled = False         # turns metrics collection for this RouterOS device on / off
-    
+[Sample-Router-1]
+    # for specific configuration on the router level, overload the defaults here
+    hostname = 192.168.88.1
+
+[Sample-Router-2]
+    # for specific configuration on the router level, overload the defaults here
+    hostname = 192.168.88.2
+
+[default]
+    # this affects configuration of all routers, unless overloaded on their specific levels
+    enabled = True          # turns metrics collection for this RouterOS device on / off
+
     hostname = localhost    # RouterOS IP address
-    port = 8728             # RouterOS API / API-SSL service port
+    port = 8728             # RouterOS IP Port
     
     username = username     # RouterOS user, needs to have 'read' and 'api' permissions
     password = password
     
     use_ssl = False                 # enables connection via API-SSL servis
     no_ssl_certificate = False      # enables API_SSL connect without router SSL certificate
     ssl_certificate_verify = False  # turns SSL certificate verification on / off   
+    plaintext_login = True          # for legacy RouterOS versions below 6.43 use False
 
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
@@ -83,15 +93,16 @@
     public_ip = True                # Public IP metrics
     route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
-    kid_control_devices = False     # Kid Control metrics 
+    kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
+    kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
 
     bgp = False                     # BGP sessions metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
@@ -99,14 +110,15 @@
     use_comments_over_names = True  # when available, forces using comments over the interfaces names
 
     check_for_updates = False       # check for available ROS updates
 ```
 
 Most options are easy to understand at first glance, and some are described in more details [later](https://github.com/akpw/mktxp#advanced-features).
 
+<sup>💡</sup> To automatically migrate from the older `mktxp.conf` format in the existing installs, just set `compact_default_conf_values = True` in [the mktxp system config](https://github.com/akpw/mktxp#mktxp-system-configuration)
 
 #### Local install
 If you have a local MKTXP installation, you can edit the configuration file with your default system editor directly from mktxp:
 ```bash
 ❯ mktxp edit
 ```
 In case you prefer a different editor, run the ```edit``` command with its optional `-ed` parameter:
@@ -129,15 +141,15 @@
 ```
 docker run -v "$(pwd)/mktxp:/home/mktxp/mktxp/" -p 49090:49090 -it --rm ghcr.io/akpw/mktxp:latest
 ```
 
 #### MKTXP stack install
 [MKTXP Stack Getting Started](https://github.com/akpw/mktxp-stack#install--getting-started) provides similar instructions around editing the mktxp.conf file and, if needed, adding a dedicated API user to your Mikrotik RouterOS devices as mentioned below.
 
-💡 *In the case of usage within a [Docker Swarm](https://docs.docker.com/engine/swarm/), please do make sure to have all settings explicitly set in both the `mktxp.conf` and `_mktxp.conf` files.  Not doing this may cause [issues](https://github.com/akpw/mktxp/issues/55#issuecomment-1346693843) regarding a `read-only` filesystem.*
+<sup>💡</sup> *In the case of usage within a [Docker Swarm](https://docs.docker.com/engine/swarm/), please do make sure to have all settings explicitly set in both the `mktxp.conf` and `_mktxp.conf` files.  Not doing this may cause [issues](https://github.com/akpw/mktxp/issues/55#issuecomment-1346693843) regarding a `read-only` filesystem.*
 
 ## Mikrotik Device Config
 For the purpose of RouterOS device monitoring, it's best to create a dedicated user with minimal required permissions. \
 MKTXP only needs ```API``` and ```Read```, so at that point you can go to your router's terminal and type:
 ```
 /user group add name=mktxp_group policy=api,read
 /user add name=mktxp_user group=mktxp_group password=mktxp_user_password
@@ -222,18 +234,20 @@
 
     bandwidth = False               # Turns metrics bandwidth metrics collection on / off    
     bandwidth_test_interval = 600   # Interval for colllecting bandwidth metrics
     minimal_collect_interval = 5    # Minimal metric collection interval
 
     verbose_mode = False            # Set it on for troubleshooting
 
-    fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
+    fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers in parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
     total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
+
+    compact_default_conf_values = False # Compact mktxp.conf, so only specific values are kept on the individual routers' level    
 ```    
 <sup>💡</sup> *When changing the default mktxp port for [docker image installs](https://github.com/akpw/mktxp#docker-image-install), you'll need to adjust the `docker run ... -p 49090:49090 ...` command to reflect the new port*
 
 ## Grafana dashboard
 Now with your RouterOS metrics being exported to Prometheus, it's easy to visualize them with this [Grafana dashboard](https://grafana.com/grafana/dashboards/13679)
 
 
@@ -319,15 +333,15 @@
 max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
 max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
 total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
 ```
 To keeps things within expected boundaries, the last two parameters allows for controlling both individual and overall scrape durations
 
 
-### mktxp listening socket addresses
+### mktxp endpoint listen addresses
 By default, mktxp runs it's HTTP metrics endpoint on any IPv4 address on port 49090. However, it is also able to listen on multiple socket addresses, both IPv4 and IPv6. 
 You can configure this behaviour via the following [system option](https://github.com/akpw/mktxp/blob/main/README.md#mktxp-system-configuration), setting ```listen``` to a space-separated list of sockets to listen to, e.g.:
 ```
 listen = '0.0.0.0:49090 [::1]:49090'
 ```
 A wildcard for the hostname is supported as well, and binding to both IPv4/IPv6 as available.
```

### Comparing `mktxp-1.2.3/mktxp/cli/checks/chk_pv.py` & `mktxp-1.2.4/mktxp/cli/checks/chk_pv.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/cli/config/_mktxp.conf` & `mktxp-1.2.4/mktxp/cli/config/_mktxp.conf`

 * *Files 24% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 [MKTXP]
     listen = '0.0.0.0:49090'         # Space separated list of socket addresses to listen to, both IPV4 and IPV6
-    socket_timeout = 2
+    socket_timeout = 4
     
     initial_delay_on_failure = 120
     max_delay_on_failure = 900
     delay_inc_div = 5
 
     bandwidth = False                # Turns metrics bandwidth metrics collection on / off    
     bandwidth_test_interval = 600    # Interval for collecting bandwidth metrics
     minimal_collect_interval = 5     # Minimal metric collection interval
 
     verbose_mode = False             # Set it on for troubleshooting
 
     fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
-    max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
-    total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
+    max_scrape_duration = 30            # Max duration of individual routers' metrics collection (parallel fetch only)
+    total_max_scrape_duration = 90      # Max overall duration of all metrics collection (parallel fetch only)
+
+    compact_default_conf_values = False  # Compact mktxp.conf, so only specific values are kept on the individual routers' level
```

### Comparing `mktxp-1.2.3/mktxp/cli/config/config.py` & `mktxp-1.2.4/mktxp/cli/config/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import os
 import sys
 import shutil
 from collections import namedtuple
 from configobj import ConfigObj
 from abc import ABCMeta, abstractmethod
-from pkg_resources import Requirement, resource_filename
+import importlib.resources
 from mktxp.utils.utils import FSHelper
 
 
 ''' MKTXP conf file handling
 '''
 
 class CollectorKeys:
@@ -60,14 +60,15 @@
     LISTEN_KEY = 'listen'
     USER_KEY = 'username'
     PASSWD_KEY = 'password'
 
     SSL_KEY = 'use_ssl'
     NO_SSL_CERTIFICATE = 'no_ssl_certificate'
     SSL_CERTIFICATE_VERIFY = 'ssl_certificate_verify'
+    PLAINTEXT_LOGIN_KEY = 'plaintext_login'
 
     FE_PACKAGE_KEY = 'installed_packages'
     FE_DHCP_KEY = 'dhcp'
     FE_DHCP_LEASE_KEY = 'dhcp_lease'
     FE_DHCP_POOL_KEY = 'pool'
     FE_IP_CONNECTIONS_KEY = 'connections'
     FE_CONNECTION_STATS_KEY = 'connection_stats'
@@ -91,94 +92,101 @@
     FE_QUEUE_KEY = 'queue'
     FE_BGP_KEY = 'bgp'
 
     FE_REMOTE_DHCP_ENTRY = 'remote_dhcp_entry'
 
     FE_CHECK_FOR_UPDATES = 'check_for_updates'
 
-    FE_KID_CONTROL_DEVICE = 'kid_control_devices'
+    FE_KID_CONTROL_DEVICE = 'kid_control_assigned'
+    FE_KID_CONTROL_DYNAMIC = 'kid_control_dynamic'
 
     MKTXP_SOCKET_TIMEOUT = 'socket_timeout'
     MKTXP_INITIAL_DELAY = 'initial_delay_on_failure'
     MKTXP_MAX_DELAY = 'max_delay_on_failure'
     MKTXP_INC_DIV = 'delay_inc_div'
     MKTXP_BANDWIDTH_KEY = 'bandwidth'
     MKTXP_BANDWIDTH_TEST_INTERVAL = 'bandwidth_test_interval'
     MKTXP_VERBOSE_MODE = 'verbose_mode'
     MKTXP_MIN_COLLECT_INTERVAL = 'minimal_collect_interval'
     MKTXP_FETCH_IN_PARALLEL = 'fetch_routers_in_parallel'
     MKTXP_MAX_WORKER_THREADS = 'max_worker_threads'
     MKTXP_MAX_SCRAPE_DURATION = 'max_scrape_duration'
     MKTXP_TOTAL_MAX_SCRAPE_DURATION = 'total_max_scrape_duration'
+    MKTXP_COMPACT_CONFIG = 'compact_default_conf_values'
 
     # UnRegistered entries placeholder
     NO_ENTRIES_REGISTERED = 'NoEntriesRegistered'
 
     MKTXP_USE_COMMENTS_OVER_NAMES = 'use_comments_over_names'
 
     # Base router id labels
     ROUTERBOARD_NAME = 'routerboard_name'
     ROUTERBOARD_ADDRESS = 'routerboard_address'
 
-    # Default values
+    # Default values    
+    DEFAULT_HOST_KEY = 'localhost'
+    DEFAULT_USER_KEY = 'user'
+    DEFAULT_PASSWORD_KEY = 'password'    
+
     DEFAULT_API_PORT = 8728
     DEFAULT_API_SSL_PORT = 8729
     DEFAULT_FE_REMOTE_DHCP_ENTRY = 'None'
     DEFAULT_MKTXP_PORT = 49090
     DEFAULT_MKTXP_SOCKET_TIMEOUT = 2
     DEFAULT_MKTXP_INITIAL_DELAY = 120
     DEFAULT_MKTXP_MAX_DELAY = 900
     DEFAULT_MKTXP_INC_DIV = 5
     DEFAULT_MKTXP_BANDWIDTH_TEST_INTERVAL = 420
     DEFAULT_MKTXP_MIN_COLLECT_INTERVAL = 5
-    DEFAULT_MKTXP_FETCH_IN_PARALLEL = False
     DEFAULT_MKTXP_MAX_WORKER_THREADS = 5
     DEFAULT_MKTXP_MAX_SCRAPE_DURATION = 10
     DEFAULT_MKTXP_TOTAL_MAX_SCRAPE_DURATION = 30
 
 
-    BOOLEAN_KEYS_NO = {ENABLED_KEY, SSL_KEY, NO_SSL_CERTIFICATE, FE_CHECK_FOR_UPDATES, FE_KID_CONTROL_DEVICE,
+    BOOLEAN_KEYS_NO = {ENABLED_KEY, SSL_KEY, NO_SSL_CERTIFICATE, FE_CHECK_FOR_UPDATES, FE_KID_CONTROL_DEVICE, FE_KID_CONTROL_DYNAMIC,
                        SSL_CERTIFICATE_VERIFY, FE_IPV6_FIREWALL_KEY, FE_IPV6_NEIGHBOR_KEY, FE_CONNECTION_STATS_KEY, FE_BGP_KEY}
 
     # Feature keys enabled by default
-    BOOLEAN_KEYS_YES = {FE_DHCP_KEY, FE_PACKAGE_KEY, FE_DHCP_LEASE_KEY, FE_DHCP_POOL_KEY, FE_IP_CONNECTIONS_KEY, FE_INTERFACE_KEY, FE_FIREWALL_KEY,
-                        FE_MONITOR_KEY, FE_ROUTE_KEY, MKTXP_USE_COMMENTS_OVER_NAMES,
+    BOOLEAN_KEYS_YES = {PLAINTEXT_LOGIN_KEY, FE_DHCP_KEY, FE_PACKAGE_KEY, FE_DHCP_LEASE_KEY, FE_DHCP_POOL_KEY, FE_IP_CONNECTIONS_KEY, FE_INTERFACE_KEY, 
+                        FE_FIREWALL_KEY, FE_MONITOR_KEY, FE_ROUTE_KEY, MKTXP_USE_COMMENTS_OVER_NAMES,
                         FE_WIRELESS_KEY, FE_WIRELESS_CLIENTS_KEY, FE_CAPSMAN_KEY, FE_CAPSMAN_CLIENTS_KEY, FE_POE_KEY,
                         FE_NETWATCH_KEY, FE_PUBLIC_IP_KEY, FE_USER_KEY, FE_QUEUE_KEY}
 
     SYSTEM_BOOLEAN_KEYS_YES = set()
-    SYSTEM_BOOLEAN_KEYS_NO = {MKTXP_BANDWIDTH_KEY, MKTXP_VERBOSE_MODE, MKTXP_FETCH_IN_PARALLEL}
+    SYSTEM_BOOLEAN_KEYS_NO = {MKTXP_BANDWIDTH_KEY, MKTXP_VERBOSE_MODE, MKTXP_FETCH_IN_PARALLEL, MKTXP_COMPACT_CONFIG}
 
     STR_KEYS = (HOST_KEY, USER_KEY, PASSWD_KEY, FE_REMOTE_DHCP_ENTRY)
     INT_KEYS =  ()
     MKTXP_INT_KEYS = (PORT_KEY, MKTXP_SOCKET_TIMEOUT, MKTXP_INITIAL_DELAY, MKTXP_MAX_DELAY,
                       MKTXP_INC_DIV, MKTXP_BANDWIDTH_TEST_INTERVAL, MKTXP_MIN_COLLECT_INTERVAL,
                       MKTXP_MAX_WORKER_THREADS, MKTXP_MAX_SCRAPE_DURATION, MKTXP_TOTAL_MAX_SCRAPE_DURATION)
 
-    # MKTXP config entry name
+    # MKTXP configs entry names
+    DEFAULT_ENTRY_KEY = 'default'
     MKTXP_CONFIG_ENTRY_NAME = 'MKTXP'
 
 
 class ConfigEntry:
     MKTXPConfigEntry = namedtuple('MKTXPConfigEntry', [MKTXPConfigKeys.ENABLED_KEY, MKTXPConfigKeys.HOST_KEY, MKTXPConfigKeys.PORT_KEY,
                                                        MKTXPConfigKeys.USER_KEY, MKTXPConfigKeys.PASSWD_KEY,
-                                                       MKTXPConfigKeys.SSL_KEY, MKTXPConfigKeys.NO_SSL_CERTIFICATE, MKTXPConfigKeys.SSL_CERTIFICATE_VERIFY,
+                                                       MKTXPConfigKeys.SSL_KEY, MKTXPConfigKeys.NO_SSL_CERTIFICATE, MKTXPConfigKeys.SSL_CERTIFICATE_VERIFY, MKTXPConfigKeys.PLAINTEXT_LOGIN_KEY,
                                                        MKTXPConfigKeys.FE_DHCP_KEY, MKTXPConfigKeys.FE_PACKAGE_KEY, MKTXPConfigKeys.FE_DHCP_LEASE_KEY, MKTXPConfigKeys.FE_DHCP_POOL_KEY, MKTXPConfigKeys.FE_INTERFACE_KEY,
                                                        MKTXPConfigKeys.FE_FIREWALL_KEY, MKTXPConfigKeys.FE_MONITOR_KEY, MKTXPConfigKeys.FE_ROUTE_KEY, MKTXPConfigKeys.FE_WIRELESS_KEY, MKTXPConfigKeys.FE_WIRELESS_CLIENTS_KEY,
-                                                       MKTXPConfigKeys.FE_IP_CONNECTIONS_KEY, MKTXPConfigKeys.FE_CONNECTION_STATS_KEY, MKTXPConfigKeys.FE_CAPSMAN_KEY, MKTXPConfigKeys.FE_CAPSMAN_CLIENTS_KEY, MKTXPConfigKeys.FE_POE_KEY, MKTXPConfigKeys.FE_NETWATCH_KEY,
-                                                       MKTXPConfigKeys.MKTXP_USE_COMMENTS_OVER_NAMES, MKTXPConfigKeys.FE_PUBLIC_IP_KEY, MKTXPConfigKeys.FE_IPV6_FIREWALL_KEY, MKTXPConfigKeys.FE_IPV6_NEIGHBOR_KEY,
-                                                       MKTXPConfigKeys.FE_USER_KEY, MKTXPConfigKeys.FE_QUEUE_KEY, MKTXPConfigKeys.FE_REMOTE_DHCP_ENTRY, MKTXPConfigKeys.FE_CHECK_FOR_UPDATES, MKTXPConfigKeys.FE_KID_CONTROL_DEVICE, MKTXPConfigKeys.FE_BGP_KEY,
+                                                       MKTXPConfigKeys.FE_IP_CONNECTIONS_KEY, MKTXPConfigKeys.FE_CONNECTION_STATS_KEY, MKTXPConfigKeys.FE_CAPSMAN_KEY, MKTXPConfigKeys.FE_CAPSMAN_CLIENTS_KEY, MKTXPConfigKeys.FE_POE_KEY, 
+                                                       MKTXPConfigKeys.FE_NETWATCH_KEY, MKTXPConfigKeys.MKTXP_USE_COMMENTS_OVER_NAMES, MKTXPConfigKeys.FE_PUBLIC_IP_KEY, MKTXPConfigKeys.FE_IPV6_FIREWALL_KEY, MKTXPConfigKeys.FE_IPV6_NEIGHBOR_KEY,
+                                                       MKTXPConfigKeys.FE_USER_KEY, MKTXPConfigKeys.FE_QUEUE_KEY, MKTXPConfigKeys.FE_REMOTE_DHCP_ENTRY, MKTXPConfigKeys.FE_CHECK_FOR_UPDATES, MKTXPConfigKeys.FE_BGP_KEY,
+                                                       MKTXPConfigKeys.FE_KID_CONTROL_DEVICE, MKTXPConfigKeys.FE_KID_CONTROL_DYNAMIC
                                                        ])
     MKTXPSystemEntry = namedtuple('MKTXPSystemEntry', [MKTXPConfigKeys.PORT_KEY, MKTXPConfigKeys.LISTEN_KEY, MKTXPConfigKeys.MKTXP_SOCKET_TIMEOUT,
                                                        MKTXPConfigKeys.MKTXP_INITIAL_DELAY, MKTXPConfigKeys.MKTXP_MAX_DELAY,
                                                        MKTXPConfigKeys.MKTXP_INC_DIV, MKTXPConfigKeys.MKTXP_BANDWIDTH_KEY,
                                                        MKTXPConfigKeys.MKTXP_VERBOSE_MODE, MKTXPConfigKeys.MKTXP_BANDWIDTH_TEST_INTERVAL,
                                                        MKTXPConfigKeys.MKTXP_MIN_COLLECT_INTERVAL, MKTXPConfigKeys.MKTXP_FETCH_IN_PARALLEL,
                                                        MKTXPConfigKeys.MKTXP_MAX_WORKER_THREADS, MKTXPConfigKeys.MKTXP_MAX_SCRAPE_DURATION, 
-                                                       MKTXPConfigKeys.MKTXP_TOTAL_MAX_SCRAPE_DURATION])
+                                                       MKTXPConfigKeys.MKTXP_TOTAL_MAX_SCRAPE_DURATION, MKTXPConfigKeys.MKTXP_COMPACT_CONFIG])
 
 
 class OSConfig(metaclass=ABCMeta):
     ''' OS-related config
     '''
     @staticmethod
     def os_config():
@@ -253,163 +261,222 @@
         # if needed, stage the user config data
         self.usr_conf_data_path = os.path.join(
             self.os_config.mktxp_user_dir_path, 'mktxp.conf')
         self.mktxp_conf_path = os.path.join(
             self.os_config.mktxp_user_dir_path, '_mktxp.conf')
 
         self._create_os_path(self.usr_conf_data_path,
-                             'mktxp/cli/config/mktxp.conf')
+                             'cli/config/mktxp.conf')
         self._create_os_path(self.mktxp_conf_path,
-                             'mktxp/cli/config/_mktxp.conf')
+                             'cli/config/_mktxp.conf')
 
         self.re_compiled = {}
 
         self._read_from_disk()
 
+        self.default_config_entry_reader = self._default_config_entry_reader()
+        self.system_entry = self._system_entry()
+
     # MKTXP entries
     def registered_entries(self):
         ''' All MKTXP registered entries
         '''
-        return (entry_name for entry_name in self.config.keys())
+        return (entry_name for entry_name in self.config.keys() if entry_name != MKTXPConfigKeys.DEFAULT_ENTRY_KEY )
 
     def registered_entry(self, entry_name):
         ''' A specific MKTXP registered entry by name
         '''
         return self.config.get(entry_name)
 
     def config_entry(self, entry_name):
         ''' Given an entry name, reads and returns the entry info
         '''
         entry_reader = self._config_entry_reader(entry_name)
         return ConfigEntry.MKTXPConfigEntry(**entry_reader) if entry_reader else None
 
-    def system_entry(self):
+    # Helpers
+    def _system_entry(self):
         ''' MKTXP internal config entry
         '''
         _entry_reader = self._system_entry_reader()
         return ConfigEntry.MKTXPSystemEntry(**_entry_reader)
 
-    # Helpers
     def _read_from_disk(self):
         ''' (Force-)Read conf data from disk
         '''
         self.config = ConfigObj(self.usr_conf_data_path, indent_type = '    ')
         self.config.preserve_comments = True
 
         self._config = ConfigObj(self.mktxp_conf_path, indent_type = '    ')
         self._config.preserve_comments = True
 
     def _create_os_path(self, os_path, resource_path):
         if not os.path.exists(os_path):
             # stage from the conf templates
-            lookup_path = resource_filename(
-                Requirement.parse("mktxp"), resource_path)
-            shutil.copy(lookup_path, os_path)
+            ref = importlib.resources.files('mktxp') / resource_path
+            with importlib.resources.as_file(ref) as path:
+                shutil.copy(path, os_path)
+
+    def _system_entry_reader(self):
+        system_entry_reader = {}
+        entry_name = MKTXPConfigKeys.MKTXP_CONFIG_ENTRY_NAME
+        new_keys = []
+
+        for key in MKTXPConfigKeys.MKTXP_INT_KEYS:
+            if self._config[entry_name].get(key):
+                system_entry_reader[key] = self._config[entry_name].as_int(key)
+            else:
+                system_entry_reader[key] = self._default_value_for_key(key)
+                if key not in (MKTXPConfigKeys.PORT_KEY):  # Port key has been depricated
+                    new_keys.append(key) # read from disk next time
+
+        for key in MKTXPConfigKeys.SYSTEM_BOOLEAN_KEYS_NO.union(MKTXPConfigKeys.SYSTEM_BOOLEAN_KEYS_YES):
+            if self._config[entry_name].get(key) is not None:
+                system_entry_reader[key] = self._config[entry_name].as_bool(key)
+            else:
+                system_entry_reader[key] = True if key in MKTXPConfigKeys.SYSTEM_BOOLEAN_KEYS_YES else False
+                new_keys.append(key) # read from disk next time
+
+        # listen 
+        if self._config[entry_name].get(MKTXPConfigKeys.LISTEN_KEY):
+            system_entry_reader[MKTXPConfigKeys.LISTEN_KEY] = self._config[entry_name].get(MKTXPConfigKeys.LISTEN_KEY)
+        else:
+            system_entry_reader[MKTXPConfigKeys.LISTEN_KEY] = f'0.0.0.0:{system_entry_reader[MKTXPConfigKeys.PORT_KEY]}'
+            new_keys.append(MKTXPConfigKeys.LISTEN_KEY) # read from disk next time
+
+        if new_keys:
+            self._config[entry_name] = system_entry_reader
+            try:
+                self._config[entry_name].pop(MKTXPConfigKeys.PORT_KEY, None) # Port key has been depricated
+                self._config.write()
+                if self._config[entry_name].as_bool(MKTXPConfigKeys.MKTXP_VERBOSE_MODE):
+                    print(f'Updated system entry {entry_name} with new system keys {new_keys}')    
+            except Exception as exc:
+                print(f'Error updating system entry {entry_name} with new system keys {new_keys}: {exc}')
+                print('Please update _mktxp.conf to its latest version manually')
+
+        return system_entry_reader
 
     def _config_entry_reader(self, entry_name):
         config_entry_reader = {}
-        new_keys = []
+        compact_config = self._config[MKTXPConfigKeys.MKTXP_CONFIG_ENTRY_NAME].as_bool(MKTXPConfigKeys.MKTXP_COMPACT_CONFIG)
+        drop_keys = []
 
         for key in MKTXPConfigKeys.BOOLEAN_KEYS_NO.union(MKTXPConfigKeys.BOOLEAN_KEYS_YES):
             if self.config[entry_name].get(key) is not None:
                 config_entry_reader[key] = self.config[entry_name].as_bool(key)
+                if compact_config and config_entry_reader[key] == self.default_config_entry_reader[key]:
+                    drop_keys.append(key)
             else:
-                config_entry_reader[key] = True if key in MKTXPConfigKeys.BOOLEAN_KEYS_YES else False
-                new_keys.append(key) # read from disk next time
+                config_entry_reader[key] = self.default_config_entry_reader[key]
 
         for key in MKTXPConfigKeys.STR_KEYS:
             if self.config[entry_name].get(key):
                 config_entry_reader[key] = self.config[entry_name].get(key)
-            else:
-                config_entry_reader[key] = self._default_value_for_key(key)
-                new_keys.append(key) # read from disk next time
+                if key is MKTXPConfigKeys.PASSWD_KEY and type(config_entry_reader[key]) is list:
+                    config_entry_reader[key] = ','.join(config_entry_reader[key])         
 
-            if key is MKTXPConfigKeys.PASSWD_KEY and type(config_entry_reader[key]) is list:
-                config_entry_reader[key] = ','.join(config_entry_reader[key])
+                if compact_config and config_entry_reader[key] == self.default_config_entry_reader[key]:
+                    drop_keys.append(key)
+            else:
+                config_entry_reader[key] = self.default_config_entry_reader[key]
 
         for key in MKTXPConfigKeys.INT_KEYS:
             if self.config[entry_name].get(key):
                 config_entry_reader[key] = self.config[entry_name].as_int(key)
+                if compact_config and config_entry_reader[key] == self.default_config_entry_reader[key]:
+                    drop_keys.append(key)                
             else:
-                config_entry_reader[key] = self._default_value_for_key(key)
-                new_keys.append(key) # read from disk next time
+                config_entry_reader[key] = self.default_config_entry_reader[key]
 
         # port
         if self.config[entry_name].get(MKTXPConfigKeys.PORT_KEY):
-            config_entry_reader[MKTXPConfigKeys.PORT_KEY] = self.config[entry_name].as_int(
-                MKTXPConfigKeys.PORT_KEY)
+            config_entry_reader[MKTXPConfigKeys.PORT_KEY] = self.config[entry_name].as_int(MKTXPConfigKeys.PORT_KEY)
+            if compact_config and config_entry_reader[MKTXPConfigKeys.PORT_KEY] == self.default_config_entry_reader[MKTXPConfigKeys.PORT_KEY]:
+                drop_keys.append(MKTXPConfigKeys.PORT_KEY)    
         else:
-            config_entry_reader[MKTXPConfigKeys.PORT_KEY] = self._default_value_for_key(
-                MKTXPConfigKeys.SSL_KEY, config_entry_reader[MKTXPConfigKeys.SSL_KEY])
-            new_keys.append(MKTXPConfigKeys.PORT_KEY) # read from disk next time
-        
-        if new_keys:
-            self.config[entry_name] = config_entry_reader
+            config_entry_reader[MKTXPConfigKeys.PORT_KEY] = self.default_config_entry_reader[MKTXPConfigKeys.PORT_KEY]
+
+        # If allowed, compact mktxp.conf entry
+        if drop_keys and compact_config:
+            for key in drop_keys:
+                self.config[entry_name].pop(key, None)
             try:
                 self.config.write()
                 if self._config[MKTXPConfigKeys.MKTXP_CONFIG_ENTRY_NAME].as_bool(MKTXPConfigKeys.MKTXP_VERBOSE_MODE):
-                    print(f'Updated router entry {entry_name} with new feature keys {new_keys}')                    
+                    print(f'compacted router entry {entry_name} for default values of the feature keys {drop_keys}')                    
             except Exception as exc:
-                print(f'Error updating router entry {entry_name} with new feature keys {new_keys}: {exc}')
-                print('Please update mktxp.conf to its latest version manually')
+                print(f'Error compacting router entry {entry_name} for default values of feature keys {drop_keys}: {exc}')
+                print(f'Error compacting router entry {entry_name} for default values of feature keys {drop_keys}: {exc}')
+                print('Please compact mktxp.conf manually')
 
         return config_entry_reader
 
-    def _system_entry_reader(self):
-        system_entry_reader = {}
-        entry_name = MKTXPConfigKeys.MKTXP_CONFIG_ENTRY_NAME
+    def _default_config_entry_reader(self):
+        default_config_entry_reader = {}
         new_keys = []
 
-        for key in MKTXPConfigKeys.MKTXP_INT_KEYS:
-            if self._config[entry_name].get(key):
-                system_entry_reader[key] = self._config[entry_name].as_int(key)
+        if not self.config.get(MKTXPConfigKeys.DEFAULT_ENTRY_KEY):
+            self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY] = {}
+
+        for key in MKTXPConfigKeys.BOOLEAN_KEYS_NO.union(MKTXPConfigKeys.BOOLEAN_KEYS_YES):
+            if self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].get(key) is not None:
+                default_config_entry_reader[key] = self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].as_bool(key)
             else:
-                system_entry_reader[key] = self._default_value_for_key(key)
-                if key not in (MKTXPConfigKeys.PORT_KEY):  # Port key has been depricated
-                    new_keys.append(key) # read from disk next time
+                default_config_entry_reader[key] = True if key in MKTXPConfigKeys.BOOLEAN_KEYS_YES else False
+                new_keys.append(key) # read from disk next time
 
-        for key in MKTXPConfigKeys.SYSTEM_BOOLEAN_KEYS_NO.union(MKTXPConfigKeys.SYSTEM_BOOLEAN_KEYS_YES):
-            if self._config[entry_name].get(key) is not None:
-                system_entry_reader[key] = self._config[entry_name].as_bool(key)
+        for key in MKTXPConfigKeys.STR_KEYS:
+            if self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].get(key):
+                default_config_entry_reader[key] = self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].get(key)
             else:
-                system_entry_reader[key] = True if key in MKTXPConfigKeys.SYSTEM_BOOLEAN_KEYS_YES else False
+                default_config_entry_reader[key] = self._default_value_for_key(key)
                 new_keys.append(key) # read from disk next time
 
-        # listen 
-        if self._config[entry_name].get(MKTXPConfigKeys.LISTEN_KEY):
-            system_entry_reader[MKTXPConfigKeys.LISTEN_KEY] = self._config[entry_name].get(MKTXPConfigKeys.LISTEN_KEY)
-        else:
-            system_entry_reader[MKTXPConfigKeys.LISTEN_KEY] = f'0.0.0.0:{system_entry_reader[MKTXPConfigKeys.PORT_KEY]}'
-            new_keys.append(MKTXPConfigKeys.LISTEN_KEY) # read from disk next time
+        for key in MKTXPConfigKeys.INT_KEYS:
+            if self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].get(key):
+                default_config_entry_reader[key] = self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].as_int(key)
+            else:
+                default_config_entry_reader[key] = self._default_value_for_key(key)
+                new_keys.append(key) # read from disk next time
 
+        # port
+        if self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].get(MKTXPConfigKeys.PORT_KEY):
+            default_config_entry_reader[MKTXPConfigKeys.PORT_KEY] = self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY].as_int(MKTXPConfigKeys.PORT_KEY)
+        else:
+            default_config_entry_reader[MKTXPConfigKeys.PORT_KEY] = self._default_value_for_key(
+                MKTXPConfigKeys.SSL_KEY, default_config_entry_reader[MKTXPConfigKeys.SSL_KEY])
+            new_keys.append(MKTXPConfigKeys.PORT_KEY) # read from disk next time
+        
         if new_keys:
-            self._config[entry_name] = system_entry_reader
+            self.config[MKTXPConfigKeys.DEFAULT_ENTRY_KEY] = default_config_entry_reader
             try:
-                self._config[entry_name].pop(MKTXPConfigKeys.PORT_KEY, None) # Port key has been depricated
-                self._config.write()
-                if self._config[entry_name].as_bool(MKTXPConfigKeys.MKTXP_VERBOSE_MODE):
-                    print(f'Updated system entry {entry_name} with new system keys {new_keys}')    
+                self.config.write()
+                if self._config[MKTXPConfigKeys.MKTXP_CONFIG_ENTRY_NAME].as_bool(MKTXPConfigKeys.MKTXP_VERBOSE_MODE):
+                    print(f'Updated default router entry with new feature keys {new_keys}')                    
             except Exception as exc:
-                print(f'Error updating system entry {entry_name} with new system keys {new_keys}: {exc}')
-                print('Please update _mktxp.conf to its latest version manually')
+                print(f'Error updating default router entry with new feature keys {new_keys}: {exc}')
+                print('Please update mktxp.conf to its latest version manually')
 
-        return system_entry_reader
+        return default_config_entry_reader
 
     def _default_value_for_key(self, key, value=None):
         return {
             MKTXPConfigKeys.SSL_KEY: lambda value: MKTXPConfigKeys.DEFAULT_API_SSL_PORT if value else MKTXPConfigKeys.DEFAULT_API_PORT,
+            MKTXPConfigKeys.HOST_KEY: lambda _: MKTXPConfigKeys.DEFAULT_HOST_KEY,
+            MKTXPConfigKeys.USER_KEY: lambda _: MKTXPConfigKeys.DEFAULT_USER_KEY,
+            MKTXPConfigKeys.PASSWD_KEY: lambda _: MKTXPConfigKeys.DEFAULT_PASSWORD_KEY,
             MKTXPConfigKeys.PORT_KEY: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_PORT,
             MKTXPConfigKeys.FE_REMOTE_DHCP_ENTRY:  lambda _: MKTXPConfigKeys.DEFAULT_FE_REMOTE_DHCP_ENTRY,
             MKTXPConfigKeys.MKTXP_SOCKET_TIMEOUT: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_SOCKET_TIMEOUT,
             MKTXPConfigKeys.MKTXP_INITIAL_DELAY: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_INITIAL_DELAY,
             MKTXPConfigKeys.MKTXP_MAX_DELAY: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_MAX_DELAY,
             MKTXPConfigKeys.MKTXP_INC_DIV: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_INC_DIV,
             MKTXPConfigKeys.MKTXP_BANDWIDTH_TEST_INTERVAL: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_BANDWIDTH_TEST_INTERVAL,
             MKTXPConfigKeys.MKTXP_MIN_COLLECT_INTERVAL: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_MIN_COLLECT_INTERVAL,
-            MKTXPConfigKeys.MKTXP_FETCH_IN_PARALLEL: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_FETCH_IN_PARALLEL,
             MKTXPConfigKeys.MKTXP_MAX_WORKER_THREADS: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_MAX_WORKER_THREADS,
             MKTXPConfigKeys.MKTXP_MAX_SCRAPE_DURATION: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_MAX_SCRAPE_DURATION,
             MKTXPConfigKeys.MKTXP_TOTAL_MAX_SCRAPE_DURATION: lambda _: MKTXPConfigKeys.DEFAULT_MKTXP_TOTAL_MAX_SCRAPE_DURATION,
         }[key](value)
 
 
 # Simplest possible Singleton impl
```

### Comparing `mktxp-1.2.3/mktxp/cli/dispatch.py` & `mktxp-1.2.4/mktxp/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/cli/options.py` & `mktxp-1.2.4/mktxp/cli/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 ## This program is distributed in the hope that it will be useful,
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 import os
-import pkg_resources
 from argparse import ArgumentParser, HelpFormatter
 from mktxp.cli.config.config import config_handler, MKTXPConfigKeys, CustomConfig
 from mktxp.utils.utils import FSHelper, UniquePartialMatchList, run_cmd
-
+from importlib.metadata import version as Version
 
 class MKTXPCommands:
     INFO = 'info'
     EDIT = 'edit'
     EXPORT = 'export'
     PRINT = 'print'
     SHOW = 'show'
@@ -37,15 +36,15 @@
                         '}'))
 
 class MKTXPOptionsParser:
     ''' Base MKTXP Options Parser
     '''
     def __init__(self):
         self._script_name = f'MKTXP'
-        version = pkg_resources.require("mktxp")[0].version
+        version = Version('mktxp')
         self._description =  \
 f'''
 Prometheus Exporter for Mikrotik RouterOS, version {version}
 Supports gathering metrics across multiple RouterOS devices, all easily configurable via built-in CLI interface.
 Comes along with a dedicated Grafana dashboard (https://grafana.com/grafana/dashboards/13679)
 Selected metrics info can be printed on the command line. For more information, run: 'mktxp -h'
 '''
@@ -228,15 +227,15 @@
     @staticmethod
     def _system_editor():
         editor = os.environ.get('EDITOR')
         if editor:
             return editor
 
         commands = ['which nano', 'which vi', 'which vim']
-        quiet = not config_handler.system_entry().verbose_mode
+        quiet = not config_handler.system_entry.verbose_mode
         for command in commands:
             editor = run_cmd(command, quiet = quiet).rstrip()
             if editor:
                 break                                  
         return editor
```

### Comparing `mktxp-1.2.3/mktxp/cli/output/capsman_out.py` & `mktxp-1.2.4/mktxp/cli/output/capsman_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/cli/output/conn_stats_out.py` & `mktxp-1.2.4/mktxp/cli/output/conn_stats_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/cli/output/dhcp_out.py` & `mktxp-1.2.4/mktxp/cli/output/dhcp_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/cli/output/wifi_out.py` & `mktxp-1.2.4/mktxp/cli/output/wifi_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/bandwidth_collector.py` & `mktxp-1.2.4/mktxp/collector/bandwidth_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ''' MKTXP collector
     '''    
     def __init__(self):
         self.pool = Pool()
         self.last_call_timestamp = 0        
     
     def collect(self):
-        if not config_handler.system_entry().bandwidth:
+        if not config_handler.system_entry.bandwidth:
             return
 
         if result_list:      
             result_dict = result_list[0]
             bandwidth_records = [{'direction': key, 'bandwidth': str(result_dict[key])} for key in ('download', 'upload')]     
             bandwidth_metrics = BaseCollector.gauge_collector('internet_bandwidth', 'Internet bandwidth in bits per second', 
                                                                             bandwidth_records, 'bandwidth', ['direction'], add_id_labels = False)
@@ -45,15 +45,15 @@
 
             latency_records = [{'latency': str(result_dict['ping'])}]
             latency_metrics = BaseCollector.gauge_collector('internet_latency', 'Internet latency in milliseconds', 
                                                                             latency_records, 'latency', [], add_id_labels = False)
             yield latency_metrics
 
         ts =  datetime.now().timestamp()       
-        if (ts - self.last_call_timestamp) > config_handler.system_entry().bandwidth_test_interval:
+        if (ts - self.last_call_timestamp) > config_handler.system_entry.bandwidth_test_interval:
             self.pool.apply_async(BandwidthCollector.bandwidth_worker, callback=get_result)            
             self.last_call_timestamp = ts
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
```

### Comparing `mktxp-1.2.3/mktxp/collector/base_collector.py` & `mktxp-1.2.4/mktxp/collector/base_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/bgp_collector.py` & `mktxp-1.2.4/mktxp/collector/bgp_collector.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,26 +21,21 @@
     '''BGP collector'''
     @staticmethod
     def collect(router_entry):
         if not router_entry.config_entry.bgp:
             return
 
         bgp_labels = ['name', 'remote_address', 'remote_as', 'local_as', 'remote_afi', 'local_afi', 'remote_messages', 'remote_bytes', 'local_messages', 'local_bytes', 'prefix_count', 'established', 'uptime']
-        bgp_records = BGPMetricsDataSource.metric_records(router_entry, metric_labels=bgp_labels)
+        translation_table = {
+                'established': lambda value: '1' if value=='true' else '0',
+                'uptime': lambda value: BaseOutputProcessor.parse_timedelta_milliseconds(value) if value else '0'
+                }
+        bgp_records = BGPMetricsDataSource.metric_records(router_entry, metric_labels=bgp_labels, translation_table = translation_table)
         
-
         if bgp_records:
-            # translate records to appropriate values
-            translated_fields = ['established', 'uptime']        
-            for bgp_record in bgp_records:
-                for translated_field in translated_fields:
-                    value = bgp_record.get(translated_field, None)    
-                    if value:            
-                        bgp_record[translated_field] = BGPCollector._translated_values(translated_field, value)
-
             session_info_labes = ['name', 'remote_address', 'remote_as', 'local_as', 'remote_afi', 'local_afi']
             bgp_sessions_metrics = BaseCollector.info_collector('bgp_sessions_info', 'BGP sessions info', bgp_records, session_info_labes)
             yield bgp_sessions_metrics
 
             session_id_labes = ['name']
             remote_messages_metrics = BaseCollector.counter_collector('bgp_remote_messages', 'Number of remote messages', bgp_records, 'remote_messages', session_id_labes)
             yield remote_messages_metrics
@@ -65,16 +60,7 @@
             established_metrics = BaseCollector.gauge_collector('bgp_established', 'BGP established', bgp_records, 'established', session_id_labes)
             yield established_metrics
 
 
             uptime_metrics = BaseCollector.gauge_collector('bgp_uptime', 'BGP uptime in milliseconds', bgp_records, 'uptime', session_id_labes)
             yield uptime_metrics
 
-
-    # Helpers
-    @staticmethod
-    def _translated_values(translated_field, value):
-        return {
-                'established': lambda value: '1' if value=='true' else '0',
-                'uptime': lambda value: BaseOutputProcessor.parse_timedelta_milliseconds(value)
-                }[translated_field](value)
-
```

### Comparing `mktxp-1.2.3/mktxp/collector/capsman_collector.py` & `mktxp-1.2.4/mktxp/collector/capsman_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/connection_collector.py` & `mktxp-1.2.4/mktxp/collector/connection_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/dhcp_collector.py` & `mktxp-1.2.4/mktxp/collector/dhcp_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,45 +15,44 @@
 from mktxp.cli.config.config import MKTXPConfigKeys
 from mktxp.collector.base_collector import BaseCollector
 from mktxp.datasource.dhcp_ds import DHCPMetricsDataSource
 
 
 class DHCPCollector(BaseCollector):
     ''' DHCP Metrics collector
-    '''    
+    '''
     @staticmethod
     def collect(router_entry):
         if not router_entry.config_entry.dhcp:
             return
 
-        dhcp_lease_labels = ['active_address', 'address', 'mac_address', 'host_name', 'comment', 'server', 'expires_after']
-        dhcp_lease_records = DHCPMetricsDataSource.metric_records(router_entry, metric_labels = dhcp_lease_labels)   
+        dhcp_lease_labels = ['active_address', 'address', 'mac_address', 'host_name', 'comment', 'server', 'expires_after', 'client_id', 'active_mac_address']
+        dhcp_lease_records = DHCPMetricsDataSource.metric_records(router_entry, metric_labels = dhcp_lease_labels)
         if dhcp_lease_records:
             # calculate number of leases per DHCP server
             dhcp_lease_servers = {}
             for dhcp_lease_record in dhcp_lease_records:
                 if dhcp_lease_record.get('server'):
                     dhcp_lease_servers[dhcp_lease_record['server']] = dhcp_lease_servers.get(dhcp_lease_record['server'], 0) + 1
 
             # compile leases-per-server records
             dhcp_lease_servers_records = [{ MKTXPConfigKeys.ROUTERBOARD_NAME: router_entry.router_id[MKTXPConfigKeys.ROUTERBOARD_NAME],
                                             MKTXPConfigKeys.ROUTERBOARD_ADDRESS: router_entry.router_id[MKTXPConfigKeys.ROUTERBOARD_ADDRESS],
                                             'server': key, 'count': value} for key, value in dhcp_lease_servers.items()]
-            
+
             # yield lease-per-server metrics
-            dhcp_lease_server_metrics = BaseCollector.gauge_collector('dhcp_lease_active_count', 
-                                                                        'Number of active leases per DHCP server', 
+            dhcp_lease_server_metrics = BaseCollector.gauge_collector('dhcp_lease_active_count',
+                                                                        'Number of active leases per DHCP server',
                                                                         dhcp_lease_servers_records, 'count', ['server'])
             yield dhcp_lease_server_metrics
 
             # active lease metrics
             dhcp_lease_labels.remove('expires_after')
             if router_entry.config_entry.dhcp_lease:
-                dhcp_lease_metrics_gauge = BaseCollector.gauge_collector('dhcp_lease_info', 'DHCP Active Leases', 
+                dhcp_lease_metrics_gauge = BaseCollector.gauge_collector('dhcp_lease_info', 'DHCP Active Leases',
                                                                         dhcp_lease_records, 'expires_after', dhcp_lease_labels)
                 yield dhcp_lease_metrics_gauge
 
             # active lease metrics
             #if router_entry.config_entry.dhcp_lease:
             #    dhcp_lease_metrics = BaseCollector.info_collector('dhcp_lease', 'DHCP Active Leases', dhcp_lease_records, dhcp_lease_labels)
             #    yield dhcp_lease_metrics
-
```

### Comparing `mktxp-1.2.3/mktxp/collector/firewall_collector.py` & `mktxp-1.2.4/mktxp/collector/firewall_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/health_collector.py` & `mktxp-1.2.4/mktxp/collector/health_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/identity_collector.py` & `mktxp-1.2.4/mktxp/collector/identity_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/interface_collector.py` & `mktxp-1.2.4/mktxp/collector/interface_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/ipv6_neighbor_collector.py` & `mktxp-1.2.4/mktxp/collector/ipv6_neighbor_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/kid_control_device_collector.py` & `mktxp-1.2.4/mktxp/collector/kid_control_device_collector.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,47 +19,38 @@
 
 class KidDeviceCollector(BaseCollector):
     """ Kid-control device Metrics collector
     """
 
     @staticmethod
     def collect(router_entry):
-        if not router_entry.config_entry.kid_control_devices:
+        if not (router_entry.config_entry.kid_control_assigned or router_entry.config_entry.kid_control_dynamic):
             return
 
-        labels = ['name', 'user', 'mac_address', 'ip_address', 'bytes_down', 'bytes_up', 'rate_up', 'rate_down',
-                  'bytes_up', 'idle_time',
-                  'blocked', 'limited', 'inactive', 'disabled']
-        info_labels = ['name', 'user', 'mac_address', 'ip_address', 'disabled']
-        records = KidDeviceMetricsDataSource.metric_records(router_entry, metric_labels=labels)
+        labels = ['name', 'user', 'mac_address', 'ip_address', 'bytes_down', 'bytes_up', 'rate_up', 
+                    'rate_down','bytes_up', 'idle_time','blocked', 'limited', 'inactive', 'disabled']
 
+        translation_table = {
+            'rate_up': lambda value: BaseOutputProcessor.parse_rates(value),
+            'rate_down': lambda value: BaseOutputProcessor.parse_rates(value),
+            'idle_time': lambda value: BaseOutputProcessor.parse_timedelta_seconds(value) if value else 0,
+            'blocked': lambda value: '1' if value == 'true' else '0',
+            'limited': lambda value: '1' if value == 'true' else '0',
+            'inactive': lambda value: '1' if value == 'true' else '0',
+            'disabled': lambda value: '1' if value == 'true' else '0'}
+
+        records = KidDeviceMetricsDataSource.metric_records(router_entry, metric_labels=labels, translation_table=translation_table)
         if records:
-            # translate records to appropriate values
-            for record in records:
-                for label in record:
-                    value = record.get(label, None)
-                    if value:
-                        record[label] = KidDeviceCollector._translated_values(label, value)
+            # dhcp resolution
+            for registration_record in records:
+                BaseOutputProcessor.resolve_dhcp(router_entry, registration_record, resolve_address=False)
 
+            info_labels = ['name', 'dhcp_name', 'mac_address', 'user', 'ip_address', 'disabled']
             yield BaseCollector.info_collector('kid_control_device', 'Kid-control device Info', records, info_labels)
-            yield BaseCollector.gauge_collector('kid_control_device_bytes_down', 'Number of received bytes', records, 'bytes_down', ['name', 'mac_address', 'user'])
-            yield BaseCollector.gauge_collector('kid_control_device_bytes_up', 'Number of transmitted bytes', records, 'bytes_up', ['name', 'mac_address', 'user'])
-            yield BaseCollector.gauge_collector('kid_control_device_rate_down', 'Device rate down', records, 'rate_down', ['name', 'mac_address', 'user'])
-            yield BaseCollector.gauge_collector('kid_control_device_rate_up', 'Device rate up', records, 'rate_up', ['name', 'mac_address', 'user'])
-            yield BaseCollector.gauge_collector('kid_control_device_idle_time', 'Device idle time', records, 'idle_time', ['name', 'mac_address', 'user'])
 
-    # Helpers
-    @staticmethod
-    def _translated_values(monitor_label, value):
-        try:
-            return {
-                'rate_up': lambda value: BaseOutputProcessor.parse_rates(value),
-                'rate_down': lambda value: BaseOutputProcessor.parse_rates(value),
-                'idle_time': lambda value: BaseOutputProcessor.parse_timedelta_seconds(value),
-                'blocked': lambda value: '1' if value == 'true' else '0',
-                'limited': lambda value: '1' if value == 'true' else '0',
-                'inactive': lambda value: '1' if value == 'true' else '0',
-                'disabled': lambda value: '1' if value == 'true' else '0',
-            }[monitor_label](value)
-        except KeyError:
-            # default to just returning the value
-            return value
+            id_labels = ['name', 'dhcp_name', 'mac_address', 'user']
+            yield BaseCollector.counter_collector('kid_control_device_bytes_down', 'Number of received bytes', records, 'bytes_down', id_labels)
+            yield BaseCollector.counter_collector('kid_control_device_bytes_up', 'Number of transmitted bytes', records, 'bytes_up', id_labels)
+
+            yield BaseCollector.gauge_collector('kid_control_device_rate_up', 'Device rate up', records, 'rate_up', id_labels)        
+            yield BaseCollector.gauge_collector('kid_control_device_idle_time', 'Device idle time', records, 'idle_time', id_labels)
+            yield BaseCollector.gauge_collector('kid_control_device_rate_down', 'Device rate down', records, 'rate_down', id_labels)
```

### Comparing `mktxp-1.2.3/mktxp/collector/mktxp_collector.py` & `mktxp-1.2.4/mktxp/collector/mktxp_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/monitor_collector.py` & `mktxp-1.2.4/mktxp/collector/monitor_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,24 @@
     '''    
     @staticmethod
     def collect(router_entry):
         if not router_entry.config_entry.monitor:
             return
 
         monitor_labels = ['status', 'rate', 'full_duplex', 'name', 'sfp_temperature']
-        monitor_records = InterfaceMonitorMetricsDataSource.metric_records(router_entry, metric_labels = monitor_labels, include_comments = True)   
+        translation_table = {
+                'status': lambda value: '1' if value=='link-ok' else '0',
+                'rate': lambda value: MonitorCollector._rates(value) if value else '0',
+                'full_duplex': lambda value: '1' if value=='true' else '0',
+                'name': lambda value: value if value else '',
+                'sfp_temperature': lambda value: value if value else '0'
+                }
+        monitor_records = InterfaceMonitorMetricsDataSource.metric_records(router_entry, metric_labels = monitor_labels, 
+                                                                                        translation_table=translation_table, include_comments = True)   
         if monitor_records:
-            # translate records to appropriate values
-            for monitor_record in monitor_records:
-                for monitor_label in monitor_labels:
-                    value = monitor_record.get(monitor_label, None)    
-                    if value:            
-                        monitor_record[monitor_label] = MonitorCollector._translated_values(monitor_label, value)
-
             monitor_status_metrics = BaseCollector.gauge_collector('interface_status', 'Current interface link status', monitor_records, 'status', ['name'])
             yield monitor_status_metrics
 
             # limit records according to the relevant metrics
             rate_records = [monitor_record for monitor_record in monitor_records if monitor_record.get('rate', None)]
             monitor_rates_metrics = BaseCollector.gauge_collector('interface_rate', 'Actual interface connection data rate', rate_records, 'rate', ['name'])
             yield monitor_rates_metrics
@@ -46,25 +47,14 @@
             full_duplex_records = [monitor_record for monitor_record in monitor_records if monitor_record.get('full_duplex', None)]
             monitor_rates_metrics = BaseCollector.gauge_collector('interface_full_duplex', 'Full duplex data transmission', full_duplex_records, 'full_duplex', ['name'])
             yield monitor_rates_metrics
 
             sfp_temperature_metrics = BaseCollector.gauge_collector('interface_sfp_temperature', 'Current SFP temperature', monitor_records, 'sfp_temperature', ['name'])
             yield sfp_temperature_metrics
 
-    # Helpers
-    @staticmethod
-    def _translated_values(monitor_label, value):
-        return {
-                'status': lambda value: '1' if value=='link-ok' else '0',
-                'rate': lambda value: MonitorCollector._rates(value),
-                'full_duplex': lambda value: '1' if value=='true' else '0',
-                'name': lambda value: value,
-                'sfp_temperature': lambda value: value
-                }[monitor_label](value)
-
     @staticmethod
     def _rates(rate_option):
         # according mikrotik docs, an interface rate should be one of these
         rate_value =  {
                 '10Mbps': '10',
                 '100Mbps': '100',
                 '1Gbps': '1000',
```

### Comparing `mktxp-1.2.3/mktxp/collector/package_collector.py` & `mktxp-1.2.4/mktxp/collector/package_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/poe_collector.py` & `mktxp-1.2.4/mktxp/collector/poe_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/pool_collector.py` & `mktxp-1.2.4/mktxp/collector/pool_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/public_ip_collector.py` & `mktxp-1.2.4/mktxp/collector/public_ip_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/queue_collector.py` & `mktxp-1.2.4/mktxp/collector/queue_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/resource_collector.py` & `mktxp-1.2.4/mktxp/collector/resource_collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,25 +23,18 @@
     '''        
     @staticmethod
     def collect(router_entry):
         resource_labels = ['uptime', 'version', 'free_memory', 'total_memory', 
                            'cpu', 'cpu_count', 'cpu_frequency', 'cpu_load', 
                            'free_hdd_space', 'total_hdd_space', 
                            'architecture_name', 'board_name']
-                                   
-        resource_records = SystemResourceMetricsDataSource.metric_records(router_entry, metric_labels = resource_labels)   
-        if resource_records:
-            # translate records to appropriate values
-            translated_fields = ['uptime']        
-            for resource_record in resource_records:
-                for translated_field in translated_fields:
-                    value = resource_record.get(translated_field, None)    
-                    if value:            
-                        resource_record[translated_field] = SystemResourceCollector._translated_values(translated_field, value)
+        translation_table = {'uptime': lambda value: BaseOutputProcessor.parse_timedelta_seconds(value)}
 
+        resource_records = SystemResourceMetricsDataSource.metric_records(router_entry, metric_labels = resource_labels, translation_table=translation_table)   
+        if resource_records:
             uptime_metrics = BaseCollector.gauge_collector('system_uptime', 'Time interval since boot-up', resource_records, 'uptime', ['version', 'board_name', 'cpu', 'architecture_name'])
             yield uptime_metrics
 
             free_memory_metrics = BaseCollector.gauge_collector('system_free_memory', 'Unused amount of RAM', resource_records, 'free_memory', ['version', 'board_name', 'cpu', 'architecture_name'])
             yield free_memory_metrics
 
             total_memory_metrics = BaseCollector.gauge_collector('system_total_memory', 'Amount of installed RAM', resource_records, 'total_memory', ['version', 'board_name', 'cpu', 'architecture_name'])
@@ -67,16 +60,7 @@
                 for record in resource_records:
                     cur_version, newest_version = check_for_updates(record['version'])
                     record['newest_version'] = str(newest_version)
                     record['update_available'] = cur_version < newest_version
 
                 update_available_metrics = BaseCollector.gauge_collector('system_update_available', 'Is there a newer version available', resource_records, 'update_available', ['newest_version',])
                 yield update_available_metrics
-
-
-    # Helpers
-    @staticmethod
-    def _translated_values(translated_field, value):
-        return {
-                'uptime': lambda value: BaseOutputProcessor.parse_timedelta_seconds(value)
-                }[translated_field](value)
-
```

### Comparing `mktxp-1.2.3/mktxp/collector/route_collector.py` & `mktxp-1.2.4/mktxp/collector/route_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/user_collector.py` & `mktxp-1.2.4/mktxp/collector/user_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/collector/wlan_collector.py` & `mktxp-1.2.4/mktxp/collector/wlan_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/base_ds.py` & `mktxp-1.2.4/mktxp/datasource/base_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/bgp_ds.py` & `mktxp-1.2.4/mktxp/datasource/route_ds.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
-class BGPMetricsDataSource:
-    ''' Wireless Metrics data provider
+class RouteMetricsDataSource:
+    ''' Routes Metrics data provider
     '''             
     @staticmethod
-    def metric_records(router_entry, *, metric_labels = None, add_router_id = True):
+    def metric_records(router_entry, *, metric_labels = None):
         if metric_labels is None:
             metric_labels = []                
         try:
-            bgp_records = router_entry.api_connection.router_api().get_resource('/routing/bgp/session').get()
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = bgp_records, metric_labels = metric_labels, add_router_id = add_router_id)
+            route_records = router_entry.api_connection.router_api().get_resource('/ip/route').get(active='yes')
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = route_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting BGP sessions info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting routes info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
-
```

### Comparing `mktxp-1.2.3/mktxp/datasource/capsman_ds.py` & `mktxp-1.2.4/mktxp/datasource/capsman_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/connection_ds.py` & `mktxp-1.2.4/mktxp/datasource/connection_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/dhcp_ds.py` & `mktxp-1.2.4/mktxp/datasource/dhcp_ds.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,42 +14,40 @@
 
 from mktxp.datasource.base_ds import BaseDSProcessor
 from mktxp.utils.utils import parse_mkt_uptime
 
 
 class DHCPMetricsDataSource:
     ''' DHCP Metrics data provider
-    '''             
+    '''
     @staticmethod
     def metric_records(router_entry, *, metric_labels = None, add_router_id = True, dhcp_cache = True, translate = True, bound = False):
         if metric_labels is None or dhcp_cache:
-            metric_labels = ['host_name', 'comment', 'active_address', 'address', 'mac_address', 'server', 'expires_after']  
+            metric_labels = ['host_name', 'comment', 'active_address', 'address', 'mac_address', 'server', 'expires_after', 'client_id', 'active_mac_address']
 
         if dhcp_cache and router_entry.dhcp_records:
             return router_entry.dhcp_records
         try:
             if bound:
                 dhcp_lease_records = router_entry.dhcp_entry.api_connection.router_api().get_resource('/ip/dhcp-server/lease').get(status='bound')
             else:
                 dhcp_lease_records = router_entry.dhcp_entry.api_connection.router_api().get_resource('/ip/dhcp-server/lease').call('print', {'active':''})
 
             # translation rules
             translation_table = {}
             if 'comment' in metric_labels:
-                translation_table['comment'] = lambda c: c if c else ''           
+                translation_table['comment'] = lambda c: c if c else ''
             if 'host_name' in metric_labels:
-                translation_table['host_name'] = lambda c: c if c else ''           
+                translation_table['host_name'] = lambda c: c if c else ''
             if 'expires_after' in metric_labels and translate:
-                translation_table['expires_after'] = lambda c: parse_mkt_uptime(c) if c else 0       
+                translation_table['expires_after'] = lambda c: parse_mkt_uptime(c) if c else 0
             if 'active_address' in metric_labels:
-                translation_table['active_address'] = lambda c: c if c else ''        
+                translation_table['active_address'] = lambda c: c if c else ''
 
             records = BaseDSProcessor.trimmed_records(router_entry, router_records = dhcp_lease_records, metric_labels = metric_labels, add_router_id = add_router_id, translation_table = translation_table)
             if dhcp_cache:
                 router_entry.dhcp_records = records
             return records
-            
+
         except Exception as exc:
             print(f'Error getting dhcp info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
-
-
```

### Comparing `mktxp-1.2.3/mktxp/datasource/firewall_ds.py` & `mktxp-1.2.4/mktxp/datasource/firewall_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/health_ds.py` & `mktxp-1.2.4/mktxp/datasource/health_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/identity_ds.py` & `mktxp-1.2.4/mktxp/datasource/identity_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/interface_ds.py` & `mktxp-1.2.4/mktxp/datasource/interface_ds.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             return None
 
 
 class InterfaceMonitorMetricsDataSource:
     ''' Interface Monitor Metrics data provider
     '''             
     @staticmethod
-    def metric_records(router_entry, *, metric_labels = None, kind = 'ethernet', include_comments = False, running_only = True):
+    def metric_records(router_entry, *, metric_labels = None, translation_table = None, kind = 'ethernet', include_comments = False, running_only = True):
         if metric_labels is None:
             metric_labels = []                
         try:
             interfaces = router_entry.api_connection.router_api().get_resource(f'/interface/{kind}').call('print', {'proplist':'name,comment,running'})
 
             interface_monitor_records = []
             for int_num, interface in enumerate(interfaces):
@@ -56,12 +56,12 @@
                 interface_monitor_records.append(interface_monitor_record)
                 
             # With wifiwave2, Mikrotik renamed the field 'registered-clients' to 'registered-peers'
             # For backward compatibility, including both variants
             for interface_monitor_record in interface_monitor_records:
                 if 'registered-peers' in interface_monitor_record:
                     interface_monitor_record['registered-clients'] = interface_monitor_record['registered-peers']
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = interface_monitor_records, metric_labels = metric_labels)
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = interface_monitor_records, metric_labels = metric_labels, translation_table=translation_table)
         except Exception as exc:
             print(f'Error getting {kind} interface monitor info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.3/mktxp/datasource/ipv6_neighbor_ds.py` & `mktxp-1.2.4/mktxp/datasource/ipv6_neighbor_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/kid_control_device_ds.py` & `mktxp-1.2.4/mktxp/datasource/kid_control_device_ds.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 
 class KidDeviceMetricsDataSource:
     """ Kid-control device Metrics data provider
     """
 
     @staticmethod
-    def metric_records(router_entry, *, metric_labels=None):
+    def metric_records(router_entry, *, metric_labels=None, translation_table=None):
         if metric_labels is None:
             metric_labels = []
         try:
             device_records = []
             records = router_entry.api_connection.router_api().get_resource('/ip/kid-control/device').get()
             for record in records:
-                if record.get('user'):
+                if record.get('user') or router_entry.config_entry.kid_control_dynamic:
                     device_records.append(record)
-            return BaseDSProcessor.trimmed_records(router_entry, router_records=device_records, metric_labels=metric_labels)
+            return BaseDSProcessor.trimmed_records(router_entry, router_records=device_records, metric_labels=metric_labels, translation_table=translation_table)
         except Exception as exc:
             print(
                 f'Error getting Kid-control device info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.3/mktxp/datasource/mktxp_ds.py` & `mktxp-1.2.4/mktxp/datasource/mktxp_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/netwatch_ds.py` & `mktxp-1.2.4/mktxp/datasource/netwatch_ds.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,26 @@
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
 class NetwatchMetricsDataSource:
     ''' Netwatch Metrics data provider
     '''             
     @staticmethod
-    def metric_records(router_entry, *, metric_labels = None):
+    def metric_records(router_entry, *, metric_labels=None, translation_table=None):
         if metric_labels is None:
             metric_labels = []                
         try:
             netwatch_records = router_entry.api_connection.router_api().get_resource('/tool/netwatch').get(disabled='false')
             if 'name' in metric_labels:
-
                 for netwatch_record in netwatch_records:
                     comment = netwatch_record.get('comment')
                     host = netwatch_record.get('host')        
                     if comment:
                         netwatch_record['name'] = f'{host} ({comment[0:20]})' if not router_entry.config_entry.use_comments_over_names else comment
                     else:
                         netwatch_record['name'] = host
-                                            
-            # translation rules
-            translation_table = {}
-            if 'status' in metric_labels:
-                translation_table['status'] = lambda value: '1' if value == 'up' else '0'      
 
             return BaseDSProcessor.trimmed_records(router_entry, router_records = netwatch_records, translation_table = translation_table, metric_labels = metric_labels)
         except Exception as exc:
             print(f'Error getting Netwatch info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.3/mktxp/datasource/package_ds.py` & `mktxp-1.2.4/mktxp/datasource/package_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/poe_ds.py` & `mktxp-1.2.4/mktxp/datasource/poe_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/pool_ds.py` & `mktxp-1.2.4/mktxp/datasource/pool_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/public_ip_ds.py` & `mktxp-1.2.4/mktxp/datasource/public_ip_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/queue_ds.py` & `mktxp-1.2.4/mktxp/datasource/queue_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/route_ds.py` & `mktxp-1.2.4/mktxp/datasource/user_ds.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
-class RouteMetricsDataSource:
-    ''' Routes Metrics data provider
+class UserMetricsDataSource:
+    ''' Active Users Metrics data provider
     '''             
-    @staticmethod
+    @staticmethod    
     def metric_records(router_entry, *, metric_labels = None):
         if metric_labels is None:
             metric_labels = []                
         try:
-            route_records = router_entry.api_connection.router_api().get_resource('/ip/route').get(active='yes')
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = route_records, metric_labels = metric_labels)
+            active_users_records = router_entry.api_connection.router_api().get_resource('/user/active/').get()
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = active_users_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting routes info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.3/mktxp/datasource/routerboard_ds.py` & `mktxp-1.2.4/mktxp/datasource/routerboard_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/datasource/system_resource_ds.py` & `mktxp-1.2.4/mktxp/datasource/system_resource_ds.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 from mktxp.utils.utils import builtin_wifi_capsman_version
 
 
 class SystemResourceMetricsDataSource:
     ''' System Resource Metrics data provider
     '''             
     @staticmethod    
-    def metric_records(router_entry, *, metric_labels = None):
+    def metric_records(router_entry, *, metric_labels = None, translation_table=None):
         if metric_labels is None:
             metric_labels = []                
         try:
             system_resource_records = router_entry.api_connection.router_api().get_resource('/system/resource').get()
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = system_resource_records, metric_labels = metric_labels)
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = system_resource_records, metric_labels = metric_labels, translation_table=translation_table)
         except Exception as exc:
             print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
     @staticmethod
     def os_version(router_entry):
         try:
```

### Comparing `mktxp-1.2.3/mktxp/datasource/user_ds.py` & `mktxp-1.2.4/mktxp/datasource/bgp_ds.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
-class UserMetricsDataSource:
-    ''' Active Users Metrics data provider
+class BGPMetricsDataSource:
+    ''' Wireless Metrics data provider
     '''             
-    @staticmethod    
-    def metric_records(router_entry, *, metric_labels = None):
+    @staticmethod
+    def metric_records(router_entry, *, metric_labels = None, translation_table = None):
         if metric_labels is None:
             metric_labels = []                
         try:
-            active_users_records = router_entry.api_connection.router_api().get_resource('/user/active/').get()
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = active_users_records, metric_labels = metric_labels)
+            bgp_records = router_entry.api_connection.router_api().get_resource('/routing/bgp/session').get()
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = bgp_records, metric_labels = metric_labels, translation_table = translation_table)
         except Exception as exc:
-            print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting BGP sessions info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
+
```

### Comparing `mktxp-1.2.3/mktxp/datasource/wireless_ds.py` & `mktxp-1.2.4/mktxp/datasource/wireless_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/flow/collector_handler.py` & `mktxp-1.2.4/mktxp/flow/collector_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         """
 
         def timeout(timeout_event):
             timeout_event.set()
 
         # overall scrape duration 
         total_scrape_timeout_event = Event()
-        total_scrape_timer = Timer(config_handler.system_entry().total_max_scrape_duration, timeout, args=(total_scrape_timeout_event,))
+        total_scrape_timer = Timer(config_handler.system_entry.total_max_scrape_duration, timeout, args=(total_scrape_timeout_event,))
         total_scrape_timer.start()
 
         with ThreadPoolExecutor(max_workers=max_worker_threads) as executor:
             futures = {}
 
             for router_entry in self.entries_handler.router_entries:
                 if total_scrape_timeout_event.is_set():
@@ -90,15 +90,15 @@
 
                 if not router_entry.is_ready():
                     # let's pick up on things in the next run
                     continue
                 
                 # Duration of individual scrapes
                 scrape_timeout_event = Event()
-                scrape_timer = Timer(config_handler.system_entry().max_scrape_duration, timeout, args=(scrape_timeout_event,))
+                scrape_timer = Timer(config_handler.system_entry.max_scrape_duration, timeout, args=(scrape_timeout_event,))
                 scrape_timer.start()
 
                 futures[executor.submit(self.collect_router_entry_async, router_entry, scrape_timeout_event, total_scrape_timeout_event)] = scrape_timer
 
             for future in as_completed(futures):
                 # cancel unused timers for scrapes finished regularly (within set duration)
                 futures[future].cancel()
@@ -113,28 +113,28 @@
             return
 
         # bandwidth collector
         yield from self.collector_registry.bandwidthCollector.collect()
 
         # all other collectors
         # Check whether to run in parallel by looking at the mktxp system configuration
-        parallel = config_handler.system_entry().fetch_routers_in_parallel
-        max_worker_threads = config_handler.system_entry().max_worker_threads
+        parallel = config_handler.system_entry.fetch_routers_in_parallel
+        max_worker_threads = config_handler.system_entry.max_worker_threads
         if parallel:
             yield from self.collect_async(max_worker_threads=max_worker_threads)
         else:
             yield from self.collect_sync()
 
 
     def _valid_collect_interval(self):
         now = datetime.now().timestamp()
         diff = now - self.last_collect_timestamp
-        if diff < config_handler.system_entry().minimal_collect_interval:
-            if config_handler.system_entry().verbose_mode:
-                print(f'An attemp to collect metrics within minimal metrics collection interval: {diff} < {config_handler.system_entry().minimal_collect_interval}')
+        if diff < config_handler.system_entry.minimal_collect_interval:
+            if config_handler.system_entry.verbose_mode:
+                print(f'An attemp to collect metrics within minimal metrics collection interval: {diff} < {config_handler.system_entry.minimal_collect_interval}')
                 print('deferring..')
             return False
 
         self.last_collect_timestamp = now       
         return True
```

### Comparing `mktxp-1.2.3/mktxp/flow/collector_registry.py` & `mktxp-1.2.4/mktxp/flow/collector_registry.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/flow/processor/base_proc.py` & `mktxp-1.2.4/mktxp/flow/processor/base_proc.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 class ExportProcessor:
     ''' Base Export Processing
     '''    
     @staticmethod
     def start():
         REGISTRY.register(CollectorHandler(RouterEntriesHandler(), CollectorRegistry()))
         current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-        print(f'{current_time} Running HTTP metrics server on: {config_handler.system_entry().listen}')
-        serve(make_wsgi_app(), listen = config_handler.system_entry().listen)
+        print(f'{current_time} Running HTTP metrics server on: {config_handler.system_entry.listen}')
+        serve(make_wsgi_app(), listen = config_handler.system_entry.listen)
 
 class OutputProcessor:
     ''' Base CLI Processing
     '''    
     @staticmethod
     def capsman_clients(entry_name):
         router_entry = RouterEntriesHandler.router_entry(entry_name)
```

### Comparing `mktxp-1.2.3/mktxp/flow/processor/output.py` & `mktxp-1.2.4/mktxp/flow/processor/output.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,29 +110,32 @@
             rate = int(rate)
         except:
             return BaseOutputProcessor.parse_rates(rate)
         power = floor(log(rate, 1000))
         return f"{int(rate / 1000 ** power)} {['bps', 'Kbps', 'Mbps', 'Gbps'][int(power)]}"
 
     @staticmethod
-    def parse_timedelta(time):
-        duration_interval_rgx = config_handler.re_compiled.get('duration_interval_rgx')
+    def parse_timedelta(time, ms_span=False):
+        # ms_span for milliseconds-long durations, since otherwise minutes would match the ms in the value
+        rgx_key = 'duration_interval_rgx_sp' if ms_span else 'duration_interval_rgx'
+        duration_interval_rgx = config_handler.re_compiled.get(rgx_key)
         if not duration_interval_rgx:
-            duration_interval_rgx = re.compile(r'((?P<weeks>\d+)w)?((?P<days>\d+)d)?((?P<hours>\d+)h)?((?P<minutes>\d+)m)?((?P<seconds>\d+)s)?((?P<milliseconds>\d+)ms)?')
-            config_handler.re_compiled['duration_interval_rgx'] = duration_interval_rgx                        
+            duration_interval_rgx = re.compile(r'((?P<seconds>\d+)s)?((?P<milliseconds>\d+)ms)?((?P<microseconds>\d+)us)?') if ms_span else\
+                    re.compile(r'((?P<weeks>\d+)w)?((?P<days>\d+)d)?((?P<hours>\d+)h)?((?P<minutes>\d+)m)?((?P<seconds>\d+)s)?((?P<milliseconds>\d+)ms)?')
+            config_handler.re_compiled[rgx_key] = duration_interval_rgx                        
         time_dict = duration_interval_rgx.match(time).groupdict()
         return timedelta(**{key: int(value) for key, value in time_dict.items() if value})
 
     @staticmethod
-    def parse_timedelta_seconds(time):
-        return BaseOutputProcessor.parse_timedelta(time).total_seconds()
+    def parse_timedelta_seconds(time, ms_span=False):
+        return BaseOutputProcessor.parse_timedelta(time, ms_span=ms_span).total_seconds()
 
     @staticmethod
-    def parse_timedelta_milliseconds(time):
-        return BaseOutputProcessor.parse_timedelta(time) / timedelta(milliseconds=1)
+    def parse_timedelta_milliseconds(time, ms_span=False):
+        return BaseOutputProcessor.parse_timedelta(time, ms_span=ms_span) / timedelta(milliseconds=1)
 
     @staticmethod
     def parse_signal_strength(signal_strength):
         wifi_signal_strength_rgx = config_handler.re_compiled.get('wifi_signal_strength_rgx')
         if not wifi_signal_strength_rgx:
             # wifi_signal_strength_rgx = re.compile(r'(-?\d+(?:\.\d+)?)(dBm)?')
             wifi_signal_strength_rgx = re.compile(r'(-?\d+(?:\.\d+)?)')
```

### Comparing `mktxp-1.2.3/mktxp/flow/router_connection.py` & `mktxp-1.2.4/mktxp/flow/router_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 password = self.config_entry.password,
                 port = self.config_entry.port,
                 plaintext_login = True,
                 use_ssl = self.config_entry.use_ssl,
                 ssl_verify = self.config_entry.ssl_certificate_verify,
                 ssl_context = ctx)
         
-        self.connection.socket_timeout = config_handler.system_entry().socket_timeout
+        self.connection.socket_timeout = config_handler.system_entry.socket_timeout
         self.api = None
 
     def is_connected(self):
         if not (self.connection and self.connection.connected and self.api):
             return False
         try:
             self.api.get_resource('/system/identity').get()
@@ -74,41 +74,42 @@
 
     def connect(self):
         connect_time = datetime.now()
         if self.is_connected() or self._in_connect_timeout(connect_time.timestamp()):
             return
         try:
             print(f'Connecting to router {self.router_name}@{self.config_entry.hostname}')
+            self.connection.plaintext_login = self.config_entry.plaintext_login
             self.api = self.connection.get_api()
             self._set_connect_state(success = True, connect_time = connect_time)
         except (socket.error, socket.timeout, Exception) as exc:
             self._set_connect_state(success = False, connect_time = connect_time, exc = exc)
             #raise RouterAPIConnectionError
 
     def router_api(self):
         if not self.is_connected():
             self.connect()
         return self.api
 
     def _in_connect_timeout(self, connect_timestamp):
         connect_delay = self._connect_delay()
         if (connect_timestamp - self.last_failure_timestamp) < connect_delay:
-            if config_handler.system_entry().verbose_mode: 
+            if config_handler.system_entry.verbose_mode: 
                 print(f'{self.router_name}@{self.config_entry.hostname}: in connect timeout, {int(connect_delay - (connect_timestamp - self.last_failure_timestamp))}secs remaining')
                 print(f'Successive failure count: {self.successive_failure_count}')
             return True
-        if config_handler.system_entry().verbose_mode: 
+        if config_handler.system_entry.verbose_mode: 
             print(f'{self.router_name}@{self.config_entry.hostname}: OK to connect')
             if self.last_failure_timestamp > 0:
                 print(f'Seconds since last failure: {connect_timestamp - self.last_failure_timestamp}')
                 print(f'Prior successive failure count: {self.successive_failure_count}')
         return False
 
     def _connect_delay(self):
-        mktxp_entry = config_handler.system_entry()
+        mktxp_entry = config_handler.system_entry
         connect_delay = (1 + self.successive_failure_count / mktxp_entry.delay_inc_div) * mktxp_entry.initial_delay_on_failure
         return connect_delay if connect_delay < mktxp_entry.max_delay_on_failure else mktxp_entry.max_delay_on_failure
 
 
     def _set_connect_state(self, success = False, connect_time = datetime.now(), exc = None):
         if success:
             self.last_failure_timestamp = 0
```

### Comparing `mktxp-1.2.3/mktxp/flow/router_entries_handler.py` & `mktxp-1.2.4/mktxp/flow/router_entries_handler.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/flow/router_entry.py` & `mktxp-1.2.4/mktxp/flow/router_entry.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/mktxp/utils/utils.py` & `mktxp-1.2.4/mktxp/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 import time
 from timeit import default_timer
 from collections.abc import Iterable
 import xml.etree.ElementTree as ET
 from contextlib import contextmanager
 from multiprocessing import Process, Event
 from datetime import timedelta
-from pkg_resources import packaging
-
-
+from packaging.version import parse
 
 ''' Utilities / Helpers
 '''
 @contextmanager
 def temp_dir(quiet = True):
     ''' Temp dir context manager
     '''
@@ -302,39 +300,39 @@
         result = response.read()
         root = ET.fromstring(result)
         channel = root[0]
 
         for child in channel:
             # iterate over all updates
             if child.tag == 'item':
-                title, _, _, _, _, _ = child
+                title, _, _, _, _ = child
                 # extract and parse the version number from title
                 version_text = re.findall(r'[\d+\.]+', title.text)[0]
-                version_number = packaging.version.parse(version_text)
+                version_number = parse(version_text)
                 versions.append(version_number)
     return versions
 
 
 def parse_ros_version(string):
     """Parse the version returned from the /system/resource command.
     Returns a tuple: (<version>, <channel>).
 
     >>> parse_ros_version('1.2.3 (stable)')
     1.2.3, stable
     """
     version, channel = re.findall(r'([\d\.]+).*?([\w]+)', string)[0]
-    return packaging.version.parse(version), channel
+    return parse(version), channel
 
-def builtin_wifi_capsman_version(string):
+def builtin_wifi_capsman_version(version):
     """Try to check if the version is Wifi version of RouterOS (>= 7.13).
     If anything goes wrong, return None.
     Returns a boolean"""
     try:
-        cur_version, _ = parse_ros_version(string)
-        if cur_version >= packaging.version.parse('7.13'):
+        cur_version, _ = parse_ros_version(version)
+        if cur_version >= parse('7.13'):
             return True
     except Exception as err:
         print(f'could not get current RouterOS version, because: {str(err)}')
         return None
 
     return False
```

### Comparing `mktxp-1.2.3/mktxp.egg-info/PKG-INFO` & `mktxp-1.2.4/mktxp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktxp
-Version: 1.2.3
+Version: 1.2.4
 Summary: Prometheus Exporter for Mikrotik RouterOS devices
 Home-page: https://github.com/akpw/mktxp
 Author: Arseniy Kuznetsov
 Author-email: k.arseniy@gmail.com
 License: GNU General Public License v2 (GPLv2)
 Keywords: Mikrotik RouterOS Prometheus Exporter
 Classifier: Development Status :: 4 - Beta
@@ -26,27 +26,28 @@
 Requires-Dist: prometheus-client>=0.9.0
 Requires-Dist: RouterOS-api>=0.17.0
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: humanize>=3.2.0
 Requires-Dist: texttable>=1.6.3
 Requires-Dist: speedtest-cli>=2.1.2
 Requires-Dist: waitress>=3.0.0
+Requires-Dist: packaging>=24.0
 
 
 ![License](https://img.shields.io/badge/License-GNU%20GPL-blue.svg)
-![Language](https://img.shields.io/badge/python-v3.6-blue)
+![Language](https://img.shields.io/badge/python-v3.8-blue)
 ![License](https://img.shields.io/badge/mikrotik-routeros-orange)
 ![License](https://img.shields.io/badge/prometheus-exporter-blueviolet)
 
 
 ## Description
 MKTXP is a Prometheus Exporter for Mikrotik RouterOS devices.\
 It gathers and exports a rich set of metrics across multiple routers, all easily configurable via built-in CLI interface. 
 
-While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, etc.
+While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, optional bandwidth testing, etc.
 
 Apart from exporting to Prometheus, MKTXP can print selected metrics directly on the command line (see examples below). 
 
 For effortless visualization of the RouterOS metrics exported to Prometheus, MKTXP comes with a dedicated [Grafana dashboard](https://grafana.com/grafana/dashboards/13679):
 
 <img width="32%" alt="1" src="https://user-images.githubusercontent.com/5028474/217029083-3c2f561e-853f-45a7-b9f1-d818a830daf5.png"> <img width="32%" alt="2" src="https://user-images.githubusercontent.com/5028474/217029092-2b86b41b-1f89-4383-ac48-16652e820f7e.png"> <img width="32%" alt="3" src="https://user-images.githubusercontent.com/5028474/217029096-dbf6b46c-3ed7-4c76-a57b-8cebfb3b671c.png">
 
@@ -79,26 +80,36 @@
 
 
 ## Getting started
 To get started with MKTXP, you need to edit its main configuration file. This essentially involves filling in your Mikrotik devices IP addresses & authentication info, optionally modifying various settings to specific needs. 
 
 The default configuration file comes with a sample configuration, making it easy to copy / edit parameters for your RouterOS devices as needed:
 ```
-[Sample-Router]
-    enabled = False         # turns metrics collection for this RouterOS device on / off
-    
+[Sample-Router-1]
+    # for specific configuration on the router level, overload the defaults here
+    hostname = 192.168.88.1
+
+[Sample-Router-2]
+    # for specific configuration on the router level, overload the defaults here
+    hostname = 192.168.88.2
+
+[default]
+    # this affects configuration of all routers, unless overloaded on their specific levels
+    enabled = True          # turns metrics collection for this RouterOS device on / off
+
     hostname = localhost    # RouterOS IP address
-    port = 8728             # RouterOS API / API-SSL service port
+    port = 8728             # RouterOS IP Port
     
     username = username     # RouterOS user, needs to have 'read' and 'api' permissions
     password = password
     
     use_ssl = False                 # enables connection via API-SSL servis
     no_ssl_certificate = False      # enables API_SSL connect without router SSL certificate
     ssl_certificate_verify = False  # turns SSL certificate verification on / off   
+    plaintext_login = True          # for legacy RouterOS versions below 6.43 use False
 
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
@@ -116,15 +127,16 @@
     public_ip = True                # Public IP metrics
     route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
-    kid_control_devices = False     # Kid Control metrics 
+    kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
+    kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
 
     bgp = False                     # BGP sessions metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
@@ -132,14 +144,15 @@
     use_comments_over_names = True  # when available, forces using comments over the interfaces names
 
     check_for_updates = False       # check for available ROS updates
 ```
 
 Most options are easy to understand at first glance, and some are described in more details [later](https://github.com/akpw/mktxp#advanced-features).
 
+<sup>💡</sup> To automatically migrate from the older `mktxp.conf` format in the existing installs, just set `compact_default_conf_values = True` in [the mktxp system config](https://github.com/akpw/mktxp#mktxp-system-configuration)
 
 #### Local install
 If you have a local MKTXP installation, you can edit the configuration file with your default system editor directly from mktxp:
 ```bash
 ❯ mktxp edit
 ```
 In case you prefer a different editor, run the ```edit``` command with its optional `-ed` parameter:
@@ -162,15 +175,15 @@
 ```
 docker run -v "$(pwd)/mktxp:/home/mktxp/mktxp/" -p 49090:49090 -it --rm ghcr.io/akpw/mktxp:latest
 ```
 
 #### MKTXP stack install
 [MKTXP Stack Getting Started](https://github.com/akpw/mktxp-stack#install--getting-started) provides similar instructions around editing the mktxp.conf file and, if needed, adding a dedicated API user to your Mikrotik RouterOS devices as mentioned below.
 
-💡 *In the case of usage within a [Docker Swarm](https://docs.docker.com/engine/swarm/), please do make sure to have all settings explicitly set in both the `mktxp.conf` and `_mktxp.conf` files.  Not doing this may cause [issues](https://github.com/akpw/mktxp/issues/55#issuecomment-1346693843) regarding a `read-only` filesystem.*
+<sup>💡</sup> *In the case of usage within a [Docker Swarm](https://docs.docker.com/engine/swarm/), please do make sure to have all settings explicitly set in both the `mktxp.conf` and `_mktxp.conf` files.  Not doing this may cause [issues](https://github.com/akpw/mktxp/issues/55#issuecomment-1346693843) regarding a `read-only` filesystem.*
 
 ## Mikrotik Device Config
 For the purpose of RouterOS device monitoring, it's best to create a dedicated user with minimal required permissions. \
 MKTXP only needs ```API``` and ```Read```, so at that point you can go to your router's terminal and type:
 ```
 /user group add name=mktxp_group policy=api,read
 /user add name=mktxp_user group=mktxp_group password=mktxp_user_password
@@ -255,18 +268,20 @@
 
     bandwidth = False               # Turns metrics bandwidth metrics collection on / off    
     bandwidth_test_interval = 600   # Interval for colllecting bandwidth metrics
     minimal_collect_interval = 5    # Minimal metric collection interval
 
     verbose_mode = False            # Set it on for troubleshooting
 
-    fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
+    fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers in parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
     total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
+
+    compact_default_conf_values = False # Compact mktxp.conf, so only specific values are kept on the individual routers' level    
 ```    
 <sup>💡</sup> *When changing the default mktxp port for [docker image installs](https://github.com/akpw/mktxp#docker-image-install), you'll need to adjust the `docker run ... -p 49090:49090 ...` command to reflect the new port*
 
 ## Grafana dashboard
 Now with your RouterOS metrics being exported to Prometheus, it's easy to visualize them with this [Grafana dashboard](https://grafana.com/grafana/dashboards/13679)
 
 
@@ -352,15 +367,15 @@
 max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
 max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
 total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
 ```
 To keeps things within expected boundaries, the last two parameters allows for controlling both individual and overall scrape durations
 
 
-### mktxp listening socket addresses
+### mktxp endpoint listen addresses
 By default, mktxp runs it's HTTP metrics endpoint on any IPv4 address on port 49090. However, it is also able to listen on multiple socket addresses, both IPv4 and IPv6. 
 You can configure this behaviour via the following [system option](https://github.com/akpw/mktxp/blob/main/README.md#mktxp-system-configuration), setting ```listen``` to a space-separated list of sockets to listen to, e.g.:
 ```
 listen = '0.0.0.0:49090 [::1]:49090'
 ```
 A wildcard for the hostname is supported as well, and binding to both IPv4/IPv6 as available.
```

### Comparing `mktxp-1.2.3/mktxp.egg-info/SOURCES.txt` & `mktxp-1.2.4/mktxp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.3/setup.py` & `mktxp-1.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # read the README.md contents
 pkg_dir = path.abspath(path.dirname(__file__))
 with open(path.join(pkg_dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mktxp',
-    version='1.2.3',
+    version='1.2.4',
 
     url='https://github.com/akpw/mktxp',
 
     author='Arseniy Kuznetsov',
     author_email='k.arseniy@gmail.com',
 
     long_description=long_description,
@@ -46,14 +46,15 @@
     install_requires = ['prometheus-client>=0.9.0', 
                         'RouterOS-api>=0.17.0', 
                         'configobj>=5.0.6',
                         'humanize>=3.2.0',
                         'texttable>=1.6.3',
                         'speedtest-cli>=2.1.2',
                         'waitress>=3.0.0',
+                        'packaging>=24.0'
                         ],
 
     test_suite = 'tests.mktxp_test_suite',
 
     entry_points={'console_scripts': [
         'mktxp = mktxp.cli.dispatch:main',
     ]},
```

