# Comparing `tmp/pyaoscx-2.5.1.tar.gz` & `tmp/pyaoscx-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaoscx-2.5.1.tar", last modified: Thu Nov 16 21:36:46 2023, max compression
+gzip compressed data, was "pyaoscx-2.6.0.tar", last modified: Tue Apr 30 21:21:29 2024, max compression
```

## Comparing `pyaoscx-2.5.1.tar` & `pyaoscx-2.6.0.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.604548 pyaoscx-2.5.1/
--rw-r--r--   0 administrator  (1000) administrator  (1000)     4618 2023-11-16 21:36:46.604548 pyaoscx-2.5.1/PKG-INFO
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     3892 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/README.md
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.592548 pyaoscx-2.5.1/pyaoscx/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    18333 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/acl.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    21841 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/acl_entry.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    14710 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/aggregate_address.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     6635 2023-11-16 21:31:41.000000 pyaoscx-2.5.1/pyaoscx/api.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    14625 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/bgp_neighbor.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    15388 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/bgp_router.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    16247 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/configuration.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    18903 2023-11-16 21:31:41.000000 pyaoscx-2.5.1/pyaoscx/device.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    13836 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/dhcp_relay.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    11370 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/dns.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.596548 pyaoscx-2.5.1/pyaoscx/exceptions/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1087 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/generic_op_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      801 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/login_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      320 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/parameter_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      450 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/pyaoscx_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      879 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/response_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      321 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/unsupported_capability_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      871 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/exceptions/verification_error.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1005 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/firmware.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    85803 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/interface.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    12912 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/ipv6.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     7899 2023-11-16 21:31:41.000000 pyaoscx-2.5.1/pyaoscx/lldp_neighbor.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    13019 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/mac.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    11167 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/ospf_area.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    10174 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/ospf_interface.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    13376 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/ospf_router.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     8406 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/ospf_virtual_link.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      321 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/ospfv3_router.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     8680 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/poe_interface.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    56937 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/pyaoscx_factory.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    12301 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/pyaoscx_module.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     9780 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/qos.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     9149 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/qos_cos.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    11962 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/qos_dscp.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     9377 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/queue.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     7452 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/queue_profile.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     7662 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/queue_profile_entry.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.596548 pyaoscx-2.5.1/pyaoscx/rest/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/__init__.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.600548 pyaoscx-2.5.1/pyaoscx/rest/v1/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v1/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     2703 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v1/api.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    32985 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v1/interface.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.600548 pyaoscx-2.5.1/pyaoscx/rest/v10_04/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_04/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1321 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_04/api.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      286 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_04/interface.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.600548 pyaoscx-2.5.1/pyaoscx/rest/v10_08/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_08/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1322 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_08/api.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      286 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_08/interface.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.600548 pyaoscx-2.5.1/pyaoscx/rest/v10_09/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_09/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1369 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_09/api.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)      281 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/rest/v10_09/interface.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    12398 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/session.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    11182 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/static_mac.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    15678 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/static_nexthop.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    16433 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/static_route.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     8288 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/tunnel_endpoint.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.604548 pyaoscx-2.5.1/pyaoscx/utils/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/utils/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     3693 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/utils/list_attributes.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    11109 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/utils/util.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    20085 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/vlan.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     9887 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/vni.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    25340 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/vrf.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)    13186 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/vrf_address_family.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     8257 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/pyaoscx/vsx.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.596548 pyaoscx-2.5.1/pyaoscx.egg-info/
--rw-r--r--   0 administrator  (1000) administrator  (1000)     4618 2023-11-16 21:36:46.000000 pyaoscx-2.5.1/pyaoscx.egg-info/PKG-INFO
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1876 2023-11-16 21:36:46.000000 pyaoscx-2.5.1/pyaoscx.egg-info/SOURCES.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2023-11-16 21:36:46.000000 pyaoscx-2.5.1/pyaoscx.egg-info/dependency_links.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2023-09-07 20:10:21.000000 pyaoscx-2.5.1/pyaoscx.egg-info/not-zip-safe
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       48 2023-11-16 21:36:46.000000 pyaoscx-2.5.1/pyaoscx.egg-info/requires.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       18 2023-11-16 21:36:46.000000 pyaoscx-2.5.1/pyaoscx.egg-info/top_level.txt
--rw-rw-r--   0 administrator  (1000) administrator  (1000)       38 2023-11-16 21:36:46.604548 pyaoscx-2.5.1/setup.cfg
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     1159 2023-11-16 21:31:41.000000 pyaoscx-2.5.1/setup.py
-drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-11-16 21:36:46.604548 pyaoscx-2.5.1/workflows/
--rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.5.1/workflows/__init__.py
--rw-rw-r--   0 administrator  (1000) administrator  (1000)     4027 2023-11-16 21:36:10.000000 pyaoscx-2.5.1/workflows/workflow.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.105728 pyaoscx-2.6.0/
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     4618 2024-04-30 21:21:29.101728 pyaoscx-2.6.0/PKG-INFO
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     3892 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/README.md
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.073729 pyaoscx-2.6.0/pyaoscx/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    18679 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/acl.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    36176 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/acl_entry.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    14710 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/aggregate_address.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     6678 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    14625 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/bgp_neighbor.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    15388 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/bgp_router.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    16247 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/configuration.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    18616 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/device.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13836 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/dhcp_relay.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11370 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/dns.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.085729 pyaoscx-2.6.0/pyaoscx/exceptions/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1087 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/generic_op_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      801 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/login_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      320 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/parameter_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      450 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/pyaoscx_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      879 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/response_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      321 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/unsupported_capability_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      871 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/exceptions/verification_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1005 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/firmware.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    86987 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12912 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/ipv6.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     7899 2023-11-16 21:31:41.000000 pyaoscx-2.6.0/pyaoscx/lldp_neighbor.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13019 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/mac.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12905 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/object_group.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11167 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/ospf_area.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    10174 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/ospf_interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13376 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/ospf_router.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8406 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/ospf_virtual_link.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      321 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/ospfv3_router.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8680 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/poe_interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    57456 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/pyaoscx_factory.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12322 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/pyaoscx_module.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9799 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/qos.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9149 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/qos_cos.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11962 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/qos_dscp.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9377 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/queue.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     7452 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/queue_profile.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     7662 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/queue_profile_entry.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.089728 pyaoscx-2.6.0/pyaoscx/rest/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/__init__.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.089728 pyaoscx-2.6.0/pyaoscx/rest/v1/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v1/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     2703 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v1/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    32985 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v1/interface.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.093728 pyaoscx-2.6.0/pyaoscx/rest/v10_04/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_04/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1321 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_04/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      286 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_04/interface.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.093728 pyaoscx-2.6.0/pyaoscx/rest/v10_08/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_08/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1322 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_08/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      286 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_08/interface.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.097728 pyaoscx-2.6.0/pyaoscx/rest/v10_09/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_09/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1369 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_09/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      281 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/rest/v10_09/interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12630 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/session.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11182 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/static_mac.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    16026 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/static_nexthop.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    16730 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/static_route.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8288 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/tunnel_endpoint.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.101728 pyaoscx-2.6.0/pyaoscx/utils/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/utils/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     2638 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/utils/iptools.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     3693 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/utils/list_attributes.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    26689 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/utils/util.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    22088 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/vlan.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9887 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/vni.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    26546 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/pyaoscx/vrf.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13186 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/vrf_address_family.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8257 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/pyaoscx/vsx.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.101728 pyaoscx-2.6.0/pyaoscx.egg-info/
+-rw-r--r--   0 administrator  (1000) administrator  (1000)     4618 2024-04-30 21:21:29.000000 pyaoscx-2.6.0/pyaoscx.egg-info/PKG-INFO
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1925 2024-04-30 21:21:29.000000 pyaoscx-2.6.0/pyaoscx.egg-info/SOURCES.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2024-04-30 21:21:29.000000 pyaoscx-2.6.0/pyaoscx.egg-info/dependency_links.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2023-09-07 20:10:21.000000 pyaoscx-2.6.0/pyaoscx.egg-info/not-zip-safe
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)       48 2024-04-30 21:21:29.000000 pyaoscx-2.6.0/pyaoscx.egg-info/requires.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)       18 2024-04-30 21:21:29.000000 pyaoscx-2.6.0/pyaoscx.egg-info/top_level.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)       38 2024-04-30 21:21:29.105728 pyaoscx-2.6.0/setup.cfg
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1159 2024-04-30 21:20:28.000000 pyaoscx-2.6.0/setup.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2024-04-30 21:21:29.101728 pyaoscx-2.6.0/workflows/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-09-07 20:08:34.000000 pyaoscx-2.6.0/workflows/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     4027 2023-11-16 21:36:10.000000 pyaoscx-2.6.0/workflows/workflow.py
```

### Comparing `pyaoscx-2.5.1/PKG-INFO` & `pyaoscx-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaoscx
-Version: 2.5.1
+Version: 2.6.0
 Summary: AOS-CX Python Modules
 Home-page: https://github.com/aruba/pyaoscx
 Author: Aruba Automation
 Author-email: aruba-automation@hpe.com
 License: Apache 2.0
 Keywords: networking aruba aos-cx switch rest api python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyaoscx-2.5.1/README.md` & `pyaoscx-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/acl.py` & `pyaoscx-2.6.0/pyaoscx/acl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 # (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
-from random import randint
-
+from pyaoscx.device import Device
+from pyaoscx.exceptions.parameter_error import ParameterError
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
 
 from pyaoscx.utils import util as utils
-from pyaoscx.utils.list_attributes import ListDescriptor
 
 from pyaoscx.pyaoscx_module import PyaoscxModule
 
 
 class ACL(PyaoscxModule):
     """
     Provide configuration management for ACL on AOS-CX devices.
     """
 
     base_uri = "system/acls"
     resource_uri_name = "acls"
 
     indices = ["name", "list_type"]
 
-    cfg_aces = ListDescriptor("cfg_aces")
-
     def __init__(self, session, name, list_type, uri=None, **kwargs):
         self.session = session
+        device = Device(self.session)
+        device.get(selector="status")
+        self.capabilities = device.capabilities[:]
         # Assign IDs
         self.name = name
         self.list_type = list_type
         self._uri = uri
         # List used to determine attributes related to the ACL configuration
         self.config_attrs = []
         self.materialized = False
         # Attribute dictionary used to manage the original data
         # obtained from the GET
         self.__original_attributes = {}
         # Set arguments needed for correct creation
         utils.set_creation_attrs(self, **kwargs)
         # Use to manage ACL Entries
-        self.cfg_aces = []
+        self.cfg_aces = {}
         # Attribute used to know if object was changed recently
         self.__modified = False
         # Set an initial random version
-        self._update_version()
+        self.cfg_version = 0
+
+    def __eq__(self, other):
+        return (
+            isinstance(other, ACL)
+            and self.session == other.session
+            and self.name == other.name
+            and self.list_type == other.list_type
+        )
 
     @PyaoscxModule.connected
     def get(self, depth=None, selector=None):
         """
         Perform a GET call to retrieve data for an ACL table entry and fill
             the object with the incoming attributes.
 
@@ -117,22 +125,19 @@
         # Set original attributes
         self.__original_attributes = data
 
         # Sets object as materialized
         # Information is loaded from the Device
         self.materialized = True
 
-        # Clean ACL Entries settings
-        if self.cfg_aces == []:
-            # Set ACL Entries if any
-            # Adds ACL Entries to parent ACL already
-            AclEntry = self.session.api.get_module_class(
-                self.session, "AclEntry"
-            )
-            self.cfg_aces = list(AclEntry.get_all(self.session, self).values())
+        # Set ACL Entries if any
+        AclEntry = self.session.api.get_module_class(
+            self.session, "AclEntry"
+        )
+        self.cfg_aces = AclEntry.get_all(self.session, self)
         return True
 
     @classmethod
     def get_all(cls, session):
         """
         Perform a GET call to retrieve all system ACLs, and create a dictionary
             containing them.
@@ -192,63 +197,53 @@
 
         :return modified: True if Object was modified and a PUT request
             was made.
         """
         # Variable returned
         modified = False
 
-        acl_data = utils.get_attrs(self, self.config_attrs)
-
-        # Compare dictionaries
-        if acl_data == self.__original_attributes:
-            # Object was not modified
-            modified = False
-
-        else:
-            # The version should change every time the ACL (or any of
-            # its entries) change so that it is written to hardware
-            self._update_version()
-            acl_data["cfg_version"] = self.cfg_version
+        # The version should change every time the ACL (or any of
+        # its entries) change so that it is written to hardware
+        self._update_version()
+        acl_data = {}
+        acl_data["cfg_version"] = self.cfg_version
 
-            post_data = json.dumps(acl_data)
+        post_data = json.dumps(acl_data)
 
-            uri = "{0}/{1}{2}{3}".format(
-                ACL.base_uri,
-                self.name,
-                self.session.api.compound_index_separator,
-                self.list_type,
-            )
-            try:
-                response = self.session.request("PUT", uri, data=post_data)
+        uri = "{0}/{1}{2}{3}".format(
+            ACL.base_uri,
+            self.name,
+            self.session.api.compound_index_separator,
+            self.list_type,
+        )
+        try:
+            response = self.session.request("PUT", uri, data=post_data)
 
-            except Exception as e:
-                raise ResponseError("PUT", e)
+        except Exception as e:
+            raise ResponseError("PUT", e)
 
-            if not utils._response_ok(response, "PUT"):
-                raise GenericOperationError(
-                    response.text, response.status_code
-                )
+        if not utils._response_ok(response, "PUT"):
+            raise GenericOperationError(response.text, response.status_code)
 
-            logging.info("SUCCESS: Updating %s", self)
-            # Set new original attributes
-            self.__original_attributes = acl_data
-            modified = True
+        logging.info("SUCCESS: Updating %s", self)
+        modified = True
         return modified
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new ACL table entry. Only returns if no
             exception is raised.
 
         :return modified: Boolean, True if entry was created.
         """
-        acl_data = utils.get_attrs(self, self.config_attrs)
+        acl_data = {}
         acl_data["name"] = self.name
         acl_data["list_type"] = self.list_type
+        acl_data["cfg_version"] = 0
 
         post_data = json.dumps(acl_data)
 
         try:
             response = self.session.request(
                 "POST", ACL.base_uri, data=post_data
             )
@@ -306,15 +301,15 @@
             "/rest/v10.04/system/acls/{name},{list_type}"
         :return: Acl object.
         """
         acl_arr = session.api.get_keys(response_data, ACL.resource_uri_name)
         list_type = acl_arr[1]
         name = acl_arr[0]
 
-        return ACL(session, name, list_type)
+        return cls(session, name, list_type)
 
     @classmethod
     def from_uri(cls, session, uri):
         """
         Create a Acl object given a URI.
 
         :param cls: Object's class.
@@ -386,16 +381,15 @@
     def _update_version(self):
         """
         Whenever the ACL (or any of its entries) change,the version should be
             updated so that it gets written to hardware. If the version doesn't
             change, the new configuration won't get to the hardware.
         """
 
-        new_cfg_version = randint(-9007199254740991, 9007199254740991)
-
+        new_cfg_version = self.cfg_version + 1
         if self.materialized:
             if hasattr(self, "cfg_version"):
                 logging.warning(
                     "ACL %s was modified, but the version wasn't, "
                     "so the version was changed automatically to %d",
                     str(self),
                     new_cfg_version,
@@ -405,14 +399,37 @@
                     "ACL %s didn't have a version configured. %d was added",
                     str(self),
                     new_cfg_version,
                 )
 
         self.cfg_version = new_cfg_version
 
+    @property
+    def list_type(self):
+        """
+        Getter method for the list_type attribute.
+
+        :return: String value for type.
+        """
+        return self._type
+
+    @list_type.setter
+    def list_type(self, new_type):
+        """
+        Setter method for the list_type attribute.
+        """
+        valid_types = ["mac", "ipv4", "ipv6"]
+        if new_type not in valid_types:
+            raise ParameterError(
+                "Invalid ACL type {0} valid types are: {1}".format(
+                    new_type, ", ".join(valid_types)
+                )
+            )
+        self._type = new_type
+
     ####################################################################
     # IMPERATIVE FUNCTIONS
     ####################################################################
 
     def add_acl_entry(
         self,
         sequence_num,
@@ -557,12 +574,12 @@
 
         :return: True if object was changed
         """
         # Verify ACL has the latest data
         self.get()
 
         # Delete all entries
-        self.cfg_aces = []
+        self.cfg_aces = {}
 
         # ACL Entries deleted
         # Object modified
         return True
```

### Comparing `pyaoscx-2.5.1/pyaoscx/aggregate_address.py` & `pyaoscx-2.6.0/pyaoscx/aggregate_address.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/api.py` & `pyaoscx-2.6.0/pyaoscx/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             "Ipv6": "ipv6",
             "Vlan": "vlan",
             "Vrf": "vrf",
             "Vsx": "vsx",
             "BgpRouter": "bgp_router",
             "BgpNeighbor": "bgp_neighbor",
             "VrfAddressFamily": "vrf_address_family",
+            "ObjectGroup": "object_group",
             "OspfRouter": "ospf_router",
             "Ospfv3Router": "ospfv3_router",
             "OspfVlink": "ospf_virtual_link",
             "OspfArea": "ospf_area",
             "OspfInterface": "ospf_interface",
             "DhcpRelay": "dhcp_relay",
             "ACL": "acl",
```

### Comparing `pyaoscx-2.5.1/pyaoscx/bgp_neighbor.py` & `pyaoscx-2.6.0/pyaoscx/bgp_neighbor.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/bgp_router.py` & `pyaoscx-2.6.0/pyaoscx/bgp_router.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/configuration.py` & `pyaoscx-2.6.0/pyaoscx/configuration.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/device.py` & `pyaoscx-2.6.0/pyaoscx/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.config_attrs = []
         self.materialized = False
         self.__original_attributes = {}
         # Set firmware version
         self.get_firmware_version()
 
     @PyaoscxModule.connected
-    def get(self):
+    def get(self, selector=None):
         """
         Perform a GET call to retrieve device attributes. After data from
             response, Device class attributes are generated using
             create_attrs().
         """
         logging.info("Retrieving the switch attributes and capabilities")
 
@@ -55,30 +55,19 @@
             "software_images",
             "software_info",
             "software_version",
             "qos_defaults",
             "lldp_mgmt_neighbor_info",
         ]
 
-        configurable_attrs = [
-            "domain_name",
-            "hostname",
-            "other_config",
-            "qos_config",
-            "qos_default",
-            "q_profile_default",
-        ]
-
-        # Concatenate both config and non-config attrs without duplicates
-        all_attributes = list(set(non_configurable_attrs + configurable_attrs))
-
-        attributes_list = ",".join(all_attributes)
-        uri = "system?attributes={0}&depth={1}".format(
-            attributes_list, self.session.api.default_depth
-        )
+        uri = "system?depth={0}".format(self.session.api.default_depth)
+        if selector:
+            uri += "&selector={0}".format(selector)
+        else:
+            uri += "&attributes={0}".format(",".join(non_configurable_attrs))
 
         try:
             response = self.session.request("GET", uri)
         except Exception as e:
             raise ResponseError("GET", e)
 
         if not utils._response_ok(response, "GET"):
```

### Comparing `pyaoscx-2.5.1/pyaoscx/dhcp_relay.py` & `pyaoscx-2.6.0/pyaoscx/dhcp_relay.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/dns.py` & `pyaoscx-2.6.0/pyaoscx/dns.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/exceptions/generic_op_error.py` & `pyaoscx-2.6.0/pyaoscx/exceptions/generic_op_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/exceptions/login_error.py` & `pyaoscx-2.6.0/pyaoscx/exceptions/login_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/exceptions/response_error.py` & `pyaoscx-2.6.0/pyaoscx/exceptions/response_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/exceptions/verification_error.py` & `pyaoscx-2.6.0/pyaoscx/exceptions/verification_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/firmware.py` & `pyaoscx-2.6.0/pyaoscx/firmware.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/interface.py` & `pyaoscx-2.6.0/pyaoscx/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# (C) Copyright 2019-2022 Hewlett Packard Enterprise Development LP.
+# (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
 import re
 
 from copy import deepcopy
-from random import randint
+
 from urllib.parse import quote_plus, unquote_plus
 from warnings import warn
 
 from netaddr import mac_eui48
 from netaddr import EUI as MacAddress
 from netaddr.core import AddrFormatError
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.parameter_error import ParameterError
 from pyaoscx.exceptions.response_error import ResponseError
 from pyaoscx.exceptions.verification_error import VerificationError
 
 from pyaoscx.utils import util as utils
+from pyaoscx.utils.iptools import overlapping_ips
 from pyaoscx.utils.list_attributes import ListDescriptor
 
 import pyaoscx.vrf as vrf_mod
 
 from pyaoscx.ipv6 import Ipv6
 from pyaoscx.vlan import Vlan
 
@@ -234,15 +235,15 @@
                 vlan_id, vlan = Vlan.from_uri(self.session, uri)
                 # Add VLAN to dictionary
                 vlan_trunks.append(vlan)
             # Set list as VLANs
             self.vlan_trunks = vlan_trunks
 
         # Set all ACLs
-        from pyaoscx.acl import ACL
+        ACL = self.session.api.get_module_class(self.session, "ACL")
 
         if hasattr(self, "aclmac_in_cfg") and self.aclmac_in_cfg is not None:
             # Create Acl object
             acl = ACL.from_response(self.session, self.aclmac_in_cfg)
             # Materialize Acl object
             acl.get()
             self.aclmac_in_cfg = acl
@@ -613,61 +614,97 @@
 
             # Set values in correct form
             iface_data["vlan_trunks"] = formated_vlans
 
         # Set all ACLs
         if "aclmac_in_cfg" in iface_data and self.aclmac_in_cfg:
             # Set values in correct form
+            self.aclmac_in_cfg.get()
             iface_data["aclmac_in_cfg"] = self.aclmac_in_cfg.get_info_format()
+            iface_data[
+                "aclmac_in_cfg_version"
+            ] = self.aclmac_in_cfg_version
 
         if "aclmac_out_cfg" in iface_data and self.aclmac_out_cfg:
             # Set values in correct form
+            self.aclmac_out_cfg.get()
             iface_data[
                 "aclmac_out_cfg"
             ] = self.aclmac_out_cfg.get_info_format()
+            iface_data[
+                "aclmac_out_cfg_version"
+            ] = self.aclmac_out_cfg_version
 
         if "aclv4_in_cfg" in iface_data and self.aclv4_in_cfg:
             # Set values in correct form
+            self.aclv4_in_cfg.get()
             iface_data["aclv4_in_cfg"] = self.aclv4_in_cfg.get_info_format()
+            iface_data["aclv4_in_cfg_version"] = self.aclv4_in_cfg_version
 
         if "aclv4_out_cfg" in iface_data and self.aclv4_out_cfg:
             # Set values in correct form
+            self.aclv4_out_cfg.get()
             iface_data["aclv4_out_cfg"] = self.aclv4_out_cfg.get_info_format()
+            iface_data[
+                "aclv4_out_cfg_version"
+            ] = self.aclv4_out_cfg_version
 
         if "aclv4_routed_in_cfg" in iface_data and self.aclv4_routed_in_cfg:
             # Set values in correct form
+            self.aclv4_routed_in_cfg.get()
             iface_data[
                 "aclv4_routed_in_cfg"
             ] = self.aclv4_routed_in_cfg.get_info_format()
+            iface_data[
+                "aclv4_routed_in_cfg_version"
+            ] = self.aclv4_routed_in_cfg_version
 
         if "aclv4_routed_out_cfg" in iface_data and self.aclv4_routed_out_cfg:
             # Set values in correct form
+            self.aclv4_routed_out_cfg.get()
             iface_data[
                 "aclv4_routed_out_cfg"
             ] = self.aclv4_routed_out_cfg.get_info_format()
+            iface_data[
+                "aclv4_routed_out_cfg_version"
+            ] = self.aclv4_routed_out_cfg_version
 
         if "aclv6_in_cfg" in iface_data and self.aclv6_in_cfg:
             # Set values in correct form
+            self.aclv6_in_cfg.get()
             iface_data["aclv6_in_cfg"] = self.aclv6_in_cfg.get_info_format()
+            iface_data["aclv6_in_cfg_version"] = self.aclv6_in_cfg_version
 
         if "aclv6_out_cfg" in iface_data and self.aclv6_out_cfg:
             # Set values in correct form
+            self.aclv6_out_cfg.get()
             iface_data["aclv6_out_cfg"] = self.aclv6_out_cfg.get_info_format()
+            iface_data[
+                "aclv6_out_cfg_version"
+            ] = self.aclv6_out_cfg_version
 
         if "aclv6_routed_in_cfg" in iface_data and self.aclv6_routed_in_cfg:
             # Set values in correct form
+            self.aclv6_routed_in_cfg.get()
             iface_data[
                 "aclv6_routed_in_cfg"
             ] = self.aclv6_routed_in_cfg.get_info_format()
+            iface_data[
+                "aclv6_routed_in_cfg_version"
+            ] = self.aclv6_routed_in_cfg_version
 
         if "aclv6_routed_out_cfg" in iface_data and self.aclv6_routed_out_cfg:
             # Set values in correct form
+            self.aclv6_routed_out_cfg.get()
             iface_data[
                 "aclv6_routed_out_cfg"
             ] = self.aclv6_routed_out_cfg.get_info_format()
+            iface_data[
+                "aclv6_routed_out_cfg_version"
+            ] = self.aclv6_routed_out_cfg_version
 
         uri = "{0}/{1}".format(Interface.base_uri, self.percents_name)
 
         # Compare dictionaries
         if iface_data == self.__original_attributes:
             # Object was not modified
             modified = False
@@ -1035,21 +1072,36 @@
                 self.interfaces.append(port_obj)
 
         # Set IPv4
         if ipv4 == []:
             self.ip4_address = None
             self.ip4_address_secondary = None
         elif isinstance(ipv4, list):
+            for ip_address in ipv4:
+                overlapping_ips(
+                    self.session,
+                    self.name,
+                    ip4_addr=ip_address,
+                    ip6_addr=None,
+                    new_vrf=vrf,
+                )
             self.ip4_address = ipv4[0]
             self.ip4_address_secondary = ipv4[1:]
 
         # Set IPv6
         ipv6_configured = False
         if ipv6 is not None and ipv6 != []:
             for ip_address in ipv6:
+                overlapping_ips(
+                    self.session,
+                    self.name,
+                    ip4_addr=None,
+                    ip6_addr=ip_address,
+                    new_vrf=vrf,
+                )
                 # Verify if incoming address is a string
                 if isinstance(ip_address, str):
                     # Create Ipv6 object -- add it to ipv6_addresses internal
                     # list
                     ip_address = self.session.api.get_module(
                         self.session,
                         "Ipv6",
@@ -1152,26 +1204,40 @@
                     vlan_tag.apply()
 
             self.vlan_tag = vlan_tag
 
         # Set IPv4
         if ipv4 is not None and ipv4 != []:
             for i in range(len(ipv4)):
+                overlapping_ips(
+                    self.session,
+                    self.name,
+                    ip4_addr=ipv4[i],
+                    ip6_addr=None,
+                    new_vrf=vrf,
+                )
                 if i == 0:
                     self.ip4_address = ipv4[i]
                 else:
                     self.ip4_address_secondary.append(ipv4[i])
         # If IPv4 is empty, delete
         elif ipv4 == []:
             self.ip4_address = None
             self.ip4_address_secondary = None
         # Set IPv6
         ipv6_configured = False
         if ipv6 is not None and ipv6 != []:
             for ip_address in ipv6:
+                overlapping_ips(
+                    self.session,
+                    self.name,
+                    ip4_addr=None,
+                    ip6_addr=ip_address,
+                    new_vrf=vrf,
+                )
                 # Verify if incoming address is a string
                 if isinstance(ip_address, str):
                     # Create Ipv6 object -- add it to ipv6_addresses internal
                     # list
                     ip_address = self.session.api.get_module(
                         self.session,
                         "Ipv6",
@@ -1599,47 +1665,14 @@
             if member.name == interface_name:
                 # Remove interface from Member
                 self.interfaces.remove(member)
 
         # When changes are applied, port is disabled and lacp key changed
         return self.apply()
 
-    def clear_acl(self, acl_type, acl_direction):
-        """
-        Clear an interface's ACL.
-
-        :param acl_type: Type of ACL: options are 'aclv4_out', 'aclv4_in',
-            'aclv6_in', or 'aclv6_out'.
-        :return: True if object was changed.
-        """
-        if acl_type == "ipv6":
-            if acl_direction == "in":
-                self.aclv6_in_cfg = None
-                self.aclv6_in_cfg_version = None
-            else:
-                self.aclv6_out_cfg = None
-                self.aclv6_out_cfg_version = None
-        if acl_type == "ipv4":
-            if acl_direction == "in":
-                self.aclv4_in_cfg = None
-                self.aclv4_in_cfg_version = None
-            else:
-                self.aclv4_out_cfg = None
-                self.aclv4_out_cfg_version = None
-        if acl_type == "mac":
-            if acl_direction == "in":
-                self.aclmac_in_cfg = None
-                self.aclmac_in_cfg_version = None
-            else:
-                self.aclmac_out_cfg = None
-                self.aclmac_out_cfg_version = None
-
-        # Apply Changes
-        return self.apply()
-
     def initialize_interface_entry(self):
         """
         Initialize Interface to its default state.
 
         :return: True if object was changed.
         """
         # Set interface to default settings
@@ -1794,14 +1827,26 @@
         self.vsx_sync = []
         self.vsx_virtual_gw_mac_v4 = None
         self.vsx_virtual_ip4 = []
 
         # Apply changes
         return self.apply()
 
+    def delete_active_gateway(self):
+        """
+        Deelte only IPv4 settings on a VLAN Interface.
+
+        :return: True if object was changed.
+        """
+
+        self.vsx_virtual_gw_mac_v4 = None
+        self.vsx_virtual_ip4 = []
+
+        return self.apply()
+
     def configure_l3_ipv4_port(
         self, ip_address=None, port_desc=None, vrf="default"
     ):
         """
         Function will enable routing on the port and update the IPv4 address
             if given.
 
@@ -2041,14 +2086,40 @@
                 rate_limits[traffic_type + "_units"] = unit
 
         self.rate_limits = rate_limits
 
         # Apply changes
         return self.apply()
 
+    @PyaoscxModule.materialized
+    def set_acl(self, acl_name, list_type, direction):
+        """
+        Attach ACL to an interface
+
+        :param acl_name: The name of the ACL.
+        :param list_type: The type of the ACL (mac, ipv4 or ipv6).
+        :param direction: The direction of the ACL (in, out, routed-in,
+            routed-out)
+        :return: True if the object was changed
+        """
+        return utils.set_acl(self, acl_name, list_type, direction)
+
+    @PyaoscxModule.materialized
+    def clear_acl(self, list_type, direction):
+        """
+        Removes ACL from an interface
+
+        :param list_type: The type of the ACL (mac, ipv4 or ipv6).
+        :param direction: The direction of the ACL (in, out, routed-in,
+            routed-out)
+        :return: True if the object was changed
+        """
+        return utils.clear_acl(self, list_type, direction)
+
+    @PyaoscxModule.deprecated
     def update_acl_in(self, acl_name, list_type):
         """
         Perform GET and PUT calls to apply ACL on an interface. This function
             specifically applies an ACL to Ingress traffic of the interface.
 
         :param acl_name: Alphanumeric String that is the name of the ACL
         :param list_type: Alphanumeric String of IPv4, IPv6 or MAC to specify
@@ -2058,41 +2129,25 @@
         # Create Acl object
         acl_obj = self.session.api.get_module(
             self.session, "ACL", index_id=acl_name, list_type=list_type
         )
         # Get the current version
         acl_obj.get()
 
-        new_cfg_version = randint(-9007199254740991, 9007199254740991)
-
         if list_type == "ipv6":
             self.aclv6_in_cfg = acl_obj
-            if (
-                hasattr(self, "aclv6_in_cfg_version")
-                and self.aclv6_in_cfg_version is None
-            ):
-                self.aclv6_in_cfg_version = new_cfg_version
         elif list_type == "ipv4":
             self.aclv4_in_cfg = acl_obj
-            if (
-                hasattr(self, "aclv4_in_cfg_version")
-                and self.aclv4_in_cfg_version is None
-            ):
-                self.aclv4_in_cfg_version = new_cfg_version
         elif list_type == "mac":
             self.aclmac_in_cfg = acl_obj
-            if (
-                hasattr(self, "aclmac_in_cfg_version")
-                and self.aclmac_in_cfg_version is None
-            ):
-                self.aclmac_in_cfg_version = new_cfg_version
 
         # Apply changes
         return self.apply()
 
+    @PyaoscxModule.deprecated
     def update_acl_out(self, acl_name, list_type):
         """
         Perform GET and PUT calls to apply ACL on an interface. This function
             specifically applies an ACL to Egress traffic of the interface,
             which must be a routing interface.
 
         :param acl_name: Alphanumeric String that is the name of the ACL.
@@ -2103,37 +2158,20 @@
         # Create Acl object
         acl_obj = self.session.api.get_module(
             self.session, "ACL", index_id=acl_name, list_type=list_type
         )
         # Get the current version
         acl_obj.get()
 
-        new_cfg_version = randint(-9007199254740991, 9007199254740991)
-
         if list_type == "ipv6":
             self.aclv6_out_cfg = acl_obj
-            if (
-                hasattr(self, "aclv6_out_cfg_version")
-                and self.aclv6_out_cfg_version is None
-            ):
-                self.aclv6_out_cfg_version = new_cfg_version
         elif list_type == "ipv4":
             self.aclv4_out_cfg = acl_obj
-            if (
-                hasattr(self, "aclv4_out_cfg_version")
-                and self.aclv4_out_cfg_version is None
-            ):
-                self.aclv4_out_cfg_version = new_cfg_version
         elif list_type == "mac":
             self.aclmac_out_cfg = acl_obj
-            if (
-                hasattr(self, "aclmac_out_cfg_version")
-                and self.aclmac_out_cfg_version is None
-            ):
-                self.aclmac_out_cfg_version = new_cfg_version
 
         # Routing
         self.routing = True
 
         # Apply changes
         return self.apply()
 
@@ -2178,15 +2216,15 @@
             raise VerificationError(
                 "Configuring port-security is allowed only on bridged ports."
             )
 
         self.port_security["enable"] = True
 
         device = Device(self.session)
-        device.get()
+        device.get(selector="status")
         max_clients = device.capacities[
             "port_access_port_security_max_client_limit"
         ]
         if client_limit and (1 > client_limit or client_limit > max_clients):
             raise ParameterError(
                 "Can only authorize 1 to {0} clients".format(max_clients)
             )
```

### Comparing `pyaoscx-2.5.1/pyaoscx/ipv6.py` & `pyaoscx-2.6.0/pyaoscx/ipv6.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/lldp_neighbor.py` & `pyaoscx-2.6.0/pyaoscx/lldp_neighbor.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/mac.py` & `pyaoscx-2.6.0/pyaoscx/mac.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/ospf_area.py` & `pyaoscx-2.6.0/pyaoscx/ospf_area.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/ospf_interface.py` & `pyaoscx-2.6.0/pyaoscx/ospf_interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/ospf_router.py` & `pyaoscx-2.6.0/pyaoscx/ospf_router.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/ospf_virtual_link.py` & `pyaoscx-2.6.0/pyaoscx/ospf_virtual_link.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/poe_interface.py` & `pyaoscx-2.6.0/pyaoscx/poe_interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/pyaoscx_factory.py` & `pyaoscx-2.6.0/pyaoscx/pyaoscx_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1618,7 +1618,24 @@
             utils.create_attrs(tep, kwargs)
         except GenericOperationError:
             pass
         finally:
             tep.apply()
 
         return tep
+
+    def object_group(self, name, group_type):
+        """
+        Create an Object Group
+        :param name: Name of Object Group
+        :param group_type: Type of Object Group (ipv4, ipv6, l4port)
+        """
+        group_obj = self.session.api.get_module(
+            self.session, "ObjectGroup", index_id=name, object_type=group_type
+        )
+        try:
+            group_obj.get()
+        except GenericOperationError:
+            pass
+        finally:
+            group_obj.apply()
+        return group_obj
```

### Comparing `pyaoscx-2.5.1/pyaoscx/pyaoscx_module.py` & `pyaoscx-2.6.0/pyaoscx/pyaoscx_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,15 @@
                 if new is not None and old != new:
                     return True
             elif hasattr(replacement, param_name):
                 # In this case the replacement has an attribute that the
                 # current lacks, so a replacement is required
                 if getattr(replacement, param_name) is not None:
                     return True
+        return False
 
     def _extract_missing_parameters_from(self, other):
         """
         Extract the missing configuration parameters from another PYAOSCX
             Module, to incorporate them as their own. This is useful when
             replacing (delete+create) Modules. If the Module has to be
             replaced, the parameters that are not specified (locally) should
```

### Comparing `pyaoscx-2.5.1/pyaoscx/qos.py` & `pyaoscx-2.6.0/pyaoscx/qos.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         if trust_mode not in allowed_trust_modes:
             raise VerificationError(
                 "ERROR: QoS trust mode must be one of: ", allowed_trust_modes
             )
 
         device = Device(session)
         if not device.materialized:
-            device.get()
+            device.get(selector="writable")
         # If the incoming value is the same as the current one,
         # there's no need to change it
         if device.qos_config.get("qos_trust") == trust_mode:
             return False
 
         modified = False
         if trust_mode == "default":
```

### Comparing `pyaoscx-2.5.1/pyaoscx/qos_cos.py` & `pyaoscx-2.6.0/pyaoscx/qos_cos.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/qos_dscp.py` & `pyaoscx-2.6.0/pyaoscx/qos_dscp.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/queue.py` & `pyaoscx-2.6.0/pyaoscx/queue.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/queue_profile.py` & `pyaoscx-2.6.0/pyaoscx/queue_profile.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/queue_profile_entry.py` & `pyaoscx-2.6.0/pyaoscx/queue_profile_entry.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/rest/v1/api.py` & `pyaoscx-2.6.0/pyaoscx/rest/v1/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/rest/v1/interface.py` & `pyaoscx-2.6.0/pyaoscx/rest/v1/interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/rest/v10_04/api.py` & `pyaoscx-2.6.0/pyaoscx/rest/v10_04/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/rest/v10_08/api.py` & `pyaoscx-2.6.0/pyaoscx/rest/v10_08/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/rest/v10_09/api.py` & `pyaoscx-2.6.0/pyaoscx/rest/v10_09/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/session.py` & `pyaoscx-2.6.0/pyaoscx/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,22 @@
 
         # TODO: remove base_url once all modules use the internal
         # request methods
         self.base_url = "https://{0}/rest/v{1}/".format(self.ip, self.api)
         self.resource_prefix = "/rest/v{0}/".format(self.api)
         self.__username = self.__password = ""
 
+    def __eq__(self, other):
+        return (
+            isinstance(other, Session)
+            and self.ip == other.ip
+            and str(self.api) == str(other.api)
+            and self.__username == other.__username
+        )
+
     def cookies(self):
         """
         Return the cookie stored in the requests' session.
         """
         return self.s.cookies._cookies
 
     @classmethod
```

### Comparing `pyaoscx-2.5.1/pyaoscx/static_mac.py` & `pyaoscx-2.6.0/pyaoscx/static_mac.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/static_nexthop.py` & `pyaoscx-2.6.0/pyaoscx/static_nexthop.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,21 +122,19 @@
         # Remove ID
         if "id" in self.__original_attributes:
             self.__original_attributes.pop("id")
 
         # If the Static Route has a port inside the switch
         if "port" in data and self.port:
             port_response = self.port
-            interface_cls = self.session.api.get_module(
-                self.session, "Interface", ""
+            Interface = self.session.api.get_module_class(
+                self.session, "Interface"
             )
             # Set port as a Interface Object
-            self.port = interface_cls.from_response(
-                self.session, port_response
-            )
+            self.port = Interface.from_response(self.session, port_response)
             # Materialize port
             self.port.get()
 
         # Sets object as materialized
         # Information is loaded from the Device
         self.materialized = True
 
@@ -224,14 +222,20 @@
 
         static_nexthop_data = utils.get_attrs(self, self.config_attrs)
 
         # Get port uri
         if hasattr(self, "port") and self.port:
             static_nexthop_data["port"] = self.port.get_info_format()
 
+        if (
+            "bfd" not in self.__parent_static_route.capabilities
+            and "bfd_enable" in static_nexthop_data
+        ):
+            del static_nexthop_data["bfd_enable"]
+
         uri = "{0}/{1}".format(self.base_uri, self.id)
 
         # Compare dictionaries
         if static_nexthop_data == self.__original_attributes:
             # Object was not modified
             modified = False
 
@@ -269,14 +273,20 @@
         static_nexthop_data = utils.get_attrs(self, self.config_attrs)
         static_nexthop_data["id"] = self.id
 
         # Get port uri
         if hasattr(self, "port") and self.port:
             static_nexthop_data["port"] = self.port.get_info_format()
 
+        if (
+            "bfd" not in self.__parent_static_route.capabilities
+            and "bfd_enable" in static_nexthop_data
+        ):
+            del static_nexthop_data["bfd_enable"]
+
         post_data = json.dumps(static_nexthop_data)
 
         try:
             response = self.session.request(
                 "POST", self.base_uri, data=post_data
             )
```

### Comparing `pyaoscx-2.5.1/pyaoscx/static_route.py` & `pyaoscx-2.6.0/pyaoscx/static_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,42 @@
 
 import json
 import logging
 import re
 
 from urllib.parse import quote_plus, unquote_plus
 
+from pyaoscx.device import Device
+
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
 
+from pyaoscx.pyaoscx_module import PyaoscxModule
+
 from pyaoscx.utils import util as utils
 from pyaoscx.utils.list_attributes import ListDescriptor
 
-from pyaoscx.static_nexthop import StaticNexthop
-
-from pyaoscx.pyaoscx_module import PyaoscxModule
-
 
 class StaticRoute(PyaoscxModule):
     """
     Provide configuration management for Static Route on AOS-CX devices.
     """
 
     indices = ["prefix"]
     static_nexthops = ListDescriptor("static_nexthops")
     resource_uri_name = "static_routes"
 
     def __init__(self, session, prefix, parent_vrf, uri=None, **kwargs):
 
         self.session = session
+        # Need to check capabilities to verify
+        # switch is BFD capable
+        device = Device(session)
+        device.get(selector="status")
+        self.capabilities = device.capabilities[:]
         # Assign IP
         self.prefix = unquote_plus(prefix)
         self.reference_address = quote_plus(self.prefix)
         self.address_family = utils.get_ip_version(self.prefix)
         # Assign parent Vrf object
         self.__set_vrf(parent_vrf)
         self._uri = uri
@@ -136,14 +141,17 @@
         if "prefix" in self.__original_attributes:
             self.__original_attributes.pop("prefix")
         # Remove Static Nexthops
         if "static_nexthops" in self.__original_attributes:
             self.__original_attributes.pop("static_nexthops")
 
         # Clean Static Nexthops settings
+        StaticNexthop = self.session.api.get_module_class(
+            self.session, "StaticNexthop"
+        )
         if self.static_nexthops == []:
             # Set Static Nexthops if any
             # Adds Static Nexthop to parent Vrf object
             StaticNexthop.get_all(self.session, self)
 
         # Sets object as materialized
         # Information is loaded from the Device
```

### Comparing `pyaoscx-2.5.1/pyaoscx/tunnel_endpoint.py` & `pyaoscx-2.6.0/pyaoscx/tunnel_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/utils/list_attributes.py` & `pyaoscx-2.6.0/pyaoscx/utils/list_attributes.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/vlan.py` & `pyaoscx-2.6.0/pyaoscx/vlan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # (C) Copyright 2019-2023 Hewlett Packard Enterprise Development LP.
 # Apache License 2.0
 
 import json
 import logging
-from random import randint
 import re
 
 from pyaoscx.exceptions.generic_op_error import GenericOperationError
 from pyaoscx.exceptions.response_error import ResponseError
 from pyaoscx.exceptions.verification_error import VerificationError
 from pyaoscx.device import Device
 
@@ -98,37 +97,58 @@
         if "id" in self._original_attributes:
             self._original_attributes.pop("id")
         # Remove macs
         if "macs" in self._original_attributes:
             self._original_attributes.pop("macs")
 
         # Set all ACLs
-        from pyaoscx.acl import ACL
+        ACL = self.session.api.get_module_class(self.session, "ACL")
 
         if hasattr(self, "aclmac_in_cfg") and self.aclmac_in_cfg is not None:
             # Create Acl object
             acl = ACL.from_response(self.session, self.aclmac_in_cfg)
             # Materialize Acl object
             acl.get()
             self.aclmac_in_cfg = acl
 
+        if hasattr(self, "aclmac_out_cfg") and self.aclmac_out_cfg is not None:
+            # Create Acl object
+            acl = ACL.from_response(self.session, self.aclmac_out_cfg)
+            # Materialize Acl object
+            acl.get()
+            self.aclmac_out_cfg = acl
+
         if hasattr(self, "aclv4_in_cfg") and self.aclv4_in_cfg is not None:
             # Create Acl object
             acl = ACL.from_response(self.session, self.aclv4_in_cfg)
             # Materialize Acl object
             acl.get()
             self.aclv4_in_cfg = acl
 
+        if hasattr(self, "aclv4_out_cfg") and self.aclv4_out_cfg is not None:
+            # Create Acl object
+            acl = ACL.from_response(self.session, self.aclv4_out_cfg)
+            # Materialize Acl object
+            acl.get()
+            self.aclv4_out_cfg = acl
+
         if hasattr(self, "aclv6_in_cfg") and self.aclv6_in_cfg is not None:
             # Create Acl object
             acl = ACL.from_response(self.session, self.aclv6_in_cfg)
             # Materialize Acl object
             acl.get()
             self.aclv6_in_cfg = acl
 
+        if hasattr(self, "aclv6_out_cfg") and self.aclv6_out_cfg is not None:
+            # Create Acl object
+            acl = ACL.from_response(self.session, self.aclv6_out_cfg)
+            # Materialize Acl object
+            acl.get()
+            self.aclv6_out_cfg = acl
+
         # Clean MACs
         if not self.macs:
             # Set MACs if any
             # Adds macs to parent Vlan object
             Mac.get_all(self.session, self)
 
         # Set Static MACs
@@ -208,25 +228,51 @@
         if self.vsx_sync is not None:
             vlan_data["vsx_sync"] = self.vsx_sync
         if hasattr(self, "voice"):
             vlan_data["voice"] = self.voice
         if hasattr(self, "mgmd_enable"):
             vlan_data["mgmd_enable"] = self.mgmd_enable
         # Set all ACLs
-        if "aclmac_in_cfg" in vlan_data and self.aclmac_in_cfg is not None:
+        if "aclmac_in_cfg" in vlan_data and self.aclmac_in_cfg:
             # Set values in correct form
+            self.aclmac_in_cfg.get()
             vlan_data["aclmac_in_cfg"] = self.aclmac_in_cfg.get_info_format()
+            vlan_data["aclmac_in_cfg_version"] = self.aclmac_in_cfg_version
 
-        if "aclv4_in_cfg" in vlan_data and self.aclv4_in_cfg is not None:
+        if "aclmac_out_cfg" in vlan_data and self.aclmac_out_cfg:
             # Set values in correct form
+            self.aclmac_out_cfg.get()
+            vlan_data["aclmac_out_cfg"] = self.aclmac_out_cfg.get_info_format()
+            vlan_data[
+                "aclmac_out_cfg_version"
+            ] = self.aclmac_out_cfg_version
+
+        if "aclv4_in_cfg" in vlan_data and self.aclv4_in_cfg:
+            # Set values in correct form
+            self.aclv4_in_cfg.get()
             vlan_data["aclv4_in_cfg"] = self.aclv4_in_cfg.get_info_format()
+            vlan_data["aclv4_in_cfg_version"] = self.aclv4_in_cfg_version
+
+        if "aclv4_out_cfg" in vlan_data and self.aclv4_out_cfg:
+            # Set values in correct form
+            self.aclv4_out_cfg.get()
+            vlan_data["aclv4_out_cfg"] = self.aclv4_out_cfg.get_info_format()
+            vlan_data["aclv4_out_cfg_version"] = self.aclv4_out_cfg_version
 
-        if "aclv6_in_cfg" in vlan_data and self.aclv6_in_cfg is not None:
+        if "aclv6_in_cfg" in vlan_data and self.aclv6_in_cfg:
             # Set values in correct form
+            self.aclv6_in_cfg.get()
             vlan_data["aclv6_in_cfg"] = self.aclv6_in_cfg.get_info_format()
+            vlan_data["aclv6_in_cfg_version"] = self.aclv6_in_cfg_version
+
+        if "aclv6_out_cfg" in vlan_data and self.aclv6_out_cfg:
+            # Set values in correct form
+            self.aclv6_out_cfg.get()
+            vlan_data["aclv6_out_cfg"] = self.aclv6_out_cfg.get_info_format()
+            vlan_data["aclv6_out_cfg_version"] = self.aclv6_out_cfg_version
 
         return self._put_data(vlan_data)
 
     @PyaoscxModule.connected
     def create(self):
         """
         Perform a POST call to create a new VLAN using the object's attributes
@@ -244,26 +290,26 @@
             vlan_data["voice"] = self.voice
         if hasattr(self, "mgmd_enable"):
             vlan_data["mgmd_enable"] = self.mgmd_enable
         if isinstance(self.id, str):
             self.id = int(self.id)
         vlan_data["id"] = self.id
         vlan_data["name"] = (
-            self.name if self.name else "VLAN {}". format(str(self.id))
+            self.name if self.name else "VLAN {}".format(str(self.id))
         )
         return self._post_data(vlan_data)
 
     @property
     def vsx_sync(self):
         return self._vsx_valid if hasattr(self, "_vsx_valid") else None
 
     @vsx_sync.setter
     def vsx_sync(self, new_vsx_sync):
         device = Device(self.session)
-        device.get()
+        device.get(selector="status")
         if "vsx" not in device.capabilities:
             raise VerificationError(
                 "vsx_sync is not supported on this platform"
             )
         self._vsx_valid = new_vsx_sync
 
     @PyaoscxModule.connected
@@ -433,14 +479,15 @@
         if self.type == "static" and admin_conf_state is not None:
             # admin-configured state can only be set on static VLANs
             self.admin = admin_conf_state
 
         # Apply changes inside switch
         return self.apply()
 
+    @PyaoscxModule.deprecated
     def attach_acl_in(self, acl_name, list_type):
         """
         Update ACL IN values inside a Vlan object.
 
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
@@ -449,34 +496,23 @@
         # Create Acl object
         acl_obj = self.session.api.get_module(
             self.session, "ACL", index_id=acl_name, list_type=list_type
         )
 
         if list_type == "ipv6":
             self.aclv6_in_cfg = acl_obj
-            if self.aclv6_in_cfg_version is None:
-                self.aclv6_in_cfg_version = randint(
-                    -9007199254740991, 9007199254740991
-                )
         if list_type == "ipv4":
             self.aclv4_in_cfg = acl_obj
-            if self.aclv4_in_cfg_version is None:
-                self.aclv4_in_cfg_version = randint(
-                    -9007199254740991, 9007199254740991
-                )
         if list_type == "mac":
             self.aclmac_in_cfg = acl_obj
-            if self.aclmac_in_cfg_version is None:
-                self.aclmac_in_cfg_version = randint(
-                    -9007199254740991, 9007199254740991
-                )
 
         # Apply changes
         return self.apply()
 
+    @PyaoscxModule.deprecated
     def attach_acl_out(self, acl_name, list_type):
         """
         Update ACL OUT values inside a Vlan object.
 
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
@@ -485,34 +521,23 @@
         # Create Acl object
         acl_obj = self.session.api.get_module(
             self.session, "ACL", index_id=acl_name, list_type=list_type
         )
 
         if list_type == "ipv6":
             self.aclv6_out_cfg = acl_obj
-            if self.aclv6_out_cfg_version is None:
-                self.aclv6_out_cfg_version = randint(
-                    -9007199254740991, 9007199254740991
-                )
         if list_type == "ipv4":
             self.aclv4_out_cfg = acl_obj
-            if self.aclv4_out_cfg_version is None:
-                self.aclv4_out_cfg_version = randint(
-                    -9007199254740991, 9007199254740991
-                )
         if list_type == "mac":
             self.aclmac_out_cfg = acl_obj
-            if self.aclmac_out_cfg_version is None:
-                self.aclmac_out_cfg_version = randint(
-                    -9007199254740991, 9007199254740991
-                )
 
         # Apply changes
         return self.apply()
 
+    @PyaoscxModule.deprecated
     def detach_acl_in(self, acl_name, list_type):
         """
         Detach an ACL from a VLAN.
 
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
@@ -527,14 +552,15 @@
         elif list_type == "mac":
             self.aclmac_in_cfg = None
             self.aclmac_in_cfg_version = None
 
         # Apply changes
         return self.apply()
 
+    @PyaoscxModule.deprecated
     def detach_acl_out(self, acl_name, list_type):
         """
         Detach an ACL from a VLAN.
 
         :param acl_name: Alphanumeric String that is the name of the ACL.
         :param list_type: Alphanumeric String of ipv4, ipv6, or mac to specify
             the type of ACL.
@@ -549,14 +575,39 @@
         elif list_type == "mac":
             self.aclmac_out_cfg = None
             self.aclmac_out_cfg_version = None
 
         # Apply changes
         return self.apply()
 
+    @PyaoscxModule.materialized
+    def set_acl(self, acl_name, list_type, direction):
+        """
+        Attach ACL to a VLAN
+
+        :param acl_name: The name of the ACL.
+        :param list_type: The type of the ACL (mac, ipv4 or ipv6).
+        :param direction: The direction of the ACL (in, out, routed-in,
+            routed-out)
+        :return: True if the object was changed
+        """
+        return utils.set_acl(self, acl_name, list_type, direction)
+
+    @PyaoscxModule.materialized
+    def clear_acl(self, list_type, direction):
+        """
+        Removes ACL from a VLAN
+
+        :param list_type: The type of the ACL (mac, ipv4 or ipv6).
+        :param direction: The direction of the ACL (in, out, routed-in,
+            routed-out)
+        :return: True if the object was changed
+        """
+        return utils.clear_acl(self, list_type, direction)
+
     def get_mac(self, from_id, mac_address):
         """
         Create an Mac object.
 
         :param from_id: String source of the MAC address. Must be "dynamic",
             "VSX", "static", "VRRP", "port-access-security", "evpn", or "hsc".
         :param mac_address: String MAC address. Example: '01:02:03:04:05:06'
```

### Comparing `pyaoscx-2.5.1/pyaoscx/vni.py` & `pyaoscx-2.6.0/pyaoscx/vni.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/vrf.py` & `pyaoscx-2.6.0/pyaoscx/vrf.py`

 * *Files 7% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
         # Sets object as materialized
         # Information is loaded from the Device
         self.materialized = True
 
         device = Device(self.session)
         if not device.materialized:
-            device.get()
+            device.get(selector="status")
 
         # Clean BGP Router settings
         if "bgp" in device.capabilities and self.bgp_routers == []:
             # gotta use deferred import to avoid cyclical import error
             from pyaoscx.bgp_router import BgpRouter
 
             # Set BGP Routers if any
@@ -336,14 +336,48 @@
 
         # Get all objects data
         self.get()
 
         # Object was modified
         return True
 
+    def get_interfaces(self):
+        """
+        Get interfaces that belong to this VRF
+
+        :return: list of interface members of this VRF
+        """
+
+        list_interf = []
+        device = Device(self.session)
+        configuration = device.configuration()
+        running_config = configuration.get_full_config()
+        interfaces = running_config["Port"]
+        for interface in interfaces.values():
+            if "vrf" in interface:
+                # Get interfaces that belong to this another VRF
+                if interface["vrf"] == self.name:
+                    list_interf.append(
+                        self.session.api.get_module(
+                            self.session, "Interface", interface["name"]
+                        )
+                    )
+
+            # Get interfaces that belong at vrf "default"
+            elif (
+                "routing" not in interface or interface["routing"]
+            ) and self.name == "default":
+                list_interf.append(
+                    self.session.api.get_module(
+                        self.session, "Interface", interface["name"]
+                    )
+                )
+
+        return list_interf
+
     @PyaoscxModule.connected
     def delete(self):
         """
         Perform DELETE call to delete VRF table entry.
         """
         # Delete object attributes
         utils.delete_attrs(self, self.config_attrs)
```

### Comparing `pyaoscx-2.5.1/pyaoscx/vrf_address_family.py` & `pyaoscx-2.6.0/pyaoscx/vrf_address_family.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx/vsx.py` & `pyaoscx-2.6.0/pyaoscx/vsx.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.5.1/pyaoscx.egg-info/PKG-INFO` & `pyaoscx-2.6.0/pyaoscx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaoscx
-Version: 2.5.1
+Version: 2.6.0
 Summary: AOS-CX Python Modules
 Home-page: https://github.com/aruba/pyaoscx
 Author: Aruba Automation
 Author-email: aruba-automation@hpe.com
 License: Apache 2.0
 Keywords: networking aruba aos-cx switch rest api python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyaoscx-2.5.1/pyaoscx.egg-info/SOURCES.txt` & `pyaoscx-2.6.0/pyaoscx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pyaoscx/dhcp_relay.py
 pyaoscx/dns.py
 pyaoscx/firmware.py
 pyaoscx/interface.py
 pyaoscx/ipv6.py
 pyaoscx/lldp_neighbor.py
 pyaoscx/mac.py
+pyaoscx/object_group.py
 pyaoscx/ospf_area.py
 pyaoscx/ospf_interface.py
 pyaoscx/ospf_router.py
 pyaoscx/ospf_virtual_link.py
 pyaoscx/ospfv3_router.py
 pyaoscx/poe_interface.py
 pyaoscx/pyaoscx_factory.py
@@ -64,11 +65,12 @@
 pyaoscx/rest/v10_08/__init__.py
 pyaoscx/rest/v10_08/api.py
 pyaoscx/rest/v10_08/interface.py
 pyaoscx/rest/v10_09/__init__.py
 pyaoscx/rest/v10_09/api.py
 pyaoscx/rest/v10_09/interface.py
 pyaoscx/utils/__init__.py
+pyaoscx/utils/iptools.py
 pyaoscx/utils/list_attributes.py
 pyaoscx/utils/util.py
 workflows/__init__.py
 workflows/workflow.py
```

### Comparing `pyaoscx-2.5.1/setup.py` & `pyaoscx-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyaoscx",
-    version="2.5.1",
+    version="2.6.0",
     description="AOS-CX Python Modules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aruba/pyaoscx",
     author="Aruba Automation",
     author_email="aruba-automation@hpe.com",
     license="Apache 2.0",
```

### Comparing `pyaoscx-2.5.1/workflows/workflow.py` & `pyaoscx-2.6.0/workflows/workflow.py`

 * *Files identical despite different names*

