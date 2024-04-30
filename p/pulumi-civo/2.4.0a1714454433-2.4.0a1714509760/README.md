# Comparing `tmp/pulumi_civo-2.4.0a1714454433.tar.gz` & `tmp/pulumi_civo-2.4.0a1714509760.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1714454433.tar", last modified: Tue Apr 30 05:23:23 2024, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1714509760.tar", last modified: Tue Apr 30 20:46:35 2024, max compression
```

## Comparing `pulumi_civo-2.4.0a1714454433.tar` & `pulumi_civo-2.4.0a1714509760.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:23:23.778268 pulumi_civo-2.4.0a1714454433/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 05:23:23.778268 pulumi_civo-2.4.0a1714454433/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:23:23.774268 pulumi_civo-2.4.0a1714454433/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:23:23.778268 pulumi_civo-2.4.0a1714454433/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_database_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:23:23.778268 pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 05:23:23.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 05:23:23.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:23:23.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 05:23:23.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 05:23:23.000000 pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 05:23:16.000000 pulumi_civo-2.4.0a1714454433/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:23:23.778268 pulumi_civo-2.4.0a1714454433/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:46:35.871044 pulumi_civo-2.4.0a1714509760/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 20:46:35.871044 pulumi_civo-2.4.0a1714509760/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:46:35.867043 pulumi_civo-2.4.0a1714509760/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43299 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:46:35.867043 pulumi_civo-2.4.0a1714509760/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49735 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58435 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:46:35.867043 pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 20:46:35.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-30 20:46:35.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:46:35.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 20:46:35.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 20:46:35.000000 pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 20:46:29.000000 pulumi_civo-2.4.0a1714509760/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:46:35.871044 pulumi_civo-2.4.0a1714509760/setup.cfg
```

### Comparing `pulumi_civo-2.4.0a1714454433/PKG-INFO` & `pulumi_civo-2.4.0a1714509760/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1714454433
+Version: 2.4.0a1714509760
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1714454433/README.md` & `pulumi_civo-2.4.0a1714509760/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .database import *
 from .dns_domain_name import *
 from .dns_domain_record import *
 from .firewall import *
-from .firewall_rule import *
 from .get_database import *
 from .get_database_version import *
 from .get_disk_image import *
 from .get_dns_domain_name import *
 from .get_dns_domain_record import *
 from .get_firewall import *
 from .get_instance import *
@@ -84,22 +83,14 @@
   "fqn": "pulumi_civo",
   "classes": {
    "civo:index/firewall:Firewall": "Firewall"
   }
  },
  {
   "pkg": "civo",
-  "mod": "index/firewallRule",
-  "fqn": "pulumi_civo",
-  "classes": {
-   "civo:index/firewallRule:FirewallRule": "FirewallRule"
-  }
- },
- {
-  "pkg": "civo",
   "mod": "index/instance",
   "fqn": "pulumi_civo",
   "classes": {
    "civo:index/instance:Instance": "Instance"
   }
  },
  {
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from . import _utilities
 
 __all__ = [
     'FirewallEgressRuleArgs',
     'FirewallIngressRuleArgs',
     'KubernetesClusterInstalledApplicationArgs',
     'KubernetesClusterPoolsArgs',
+    'KubernetesClusterPoolsTaintArgs',
     'KubernetesNodePoolTaintArgs',
     'GetDatabaseVersionFilterArgs',
     'GetDatabaseVersionSortArgs',
     'GetDiskImageFilterArgs',
     'GetDiskImageSortArgs',
     'GetInstancesFilterArgs',
     'GetInstancesSortArgs',
@@ -297,30 +298,36 @@
 @pulumi.input_type
 class KubernetesClusterPoolsArgs:
     def __init__(__self__, *,
                  node_count: pulumi.Input[int],
                  size: pulumi.Input[str],
                  instance_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  label: Optional[pulumi.Input[str]] = None,
-                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None):
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
+                 taints: Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesClusterPoolsTaintArgs']]]] = None):
         """
         :param pulumi.Input[int] node_count: Number of nodes in the nodepool
         :param pulumi.Input[str] size: Size of the nodes in the nodepool
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_names: Instance names in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
         :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
         """
         pulumi.set(__self__, "node_count", node_count)
         pulumi.set(__self__, "size", size)
         if instance_names is not None:
             pulumi.set(__self__, "instance_names", instance_names)
         if label is not None:
             pulumi.set(__self__, "label", label)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
         if public_ip_node_pool is not None:
             pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> pulumi.Input[int]:
         """
         Number of nodes in the nodepool
         """
@@ -363,25 +370,81 @@
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "label", value)
 
     @property
+    @pulumi.getter
+    def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "labels")
+
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "labels", value)
+
+    @property
     @pulumi.getter(name="publicIpNodePool")
     def public_ip_node_pool(self) -> Optional[pulumi.Input[bool]]:
         """
         Node pool belongs to the public ip node pool
         """
         return pulumi.get(self, "public_ip_node_pool")
 
     @public_ip_node_pool.setter
     def public_ip_node_pool(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "public_ip_node_pool", value)
 
+    @property
+    @pulumi.getter
+    def taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesClusterPoolsTaintArgs']]]]:
+        return pulumi.get(self, "taints")
+
+    @taints.setter
+    def taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesClusterPoolsTaintArgs']]]]):
+        pulumi.set(self, "taints", value)
+
+
+@pulumi.input_type
+class KubernetesClusterPoolsTaintArgs:
+    def __init__(__self__, *,
+                 effect: pulumi.Input[str],
+                 key: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        pulumi.set(__self__, "effect", effect)
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "effect")
+
+    @effect.setter
+    def effect(self, value: pulumi.Input[str]):
+        pulumi.set(self, "effect", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
 
 @pulumi.input_type
 class KubernetesNodePoolTaintArgs:
     def __init__(__self__, *,
                  effect: pulumi.Input[str],
                  key: pulumi.Input[str],
                  value: pulumi.Input[str]):
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/config/__init__.pyi` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_database_version.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_database_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,24 +99,14 @@
     """
     Retrieve information about a network for use in other resources.
 
     This data source provides all of the network's properties as configured on your Civo account.
 
     Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for a specific network inside that region.
 
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_civo as civo
-
-    test = civo.get_network(label="test-network",
-        region="LON1")
-    ```
-
 
     :param str id: The ID of this resource.
     :param str label: The label of an existing network
     :param str region: The region of an existing network
     """
     __args__ = dict()
     __args__['id'] = id
@@ -141,23 +131,13 @@
     """
     Retrieve information about a network for use in other resources.
 
     This data source provides all of the network's properties as configured on your Civo account.
 
     Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for a specific network inside that region.
 
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_civo as civo
-
-    test = civo.get_network(label="test-network",
-        region="LON1")
-    ```
-
 
     :param str id: The ID of this resource.
     :param str label: The label of an existing network
     :param str region: The region of an existing network
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[str]] = None):
         """
@@ -34,14 +35,15 @@
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] hostname: A fully qualified domain name that should be set as the instance's hostname
         :param pulumi.Input[str] initial_user: The name of the initial user created on the server (optional; this will default to the template's default_username and fallback to civo)
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
+        :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
         :param pulumi.Input[str] size: The name of the size, from the current list, e.g. g3.xsmall
         :param pulumi.Input[str] sshkey_id: The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: An optional list of tags, represented as a key, value pair
         :param pulumi.Input[str] template: The ID for the template to use to build the instance
         """
@@ -57,14 +59,16 @@
             pulumi.set(__self__, "network_id", network_id)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
         if public_ip_required is not None:
             pulumi.set(__self__, "public_ip_required", public_ip_required)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if reserved_ipv4 is not None:
+            pulumi.set(__self__, "reserved_ipv4", reserved_ipv4)
         if reverse_dns is not None:
             pulumi.set(__self__, "reverse_dns", reverse_dns)
         if script is not None:
             pulumi.set(__self__, "script", script)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if sshkey_id is not None:
@@ -170,14 +174,26 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="reservedIpv4")
+    def reserved_ipv4(self) -> Optional[pulumi.Input[str]]:
+        """
+        Can be either the UUID, name, or the IP address of the reserved IP
+        """
+        return pulumi.get(self, "reserved_ipv4")
+
+    @reserved_ipv4.setter
+    def reserved_ipv4(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "reserved_ipv4", value)
+
+    @property
     @pulumi.getter(name="reverseDns")
     def reverse_dns(self) -> Optional[pulumi.Input[str]]:
         """
         A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         """
         return pulumi.get(self, "reverse_dns")
 
@@ -263,14 +279,15 @@
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  private_ip: Optional[pulumi.Input[str]] = None,
                  public_ip: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  ram_mb: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  source_id: Optional[pulumi.Input[str]] = None,
                  source_type: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
@@ -289,14 +306,15 @@
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
         :param pulumi.Input[str] private_ip: Instance's private IP address
         :param pulumi.Input[str] public_ip: Instance's public IP address
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[int] ram_mb: Instance's RAM (MB)
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
+        :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
         :param pulumi.Input[str] size: The name of the size, from the current list, e.g. g3.xsmall
         :param pulumi.Input[str] source_id: Instance's source ID
         :param pulumi.Input[str] source_type: Instance's source type
         :param pulumi.Input[str] sshkey_id: The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
         :param pulumi.Input[str] status: Instance's status
@@ -329,14 +347,16 @@
             pulumi.set(__self__, "public_ip", public_ip)
         if public_ip_required is not None:
             pulumi.set(__self__, "public_ip_required", public_ip_required)
         if ram_mb is not None:
             pulumi.set(__self__, "ram_mb", ram_mb)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if reserved_ipv4 is not None:
+            pulumi.set(__self__, "reserved_ipv4", reserved_ipv4)
         if reverse_dns is not None:
             pulumi.set(__self__, "reverse_dns", reverse_dns)
         if script is not None:
             pulumi.set(__self__, "script", script)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if source_id is not None:
@@ -532,14 +552,26 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="reservedIpv4")
+    def reserved_ipv4(self) -> Optional[pulumi.Input[str]]:
+        """
+        Can be either the UUID, name, or the IP address of the reserved IP
+        """
+        return pulumi.get(self, "reserved_ipv4")
+
+    @reserved_ipv4.setter
+    def reserved_ipv4(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "reserved_ipv4", value)
+
+    @property
     @pulumi.getter(name="reverseDns")
     def reverse_dns(self) -> Optional[pulumi.Input[str]]:
         """
         A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         """
         return pulumi.get(self, "reverse_dns")
 
@@ -656,14 +688,15 @@
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -684,14 +717,15 @@
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] hostname: A fully qualified domain name that should be set as the instance's hostname
         :param pulumi.Input[str] initial_user: The name of the initial user created on the server (optional; this will default to the template's default_username and fallback to civo)
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
+        :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
         :param pulumi.Input[str] size: The name of the size, from the current list, e.g. g3.xsmall
         :param pulumi.Input[str] sshkey_id: The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: An optional list of tags, represented as a key, value pair
         :param pulumi.Input[str] template: The ID for the template to use to build the instance
         """
@@ -731,14 +765,15 @@
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -754,14 +789,15 @@
             __props__.__dict__["firewall_id"] = firewall_id
             __props__.__dict__["hostname"] = hostname
             __props__.__dict__["initial_user"] = initial_user
             __props__.__dict__["network_id"] = network_id
             __props__.__dict__["notes"] = notes
             __props__.__dict__["public_ip_required"] = public_ip_required
             __props__.__dict__["region"] = region
+            __props__.__dict__["reserved_ipv4"] = reserved_ipv4
             __props__.__dict__["reverse_dns"] = reverse_dns
             __props__.__dict__["script"] = script
             __props__.__dict__["size"] = size
             __props__.__dict__["sshkey_id"] = sshkey_id
             __props__.__dict__["tags"] = tags
             __props__.__dict__["template"] = template
             __props__.__dict__["cpu_cores"] = None
@@ -797,14 +833,15 @@
             network_id: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             private_ip: Optional[pulumi.Input[str]] = None,
             public_ip: Optional[pulumi.Input[str]] = None,
             public_ip_required: Optional[pulumi.Input[str]] = None,
             ram_mb: Optional[pulumi.Input[int]] = None,
             region: Optional[pulumi.Input[str]] = None,
+            reserved_ipv4: Optional[pulumi.Input[str]] = None,
             reverse_dns: Optional[pulumi.Input[str]] = None,
             script: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
             source_id: Optional[pulumi.Input[str]] = None,
             source_type: Optional[pulumi.Input[str]] = None,
             sshkey_id: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
@@ -828,14 +865,15 @@
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
         :param pulumi.Input[str] private_ip: Instance's private IP address
         :param pulumi.Input[str] public_ip: Instance's public IP address
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[int] ram_mb: Instance's RAM (MB)
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
+        :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
         :param pulumi.Input[str] size: The name of the size, from the current list, e.g. g3.xsmall
         :param pulumi.Input[str] source_id: Instance's source ID
         :param pulumi.Input[str] source_type: Instance's source type
         :param pulumi.Input[str] sshkey_id: The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
         :param pulumi.Input[str] status: Instance's status
@@ -857,14 +895,15 @@
         __props__.__dict__["network_id"] = network_id
         __props__.__dict__["notes"] = notes
         __props__.__dict__["private_ip"] = private_ip
         __props__.__dict__["public_ip"] = public_ip
         __props__.__dict__["public_ip_required"] = public_ip_required
         __props__.__dict__["ram_mb"] = ram_mb
         __props__.__dict__["region"] = region
+        __props__.__dict__["reserved_ipv4"] = reserved_ipv4
         __props__.__dict__["reverse_dns"] = reverse_dns
         __props__.__dict__["script"] = script
         __props__.__dict__["size"] = size
         __props__.__dict__["source_id"] = source_id
         __props__.__dict__["source_type"] = source_type
         __props__.__dict__["sshkey_id"] = sshkey_id
         __props__.__dict__["status"] = status
@@ -989,14 +1028,22 @@
     def region(self) -> pulumi.Output[Optional[str]]:
         """
         The region for the instance, if not declare we use the region in declared in the provider
         """
         return pulumi.get(self, "region")
 
     @property
+    @pulumi.getter(name="reservedIpv4")
+    def reserved_ipv4(self) -> pulumi.Output[Optional[str]]:
+        """
+        Can be either the UUID, name, or the IP address of the reserved IP
+        """
+        return pulumi.get(self, "reserved_ipv4")
+
+    @property
     @pulumi.getter(name="reverseDns")
     def reverse_dns(self) -> pulumi.Output[Optional[str]]:
         """
         A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         """
         return pulumi.get(self, "reverse_dns")
 
@@ -1030,15 +1077,15 @@
         """
         Instance's source type
         """
         return pulumi.get(self, "source_type")
 
     @property
     @pulumi.getter(name="sshkeyId")
-    def sshkey_id(self) -> pulumi.Output[Optional[str]]:
+    def sshkey_id(self) -> pulumi.Output[str]:
         """
         The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
         """
         return pulumi.get(self, "sshkey_id")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/kubernetes_node_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,42 +13,37 @@
 
 __all__ = ['KubernetesNodePoolArgs', 'KubernetesNodePool']
 
 @pulumi.input_type
 class KubernetesNodePoolArgs:
     def __init__(__self__, *,
                  cluster_id: pulumi.Input[str],
-                 region: pulumi.Input[str],
+                 node_count: pulumi.Input[int],
+                 size: pulumi.Input[str],
                  label: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 node_count: Optional[pulumi.Input[int]] = None,
                  public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
-                 size: Optional[pulumi.Input[str]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesNodePoolTaintArgs']]]] = None):
         """
         The set of arguments for constructing a KubernetesNodePool resource.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
-        :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
+        :param pulumi.Input[int] node_count: Number of nodes in the nodepool
+        :param pulumi.Input[str] size: Size of the nodes in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
-        :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
         :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
-        :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
-        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "node_count", node_count)
+        pulumi.set(__self__, "size", size)
         if label is not None:
             pulumi.set(__self__, "label", label)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
-        if node_count is not None:
-            pulumi.set(__self__, "node_count", node_count)
         if public_ip_node_pool is not None:
             pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
-        if size is not None:
-            pulumi.set(__self__, "size", size)
         if taints is not None:
             pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> pulumi.Input[str]:
         """
@@ -57,24 +52,36 @@
         return pulumi.get(self, "cluster_id")
 
     @cluster_id.setter
     def cluster_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "cluster_id", value)
 
     @property
+    @pulumi.getter(name="nodeCount")
+    def node_count(self) -> pulumi.Input[int]:
+        """
+        Number of nodes in the nodepool
+        """
+        return pulumi.get(self, "node_count")
+
+    @node_count.setter
+    def node_count(self, value: pulumi.Input[int]):
+        pulumi.set(self, "node_count", value)
+
+    @property
     @pulumi.getter
-    def region(self) -> pulumi.Input[str]:
+    def size(self) -> pulumi.Input[str]:
         """
-        The region of the node pool, has to match that of the cluster
+        Size of the nodes in the nodepool
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "size")
 
-    @region.setter
-    def region(self, value: pulumi.Input[str]):
-        pulumi.set(self, "region", value)
+    @size.setter
+    def size(self, value: pulumi.Input[str]):
+        pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
     def label(self) -> Optional[pulumi.Input[str]]:
         """
         Node pool label, if you don't provide one, we will generate one for you
         """
@@ -90,51 +97,27 @@
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
-    @pulumi.getter(name="nodeCount")
-    def node_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        the number of instances to create (optional, the default at the time of writing is 3)
-        """
-        return pulumi.get(self, "node_count")
-
-    @node_count.setter
-    def node_count(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "node_count", value)
-
-    @property
     @pulumi.getter(name="publicIpNodePool")
     def public_ip_node_pool(self) -> Optional[pulumi.Input[bool]]:
         """
         Node pool belongs to the public ip node pool
         """
         return pulumi.get(self, "public_ip_node_pool")
 
     @public_ip_node_pool.setter
     def public_ip_node_pool(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "public_ip_node_pool", value)
 
     @property
     @pulumi.getter
-    def size(self) -> Optional[pulumi.Input[str]]:
-        """
-        the size of each node (optional, the default is currently g4s.kube.medium)
-        """
-        return pulumi.get(self, "size")
-
-    @size.setter
-    def size(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "size", value)
-
-    @property
-    @pulumi.getter
     def taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesNodePoolTaintArgs']]]]:
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesNodePoolTaintArgs']]]]):
         pulumi.set(self, "taints", value)
 
@@ -144,41 +127,37 @@
     def __init__(__self__, *,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  instance_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input['KubernetesNodePoolTaintArgs']]]] = None):
         """
         Input properties used for looking up and filtering KubernetesNodePool resources.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_names: Instance names in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
-        :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[int] node_count: Number of nodes in the nodepool
         :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
-        :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
-        :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
+        :param pulumi.Input[str] size: Size of the nodes in the nodepool
         """
         if cluster_id is not None:
             pulumi.set(__self__, "cluster_id", cluster_id)
         if instance_names is not None:
             pulumi.set(__self__, "instance_names", instance_names)
         if label is not None:
             pulumi.set(__self__, "label", label)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if node_count is not None:
             pulumi.set(__self__, "node_count", node_count)
         if public_ip_node_pool is not None:
             pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if taints is not None:
             pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter(name="clusterId")
@@ -225,15 +204,15 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> Optional[pulumi.Input[int]]:
         """
-        the number of instances to create (optional, the default at the time of writing is 3)
+        Number of nodes in the nodepool
         """
         return pulumi.get(self, "node_count")
 
     @node_count.setter
     def node_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "node_count", value)
 
@@ -247,29 +226,17 @@
 
     @public_ip_node_pool.setter
     def public_ip_node_pool(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "public_ip_node_pool", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        The region of the node pool, has to match that of the cluster
-        """
-        return pulumi.get(self, "region")
-
-    @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "region", value)
-
-    @property
-    @pulumi.getter
     def size(self) -> Optional[pulumi.Input[str]]:
         """
-        the size of each node (optional, the default is currently g4s.kube.medium)
+        Size of the nodes in the nodepool
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size", value)
 
@@ -289,33 +256,31 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KubernetesNodePoolTaintArgs']]]]] = None,
                  __props__=None):
         """
         ## Import
 
         ```sh
         $ pulumi import civo:index/kubernetesNodePool:KubernetesNodePool my-pool 1b8b2100-0e9f-4e8f-ad78-9eb578c2a0af:502c1130-cb9b-4a88-b6d2-307bd96d946a
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
-        :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[int] node_count: Number of nodes in the nodepool
         :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
-        :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
-        :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
+        :param pulumi.Input[str] size: Size of the nodes in the nodepool
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: KubernetesNodePoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -342,15 +307,14 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KubernetesNodePoolTaintArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -359,19 +323,20 @@
             __props__ = KubernetesNodePoolArgs.__new__(KubernetesNodePoolArgs)
 
             if cluster_id is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster_id'")
             __props__.__dict__["cluster_id"] = cluster_id
             __props__.__dict__["label"] = label
             __props__.__dict__["labels"] = labels
+            if node_count is None and not opts.urn:
+                raise TypeError("Missing required property 'node_count'")
             __props__.__dict__["node_count"] = node_count
             __props__.__dict__["public_ip_node_pool"] = public_ip_node_pool
-            if region is None and not opts.urn:
-                raise TypeError("Missing required property 'region'")
-            __props__.__dict__["region"] = region
+            if size is None and not opts.urn:
+                raise TypeError("Missing required property 'size'")
             __props__.__dict__["size"] = size
             __props__.__dict__["taints"] = taints
             __props__.__dict__["instance_names"] = None
         super(KubernetesNodePool, __self__).__init__(
             'civo:index/kubernetesNodePool:KubernetesNodePool',
             resource_name,
             __props__,
@@ -383,43 +348,40 @@
             opts: Optional[pulumi.ResourceOptions] = None,
             cluster_id: Optional[pulumi.Input[str]] = None,
             instance_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             label: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             node_count: Optional[pulumi.Input[int]] = None,
             public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
-            region: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
             taints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KubernetesNodePoolTaintArgs']]]]] = None) -> 'KubernetesNodePool':
         """
         Get an existing KubernetesNodePool resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_names: Instance names in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
-        :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[int] node_count: Number of nodes in the nodepool
         :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
-        :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
-        :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
+        :param pulumi.Input[str] size: Size of the nodes in the nodepool
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _KubernetesNodePoolState.__new__(_KubernetesNodePoolState)
 
         __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["instance_names"] = instance_names
         __props__.__dict__["label"] = label
         __props__.__dict__["labels"] = labels
         __props__.__dict__["node_count"] = node_count
         __props__.__dict__["public_ip_node_pool"] = public_ip_node_pool
-        __props__.__dict__["region"] = region
         __props__.__dict__["size"] = size
         __props__.__dict__["taints"] = taints
         return KubernetesNodePool(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> pulumi.Output[str]:
@@ -449,39 +411,31 @@
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> pulumi.Output[int]:
         """
-        the number of instances to create (optional, the default at the time of writing is 3)
+        Number of nodes in the nodepool
         """
         return pulumi.get(self, "node_count")
 
     @property
     @pulumi.getter(name="publicIpNodePool")
     def public_ip_node_pool(self) -> pulumi.Output[bool]:
         """
         Node pool belongs to the public ip node pool
         """
         return pulumi.get(self, "public_ip_node_pool")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[str]:
-        """
-        The region of the node pool, has to match that of the cluster
-        """
-        return pulumi.get(self, "region")
-
-    @property
-    @pulumi.getter
     def size(self) -> pulumi.Output[str]:
         """
-        the size of each node (optional, the default is currently g4s.kube.medium)
+        Size of the nodes in the nodepool
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
     def taints(self) -> pulumi.Output[Optional[Sequence['outputs.KubernetesNodePoolTaint']]]:
         return pulumi.get(self, "taints")
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/reserved_ip.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,279 +5,242 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['NetworkArgs', 'Network']
+__all__ = ['ReservedIpArgs', 'ReservedIp']
 
 @pulumi.input_type
-class NetworkArgs:
+class ReservedIpArgs:
     def __init__(__self__, *,
-                 label: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Network resource.
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] region: The region of the network
+        The set of arguments for constructing a ReservedIp resource.
+        :param pulumi.Input[str] name: Name for the ip address
+        :param pulumi.Input[str] region: The region of the ip
         """
-        pulumi.set(__self__, "label", label)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if region is not None:
             pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
-    def label(self) -> pulumi.Input[str]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name for the network
+        Name for the ip address
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "name")
 
-    @label.setter
-    def label(self, value: pulumi.Input[str]):
-        pulumi.set(self, "label", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the network
+        The region of the ip
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
 
 @pulumi.input_type
-class _NetworkState:
+class _ReservedIpState:
     def __init__(__self__, *,
-                 default: Optional[pulumi.Input[bool]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
+                 ip: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Network resources.
-        :param pulumi.Input[bool] default: If the network is default, this will be `true`
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] name: The name of the network
-        :param pulumi.Input[str] region: The region of the network
-        """
-        if default is not None:
-            pulumi.set(__self__, "default", default)
-        if label is not None:
-            pulumi.set(__self__, "label", label)
+        Input properties used for looking up and filtering ReservedIp resources.
+        :param pulumi.Input[str] ip: The IP Address of the resource
+        :param pulumi.Input[str] name: Name for the ip address
+        :param pulumi.Input[str] region: The region of the ip
+        """
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
             pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
-    def default(self) -> Optional[pulumi.Input[bool]]:
-        """
-        If the network is default, this will be `true`
-        """
-        return pulumi.get(self, "default")
-
-    @default.setter
-    def default(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "default", value)
-
-    @property
-    @pulumi.getter
-    def label(self) -> Optional[pulumi.Input[str]]:
+    def ip(self) -> Optional[pulumi.Input[str]]:
         """
-        Name for the network
+        The IP Address of the resource
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "ip")
 
-    @label.setter
-    def label(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "label", value)
+    @ip.setter
+    def ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the network
+        Name for the ip address
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the network
+        The region of the ip
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
 
-class Network(pulumi.CustomResource):
+class ReservedIp(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 label: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Provides a Civo network resource. This can be used to create, modify, and delete networks.
+        Provides a Civo reserved IP to represent a publicly-accessible static IP addresses that can be mapped to one of your Instancesor Load Balancer.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        custom_net = civo.Network("custom_net", label="test_network")
+        www = civo.ReservedIp("www", name="nginx-www")
         ```
 
         ## Import
 
-        using ID
-
-        ```sh
-        $ pulumi import civo:index/network:Network custom_net b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
-        ```
+        terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] region: The region of the network
+        :param pulumi.Input[str] name: Name for the ip address
+        :param pulumi.Input[str] region: The region of the ip
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NetworkArgs,
+                 args: Optional[ReservedIpArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Civo network resource. This can be used to create, modify, and delete networks.
+        Provides a Civo reserved IP to represent a publicly-accessible static IP addresses that can be mapped to one of your Instancesor Load Balancer.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        custom_net = civo.Network("custom_net", label="test_network")
+        www = civo.ReservedIp("www", name="nginx-www")
         ```
 
         ## Import
 
-        using ID
-
-        ```sh
-        $ pulumi import civo:index/network:Network custom_net b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
-        ```
+        terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
 
         :param str resource_name: The name of the resource.
-        :param NetworkArgs args: The arguments to use to populate this resource's properties.
+        :param ReservedIpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NetworkArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ReservedIpArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 label: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NetworkArgs.__new__(NetworkArgs)
+            __props__ = ReservedIpArgs.__new__(ReservedIpArgs)
 
-            if label is None and not opts.urn:
-                raise TypeError("Missing required property 'label'")
-            __props__.__dict__["label"] = label
+            __props__.__dict__["name"] = name
             __props__.__dict__["region"] = region
-            __props__.__dict__["default"] = None
-            __props__.__dict__["name"] = None
-        super(Network, __self__).__init__(
-            'civo:index/network:Network',
+            __props__.__dict__["ip"] = None
+        super(ReservedIp, __self__).__init__(
+            'civo:index/reservedIp:ReservedIp',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            default: Optional[pulumi.Input[bool]] = None,
-            label: Optional[pulumi.Input[str]] = None,
+            ip: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            region: Optional[pulumi.Input[str]] = None) -> 'Network':
+            region: Optional[pulumi.Input[str]] = None) -> 'ReservedIp':
         """
-        Get an existing Network resource's state with the given name, id, and optional extra
+        Get an existing ReservedIp resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] default: If the network is default, this will be `true`
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] name: The name of the network
-        :param pulumi.Input[str] region: The region of the network
+        :param pulumi.Input[str] ip: The IP Address of the resource
+        :param pulumi.Input[str] name: Name for the ip address
+        :param pulumi.Input[str] region: The region of the ip
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _NetworkState.__new__(_NetworkState)
+        __props__ = _ReservedIpState.__new__(_ReservedIpState)
 
-        __props__.__dict__["default"] = default
-        __props__.__dict__["label"] = label
+        __props__.__dict__["ip"] = ip
         __props__.__dict__["name"] = name
         __props__.__dict__["region"] = region
-        return Network(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def default(self) -> pulumi.Output[bool]:
-        """
-        If the network is default, this will be `true`
-        """
-        return pulumi.get(self, "default")
+        return ReservedIp(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def label(self) -> pulumi.Output[str]:
+    def ip(self) -> pulumi.Output[str]:
         """
-        Name for the network
+        The IP Address of the resource
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "ip")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the network
+        Name for the ip address
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
-        The region of the network
+        The region of the ip
         """
         return pulumi.get(self, "region")
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
     'FirewallEgressRule',
     'FirewallIngressRule',
     'KubernetesClusterInstalledApplication',
     'KubernetesClusterPools',
+    'KubernetesClusterPoolsTaint',
     'KubernetesNodePoolTaint',
     'GetDatabaseVersionFilterResult',
     'GetDatabaseVersionSortResult',
     'GetDatabaseVersionVersionResult',
     'GetDiskImageDiskimageResult',
     'GetDiskImageFilterResult',
     'GetDiskImageSortResult',
     'GetInstancesFilterResult',
     'GetInstancesInstanceResult',
     'GetInstancesSortResult',
     'GetKubernetesClusterInstalledApplicationResult',
     'GetKubernetesClusterPoolResult',
+    'GetKubernetesClusterPoolTaintResult',
     'GetKubernetesVersionFilterResult',
     'GetKubernetesVersionSortResult',
     'GetKubernetesVersionVersionResult',
     'GetLoadBalancerBackendResult',
     'GetRegionFilterResult',
     'GetRegionRegionResult',
     'GetRegionSortResult',
@@ -297,30 +300,36 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  node_count: int,
                  size: str,
                  instance_names: Optional[Sequence[str]] = None,
                  label: Optional[str] = None,
-                 public_ip_node_pool: Optional[bool] = None):
+                 labels: Optional[Mapping[str, str]] = None,
+                 public_ip_node_pool: Optional[bool] = None,
+                 taints: Optional[Sequence['outputs.KubernetesClusterPoolsTaint']] = None):
         """
         :param int node_count: Number of nodes in the nodepool
         :param str size: Size of the nodes in the nodepool
         :param Sequence[str] instance_names: Instance names in the nodepool
         :param str label: Node pool label, if you don't provide one, we will generate one for you
         :param bool public_ip_node_pool: Node pool belongs to the public ip node pool
         """
         pulumi.set(__self__, "node_count", node_count)
         pulumi.set(__self__, "size", size)
         if instance_names is not None:
             pulumi.set(__self__, "instance_names", instance_names)
         if label is not None:
             pulumi.set(__self__, "label", label)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
         if public_ip_node_pool is not None:
             pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> int:
         """
         Number of nodes in the nodepool
         """
@@ -347,21 +356,57 @@
     def label(self) -> Optional[str]:
         """
         Node pool label, if you don't provide one, we will generate one for you
         """
         return pulumi.get(self, "label")
 
     @property
+    @pulumi.getter
+    def labels(self) -> Optional[Mapping[str, str]]:
+        return pulumi.get(self, "labels")
+
+    @property
     @pulumi.getter(name="publicIpNodePool")
     def public_ip_node_pool(self) -> Optional[bool]:
         """
         Node pool belongs to the public ip node pool
         """
         return pulumi.get(self, "public_ip_node_pool")
 
+    @property
+    @pulumi.getter
+    def taints(self) -> Optional[Sequence['outputs.KubernetesClusterPoolsTaint']]:
+        return pulumi.get(self, "taints")
+
+
+@pulumi.output_type
+class KubernetesClusterPoolsTaint(dict):
+    def __init__(__self__, *,
+                 effect: str,
+                 key: str,
+                 value: str):
+        pulumi.set(__self__, "effect", effect)
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> str:
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        return pulumi.get(self, "value")
+
 
 @pulumi.output_type
 class KubernetesNodePoolTaint(dict):
     def __init__(__self__, *,
                  effect: str,
                  key: str,
                  value: str):
@@ -1028,33 +1073,39 @@
 @pulumi.output_type
 class GetKubernetesClusterPoolResult(dict):
     def __init__(__self__, *,
                  instance_names: Sequence[str],
                  label: str,
                  node_count: int,
                  public_ip_node_pool: bool,
-                 size: str):
+                 size: str,
+                 labels: Optional[Mapping[str, str]] = None,
+                 taints: Optional[Sequence['outputs.GetKubernetesClusterPoolTaintResult']] = None):
         """
-        :param Sequence[str] instance_names: A list of the instance in the pool
+        :param Sequence[str] instance_names: Instance names in the nodepool
         :param str label: Node pool label, if you don't provide one, we will generate one for you
-        :param int node_count: The size of the pool
+        :param int node_count: Number of nodes in the nodepool
         :param bool public_ip_node_pool: Node pool belongs to the public ip node pool
-        :param str size: The size of each node inside the pool
+        :param str size: Size of the nodes in the nodepool
         """
         pulumi.set(__self__, "instance_names", instance_names)
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "node_count", node_count)
         pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
         pulumi.set(__self__, "size", size)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter(name="instanceNames")
     def instance_names(self) -> Sequence[str]:
         """
-        A list of the instance in the pool
+        Instance names in the nodepool
         """
         return pulumi.get(self, "instance_names")
 
     @property
     @pulumi.getter
     def label(self) -> str:
         """
@@ -1062,15 +1113,15 @@
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> int:
         """
-        The size of the pool
+        Number of nodes in the nodepool
         """
         return pulumi.get(self, "node_count")
 
     @property
     @pulumi.getter(name="publicIpNodePool")
     def public_ip_node_pool(self) -> bool:
         """
@@ -1078,18 +1129,54 @@
         """
         return pulumi.get(self, "public_ip_node_pool")
 
     @property
     @pulumi.getter
     def size(self) -> str:
         """
-        The size of each node inside the pool
+        Size of the nodes in the nodepool
         """
         return pulumi.get(self, "size")
 
+    @property
+    @pulumi.getter
+    def labels(self) -> Optional[Mapping[str, str]]:
+        return pulumi.get(self, "labels")
+
+    @property
+    @pulumi.getter
+    def taints(self) -> Optional[Sequence['outputs.GetKubernetesClusterPoolTaintResult']]:
+        return pulumi.get(self, "taints")
+
+
+@pulumi.output_type
+class GetKubernetesClusterPoolTaintResult(dict):
+    def __init__(__self__, *,
+                 effect: str,
+                 key: str,
+                 value: str):
+        pulumi.set(__self__, "effect", effect)
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> str:
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        return pulumi.get(self, "value")
+
 
 @pulumi.output_type
 class GetKubernetesVersionFilterResult(dict):
     def __init__(__self__, *,
                  key: str,
                  values: Sequence[str],
                  all: Optional[bool] = None,
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/ssh_key.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,242 +5,257 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ReservedIpArgs', 'ReservedIp']
+__all__ = ['SshKeyArgs', 'SshKey']
 
 @pulumi.input_type
-class ReservedIpArgs:
+class SshKeyArgs:
     def __init__(__self__, *,
-                 name: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None):
+                 public_key: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ReservedIp resource.
-        :param pulumi.Input[str] name: Name for the ip address
-        :param pulumi.Input[str] region: The region of the ip
+        The set of arguments for constructing a SshKey resource.
+        :param pulumi.Input[str] public_key: a string containing the SSH public key.
+        :param pulumi.Input[str] name: a string that will be the reference for the SSH key.
         """
+        pulumi.set(__self__, "public_key", public_key)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> pulumi.Input[str]:
         """
-        Name for the ip address
+        a string containing the SSH public key.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "public_key")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @public_key.setter
+    def public_key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the ip
+        a string that will be the reference for the SSH key.
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "name")
 
-    @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "region", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _ReservedIpState:
+class _SshKeyState:
     def __init__(__self__, *,
-                 ip: Optional[pulumi.Input[str]] = None,
+                 fingerprint: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None):
+                 public_key: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering ReservedIp resources.
-        :param pulumi.Input[str] ip: The IP Address of the resource
-        :param pulumi.Input[str] name: Name for the ip address
-        :param pulumi.Input[str] region: The region of the ip
+        Input properties used for looking up and filtering SshKey resources.
+        :param pulumi.Input[str] fingerprint: a string containing the SSH finger print.
+        :param pulumi.Input[str] name: a string that will be the reference for the SSH key.
+        :param pulumi.Input[str] public_key: a string containing the SSH public key.
         """
-        if ip is not None:
-            pulumi.set(__self__, "ip", ip)
+        if fingerprint is not None:
+            pulumi.set(__self__, "fingerprint", fingerprint)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
+        if public_key is not None:
+            pulumi.set(__self__, "public_key", public_key)
 
     @property
     @pulumi.getter
-    def ip(self) -> Optional[pulumi.Input[str]]:
+    def fingerprint(self) -> Optional[pulumi.Input[str]]:
         """
-        The IP Address of the resource
+        a string containing the SSH finger print.
         """
-        return pulumi.get(self, "ip")
+        return pulumi.get(self, "fingerprint")
 
-    @ip.setter
-    def ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip", value)
+    @fingerprint.setter
+    def fingerprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "fingerprint", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name for the ip address
+        a string that will be the reference for the SSH key.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the ip
+        a string containing the SSH public key.
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "public_key")
 
-    @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "region", value)
+    @public_key.setter
+    def public_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "public_key", value)
 
 
-class ReservedIp(pulumi.CustomResource):
+class SshKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
+                 public_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Provides a Civo reserved IP to represent a publicly-accessible static IP addresses that can be mapped to one of your Instancesor Load Balancer.
+        Provides a Civo SSH key resource to allow you to manage SSH keys for instance access. Keys created with this resource can be referenced in your instance configuration via their ID.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_civo as civo
+        import pulumi_std as std
 
-        www = civo.ReservedIp("www", name="nginx-www")
+        my_user = civo.SshKey("my-user",
+            name="my-user",
+            public_key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
 
         ## Import
 
-        terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
+        using ID
+
+        ```sh
+        $ pulumi import civo:index/sshKey:SshKey mykey 87ca2ee4-57d3-4420-b9b6-411b0b4b2a0e
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: Name for the ip address
-        :param pulumi.Input[str] region: The region of the ip
+        :param pulumi.Input[str] name: a string that will be the reference for the SSH key.
+        :param pulumi.Input[str] public_key: a string containing the SSH public key.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ReservedIpArgs] = None,
+                 args: SshKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Civo reserved IP to represent a publicly-accessible static IP addresses that can be mapped to one of your Instancesor Load Balancer.
+        Provides a Civo SSH key resource to allow you to manage SSH keys for instance access. Keys created with this resource can be referenced in your instance configuration via their ID.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_civo as civo
+        import pulumi_std as std
 
-        www = civo.ReservedIp("www", name="nginx-www")
+        my_user = civo.SshKey("my-user",
+            name="my-user",
+            public_key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
 
         ## Import
 
-        terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
+        using ID
+
+        ```sh
+        $ pulumi import civo:index/sshKey:SshKey mykey 87ca2ee4-57d3-4420-b9b6-411b0b4b2a0e
+        ```
 
         :param str resource_name: The name of the resource.
-        :param ReservedIpArgs args: The arguments to use to populate this resource's properties.
+        :param SshKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ReservedIpArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SshKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
+                 public_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ReservedIpArgs.__new__(ReservedIpArgs)
+            __props__ = SshKeyArgs.__new__(SshKeyArgs)
 
             __props__.__dict__["name"] = name
-            __props__.__dict__["region"] = region
-            __props__.__dict__["ip"] = None
-        super(ReservedIp, __self__).__init__(
-            'civo:index/reservedIp:ReservedIp',
+            if public_key is None and not opts.urn:
+                raise TypeError("Missing required property 'public_key'")
+            __props__.__dict__["public_key"] = public_key
+            __props__.__dict__["fingerprint"] = None
+        super(SshKey, __self__).__init__(
+            'civo:index/sshKey:SshKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            ip: Optional[pulumi.Input[str]] = None,
+            fingerprint: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            region: Optional[pulumi.Input[str]] = None) -> 'ReservedIp':
+            public_key: Optional[pulumi.Input[str]] = None) -> 'SshKey':
         """
-        Get an existing ReservedIp resource's state with the given name, id, and optional extra
+        Get an existing SshKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] ip: The IP Address of the resource
-        :param pulumi.Input[str] name: Name for the ip address
-        :param pulumi.Input[str] region: The region of the ip
+        :param pulumi.Input[str] fingerprint: a string containing the SSH finger print.
+        :param pulumi.Input[str] name: a string that will be the reference for the SSH key.
+        :param pulumi.Input[str] public_key: a string containing the SSH public key.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ReservedIpState.__new__(_ReservedIpState)
+        __props__ = _SshKeyState.__new__(_SshKeyState)
 
-        __props__.__dict__["ip"] = ip
+        __props__.__dict__["fingerprint"] = fingerprint
         __props__.__dict__["name"] = name
-        __props__.__dict__["region"] = region
-        return ReservedIp(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["public_key"] = public_key
+        return SshKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def ip(self) -> pulumi.Output[str]:
+    def fingerprint(self) -> pulumi.Output[str]:
         """
-        The IP Address of the resource
+        a string containing the SSH finger print.
         """
-        return pulumi.get(self, "ip")
+        return pulumi.get(self, "fingerprint")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name for the ip address
+        a string that will be the reference for the SSH key.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def region(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> pulumi.Output[str]:
         """
-        The region of the ip
+        a string containing the SSH public key.
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "public_key")
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1714509760/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1714454433
+Version: 2.4.0a1714509760
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1714454433/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1714509760/pulumi_civo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pulumi_civo/__init__.py
 pulumi_civo/_inputs.py
 pulumi_civo/_utilities.py
 pulumi_civo/database.py
 pulumi_civo/dns_domain_name.py
 pulumi_civo/dns_domain_record.py
 pulumi_civo/firewall.py
-pulumi_civo/firewall_rule.py
 pulumi_civo/get_database.py
 pulumi_civo/get_database_version.py
 pulumi_civo/get_disk_image.py
 pulumi_civo/get_dns_domain_name.py
 pulumi_civo/get_dns_domain_record.py
 pulumi_civo/get_firewall.py
 pulumi_civo/get_instance.py
```

### Comparing `pulumi_civo-2.4.0a1714454433/pyproject.toml` & `pulumi_civo-2.4.0a1714509760/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_civo"
   description = "A Pulumi package for creating and managing Civo cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "civo"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1714454433"
+  version = "2.4.0a1714509760"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-civo"
 
 [build-system]
```

