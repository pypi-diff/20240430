# Comparing `tmp/pulumi_proxmoxve-6.4.1.tar.gz` & `tmp/pulumi_proxmoxve-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.4.1.tar", last modified: Sun Apr 21 08:55:43 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.5.0.tar", last modified: Tue Apr 30 06:23:57 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.4.1.tar` & `pulumi_proxmoxve-6.5.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.318213 pulumi_proxmoxve-6.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-21 08:55:43.318213 pulumi_proxmoxve-6.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.306213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14356 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.306213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    50170 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/cluster/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.310213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.310213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64365 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.310213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/get_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.310213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/ha_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.310213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/get_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.310213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/get_pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/get_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.314213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.318213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.318213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.318213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87552 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    75694 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   124005 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-04-21 08:55:42.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:55:43.306213 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 08:55:43.318213 pulumi_proxmoxve-6.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 08:55:43.000000 pulumi_proxmoxve-6.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.829352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.829352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64365 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/get_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.833352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.837352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.837352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87552 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75694 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124005 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18043 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:57.829352 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:23:57.841352 pulumi_proxmoxve-6.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 06:23:57.000000 pulumi_proxmoxve-6.5.0/setup.py
```

### Comparing `pulumi_proxmoxve-6.4.1/PKG-INFO` & `pulumi_proxmoxve-6.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 6.4.1
+Version: 6.5.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.4.1/README.md` & `pulumi_proxmoxve-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'HostsEntryArgs',
     'ProviderSshArgs',
     'ProviderSshNodeArgs',
+    'Vm2CloneArgs',
     'Vm2TimeoutsArgs',
 ]
 
 @pulumi.input_type
 class HostsEntryArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
@@ -254,14 +255,52 @@
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
 
 @pulumi.input_type
+class Vm2CloneArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[int],
+                 retries: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[int] id: The ID of the VM to clone.
+        :param pulumi.Input[int] retries: The number of retries to perform when cloning the VM (default: 3).
+        """
+        pulumi.set(__self__, "id", id)
+        if retries is not None:
+            pulumi.set(__self__, "retries", retries)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[int]:
+        """
+        The ID of the VM to clone.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[int]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def retries(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of retries to perform when cloning the VM (default: 3).
+        """
+        return pulumi.get(self, "retries")
+
+    @retries.setter
+    def retries(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "retries", value)
+
+
+@pulumi.input_type
 class Vm2TimeoutsArgs:
     def __init__(__self__, *,
                  create: Optional[pulumi.Input[str]] = None,
                  delete: Optional[pulumi.Input[str]] = None,
                  read: Optional[pulumi.Input[str]] = None,
                  update: Optional[pulumi.Input[str]] = None):
         """
```

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/cluster/options.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['OptionsArgs', 'Options']
 
 @pulumi.input_type
 class OptionsArgs:
     def __init__(__self__, *,
                  bandwidth_limit_clone: Optional[pulumi.Input[int]] = None,
@@ -27,15 +29,17 @@
                  ha_shutdown_policy: Optional[pulumi.Input[str]] = None,
                  http_proxy: Optional[pulumi.Input[str]] = None,
                  keyboard: Optional[pulumi.Input[str]] = None,
                  language: Optional[pulumi.Input[str]] = None,
                  mac_prefix: Optional[pulumi.Input[str]] = None,
                  max_workers: Optional[pulumi.Input[int]] = None,
                  migration_cidr: Optional[pulumi.Input[str]] = None,
-                 migration_type: Optional[pulumi.Input[str]] = None):
+                 migration_type: Optional[pulumi.Input[str]] = None,
+                 next_id: Optional[pulumi.Input['OptionsNextIdArgs']] = None,
+                 notify: Optional[pulumi.Input['OptionsNotifyArgs']] = None):
         """
         The set of arguments for constructing a Options resource.
         :param pulumi.Input[int] bandwidth_limit_clone: Clone I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_default: Default I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_migration: Migration I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_move: Move I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_restore: Restore I/O bandwidth limit in KiB/s.
@@ -48,14 +52,16 @@
         :param pulumi.Input[str] http_proxy: Specify external http proxy which is used for downloads (example: `http://username:password@host:port/`).
         :param pulumi.Input[str] keyboard: Default keyboard layout for vnc server. Must be `de` | `de-ch` | `da` | `en-gb` | `en-us` | `es` | `fi` | `fr` | `fr-be` | `fr-ca` | `fr-ch` | `hu` | `is` | `it` | `ja` | `lt` | `mk` | `nl` | `no` | `pl` | `pt` | `pt-br` | `sv` | `sl` | `tr`.
         :param pulumi.Input[str] language: Default GUI language. Must be `ca` | `da` | `de` | `en` | `es` | `eu` | `fa` | `fr` | `he` | `it` | `ja` | `nb` | `nn` | `pl` | `pt_BR` | `ru` | `sl` | `sv` | `tr` | `zh_CN` | `zh_TW`.
         :param pulumi.Input[str] mac_prefix: Prefix for autogenerated MAC addresses.
         :param pulumi.Input[int] max_workers: Defines how many workers (per node) are maximal started on actions like 'stopall VMs' or task from the ha-manager.
         :param pulumi.Input[str] migration_cidr: Cluster wide migration network CIDR.
         :param pulumi.Input[str] migration_type: Cluster wide migration type. Must be `secure` | `unsecure` (default is `secure`).
+        :param pulumi.Input['OptionsNextIdArgs'] next_id: The ranges for the next free VM ID auto-selection pool.
+        :param pulumi.Input['OptionsNotifyArgs'] notify: Cluster-wide notification settings.
         """
         if bandwidth_limit_clone is not None:
             pulumi.set(__self__, "bandwidth_limit_clone", bandwidth_limit_clone)
         if bandwidth_limit_default is not None:
             pulumi.set(__self__, "bandwidth_limit_default", bandwidth_limit_default)
         if bandwidth_limit_migration is not None:
             pulumi.set(__self__, "bandwidth_limit_migration", bandwidth_limit_migration)
@@ -85,14 +91,18 @@
             pulumi.set(__self__, "mac_prefix", mac_prefix)
         if max_workers is not None:
             pulumi.set(__self__, "max_workers", max_workers)
         if migration_cidr is not None:
             pulumi.set(__self__, "migration_cidr", migration_cidr)
         if migration_type is not None:
             pulumi.set(__self__, "migration_type", migration_type)
+        if next_id is not None:
+            pulumi.set(__self__, "next_id", next_id)
+        if notify is not None:
+            pulumi.set(__self__, "notify", notify)
 
     @property
     @pulumi.getter(name="bandwidthLimitClone")
     def bandwidth_limit_clone(self) -> Optional[pulumi.Input[int]]:
         """
         Clone I/O bandwidth limit in KiB/s.
         """
@@ -302,14 +312,38 @@
         """
         return pulumi.get(self, "migration_type")
 
     @migration_type.setter
     def migration_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "migration_type", value)
 
+    @property
+    @pulumi.getter(name="nextId")
+    def next_id(self) -> Optional[pulumi.Input['OptionsNextIdArgs']]:
+        """
+        The ranges for the next free VM ID auto-selection pool.
+        """
+        return pulumi.get(self, "next_id")
+
+    @next_id.setter
+    def next_id(self, value: Optional[pulumi.Input['OptionsNextIdArgs']]):
+        pulumi.set(self, "next_id", value)
+
+    @property
+    @pulumi.getter
+    def notify(self) -> Optional[pulumi.Input['OptionsNotifyArgs']]:
+        """
+        Cluster-wide notification settings.
+        """
+        return pulumi.get(self, "notify")
+
+    @notify.setter
+    def notify(self, value: Optional[pulumi.Input['OptionsNotifyArgs']]):
+        pulumi.set(self, "notify", value)
+
 
 @pulumi.input_type
 class _OptionsState:
     def __init__(__self__, *,
                  bandwidth_limit_clone: Optional[pulumi.Input[int]] = None,
                  bandwidth_limit_default: Optional[pulumi.Input[int]] = None,
                  bandwidth_limit_migration: Optional[pulumi.Input[int]] = None,
@@ -323,15 +357,17 @@
                  ha_shutdown_policy: Optional[pulumi.Input[str]] = None,
                  http_proxy: Optional[pulumi.Input[str]] = None,
                  keyboard: Optional[pulumi.Input[str]] = None,
                  language: Optional[pulumi.Input[str]] = None,
                  mac_prefix: Optional[pulumi.Input[str]] = None,
                  max_workers: Optional[pulumi.Input[int]] = None,
                  migration_cidr: Optional[pulumi.Input[str]] = None,
-                 migration_type: Optional[pulumi.Input[str]] = None):
+                 migration_type: Optional[pulumi.Input[str]] = None,
+                 next_id: Optional[pulumi.Input['OptionsNextIdArgs']] = None,
+                 notify: Optional[pulumi.Input['OptionsNotifyArgs']] = None):
         """
         Input properties used for looking up and filtering Options resources.
         :param pulumi.Input[int] bandwidth_limit_clone: Clone I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_default: Default I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_migration: Migration I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_move: Move I/O bandwidth limit in KiB/s.
         :param pulumi.Input[int] bandwidth_limit_restore: Restore I/O bandwidth limit in KiB/s.
@@ -344,14 +380,16 @@
         :param pulumi.Input[str] http_proxy: Specify external http proxy which is used for downloads (example: `http://username:password@host:port/`).
         :param pulumi.Input[str] keyboard: Default keyboard layout for vnc server. Must be `de` | `de-ch` | `da` | `en-gb` | `en-us` | `es` | `fi` | `fr` | `fr-be` | `fr-ca` | `fr-ch` | `hu` | `is` | `it` | `ja` | `lt` | `mk` | `nl` | `no` | `pl` | `pt` | `pt-br` | `sv` | `sl` | `tr`.
         :param pulumi.Input[str] language: Default GUI language. Must be `ca` | `da` | `de` | `en` | `es` | `eu` | `fa` | `fr` | `he` | `it` | `ja` | `nb` | `nn` | `pl` | `pt_BR` | `ru` | `sl` | `sv` | `tr` | `zh_CN` | `zh_TW`.
         :param pulumi.Input[str] mac_prefix: Prefix for autogenerated MAC addresses.
         :param pulumi.Input[int] max_workers: Defines how many workers (per node) are maximal started on actions like 'stopall VMs' or task from the ha-manager.
         :param pulumi.Input[str] migration_cidr: Cluster wide migration network CIDR.
         :param pulumi.Input[str] migration_type: Cluster wide migration type. Must be `secure` | `unsecure` (default is `secure`).
+        :param pulumi.Input['OptionsNextIdArgs'] next_id: The ranges for the next free VM ID auto-selection pool.
+        :param pulumi.Input['OptionsNotifyArgs'] notify: Cluster-wide notification settings.
         """
         if bandwidth_limit_clone is not None:
             pulumi.set(__self__, "bandwidth_limit_clone", bandwidth_limit_clone)
         if bandwidth_limit_default is not None:
             pulumi.set(__self__, "bandwidth_limit_default", bandwidth_limit_default)
         if bandwidth_limit_migration is not None:
             pulumi.set(__self__, "bandwidth_limit_migration", bandwidth_limit_migration)
@@ -381,14 +419,18 @@
             pulumi.set(__self__, "mac_prefix", mac_prefix)
         if max_workers is not None:
             pulumi.set(__self__, "max_workers", max_workers)
         if migration_cidr is not None:
             pulumi.set(__self__, "migration_cidr", migration_cidr)
         if migration_type is not None:
             pulumi.set(__self__, "migration_type", migration_type)
+        if next_id is not None:
+            pulumi.set(__self__, "next_id", next_id)
+        if notify is not None:
+            pulumi.set(__self__, "notify", notify)
 
     @property
     @pulumi.getter(name="bandwidthLimitClone")
     def bandwidth_limit_clone(self) -> Optional[pulumi.Input[int]]:
         """
         Clone I/O bandwidth limit in KiB/s.
         """
@@ -598,14 +640,38 @@
         """
         return pulumi.get(self, "migration_type")
 
     @migration_type.setter
     def migration_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "migration_type", value)
 
+    @property
+    @pulumi.getter(name="nextId")
+    def next_id(self) -> Optional[pulumi.Input['OptionsNextIdArgs']]:
+        """
+        The ranges for the next free VM ID auto-selection pool.
+        """
+        return pulumi.get(self, "next_id")
+
+    @next_id.setter
+    def next_id(self, value: Optional[pulumi.Input['OptionsNextIdArgs']]):
+        pulumi.set(self, "next_id", value)
+
+    @property
+    @pulumi.getter
+    def notify(self) -> Optional[pulumi.Input['OptionsNotifyArgs']]:
+        """
+        Cluster-wide notification settings.
+        """
+        return pulumi.get(self, "notify")
+
+    @notify.setter
+    def notify(self, value: Optional[pulumi.Input['OptionsNotifyArgs']]):
+        pulumi.set(self, "notify", value)
+
 
 class Options(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  bandwidth_limit_clone: Optional[pulumi.Input[int]] = None,
@@ -622,37 +688,20 @@
                  http_proxy: Optional[pulumi.Input[str]] = None,
                  keyboard: Optional[pulumi.Input[str]] = None,
                  language: Optional[pulumi.Input[str]] = None,
                  mac_prefix: Optional[pulumi.Input[str]] = None,
                  max_workers: Optional[pulumi.Input[int]] = None,
                  migration_cidr: Optional[pulumi.Input[str]] = None,
                  migration_type: Optional[pulumi.Input[str]] = None,
+                 next_id: Optional[pulumi.Input[pulumi.InputType['OptionsNextIdArgs']]] = None,
+                 notify: Optional[pulumi.Input[pulumi.InputType['OptionsNotifyArgs']]] = None,
                  __props__=None):
         """
         Manages Proxmox VE Cluster Datacenter options.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_proxmoxve as proxmoxve
-
-        options = proxmoxve.cluster.Options("options",
-            bandwidth_limit_default=666666,
-            bandwidth_limit_migration=555555,
-            email_from="ged@gont.earthsea",
-            keyboard="pl",
-            language="en",
-            max_workers=5,
-            migration_cidr="10.0.0.0/8",
-            migration_type="secure")
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         #!/usr/bin/env sh
 
         Cluster options are global and can be imported using e.g.:
 
         ```sh
@@ -675,43 +724,26 @@
         :param pulumi.Input[str] http_proxy: Specify external http proxy which is used for downloads (example: `http://username:password@host:port/`).
         :param pulumi.Input[str] keyboard: Default keyboard layout for vnc server. Must be `de` | `de-ch` | `da` | `en-gb` | `en-us` | `es` | `fi` | `fr` | `fr-be` | `fr-ca` | `fr-ch` | `hu` | `is` | `it` | `ja` | `lt` | `mk` | `nl` | `no` | `pl` | `pt` | `pt-br` | `sv` | `sl` | `tr`.
         :param pulumi.Input[str] language: Default GUI language. Must be `ca` | `da` | `de` | `en` | `es` | `eu` | `fa` | `fr` | `he` | `it` | `ja` | `nb` | `nn` | `pl` | `pt_BR` | `ru` | `sl` | `sv` | `tr` | `zh_CN` | `zh_TW`.
         :param pulumi.Input[str] mac_prefix: Prefix for autogenerated MAC addresses.
         :param pulumi.Input[int] max_workers: Defines how many workers (per node) are maximal started on actions like 'stopall VMs' or task from the ha-manager.
         :param pulumi.Input[str] migration_cidr: Cluster wide migration network CIDR.
         :param pulumi.Input[str] migration_type: Cluster wide migration type. Must be `secure` | `unsecure` (default is `secure`).
+        :param pulumi.Input[pulumi.InputType['OptionsNextIdArgs']] next_id: The ranges for the next free VM ID auto-selection pool.
+        :param pulumi.Input[pulumi.InputType['OptionsNotifyArgs']] notify: Cluster-wide notification settings.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[OptionsArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages Proxmox VE Cluster Datacenter options.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_proxmoxve as proxmoxve
-
-        options = proxmoxve.cluster.Options("options",
-            bandwidth_limit_default=666666,
-            bandwidth_limit_migration=555555,
-            email_from="ged@gont.earthsea",
-            keyboard="pl",
-            language="en",
-            max_workers=5,
-            migration_cidr="10.0.0.0/8",
-            migration_type="secure")
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         #!/usr/bin/env sh
 
         Cluster options are global and can be imported using e.g.:
 
         ```sh
@@ -747,14 +779,16 @@
                  http_proxy: Optional[pulumi.Input[str]] = None,
                  keyboard: Optional[pulumi.Input[str]] = None,
                  language: Optional[pulumi.Input[str]] = None,
                  mac_prefix: Optional[pulumi.Input[str]] = None,
                  max_workers: Optional[pulumi.Input[int]] = None,
                  migration_cidr: Optional[pulumi.Input[str]] = None,
                  migration_type: Optional[pulumi.Input[str]] = None,
+                 next_id: Optional[pulumi.Input[pulumi.InputType['OptionsNextIdArgs']]] = None,
+                 notify: Optional[pulumi.Input[pulumi.InputType['OptionsNotifyArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -774,14 +808,16 @@
             __props__.__dict__["http_proxy"] = http_proxy
             __props__.__dict__["keyboard"] = keyboard
             __props__.__dict__["language"] = language
             __props__.__dict__["mac_prefix"] = mac_prefix
             __props__.__dict__["max_workers"] = max_workers
             __props__.__dict__["migration_cidr"] = migration_cidr
             __props__.__dict__["migration_type"] = migration_type
+            __props__.__dict__["next_id"] = next_id
+            __props__.__dict__["notify"] = notify
         super(Options, __self__).__init__(
             'proxmoxve:Cluster/options:Options',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -801,15 +837,17 @@
             ha_shutdown_policy: Optional[pulumi.Input[str]] = None,
             http_proxy: Optional[pulumi.Input[str]] = None,
             keyboard: Optional[pulumi.Input[str]] = None,
             language: Optional[pulumi.Input[str]] = None,
             mac_prefix: Optional[pulumi.Input[str]] = None,
             max_workers: Optional[pulumi.Input[int]] = None,
             migration_cidr: Optional[pulumi.Input[str]] = None,
-            migration_type: Optional[pulumi.Input[str]] = None) -> 'Options':
+            migration_type: Optional[pulumi.Input[str]] = None,
+            next_id: Optional[pulumi.Input[pulumi.InputType['OptionsNextIdArgs']]] = None,
+            notify: Optional[pulumi.Input[pulumi.InputType['OptionsNotifyArgs']]] = None) -> 'Options':
         """
         Get an existing Options resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -827,14 +865,16 @@
         :param pulumi.Input[str] http_proxy: Specify external http proxy which is used for downloads (example: `http://username:password@host:port/`).
         :param pulumi.Input[str] keyboard: Default keyboard layout for vnc server. Must be `de` | `de-ch` | `da` | `en-gb` | `en-us` | `es` | `fi` | `fr` | `fr-be` | `fr-ca` | `fr-ch` | `hu` | `is` | `it` | `ja` | `lt` | `mk` | `nl` | `no` | `pl` | `pt` | `pt-br` | `sv` | `sl` | `tr`.
         :param pulumi.Input[str] language: Default GUI language. Must be `ca` | `da` | `de` | `en` | `es` | `eu` | `fa` | `fr` | `he` | `it` | `ja` | `nb` | `nn` | `pl` | `pt_BR` | `ru` | `sl` | `sv` | `tr` | `zh_CN` | `zh_TW`.
         :param pulumi.Input[str] mac_prefix: Prefix for autogenerated MAC addresses.
         :param pulumi.Input[int] max_workers: Defines how many workers (per node) are maximal started on actions like 'stopall VMs' or task from the ha-manager.
         :param pulumi.Input[str] migration_cidr: Cluster wide migration network CIDR.
         :param pulumi.Input[str] migration_type: Cluster wide migration type. Must be `secure` | `unsecure` (default is `secure`).
+        :param pulumi.Input[pulumi.InputType['OptionsNextIdArgs']] next_id: The ranges for the next free VM ID auto-selection pool.
+        :param pulumi.Input[pulumi.InputType['OptionsNotifyArgs']] notify: Cluster-wide notification settings.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _OptionsState.__new__(_OptionsState)
 
         __props__.__dict__["bandwidth_limit_clone"] = bandwidth_limit_clone
         __props__.__dict__["bandwidth_limit_default"] = bandwidth_limit_default
@@ -850,14 +890,16 @@
         __props__.__dict__["http_proxy"] = http_proxy
         __props__.__dict__["keyboard"] = keyboard
         __props__.__dict__["language"] = language
         __props__.__dict__["mac_prefix"] = mac_prefix
         __props__.__dict__["max_workers"] = max_workers
         __props__.__dict__["migration_cidr"] = migration_cidr
         __props__.__dict__["migration_type"] = migration_type
+        __props__.__dict__["next_id"] = next_id
+        __props__.__dict__["notify"] = notify
         return Options(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="bandwidthLimitClone")
     def bandwidth_limit_clone(self) -> pulumi.Output[Optional[int]]:
         """
         Clone I/O bandwidth limit in KiB/s.
@@ -996,7 +1038,23 @@
     @pulumi.getter(name="migrationType")
     def migration_type(self) -> pulumi.Output[Optional[str]]:
         """
         Cluster wide migration type. Must be `secure` | `unsecure` (default is `secure`).
         """
         return pulumi.get(self, "migration_type")
 
+    @property
+    @pulumi.getter(name="nextId")
+    def next_id(self) -> pulumi.Output[Optional['outputs.OptionsNextId']]:
+        """
+        The ranges for the next free VM ID auto-selection pool.
+        """
+        return pulumi.get(self, "next_id")
+
+    @property
+    @pulumi.getter
+    def notify(self) -> pulumi.Output[Optional['outputs.OptionsNotify']]:
+        """
+        Cluster-wide notification settings.
+        """
+        return pulumi.get(self, "notify")
+
```

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/__init__.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/get_mappings.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/get_pci.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/get_usb.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/get_usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/pci.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/mapping/usb.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/mapping/usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hardware/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hardware/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/outputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'HostsEntry',
+    'Vm2Clone',
     'Vm2Timeouts',
 ]
 
 @pulumi.output_type
 class HostsEntry(dict):
     def __init__(__self__, *,
                  address: str,
@@ -40,14 +41,44 @@
         """
         The hostnames.
         """
         return pulumi.get(self, "hostnames")
 
 
 @pulumi.output_type
+class Vm2Clone(dict):
+    def __init__(__self__, *,
+                 id: int,
+                 retries: Optional[int] = None):
+        """
+        :param int id: The ID of the VM to clone.
+        :param int retries: The number of retries to perform when cloning the VM (default: 3).
+        """
+        pulumi.set(__self__, "id", id)
+        if retries is not None:
+            pulumi.set(__self__, "retries", retries)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        """
+        The ID of the VM to clone.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def retries(self) -> Optional[int]:
+        """
+        The number of retries to perform when cloning the VM (default: 3).
+        """
+        return pulumi.get(self, "retries")
+
+
+@pulumi.output_type
 class Vm2Timeouts(dict):
     def __init__(__self__, *,
                  create: Optional[str] = None,
                  delete: Optional[str] = None,
                  read: Optional[str] = None,
                  update: Optional[str] = None):
         """
```

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve/vm2.py` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve/vm2.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,40 @@
 
 __all__ = ['Vm2Args', 'Vm2']
 
 @pulumi.input_type
 class Vm2Args:
     def __init__(__self__, *,
                  node_name: pulumi.Input[str],
+                 clone: Optional[pulumi.Input['Vm2CloneArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None):
         """
         The set of arguments for constructing a Vm2 resource.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input['Vm2CloneArgs'] clone: The cloning configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the resource.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
         """
         pulumi.set(__self__, "node_name", node_name)
+        if clone is not None:
+            pulumi.set(__self__, "clone", clone)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if template is not None:
+            pulumi.set(__self__, "template", template)
         if timeouts is not None:
             pulumi.set(__self__, "timeouts", timeouts)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> pulumi.Input[str]:
         """
@@ -44,14 +56,26 @@
 
     @node_name.setter
     def node_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "node_name", value)
 
     @property
     @pulumi.getter
+    def clone(self) -> Optional[pulumi.Input['Vm2CloneArgs']]:
+        """
+        The cloning configuration.
+        """
+        return pulumi.get(self, "clone")
+
+    @clone.setter
+    def clone(self, value: Optional[pulumi.Input['Vm2CloneArgs']]):
+        pulumi.set(self, "clone", value)
+
+    @property
+    @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         The description of the VM.
         """
         return pulumi.get(self, "description")
 
     @description.setter
@@ -68,46 +92,94 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The tags assigned to the resource.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+    @property
+    @pulumi.getter
+    def template(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Set to true to create a VM template.
+        """
+        return pulumi.get(self, "template")
+
+    @template.setter
+    def template(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "template", value)
+
+    @property
+    @pulumi.getter
     def timeouts(self) -> Optional[pulumi.Input['Vm2TimeoutsArgs']]:
         return pulumi.get(self, "timeouts")
 
     @timeouts.setter
     def timeouts(self, value: Optional[pulumi.Input['Vm2TimeoutsArgs']]):
         pulumi.set(self, "timeouts", value)
 
 
 @pulumi.input_type
 class _Vm2State:
     def __init__(__self__, *,
+                 clone: Optional[pulumi.Input['Vm2CloneArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None):
         """
         Input properties used for looking up and filtering Vm2 resources.
+        :param pulumi.Input['Vm2CloneArgs'] clone: The cloning configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the resource.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
         """
+        if clone is not None:
+            pulumi.set(__self__, "clone", clone)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if template is not None:
+            pulumi.set(__self__, "template", template)
         if timeouts is not None:
             pulumi.set(__self__, "timeouts", timeouts)
 
     @property
     @pulumi.getter
+    def clone(self) -> Optional[pulumi.Input['Vm2CloneArgs']]:
+        """
+        The cloning configuration.
+        """
+        return pulumi.get(self, "clone")
+
+    @clone.setter
+    def clone(self, value: Optional[pulumi.Input['Vm2CloneArgs']]):
+        pulumi.set(self, "clone", value)
+
+    @property
+    @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         The description of the VM.
         """
         return pulumi.get(self, "description")
 
     @description.setter
@@ -136,52 +208,100 @@
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
     @property
     @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The tags assigned to the resource.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+    @property
+    @pulumi.getter
+    def template(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Set to true to create a VM template.
+        """
+        return pulumi.get(self, "template")
+
+    @template.setter
+    def template(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "template", value)
+
+    @property
+    @pulumi.getter
     def timeouts(self) -> Optional[pulumi.Input['Vm2TimeoutsArgs']]:
         return pulumi.get(self, "timeouts")
 
     @timeouts.setter
     def timeouts(self, value: Optional[pulumi.Input['Vm2TimeoutsArgs']]):
         pulumi.set(self, "timeouts", value)
 
 
 class Vm2(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
                  __props__=None):
         """
-        > **DO NOT USE**
+        !> **DO NOT USE**
         This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
+        > Note: Many attributes are marked as **optional** _and_ **computed** in the schema,
+        hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
+        This is done to support the `clone` operation, when a VM is created from an existing one,
+        and attributes of the original VM are copied to the new one.
+
+        Computed attributes allow the provider to set those attributes without user input.
+        The attributes are marked as optional to allow the user to set (or overwrite) them if needed.
+        In order to remove the computed attribute from the plan, you can set it to an empty value (e.g. `""` for string, `[]` for collection).
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the resource.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Vm2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        > **DO NOT USE**
+        !> **DO NOT USE**
         This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
+        > Note: Many attributes are marked as **optional** _and_ **computed** in the schema,
+        hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
+        This is done to support the `clone` operation, when a VM is created from an existing one,
+        and attributes of the original VM are copied to the new one.
+
+        Computed attributes allow the provider to set those attributes without user input.
+        The attributes are marked as optional to allow the user to set (or overwrite) them if needed.
+        In order to remove the computed attribute from the plan, you can set it to an empty value (e.g. `""` for string, `[]` for collection).
+
         :param str resource_name: The name of the resource.
         :param Vm2Args args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(Vm2Args, pulumi.ResourceOptions, *args, **kwargs)
@@ -189,70 +309,93 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = Vm2Args.__new__(Vm2Args)
 
+            __props__.__dict__["clone"] = clone
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
             if node_name is None and not opts.urn:
                 raise TypeError("Missing required property 'node_name'")
             __props__.__dict__["node_name"] = node_name
+            __props__.__dict__["tags"] = tags
+            __props__.__dict__["template"] = template
             __props__.__dict__["timeouts"] = timeouts
         super(Vm2, __self__).__init__(
             'proxmoxve:index/vm2:Vm2',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
             description: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             node_name: Optional[pulumi.Input[str]] = None,
+            tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            template: Optional[pulumi.Input[bool]] = None,
             timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None) -> 'Vm2':
         """
         Get an existing Vm2 resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the resource.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _Vm2State.__new__(_Vm2State)
 
+        __props__.__dict__["clone"] = clone
         __props__.__dict__["description"] = description
         __props__.__dict__["name"] = name
         __props__.__dict__["node_name"] = node_name
+        __props__.__dict__["tags"] = tags
+        __props__.__dict__["template"] = template
         __props__.__dict__["timeouts"] = timeouts
         return Vm2(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
+    def clone(self) -> pulumi.Output[Optional['outputs.Vm2Clone']]:
+        """
+        The cloning configuration.
+        """
+        return pulumi.get(self, "clone")
+
+    @property
+    @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         The description of the VM.
         """
         return pulumi.get(self, "description")
 
     @property
@@ -269,10 +412,26 @@
         """
         The name of the node where the VM is provisioned.
         """
         return pulumi.get(self, "node_name")
 
     @property
     @pulumi.getter
+    def tags(self) -> pulumi.Output[Sequence[str]]:
+        """
+        The tags assigned to the resource.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def template(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Set to true to create a VM template.
+        """
+        return pulumi.get(self, "template")
+
+    @property
+    @pulumi.getter
     def timeouts(self) -> pulumi.Output[Optional['outputs.Vm2Timeouts']]:
         return pulumi.get(self, "timeouts")
```

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 6.4.1
+Version: 6.5.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.4.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.5.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 pulumi_proxmoxve.egg-info/PKG-INFO
 pulumi_proxmoxve.egg-info/SOURCES.txt
 pulumi_proxmoxve.egg-info/dependency_links.txt
 pulumi_proxmoxve.egg-info/not-zip-safe
 pulumi_proxmoxve.egg-info/requires.txt
 pulumi_proxmoxve.egg-info/top_level.txt
 pulumi_proxmoxve/cluster/__init__.py
+pulumi_proxmoxve/cluster/_inputs.py
 pulumi_proxmoxve/cluster/get_nodes.py
 pulumi_proxmoxve/cluster/options.py
+pulumi_proxmoxve/cluster/outputs.py
 pulumi_proxmoxve/config/__init__.py
 pulumi_proxmoxve/config/outputs.py
 pulumi_proxmoxve/config/vars.py
 pulumi_proxmoxve/ct/__init__.py
 pulumi_proxmoxve/ct/_inputs.py
 pulumi_proxmoxve/ct/container.py
 pulumi_proxmoxve/ct/outputs.py
```

### Comparing `pulumi_proxmoxve-6.4.1/setup.py` & `pulumi_proxmoxve-6.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.4.1"
+VERSION = "6.5.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

