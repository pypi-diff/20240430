# Comparing `tmp/networklab-1.8.1.post1.tar.gz` & `tmp/networklab-1.8.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.8.1.post1.tar", last modified: Wed Apr 24 08:33:48 2024, max compression
+gzip compressed data, was "networklab-1.8.2.dev1.tar", last modified: Tue Apr 30 16:59:07 2024, max compression
```

## Comparing `networklab-1.8.1.post1.tar` & `networklab-1.8.2.dev1.tar`

### file list

```diff
@@ -1,741 +1,759 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netlab
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.494491 networklab-1.8.1.post1/netsim/
--rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.498491 networklab-1.8.1.post1/netsim/ansible/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/create-config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/initial-config.ansible
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/reload-config.ansible
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.498491 networklab-1.8.1.post1/netsim/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/create-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/create-custom-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/frr/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/frr/mpls-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/initial-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/linux/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/nxos/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/vmx/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/vmx/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/wait-for-ready.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/templates/bfd/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.510491 networklab-1.8.1.post1/netsim/ansible/templates/bgp/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.514491 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/dnsmasq.j2
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/linux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.514491 networklab-1.8.1.post1/netsim/ansible/templates/eigrp/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.514491 networklab-1.8.1.post1/netsim/ansible/templates/evpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.518491 networklab-1.8.1.post1/netsim/ansible/templates/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.522491 networklab-1.8.1.post1/netsim/ansible/templates/initial/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.522491 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.526491 networklab-1.8.1.post1/netsim/ansible/templates/isis/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.530491 networklab-1.8.1.post1/netsim/ansible/templates/mpls/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/srlinux.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.534491 networklab-1.8.1.post1/netsim/ansible/templates/ospf/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/junos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.538491 networklab-1.8.1.post1/netsim/ansible/templates/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.538491 networklab-1.8.1.post1/netsim/ansible/templates/srv6/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.538491 networklab-1.8.1.post1/netsim/ansible/templates/vlan/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.546491 networklab-1.8.1.post1/netsim/ansible/templates/vrf/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.ospf-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.550491 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.550491 networklab-1.8.1.post1/netsim/api/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.550491 networklab-1.8.1.post1/netsim/augment/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.554491 networklab-1.8.1.post1/netsim/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10608 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/alias.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.554491 networklab-1.8.1.post1/netsim/cli/clab_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab_actions/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab_actions/tarball.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/down.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/external_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show-usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/cli/show_commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/module_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/up.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/daemons/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/daemons/bird.yml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/daemons/dnsmasq.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/filemaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28964 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/addressing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/automation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/hints.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/multilab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/paths.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/ports.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.562491 networklab-1.8.1.post1/netsim/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/arubacx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/asav.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/asav.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/csr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/eos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/iosv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/iosv.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/junos.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/unknown.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vmx.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vmx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vptx.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vsrx.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vsrx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.490491 networklab-1.8.1.post1/netsim/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.562491 networklab-1.8.1.post1/netsim/extra/bgp.domain/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.domain/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.domain/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.566491 networklab-1.8.1.post1/netsim/extra/bgp.originate/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.originate/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.originate/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.566491 networklab-1.8.1.post1/netsim/extra/bgp.policy/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_aoscx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/simple-attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/srlinux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/bgp.session/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/_sample_bfd_template.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/bird.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/default-originate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/topology.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/ebgp.utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.utils/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/fabric/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/fabric/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/multilab/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/multilab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/none/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/none/none.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/extra/proxy-arp/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/install/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/ansible.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/containerlab.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/grpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/install/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/install/libvirt/asav/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/asav.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/csr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/eos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/iosv.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.578491 networklab-1.8.1.post1/netsim/install/libvirt/vptx/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.578491 networklab-1.8.1.post1/netsim/install/libvirt/vsrx/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.582491 networklab-1.8.1.post1/netsim/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/_dataplane.py
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bfd.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bfd.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/eigrp.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/eigrp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/evpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/evpn.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/gateway.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/isis.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/isis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/mpls.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/mpls.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/ospf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/sr.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/sr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/srv6.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/srv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)    61378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vlan.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vrf.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vxlan.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/d2.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/d2.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/graph.yml
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/providers/
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/clab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/external.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/virtualbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.494491 networklab-1.8.1.post1/netsim/templates/provider/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/templates/provider/clab/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/interfaces.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/clab/frr/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/frr/daemons.j2
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/frr/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/clab/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/templates/provider/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/forwarded-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/vsrx-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/grpc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/graphite.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/tools/suzieq/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/suzieq.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/topology-defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/netsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/netsim/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/validate/frr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/validate/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/networklab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24814 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netlab
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.167304 networklab-1.8.2.dev1/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.167304 networklab-1.8.2.dev1/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/reload-config.ansible
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.167304 networklab-1.8.2.dev1/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/create-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/create-custom-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.171304 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sonic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/frr/mpls-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/initial-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/linux/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.175304 networklab-1.8.2.dev1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/vmx/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/tasks/wait-for-ready.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.179304 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.187304 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sonic.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.187304 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/dnsmasq.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/linux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.187304 networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.191304 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.191304 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.199304 networklab-1.8.2.dev1/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/eos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.199304 networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr/daemons.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.199304 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/bash_profile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sonic.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.203304 networklab-1.8.2.dev1/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.207305 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/srlinux.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.215304 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/junos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.215304 networklab-1.8.2.dev1/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.215304 networklab-1.8.2.dev1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.219305 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.227305 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.ospf-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.231305 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.231305 networklab-1.8.2.dev1/netsim/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.231305 networklab-1.8.2.dev1/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/augment/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10608 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/_nodeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/clab_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab_actions/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/clab_actions/tarball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/libvirt_actions/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show-usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.239305 networklab-1.8.2.dev1/netsim/cli/show_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/module_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/show_commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.243305 networklab-1.8.2.dev1/netsim/daemons/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/daemons/bird.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/daemons/dnsmasq.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.243305 networklab-1.8.2.dev1/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28964 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.243305 networklab-1.8.2.dev1/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/paths.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/sonic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.163304 networklab-1.8.2.dev1/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/extra/bgp.domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.domain/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.domain/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/extra/bgp.originate/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.originate/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.originate/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.251305 networklab-1.8.2.dev1/netsim/extra/bgp.policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_aoscx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/simple-attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.policy/srlinux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.255305 networklab-1.8.2.dev1/netsim/extra/bgp.session/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/_sample_bfd_template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/bird.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/bgp.session/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/ebgp.utils/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/fabric/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/fabric/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/multilab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.259305 networklab-1.8.2.dev1/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/asav.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/csr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/dellos10/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/dellos10/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/routeros7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/sonic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/sonic.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.263305 networklab-1.8.2.dev1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.271305 networklab-1.8.2.dev1/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    61378 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16735 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/providers/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.163304 networklab-1.8.2.dev1/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.275305 networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/interfaces.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.279305 networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/daemons.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.279305 networklab-1.8.2.dev1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.279305 networklab-1.8.2.dev1/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.283305 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/forwarded-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/sonic-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/vsrx-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/grpc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.287305 networklab-1.8.2.dev1/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/utils/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/netsim/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/validate/frr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/netsim/validate/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25397 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 16:59:07.000000 networklab-1.8.2.dev1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:59:07.291305 networklab-1.8.2.dev1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-04-30 16:59:02.000000 networklab-1.8.2.dev1/tests/test_transformation.py
```

### Comparing `networklab-1.8.1.post1/LICENSE.md` & `networklab-1.8.2.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/PKG-INFO` & `networklab-1.8.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.1.post1
+Version: 1.8.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.8.1.post1/README.md` & `networklab-1.8.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/collect-configs.ansible` & `networklab-1.8.2.dev1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/create-config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/initial-config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/reload-config.ansible` & `networklab-1.8.2.dev1/netsim/ansible/reload-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/create-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/create-custom-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/create-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/cumulus.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/linux/dhcp.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/linux/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/vptx.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/readiness-check/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.8.2.dev1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/dnsmasq.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/dnsmasq.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.server.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/eos.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.server.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/ios.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/sros.j2`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 updates:
 {% for intf in interfaces if intf.gateway.protocol is defined %}
 {{ declare_interface(intf) }}
   val:
 {%  for af in ('ipv4','ipv6') %}
 {%   if intf.gateway.protocol in ['anycast','vrrp'] and af in intf.gateway %}
    {{ af }}:
+{% if af=='ipv6' %}
+    address:
+    - ipv6-address: "{{ intf.ipv6|default('')|ipaddr('address') }}"
+      duplicate-address-detection: False
+{% endif %}
     vrrp:
     - virtual-router-id: {{ intf.gateway.vrrp.group|default(1) }}
       admin-state: enable
       ping-reply: True
       backup: [ "{{ intf.gateway[af]|ipaddr('address') }}" ]
       passive: {{ intf.gateway.protocol == 'anycast' }}
-{%    if intf.gateway.anycast.mac is defined %}
+{%    if intf.gateway.anycast.mac is defined and 'ixr' not in clab.type %}
       mac: {{ intf.gateway.anycast.mac|hwaddr('linux') }}
 {%    endif %}
 {%    if intf.gateway.protocol == 'vrrp' %}
       preempt: {{ intf.gateway.vrrp.preempt|default(False)|bool }}
 {%     if 'priority' in intf.gateway.vrrp %}
       priority: {{ intf.gateway.vrrp.priority }}
 {%     endif %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files 14% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     ip address {{ l.ipv4 }}
 {% endif %}
 {#
     Set interface IPv6 addresses
 #}
 {% if 'ipv6' in l %}
     ipv6 address {{ l.ipv6 }}
+{# need to explicitly set nd ra config #}
+    no ipv6 nd suppress-ra
+    ipv6 nd ra min-interval 3
+    ipv6 nd ra max-interval 4
 {% endif %}
 {% if l.virtual_interface is not defined %}
     no shutdown
 {% endif %}
 !
 {% endfor %}
 !
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/asa.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files 10% similar despite different names*

```diff
@@ -45,12 +45,13 @@
 /ip address add interface={{ l.ifname }} address={{ l.ipv4 }}
 {%   if l.name is defined %}
 /ip address set [find where interface={{ l.ifname }}] comment="{{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}"
 {%   endif %}
 {% endif %}
 {% if 'ipv6' in l %}
 /ipv6 address add interface={{ l.ifname }} address={{ l.ipv6 }}
+/ipv6 nd add interface={{ l.ifname }} advertise-dns=no ra-interval=3s-30s
 {% endif %}
 
 {% endfor %}
 
 /ip neighbor discovery-settings set discover-interface-list=all
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/asa.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 {% from "templates/initial/sros.j2" import if_name with context %}
 
-updates:
-- path: configure/router[router-name=Base]
+{% macro isis_config(l,vrf=None) %}
+{% set path = "router[router-name=Base]" if not vrf else "service/vprn[service-name="+vrf+"]" %}
+- path: configure/{{ path }}
   val:
    isis:
    - isis-instance: 0
      admin-state: enable
      area-address: ["{{ isis.net | default( "%s.0000.0000.%04d.00" % (isis.area,id) ) }}"]
      level-capability: "{{ '2' if isis.type=='level-2' else ('1' if isis.type=='level-1' else '1/2') }}"
 {%   if isis.af.ipv6 is defined %}
      multi-topology:
       ipv6-unicast: True
 {%   endif %}
      interface:
-     - interface-name: system
-       passive: True
-{%   for l in interfaces|default([]) if 'isis' in l %}
      - interface-name: {{ if_name(l,l.ifname) }}
        interface-type: {{ l.isis.network_type|default('broadcast') }}
        passive: {{ l.isis.passive }}
 {%     if l.isis.bfd is defined %}
        bfd-liveness:
 {%     if l.isis.bfd.ipv4|default(False) %}
         ipv4:
@@ -36,8 +34,15 @@
        - level-number: "{{ level }}"
          metric: {{ l.isis.metric|default(l.isis.cost) }}
 {%       if 'ipv6' in isis.af and 'ipv6' in l %}
          ipv6-unicast-metric: {{ l.isis.metric|default(l.isis.cost) }}
 {%       endif %}
 {%     endfor %}
 {%     endif %}
-{%   endfor %}
+{% endmacro %}
+
+updates:
+{{ isis_config( { 'ifname': 'system', 'isis': { 'passive' : True } } ) }}
+
+{% for l in interfaces|default([]) if 'isis' in l %}
+{{ isis_config(l,l.vrf|default('default' if l.vlan.mode|default('irb')!='route' else None)) }}
+{% endfor %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/srlinux.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/srlinux.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/sros.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/junos.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/junos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% set KW_NETWORK_TYPE = {'point-to-point': 'ptp','point-to-multipoint': 'ptmp', 'non-broadcast': 'nbma','broadcast': 'broadcast' } %}
 
-{% set area = ospf.area|default("0.0.0.0") %}
+{% set area = (ospf.area|default("0.0.0.0"))|string|ansible.utils.ipaddr('address') %}
 
 {% if ospf_router_id|ipv4 %}
 /routing/ospf/instance add name={{instance}} version={{ospf_version}} router-id={{ ospf_router_id }} vrf={{ospf_vrf|default('main')}}
 {% endif %}
 
 {#
   Create AREA list. If default area != 0.0.0.0, append to list
@@ -17,19 +17,19 @@
 {{ area_list.append(l.ospf.area) }}
 {% endfor %}
 
 {#
   For each unique area, add to area configuration
 #}
 {% for a_def in area_list|unique %}
-/routing/ospf/area add instance={{instance}} name="{{ospf_vrf|default('main')}}_{{ospf_version}}_{{ a_def }}" area-id={{ a_def }}
+/routing/ospf/area add instance={{instance}} name="{{ospf_vrf|default('main')}}_{{ospf_version}}_{{ a_def }}" area-id={{ a_def|string|ansible.utils.ipaddr('address') }}
 {% endfor %}
 
 {% if ospf_main_vrf is defined and ospf_main_vrf %}
-/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ l.ospf.area|default(area) }} and instance={{instance}}] interface=loopback passive
+/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ (l.ospf.area|default(area))|string|ansible.utils.ipaddr('address') }} and instance={{instance}}] interface=loopback passive
 {% endif %}
 
 {% for l in ospf_interfaces|default([]) if 'ospf' in l and ospf_afi_check in l %}
 
 {%   if "external" in l.role|default("") %}
 ## OSPF not configured on external interface {{ l.ifname }}
 {%   else %}
@@ -48,12 +48,12 @@
 {{ ospf_intf_params.append('cost='+l.ospf.cost|string) }}
 {%     endif %}
 
 {%     if l.ospf.bfd|default(False) %}
 ## BFD Currently not supported in ROS7 for OSPF
 {%     endif %}
 
-/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ l.ospf.area|default(area) }} and instance={{instance}}] interface={{ l.ifname }} {{ ospf_intf_params|join(' ') }}
+/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ (l.ospf.area|default(area))|string|ansible.utils.ipaddr('address') }} and instance={{instance}}] interface={{ l.ifname }} {{ ospf_intf_params|join(' ') }}
 
 {%   endif %}
 
 {% endfor %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/sr/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {%   endfor %}
 
 {%   for af in ('ipv4','ipv6') if af in vdata.af|default({}) %}
  address-family {{ af }} unicast
   redistribute connected
   redistribute local loopback
 {%     if af == 'ipv4' and 'ospf' in vdata %}
-  redistribute ospf {{ vdata.vrfidx }}
+  redistribute ospf {{ vdata.ospfidx }}
 {%     endif %}
 !
 {%     for n in vdata.networks|default([]) if af in n %}
 {{       bgpcfg.bgp_network(af,n[af]) }}
 {%     endfor %}
 !
 {%     for n in vdata.bgp.neighbors|default([]) if af in n %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 !
 router ospf {{ vdata.ospfidx }} vrf {{ vname }}
     router-id {{ vdata.ospf.router_id|default(ospf.router_id) }}
 
 {% if bgp.as is defined %}
     redistribute bgp
 {% endif %}
+    redistribute connected
 
 {% if ospf.reference_bandwidth is defined %}
     reference-bandwidth {{ ospf.reference_bandwidth }}
 {% endif %}
 
 {# need to define all areas in advance #}
 {% for l in vdata.ospf.interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.frr-config.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv3.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.ospf-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/junos.ospf-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+{% macro community(list) -%}
+{{ "both" if list|length >= 2 else list[0] }}
+{%- endmacro %}
 !
 route-map all
 !
 router bgp {{ bgp.as }}
 {% for vname, vdata in vrfs.items() %}
   vrf {{ vname }}
 {%   if bgp.router_id|ipv4 %}
@@ -28,19 +31,19 @@
 {%       if n.type == 'ibgp' %}
 {%         if bgp.next_hop_self is defined and bgp.next_hop_self %}
         next-hop-self
 {%         endif %}
 {%         if bgp.rr|default('') and not n.rr|default('') %}
         route-reflector-client
 {%         endif %}
-{%         if vdata.bgp.community.ibgp|default([]) %}
+{%         if bgp.community.ibgp|default([]) %}
         send-community {{ community(bgp.community.ibgp) }}
 {%         endif %}
 {%       else %}
-{%         if vdata.bgp.community.ebgp|default([]) %}
+{%         if bgp.community.ebgp|default([]) %}
         send-community {{ community(bgp.community.ebgp) }}
 {%         endif %}
 {%       endif %}
         exit
       exit
 !
 {%     endfor %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% set KW_NETWORK_TYPE = {'point-to-point': 'ptp','point-to-multipoint': 'ptmp', 'non-broadcast': 'nbma','broadcast': 'broadcast' } %}
 
-{% set area = ospf.area|default("0.0.0.0") %}
+{% set area = (ospf.area|default("0.0.0.0"))|string|ansible.utils.ipaddr('address') %}
 
 {% if ospf_router_id|ipv4 %}
 /routing/ospf/instance add name={{instance}} version={{ospf_version}} router-id={{ ospf_router_id }} vrf={{ospf_vrf|default('main')}}
 {% endif %}
 
 {#
   Create AREA list. If default area != 0.0.0.0, append to list
@@ -17,19 +17,19 @@
 {{ area_list.append(l.ospf.area) }}
 {% endfor %}
 
 {#
   For each unique area, add to area configuration
 #}
 {% for a_def in area_list|unique %}
-/routing/ospf/area add instance={{instance}} name="{{ospf_vrf|default('main')}}_{{ospf_version}}_{{ a_def }}" area-id={{ a_def }}
+/routing/ospf/area add instance={{instance}} name="{{ospf_vrf|default('main')}}_{{ospf_version}}_{{ a_def }}" area-id={{ a_def|string|ansible.utils.ipaddr('address') }}
 {% endfor %}
 
 {% if ospf_main_vrf is defined and ospf_main_vrf %}
-/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ l.ospf.area|default(area) }} and instance={{instance}}] interface=loopback passive
+/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ (l.ospf.area|default(area))|string|ansible.utils.ipaddr('address') }} and instance={{instance}}] interface=loopback passive
 {% endif %}
 
 {% for l in ospf_interfaces|default([]) if 'ospf' in l and ospf_afi_check in l %}
 
 {%   if "external" in l.role|default("") %}
 ## OSPF not configured on external interface {{ l.ifname }}
 {%   else %}
@@ -48,12 +48,12 @@
 {{ ospf_intf_params.append('cost='+l.ospf.cost|string) }}
 {%     endif %}
 
 {%     if l.ospf.bfd|default(False) %}
 ## BFD Currently not supported in ROS7 for OSPF
 {%     endif %}
 
-/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ l.ospf.area|default(area) }} and instance={{instance}}] interface={{ l.ifname }} {{ ospf_intf_params|join(' ') }}
+/routing/ospf/interface-template add area=[/routing ospf area find area-id={{ (l.ospf.area|default(area))|string|ansible.utils.ipaddr('address') }} and instance={{instance}}] interface={{ l.ifname }} {{ ospf_intf_params|join(' ') }}
 
 {%   endif %}
 
 {% endfor %}
```

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.8.2.dev1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/api/__init__.py` & `networklab-1.8.2.dev1/netsim/api/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/addressing.py` & `networklab-1.8.2.dev1/netsim/augment/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/components.py` & `networklab-1.8.2.dev1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/devices.py` & `networklab-1.8.2.dev1/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/groups.py` & `networklab-1.8.2.dev1/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/links.py` & `networklab-1.8.2.dev1/netsim/augment/links.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/main.py` & `networklab-1.8.2.dev1/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/nodes.py` & `networklab-1.8.2.dev1/netsim/augment/nodes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/plugin.py` & `networklab-1.8.2.dev1/netsim/augment/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     topology.plugin.extend(topology.defaults.plugin)                                          # ... and extend it with default plugins
 
   if not 'plugin' in topology:
     return
 
   topology.Plugin = []
   load_error = False
-  search_path = get_search_path(pkg_path_component='extra')   # Search the usual places plus the 'extra' package directory
+  search_path = topology.defaults.paths.plugin
   for pname in list(topology.plugin):                         # Iterate over all plugins
     for path in search_path:
       plugin = load_plugin_from_path(path,pname,topology)     # Try to load plugin from the current search path directory
       if plugin:                                              # Got it, get out of the loop
         break
 
     if plugin:                                                # If we found the plugin...
```

### Comparing `networklab-1.8.1.post1/netsim/augment/tools.py` & `networklab-1.8.2.dev1/netsim/augment/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/topology.py` & `networklab-1.8.2.dev1/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/augment/validate.py` & `networklab-1.8.2.dev1/netsim/augment/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/__init__.py` & `networklab-1.8.2.dev1/netsim/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/ansible.py` & `networklab-1.8.2.dev1/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/clab.py` & `networklab-1.8.2.dev1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/clab_actions/build.py` & `networklab-1.8.2.dev1/netsim/cli/clab_actions/build.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/clab_actions/tarball.py` & `networklab-1.8.2.dev1/netsim/cli/clab_actions/tarball.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/collect.py` & `networklab-1.8.2.dev1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/config.py` & `networklab-1.8.2.dev1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/connect.py` & `networklab-1.8.2.dev1/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/create.py` & `networklab-1.8.2.dev1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/down.py` & `networklab-1.8.2.dev1/netsim/cli/down.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 #
 def stop_provider_lab(
       topology: Box,
       pname: str,
       sname: typing.Optional[str] = None) -> None:
   p_name = sname or pname
   p_topology = providers.select_topology(topology,p_name)
-  p_module   = providers._Provider.load(p_name,topology.defaults.providers[p_name])
+  p_module   = providers.get_provider_module(topology,p_name)
 
   exec_command = None
   if sname is not None:
     exec_command = topology.defaults.providers[pname][sname].stop
 
   p_module.call('pre_stop_lab',p_topology)
   external_commands.stop_lab(topology.defaults,p_name,"netlab down",exec_command)
@@ -147,15 +147,15 @@
 
 def stop_all(topology: Box, args: argparse.Namespace) -> None:
   if 'tools' in topology:
     log.section_header('Stopping','external tools','yellow')
     stop_external_tools(args,topology)
 
   p_provider = topology.provider
-  p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
+  p_module = providers.get_provider_module(topology,p_provider)
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
   for s_provider in topology[p_provider].providers:
     lab_status_change(topology,f'stopping {s_provider} provider')
     try:
       log.section_header('Stopping',f'{s_provider} nodes','yellow')
```

### Comparing `networklab-1.8.1.post1/netsim/cli/external_commands.py` & `networklab-1.8.2.dev1/netsim/cli/external_commands.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/graph.py` & `networklab-1.8.2.dev1/netsim/cli/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/initial.py` & `networklab-1.8.2.dev1/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/inspect.py` & `networklab-1.8.2.dev1/netsim/cli/inspect.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Inspect data structures in transformed lab topology
 #
 import typing
 import os
 import sys
 import argparse
 
-from box import Box
+from box import Box,BoxList
 
-from . import load_snapshot
+from . import load_snapshot,_nodeset
 from ..outputs import _TopologyOutput
 from ..outputs import common as outputs_common
 from ..utils import strings,log
 from ..data.types import must_be_id
 from ..data import global_vars
 
 #
@@ -31,54 +31,65 @@
     nargs='?',
     default='netlab.snapshot.yml',
     const='netlab.snapshot.yml',
     help='Transformed topology snapshot file')
   parser.add_argument(
     '--node',
     dest='node', action='store',
-    help='Display data for selected node')
+    help='Display data for selected node(s)')
   parser.add_argument(
     '--format',
     dest='format', action='store',
     default='yaml',
     choices=['yaml','json'],
     help='Select data presentation format')
   parser.add_argument(
     dest='expr', action='store',
     nargs='?',
     help='Data selection expression')
 
   return parser.parse_args(args)
 
+def inspect_value(topology: Box, args: argparse.Namespace) -> None:
+  o_module = args.format or 'yaml'
+  o_param  = f'{o_module}:{args.expr or "."}'
+  inspect_module = _TopologyOutput.load(o_param,topology.get('defaults.outputs.{o_module}',{}))
+  if not inspect_module:
+    log.fatal(f'Cannot load the data inspection output module {o_module}, aborting')
+
+  inspect_module.write(topology)
+
+def fmt_value(v: typing.Union[Box,BoxList], fmt: str) -> str:
+  value = v.to_yaml() if fmt == 'yaml' else v.to_json()
+  return value.strip('\n')
+
+def inspect_node(topology: Box, node_list: list, args: argparse.Namespace) -> None:
+  o_format = args.format or 'yaml'
+  hdr_row: list = []
+  data_row: list = []
+
+  for node in node_list:
+    node_data = outputs_common.adjust_inventory_host(
+                  node=topology.nodes[node],
+                  defaults=topology.defaults,
+                  group_vars=True)
+    if len(node_list) == 1:
+      inspect_value(node_data,args)
+      return
+    else:
+      select = node_data.get(args.expr,None) if args.expr else node_data
+      value  = fmt_value(select,o_format) if isinstance(select,Box) or isinstance(select,BoxList) else str(select)
+      hdr_row.append(node)
+      data_row.append(value)
+
+  strings.print_table(hdr_row,[ data_row ])
+
 def run(cli_args: typing.List[str]) -> None:
   args = inspect_parse(cli_args)
   topology = load_snapshot(args)
-
-  o_module = args.format or 'yaml'
-  o_param  = f'{o_module}:{args.expr or "."}'
-  inspect_module = _TopologyOutput.load(o_param,topology.defaults.outputs[o_module])
+  log.init_log_system(False)
 
   if args.node:
-    log.init_log_system(False)
-    must_be_id(
-      parent=None,
-      key=args.node,
-      path=f'NOATTR:--node parameter',
-      max_length=global_vars.get_const('MAX_NODE_ID_LENGTH',16),
-      module='inspect')
-    log.exit_on_error()
-    if args.node in topology.nodes:
-      topology = outputs_common.adjust_inventory_host(
-                node=topology.nodes[args.node],
-                defaults=topology.defaults,
-                group_vars=True)
-    else:
-      log.fatal(
-        f'Unknown node {args.node}\n'+ \
-        strings.extra_data_printout(
-          f'Valid node names are: {", ".join(list(topology.nodes.keys()))}'),
-        module='inspect')
-
-  if inspect_module:
-    inspect_module.write(topology)
+    node_list = _nodeset.parse_nodeset(args.node,topology)
+    inspect_node(topology,node_list,args)
   else:
-    log.fatal('Cannot load the data inspection output module, aborting')
+    inspect_value(topology,args)
```

### Comparing `networklab-1.8.1.post1/netsim/cli/install.py` & `networklab-1.8.2.dev1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/read.py` & `networklab-1.8.2.dev1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/report.py` & `networklab-1.8.2.dev1/netsim/cli/report.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # netlab report command
 #
 # Create a text or HTML report from the current lab topology
 #
 import typing
 import argparse
 
-from . import load_snapshot
+from . import load_snapshot,_nodeset
 from ..outputs import _TopologyOutput, common as outputs_common
 from ..utils import strings,log
 
 #
 # CLI parser for 'netlab report' command
 #
 def report_parse(args: typing.List[str]) -> argparse.Namespace:
@@ -22,14 +22,18 @@
     dest='snapshot',
     action='store',
     nargs='?',
     default='netlab.snapshot.yml',
     const='netlab.snapshot.yml',
     help='Transformed topology snapshot file')
   parser.add_argument(
+    '--node',
+    dest='node', action='store',
+    help='Limit the report to selected node(s)')
+  parser.add_argument(
     dest='report', action='store',
     help='Name of the report you want to create')
   parser.add_argument(
     dest='output', action='store',
     nargs='?',
     help='Output file name (default: stdout)')
 
@@ -40,14 +44,17 @@
   topology = load_snapshot(args)
   report_module = _TopologyOutput.load(
                      f'report:{args.report}={args.output or "-"}',
                      topology.defaults.outputs.report)
   if not report_module:
     log.fatal('Cannot load the reporting output module, aborting')
 
+  if args.node:
+    topology = _nodeset.get_nodeset(topology,_nodeset.parse_nodeset(args.node,topology))
+
   for n in list(topology.nodes.keys()):                     # Add group variables to topology nodes
     topology.nodes[n] = outputs_common.adjust_inventory_host(
                           node=topology.nodes[n],
                           ignore=[ 'no-fields' ],
                           defaults=topology.defaults,
                           group_vars=True)
```

### Comparing `networklab-1.8.1.post1/netsim/cli/restart.py` & `networklab-1.8.2.dev1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show-usage.txt` & `networklab-1.8.2.dev1/netsim/cli/show-usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show.py` & `networklab-1.8.2.dev1/netsim/cli/show.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing
 import argparse
 import textwrap
 import sys
 from box import Box
 
 from .. import data
-from ..augment import main
+from ..augment import main,config
 from ..utils import log,read as _read
 from .usage import print_usage
 
 from .show_commands import show_common_parser
 from .show_commands import devices as _devices
 from .show_commands import images as _images
 from .show_commands import modules as _modules
@@ -106,12 +106,13 @@
 #  topology.nodes = data.get_empty_box()
   topology.nodes.dummy.device = 'none'                  # Add a dummy node
   topology.nodes.dummy.module = []                      # ... and disable all modules on that node
   if 'plugin' in args and args.plugin:
     topology.plugin = args.plugin
 
   if args.action in ['defaults']:                       # Save original paths for the "show defaults" command
+    config.adjust_paths(topology.defaults.paths)
     topology.defaults._original_paths = data.get_box(topology.defaults.paths)
 
   main.transform_setup(topology)
   settings = topology.defaults
   show_dispatch[args.action]['exec'](settings,args)
```

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/__init__.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/attributes.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/attributes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/defaults.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/defaults.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/devices.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/images.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/images.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/module_support.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/module_support.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/modules.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/modules.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/outputs.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/outputs.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/providers.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/providers.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/show_commands/reports.py` & `networklab-1.8.2.dev1/netsim/cli/show_commands/reports.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/status.py` & `networklab-1.8.2.dev1/netsim/cli/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,47 +93,46 @@
 
 def show_lab_instance(iid: Lab_Instance_ID, lab_state: Box) -> None:
   print(f'Lab {iid} in {lab_state.dir}')
   print(f'  status: {lab_state.status}')
   print(f'  provider(s): {",".join(lab_state.providers)}')
   print()
 
-def load_provider_status(p_module: dict, p_status: dict, provider: str, topology: Box) -> None:
-  if not provider in p_module:
-    p_module[provider] = providers._Provider.load(provider,topology.defaults.providers[provider])
+def load_provider_status(p_status: dict, provider: str, topology: Box) -> None:
+  p_module = providers.get_provider_module(topology,provider)
 
   if not provider in p_status:
-    p_status[provider] = p_module[provider].call('get_lab_status') or get_empty_box()
+    p_status[provider] = p_module.call('get_lab_status') or get_empty_box()
 
 def show_lab_nodes(topology: Box) -> None:
   p_status: dict = {}
-  p_module: dict = {}
   rows = []
   heading = [ 'node', 'device', 'image', 'mgmt IPv4', 'connection', 'provider', 'VM/container', 'status']
 
   for n_name,n_data in topology.nodes.items():
     n_ext = outputs_common.adjust_inventory_host(
               node=topology.nodes[n_name],
               defaults=topology.defaults,
               group_vars=True)
 
     n_provider = n_data.get('provider',topology.defaults.provider)
-    load_provider_status(p_module,p_status,n_provider,topology)
+    p_module   = providers.get_provider_module(topology,n_provider)
+    load_provider_status(p_status,n_provider,topology)
 
     row = [ n_data.name, n_data.device, n_data.box, n_data.mgmt.ipv4, n_ext.ansible_connection, n_provider ]
-    wk_name = p_module[n_provider].call('get_node_name',n_name,topology)
+    wk_name = p_module.call('get_node_name',n_name,topology)
     row.append(wk_name)
 
     wk_state = p_status[n_provider].get(wk_name,None) or p_status[n_provider].get(n_name,None)
     row.append(wk_state.status if wk_state else 'Unknown')
     rows.append(row)
 
   for t_name,t_data in topology.tools.items():
     n_provider = 'clab'
-    load_provider_status(p_module,p_status,n_provider,topology)
+    load_provider_status(p_status,n_provider,topology)
 
     wk_name = f'{topology.name}_{t_name}'
     wk_state = p_status[n_provider].get(wk_name,get_empty_box())
 
     row = [ t_name, '(tool)', wk_state.get('image',''), '', 'docker', n_provider, 
             wk_name, wk_state.get('status','Not running') ]
     rows.append(row)
```

### Comparing `networklab-1.8.1.post1/netsim/cli/test.py` & `networklab-1.8.2.dev1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/up.py` & `networklab-1.8.2.dev1/netsim/cli/up.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     external_commands.run_probes(topology.defaults,s_provider)
 
 """
 Start lab topology for a single provider
 """
 def start_provider_lab(topology: Box, pname: str, sname: typing.Optional[str] = None) -> None:
   p_name   = sname or pname
-  p_module = providers._Provider.load(p_name,topology.defaults.providers[p_name])
+  p_module = providers.get_provider_module(topology,p_name)
 
   if sname is not None:
     p_topology = providers.select_topology(topology,p_name)
   else:
     p_topology = topology
 
   status_start_provider(topology,p_name)
@@ -217,15 +217,15 @@
 Recreate secondary configuration file
 """
 def recreate_secondary_config(topology: Box, p_provider: str, s_provider: str) -> None:
   sp_data = topology.defaults.providers[p_provider][s_provider]
   if not sp_data.recreate_config:                                     # Do we need to recreate the config file?
     return
 
-  sp_module  = providers._Provider.load(s_provider,topology.defaults.providers[s_provider])
+  sp_module  = providers.get_provider_module(topology,s_provider)
   s_topology = providers.select_topology(topology,s_provider)         # Create secondary provider subtopology
   filename = sp_data.filename                                         # Get the secondary configuration filename
   print(f"Recreating {filename} configuration file for {s_provider} provider")
   sp_module.create(s_topology,filename)                               # ... and create the new configuration file
 
 """
 Deploy initial configuration
@@ -310,18 +310,20 @@
   if log.QUIET:
     os.environ["ANSIBLE_STDOUT_CALLBACK"] = "selective"
 
   external_commands.LOG_COMMANDS = True
   provider_probes(topology)
 
   p_provider = topology.provider
-  p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
+  p_module = providers.get_provider_module(topology,p_provider)
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
+  providers.validate_images(topology)
+
   status_start_lab(topology)
   if 'err_conflict' in topology.defaults:
     log.fatal(f'race condition, lab instance already running in {topology.defaults.err_conflict}')
 
   if not is_dry_run():
     _status.lock_directory()
```

### Comparing `networklab-1.8.1.post1/netsim/cli/usage.txt` & `networklab-1.8.2.dev1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/cli/validate.py` & `networklab-1.8.2.dev1/netsim/cli/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/common.py` & `networklab-1.8.2.dev1/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/daemons/bird.yml` & `networklab-1.8.2.dev1/netsim/daemons/bird.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,19 @@
   bgp: /etc/bird/bgp.mod.conf
   ospf: /etc/bird/ospf.mod.conf
 clab:
   group_vars:
     netlab_show_command: [ birdc, 'show $@' ]
     docker_shell: bash -il
   image: netlab/bird:latest
+  build: 'https://netlab.tools/netlab/clab/#netlab-clab-build'
 libvirt:                        # Not yet available on libvirt or virtualbox
-  image: 
+  image:
 virtualbox:
-  image: 
+  image:
 features:
   bgp:
     activate_af: true
     local_as: true
     local_as_ibgp: true
   ospf:
     unnumbered: false
```

### Comparing `networklab-1.8.1.post1/netsim/data/__init__.py` & `networklab-1.8.2.dev1/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/data/filemaps.py` & `networklab-1.8.2.dev1/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/data/global_vars.py` & `networklab-1.8.2.dev1/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/data/types.py` & `networklab-1.8.2.dev1/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/data/validate.py` & `networklab-1.8.2.dev1/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/defaults/attributes.yml` & `networklab-1.8.2.dev1/netsim/defaults/attributes.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Core _netlab_ attributes: global, link, interface, node, VLAN, VRF...
-# 
+#
 ---
 global:
   addressing:
   defaults:
   groups:
   links:
   module:
@@ -25,15 +25,15 @@
   version:
 internal:
   input:
   pools: dict
   Provider:
   Plugin:
   message: str
-can_be_false: [ link,interface ]
+can_be_false: [ link, interface ]
 link:
   bandwidth: int
   bridge: id
   disable: bool
   name: str
   prefix:
     type: dict
@@ -44,20 +44,20 @@
   unnumbered: bool
   interfaces:
   mtu: { type: int, min_value: 64, max_value: 65535 }
   vlan_name: id
 link_internal:
   linkindex: int
   parentindex: int
-link_no_propagate: [ prefix,interfaces,gateway ]
+link_no_propagate: [ prefix, interfaces, gateway ]
 # Do not propagate VLAN attributes to node interfaces -- see #575
 # Also: do not propagate DHCP attributes from links to interfaces
 link_module_no_propagate: [ vlan, dhcp ]
 interface:
-  node: id
+  node: node_id
   ipv4: { type: ipv4, use: interface }
   ipv6: { type: ipv6, use: interface }
   ifindex: int
   ifname: str
 node:
   name: str                                         # Validity of node name is checked in the nodes module
   interfaces: list
@@ -99,15 +99,15 @@
   allocation: { type: str, valid_values: [ p2p, sequential, id_based ] }
 group:
   members:
     type: list
     _subtype: id
   vars: dict
   config: list
-  node_data: 
+  node_data:
     type: dict
     true_value: {}
   device: device
   module: list
 _v_entry:                  # Validation entry
   _description: Single network validation test (an entry in the validate dictionary)
   description: str
```

### Comparing `networklab-1.8.1.post1/netsim/defaults/hints.yml` & `networklab-1.8.2.dev1/netsim/defaults/hints.yml`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,18 @@
   irb_group: >
     All VLANs that are part of a VRF using asymmetric IRB have to be present on all nodes
     using that VRF. The easiest way to achieve that is to create a group with all
     participating nodes and list VLANs in the 'vlans' attribute of that group
   node_bundle: |
     evpn.bundle attribute can be used only in global VRF definition
   asn: >
-    You could use 'bgp.as' parameter to specify the global AS. Otherwise, specify
-    the global AS used by EVPN in 'vrf.as' parameter if you use VRFs, or in
-    'evpn.as' parameter if you use EVPN in bridging-only scenarios.
+    You could use the global 'bgp.as' parameter to specify the AS to use in EVPN
+    route targets. 'bgp.as' specified on individual nodes or groups will not work. You
+    can also specify the global AS used by EVPN in 'vrf.as' parameter if you use
+    VRFs, or in 'evpn.as' parameter if you use EVPN in bridging-only scenarios.
 bgp:
   igp: >
     Add a supported IGP (ospf, isis, eigrp) to the list of modules.
 report:
   source: >
     A report can be specified in a file with .j2 suffix within 'reports' subdirectory in
     package-, system-, user- or current directory. You can also specify a report in a
```

### Comparing `networklab-1.8.1.post1/netsim/defaults/paths.yml` & `networklab-1.8.2.dev1/netsim/defaults/paths.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 ---
 validate:                       # Search path for validation plugins
 - topology:validate
 - validate
+- "~/.netlab/validate"
+- "/etc/netlab/validate"
 - package:validate
 
+plugin:                         # Search path for transformation plugins
+- "."
+- "topology:"
+- "~/.netlab"
+- "/etc/netlab"
+- "package:extra"
+
 custom:                         # Custom configuration templates
   dirs:                         # ... search directories
   - "topology:"
   - "."
   - "~/.netlab"
+  - "/etc/netlab"
   - "package:extra"
   files:                        # ... potential file names
   - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '-' + node_provider + '.j2' }}"
   - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
   - "{{ custom_config + '/' + inventory_hostname + '.j2' }}"
   - "{{ custom_config + '/' + inventory_hostname + '.cfg' }}"
   - "{{ custom_config + '/' + netlab_device_type + '-' + node_provider + '.j2' }}"
@@ -35,14 +45,15 @@
   - "{{ custom_config }}/deploy.yml"
 
 deploy:
   dirs:
   - "topology:tasks"
   - "tasks"
   - "~/.netlab/tasks"
+  - "/etc/netlab/tasks"
   - "package:ansible/tasks"
   tasks_generic:
   - "deploy-config/{{ netlab_device_type }}-{{ node_provider }}.yml"
   - "deploy-config/{{ netlab_device_type }}.yml"
   - "deploy-config/{{ ansible_network_os }}-{{ node_provider }}.yml"
   - "deploy-config/{{ ansible_network_os }}.yml"
   files:
@@ -56,14 +67,15 @@
   - "deploy-config/{{ ansible_network_os }}.yml"
 
 templates:
   dirs:
   - "topology:templates"
   - "templates"
   - "~/.netlab/templates"
+  - "/etc/netlab/templates"
   - "package:ansible/templates"
   - "package:daemons"
 
 t_files:
   files:
   - "{{config_module}}/{{netlab_device_type}}-{{provider|default(netlab_provider)}}.j2"
   - "{{config_module}}/{{netlab_device_type}}.j2"
@@ -74,20 +86,22 @@
   - "{{netlab_device_type}}/{{config_module}}.j2"
 
 ready:
   dirs:
   - "topology:readiness-check"
   - "readiness-check"
   - "~/.netlab/readiness-check"
+  - "/etc/netlab/readiness-check"
   - "package:ansible/tasks/readiness-check"
   files:
   - "{{netlab_device_type}}-{{provider|default(netlab_provider)}}.yml"
   - "{{netlab_device_type}}.yml"
   - "{{ansible_network_os}}-{{provider|default(netlab_provider)}}.yml"
   - "{{ansible_network_os}}.yml"
 
 collect:
   dirs:
   - "topology:fetch-config"
   - "fetch-config"
   - "~/.netlab/fetch-config"
+  - "/etc/netlab/fetch-config"
   - "package:ansible/tasks/fetch-config"
```

### Comparing `networklab-1.8.1.post1/netsim/devices/__init__.py` & `networklab-1.8.2.dev1/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/arubacx.py` & `networklab-1.8.2.dev1/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/arubacx.yml` & `networklab-1.8.2.dev1/netsim/devices/arubacx.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 interface_name: 1/1/{ifindex}
 mgmt_if: mgmt
 loopback_interface_name: "loopback {ifindex}"
 tunnel_interface_name: "tunnel {ifindex}"
 ifindex_offset: 1
 libvirt:
   image: aruba/cx
+  build: https://netlab.tools/labs/arubacx/
   create:
     virt-install --connect=qemu:///system --name=vm_box --arch=x86_64 --cpu host --vcpus=2 --hvm
       --ram=4096 --network=network:vagrant-libvirt,model=virtio --graphics none --import
       --disk path=vm.qcow2,format=qcow2,bus=ide
 clab:
   image: vrnetlab/vr-aoscx:20231110145644
+  build: https://containerlab.dev/manual/kinds/vr-aoscx/
   mtu: 1500
   node:
     kind: vr-aoscx
   interface:
     name: eth{ifindex}
 group_vars:
   ansible_network_os: arubanetworks.aoscx.aoscx
```

### Comparing `networklab-1.8.1.post1/netsim/devices/asav.py` & `networklab-1.8.2.dev1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/asav.yml` & `networklab-1.8.2.dev1/netsim/devices/asav.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Cisco ASAv
 interface_name: GigabitEthernet0/{ifindex}
 ifindex_offset: 0
 mgmt_if: Management0/0
 group_vars:
   ansible_user: vagrant
   ansible_ssh_pass: vagrant1
@@ -12,14 +13,16 @@
 external:
   image: none
 features:
   bgp: True
   isis: True
 libvirt:
   image: cisco/asav
-  create:
-    virt-install --connect=qemu:///system --network network=vagrant-libvirt,model=virtio --name=vm_box
-      --cpu host --arch=x86_64 --machine=pc-1.0 --vcpus=1 --ram=2048 --os-type=linux --noacpi
-      --virt-type=kvm --watchdog i6300esb,action=reset
-      --disk path=vm.qcow2,format=qcow2,device=disk,bus=virtio,cache=writethrough
-      --disk path=bootstrap.iso,format=iso,device=cdrom --graphics none --import
+  create_template: asav.xml.j2
+  build: https://netlab.tools/labs/asav/
+  #  create:
+  #    virt-install --connect=qemu:///system --network network=vagrant-libvirt,model=virtio --name=vm_box
+  #      --cpu host --arch=x86_64 --machine=pc-1.0 --vcpus=1 --ram=2048 --os-type=linux --noacpi
+  #      --virt-type=kvm --watchdog i6300esb,action=reset
+  #      --disk path=vm.qcow2,format=qcow2,device=disk,bus=virtio,cache=writethrough
+  #      --disk path=bootstrap.iso,format=iso,device=cdrom --graphics none --import
   create_iso: asav
```

### Comparing `networklab-1.8.1.post1/netsim/devices/csr.yml` & `networklab-1.8.2.dev1/netsim/devices/csr.yml`

 * *Files 23% similar despite different names*

```diff
@@ -21,11 +21,15 @@
     svi_interface_name: BDI{vlan}
     mixed_trunk:
     native_routed:
     subif_name:
   vxlan: true
 libvirt:
   image: cisco/csr1000v
+  build: https://netlab.tools/labs/csr/
   create_template:
   create:
-    virt-install --connect=qemu:///system --name=vm_box --os-variant=rhel4.0 --arch=x86_64 --cpu host --vcpus=1 --hvm
-      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+    virt-install --connect=qemu:///system --name=vm_box --os-variant=rhel4.0
+      --arch=x86_64 --cpu host --vcpus=1 --hvm
+      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2
+      --network=network:vagrant-libvirt,model=virtio
+      --graphics none --import
```

### Comparing `networklab-1.8.1.post1/netsim/devices/cumulus.yml` & `networklab-1.8.2.dev1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/cumulus_nvue.yml` & `networklab-1.8.2.dev1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/dellos10.yml` & `networklab-1.8.2.dev1/netsim/devices/dellos10.yml`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,30 @@
     svi_interface_name: virtual-network{vlan}
   vrf:
     ospfv2: True
     bgp: True
   vxlan: true
 clab:
   image: vrnetlab/vr-ftosv
+  build: https://containerlab.dev/manual/kinds/vr-ftosv/
   node:
     kind: vr-ftosv
   interface:
     name: eth{ifindex}
   mtu: 1500
 libvirt:
   image: dell/os10
+  build: https://netlab.tools/labs/dellos10/
   create:
     virt-install --connect=qemu:///system --name=vm_box --arch=x86_64 --cpu host --vcpus=2 --hvm
       --ram=2048 --network=network:vagrant-libvirt,model=virtio --graphics none --import
       --disk path=vm.qcow2,format=qcow2,bus=sata
       --disk path=hdb_OS10-installer.qcow2,format=qcow2,bus=virtio
       --disk path=hdc_OS10-platform.qcow2,format=qcow2,bus=virtio
+  pre_install: dellos10
 group_vars:
   ansible_network_os: dellos10
   ansible_connection: network_cli
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
 external:
   image: none
```

### Comparing `networklab-1.8.1.post1/netsim/devices/eos.py` & `networklab-1.8.2.dev1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/eos.yml` & `networklab-1.8.2.dev1/netsim/devices/eos.yml`

 * *Files 11% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     svi_interface_name: Vlan{vlan}
   vrf:
     ospfv2: True
     ospfv3: True
     bgp: True
   vxlan: true
 clab:
+  build: https://netlab.tools/labs/ceos/
   interface:
     name: et{ifindex}
   node:
     kind: ceos
     env:
       INTFTYPE: et
       CLAB_MGMT_VRF: management
@@ -78,14 +79,15 @@
   image: ceos:4.31.2F
   group_vars:
     ansible_user: admin
     ansible_ssh_pass: admin
     ansible_become: yes
     ansible_become_method: enable
 libvirt:
+  build: https://netlab.tools/labs/eos/
   image: arista/veos
   create_template: eos.xml.j2
 # create: |
 #   virt-install --connect=qemu:///system --name=vm_box --os-type=linux
 #     --arch=x86_64 --cpu host --vcpus=2 --hvm
 #     --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2
 #     --network=network:vagrant-libvirt,model=virtio --graphics none --import
```

### Comparing `networklab-1.8.1.post1/netsim/devices/fortios.yml` & `networklab-1.8.2.dev1/netsim/devices/fortios.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/frr.yml` & `networklab-1.8.2.dev1/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/iosv.py` & `networklab-1.8.2.dev1/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/iosv.yml` & `networklab-1.8.2.dev1/netsim/devices/iosv.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   ansible_become_password: vagrant
   ansible_network_os: ios
   ansible_connection: network_cli
   netlab_device_type: ios
   netlab_initial: always
 libvirt:
   image: cisco/iosv
+  build: https://netlab.tools/labs/iosv/
   create_template: iosv.xml.j2
 #      create:
 #        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=1
 #          --noacpi --machine=pc-1.0 --virt-type=kvm --watchdog i6300esb,action=reset --ram=512
 #          --disk path=vm.qcow2,bus=virtio,format=qcow2,cache=writethrough
 #          --network=network:vagrant-libvirt,model=e1000 --graphics none --import
 virtualbox:
```

### Comparing `networklab-1.8.1.post1/netsim/devices/iosxr.yml` & `networklab-1.8.2.dev1/netsim/devices/iosxr.yml`

 * *Files 13% similar despite different names*

```diff
@@ -25,25 +25,27 @@
       network: True
   bgp:
     activate_af: True
 external:
   image: none
 libvirt:
   image: cisco/iosxr
+  build: https://netlab.tools/labs/iosxr/
   create:
     virt-install --connect=qemu:///system --network network=vagrant-libvirt,model=e1000 --name=vm_box
       --cpu host --arch=x86_64 --vcpus=2 --ram=8192
       --virt-type=kvm
       --disk path=vm.qcow2,format=qcow2,device=disk,bus=ide
       --graphics none --import
 clab:
   node:
     kind: cisco_xrd
     runtime: docker
   mgmt_if: MgmtEth0/RP0/CPU0/0
   interface:
     name: Gi0-0-0-{ifindex}
   image: ios-xr/xrd-control-plane:7.11.1
+  build: https://containerlab.dev/manual/kinds/xrd/
   group_vars:
     ansible_user: clab
     ansible_ssh_pass: clab@123
     ansible_become_password: clab@123
```

### Comparing `networklab-1.8.1.post1/netsim/devices/junos.py` & `networklab-1.8.2.dev1/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/junos.yml` & `networklab-1.8.2.dev1/netsim/devices/junos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/linux.py` & `networklab-1.8.2.dev1/netsim/devices/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/linux.yml` & `networklab-1.8.2.dev1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/none.yml` & `networklab-1.8.2.dev1/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/nxos.yml` & `networklab-1.8.2.dev1/netsim/devices/nxos.yml`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,11 @@
     ospfv2: True
     bgp: True
   vxlan: true
 
 libvirt:
   create_template: nxos.xml.j2
   image: cisco/nexus9300v
+  build: https://netlab.tools/labs/nxos/
 external:
   image: none
 graphite.icon: nexus5000
```

### Comparing `networklab-1.8.1.post1/netsim/devices/routeros.yml` & `networklab-1.8.2.dev1/netsim/devices/vyos.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,60 @@
 ---
-description: Mikrotik RouterOS version 6
-interface_name: ether{ifindex}
-mgmt_if: ether1
-ifindex_offset: 2
+description: VyOS VM/container
+interface_name: eth{ifindex}
+loopback_interface_name: "dum{ifindex}"
+mgmt_if: eth0
 libvirt:
-  image: mikrotik/chr
+  image: vyos/current
 group_vars:
-  ansible_network_os: routeros
-  ansible_connection: network_cli
-  ansible_user: admin
-  ansible_ssh_pass: admin
+  ansible_network_os: vyos
+  ansible_connection: paramiko
+  ansible_user: vyos
+  ansible_ssh_pass: vyos
+  docker_shell: su - vyos
 features:
-  bgp: true
+  initial:
+    ipv4:
+      unnumbered: true
+    ipv6:
+      lla: True
+  bfd: true
+  bgp:
+    activate_af: true
+    ipv6_lla: true
+    local_as: true
+    rfc8950: true
+    vrf_local_as: true
+  evpn:
+    asymmetrical_irb: true
+    irb: true
+  gateway:
+    protocol: [ vrrp ]
+  isis: true
   mpls:
     ldp: true
     vpn: true
-  ospf: true
+  ospf:
+    unnumbered: true
   vlan:
-    model: router
-    svi_interface_name: bridge{vlan}
-    subif_name: "{ifname}-{vlan.access_id}"
-    mixed_trunk: true
+    model: l3-switch
+    svi_interface_name: "br0.{vlan}"
+    subif_name: "{ifname}.{vlan.access_id}"
     native_routed: true
   vrf:
     ospfv2: True
     bgp: True
+  vxlan:
+    vtep6: true
+clab:
+  image: ghcr.io/sysoleg/vyos-container
+  mtu: 1500
+  node:
+    kind: linux
+    binds:
+      '/lib/modules': '/lib/modules'
+  group_vars:
+    ansible_connection: docker
+    ansible_user: vyos
 external:
   image: none
 graphite.icon: router
```

### Comparing `networklab-1.8.1.post1/netsim/devices/routeros7.yml` & `networklab-1.8.2.dev1/netsim/devices/routeros7.yml`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 description: Mikrotik RouterOS version 7
 interface_name: ether{ifindex}
 mgmt_if: ether1
 loopback_interface_name: loopback{ifindex}
 ifindex_offset: 2
 libvirt:
   image: mikrotik/chr7
+  build: https://netlab.tools/labs/routeros7/
   create:
     virt-install --connect=qemu:///system --name=vm_box --arch=x86_64 --cpu host --vcpus=2 --hvm
       --ram=256 --network=network:vagrant-libvirt,model=virtio --graphics none --import
       --disk path=vm.qcow2,format=qcow2,bus=ide
 group_vars:
   ansible_network_os: routeros
   ansible_connection: network_cli
@@ -28,14 +29,15 @@
     subif_name: "{ifname}-{vlan.access_id}"
     native_routed: true
   vrf:
     ospfv2: True
     bgp: True
 clab:
   image: vrnetlab/vr-routeros:7.6
+  build: https://containerlab.dev/manual/kinds/vr-ros/
   node:
     kind: vr-ros
   interface:
     name: eth{ifindex-1}
 external:
   image: none
 graphite.icon: router
```

### Comparing `networklab-1.8.1.post1/netsim/devices/srlinux.yml` & `networklab-1.8.2.dev1/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/sros.yml` & `networklab-1.8.2.dev1/netsim/devices/sros.yml`

 * *Files 14% similar despite different names*

```diff
@@ -61,18 +61,19 @@
   srv6: True
   vrf:
     ospfv2: True
     bgp: True
 
 clab:
   image: vrnetlab/vr-sros
+  build: https://containerlab.dev/manual/kinds/vr-sros/
   mtu: 1500
   node:
     kind: vr-sros
-    type: sr-1 # By default emulate SR-1
+    type: sr-1                # By default emulate SR-1
     license: /Projects/SR_OS_VSR-SIM_license.txt
   interface:
     name: eth{ifindex}
   group_vars:
     sros_grpc_port: 57400
 external:
   image: none
```

### Comparing `networklab-1.8.1.post1/netsim/devices/unknown.py` & `networklab-1.8.2.dev1/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/vmx.py` & `networklab-1.8.2.dev1/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/vptx.py` & `networklab-1.8.2.dev1/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/vptx.yml` & `networklab-1.8.2.dev1/netsim/devices/vptx.yml`

 * *Files 17% similar despite different names*

```diff
@@ -13,19 +13,21 @@
     svi_interface_name: irb.{vlan}
     subif_name: "{ifname}.{vlan.access_id}"
     mixed_trunk: true
     native_routed: true
 
 libvirt:
   image: juniper/vptx
+  build: https://netlab.tools/labs/vptx/
   pre_install: vptx
   create_template: vptx.xml.j2
 
 clab:
   image: vrnetlab/vr-vjunosevolved:23.2R1-S1.8-EVO
+  build: https://containerlab.dev/manual/kinds/vr-vjunosevolved/
   mtu: 1500
   node:
     kind: juniper_vjunosevolved
   interface:
     name: eth{ifindex+1}
   group_vars:
     ansible_user: admin
```

### Comparing `networklab-1.8.1.post1/netsim/devices/vsrx.py` & `networklab-1.8.2.dev1/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/devices/vsrx.yml` & `networklab-1.8.2.dev1/netsim/devices/vsrx.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Juniper vSRX 3.0
 parent: junos
 group_vars:
   netlab_device_type: vsrx
 
 features:
   vlan:
@@ -10,21 +11,26 @@
     mixed_trunk: false
     native_routed: true
 
 virtualbox:
   image: juniper/vsrx3
 libvirt:
   image: juniper/vsrx3
+  build: https://netlab.tools/labs/vsrx/
   create_iso: vsrx
   create:
-    virt-install --connect=qemu:///system --name=vm_box --os-variant=freebsd10.0 --arch=x86_64 --cpu host --vcpus=2 --hvm
-      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --disk path=bootstrap.iso,device=cdrom,bus=ide
-      --boot hd --network=network:vagrant-libvirt,model=virtio --graphics none --import
+    virt-install --connect=qemu:///system --name=vm_box --os-variant=freebsd10.0
+      --arch=x86_64 --cpu host --vcpus=2 --hvm
+      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2
+      --disk path=bootstrap.iso,device=cdrom,bus=ide
+      --boot hd --network=network:vagrant-libvirt,model=virtio
+      --graphics none --import
 clab:
   image: vrnetlab/vr-vsrx:23.1R1.8
+  build: https://containerlab.dev/manual/kinds/vr-vsrx/
   node:
     kind: vr-vsrx
   interface:
     name: eth{ifindex+1}
   group_vars:
     ansible_user: admin
     ansible_ssh_pass: "admin@123"
```

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.domain/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.domain/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.originate/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.originate/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_aoscx.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_aoscx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_ios.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/_route_map_ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/arubacx.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/cumulus.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/defaults.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/eos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/frr.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/ios.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/simple-attributes.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/simple-attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.policy/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.policy/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/_sample_bfd_template.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/_sample_bfd_template.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/arubacx.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/cumulus.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/cumulus.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/bin/bash
 #
 {% macro ebgp_session(n,af) -%}
+{%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
 {%   if n.password is defined %}
-  neighbor {{ n[af] }} password {{ n.password }}
+  neighbor {{ peer }} password {{ n.password }}
 {%   endif %}
 {%   if n.gtsm is defined %}
-  neighbor {{ n[af] }} ttl-security hops {{ n.gtsm }}
+  neighbor {{ peer }} ttl-security hops {{ n.gtsm }}
 {%   endif %}
 {%   if n.timers is defined %}
-  neighbor {{ n[af] }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
+  neighbor {{ peer }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
 {%   endif %}
 {%   if n.bfd|default(False) %}
-  neighbor {{ n[af] }} bfd
+  neighbor {{ peer }} bfd
 {%   endif %}
 {%   if n.passive|default(False) %}
-  neighbor {{ n[af] }} passive
+  neighbor {{ peer }} passive
 {%   endif %}
 {%- endmacro %}
 {#
 
 #}
 {% macro ebgp_neighbor(n,af) -%}
 {%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
@@ -43,14 +44,15 @@
 #}
 set -e
 cat >/tmp/config <<CONFIG
 !
 router bgp {{ bgp.as }}
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
+{%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
 {{     ebgp_session(n,af) }}
 {%   endfor %}
 {% endfor %}
 !
 ! Global address families
 {% for af in ['ipv4','ipv6'] if af in bgp %}
 {%   for n in bgp.neighbors if n[af] is defined %}
```

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/default-originate.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/defaults.yml` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/eos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/frr.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/frr.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/bin/bash
 #
 {% macro ebgp_session(n,af) -%}
+{%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
 {%   if n.password is defined %}
-  neighbor {{ n[af] }} password {{ n.password }}
+  neighbor {{ peer }} password {{ n.password }}
 {%   endif %}
 {%   if n.gtsm is defined %}
-  neighbor {{ n[af] }} ttl-security hops {{ n.gtsm }}
+  neighbor {{ peer }} ttl-security hops {{ n.gtsm }}
 {%   endif %}
 {%   if n.timers is defined %}
-  neighbor {{ n[af] }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
+  neighbor {{ peer }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
 {%   endif %}
 {%   if n.bfd|default(False) %}
-  neighbor {{ n[af] }} bfd
+  neighbor {{ peer }} bfd
 {%   endif %}
 {%   if n.passive|default(False) %}
-  neighbor {{ n[af] }} passive
+  neighbor {{ peer }} passive
 {%   endif %}
 {%- endmacro %}
 {#
 
 #}
 {% macro ebgp_neighbor(n,af) -%}
 {%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
@@ -43,14 +44,15 @@
 #}
 set -e
 cat >/tmp/config <<CONFIG
 !
 router bgp {{ bgp.as }}
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
+{%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
 {{     ebgp_session(n,af) }}
 {%   endfor %}
 {% endfor %}
 !
 ! Global address families
 {% for af in ['ipv4','ipv6'] if af in bgp %}
 {%   for n in bgp.neighbors if n[af] is defined %}
```

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/ios.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/junos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/nxos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/nxos.j2`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 {%   endif %}
 {%   if n.passive|default(False) %}
       transport connection-mode passive
 {%   endif %}
 {%   if n.remove_private_as|default([]) %}
 {%     set rpa = { 'on': '', 'replace': 'replace-as', 'all': 'all' } %}
 {%     for rpo in n.remove_private_as if rpo in rpa %}
-      neighbor {{ n[af] }} remove-private-as {{ rpa[rpo] }}
+      remove-private-as {{ rpa[rpo] }}
 {%     endfor %}
 {%   endif %}
 {%- endmacro %}
 !
 {% macro ebgp_neighbor(n,af) -%}
 {%     if n.allowas_in is defined %}
         allowas-in {{ n.allowas_in }}
 {%     endif %}
 {%     if n.as_override|default(False) %}
+        disable-peer-as-check
         as-override
 {%     endif %}
 {%     if n.default_originate|default(False) %}
         default-originate
 {%     endif %}
 {%- endmacro %}
 !
```

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/routeros7.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/sros.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/bgp.session/vyos.j2` & `networklab-1.8.2.dev1/netsim/extra/bgp.session/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/arubacx.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/defaults.yml` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/eos.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/frr.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ios.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/sros.j2` & `networklab-1.8.2.dev1/netsim/extra/ebgp.multihop/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/fabric/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/fabric/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/multilab/__init__.py` & `networklab-1.8.2.dev1/netsim/extra/multilab/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/proxy-arp/plugin.py` & `networklab-1.8.2.dev1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.8.2.dev1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/extra/proxy-arp/sros.j2` & `networklab-1.8.2.dev1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/ansible.sh` & `networklab-1.8.2.dev1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/containerlab.sh` & `networklab-1.8.2.dev1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/grpc.sh` & `networklab-1.8.2.dev1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/arubacx.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/dellos10.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-Creating initial configuration for ArubaOS-CX
+Creating initial configuration for Dell OS10
 =============================================
 
-* Wait for the 'login' prompt
-* Login as 'admin' (no password)
-* Set the new 'admin' password as 'admin'
+* Wait for the 'login' prompt, and then wait again some more minutes
+* Login as 'admin' (password: 'admin')
+* Disable zero-touch ('ztd cancel')
+* Enter configuration mode ('configure')
 * Copy-paste the following configuration
 
-=============================================
+NOTE: the management traffic is isolated in a dedicated management VRF (management).
 
-configure
-!
-user netlab group administrators password plaintext netlab
-user netlab authorized-key ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEA6NF8iallvQVp22WDkTkyrtvp9eWW6A8YVr+kz4TjGYe7gHzIw+niNltGEFHzD8+v1I2YJ6oXevct1YeS0o9HZyN1Q9qgCgzUFtdOKLv6IedplqoPkcmF0aYet2PkEDo3MlTBckFXPITAMzF8dJSIFo9D8HfdOV0IAdx4O7PtixWKn5y2hMNG0zQPyUecp4pzC6kivAIhyfHilFR61RGL+GPXQ2MWZWFYbAGjyiYJnAmCP3NOTd0jMZEnDkbUvxhMmBYSdETk1rRgm+R4LOzFUGaHqHDLKLX+FIPKcF96hrucXzcWyLbIbEgE98OHlnVYCzRdK8jlqm8tehUc9c9WhQ==
+===============
+*** WARNING ***
+===============
+To disable zero-touch (ZTD) a full reload is required after the first configuration.
+
+=============================================
 !
-ssh server vrf mgmt
-https server vrf mgmt
+interface mgmt1/1/1
+  no ip address dhcp
+  no ipv6 address
+  exit
+!
+ip vrf management
+  interface management
+  exit
 !
-interface mgmt
+interface mgmt1/1/1
   no shutdown
-  ip dhcp
+  ip address dhcp
+  exit
 !
-ntp vrf mgmt
+service simple-password
+username vagrant password vagrant role sysadmin priv-lvl 15
+username vagrant sshkey "ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEA6NF8iallvQVp22WDkTkyrtvp9eWW6A8YVr+kz4TjGYe7gHzIw+niNltGEFHzD8+v1I2YJ6oXevct1YeS0o9HZyN1Q9qgCgzUFtdOKLv6IedplqoPkcmF0aYet2PkEDo3MlTBckFXPITAMzF8dJSIFo9D8HfdOV0IAdx4O7PtixWKn5y2hMNG0zQPyUecp4pzC6kivAIhyfHilFR61RGL+GPXQ2MWZWFYbAGjyiYJnAmCP3NOTd0jMZEnDkbUvxhMmBYSdETk1rRgm+R4LOzFUGaHqHDLKLX+FIPKcF96hrucXzcWyLbIbEgE98OHlnVYCzRdK8jlqm8tehUc9c9WhQ== vagrant insecure public key"
 !
 end
-!
 write memory
 !
-! reload cycle is required
+! reload cycle is required to disable ZTD
 !
-boot system
+reload
 !
-
 =============================================
 
-* After the reboot, check that the management interface is up (sometimes you may need to apply the config and reboot twice)
+* Wait until the reload is completed
 * Disconnect from console (ctrl-] usually works).
-* Shutdown the VM, if needed
```

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/asav/day0-config` & `networklab-1.8.2.dev1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/csr.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/eos.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/eos.txt`

 * *Files 5% similar despite different names*

```diff
@@ -67,7 +67,9 @@
 no user vagrant shell
 !
 end
 =============================================
 
 * Save the configuration with 'wr mem'
 * Poweroff the VM with 'bash sudo poweroff'
+* If the device starts reloading instead of shutting down, disconnect
+  from the console (ctrl-] usually works).
```

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/eos.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/iosv.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/iosxr.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/nxos.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/vptx.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,11 +6,14 @@
 
 * Login with username 'vagrant' and password 'Vagrant'
   (it might take a while for the username to be recognized)
 * Verify that the VM got a management IP address with 
   'show interfaces terse | match re0'
 * Verify that the FPC 0 is online with 
   'show chassis fpc'
-* Shut down the VM with 'request system power-off' (confirm with 'yes')
+* Shut down the VM with 'request system power-off', confirm with 'yes'.
+  It might take a while for the VM to power off.
+* If the device starts rebooting instead of shutting down, disconnect
+  from the console (ctrl-] usually works).
 
 NOTES:
 * The management traffic is isolated in a dedicated management VRF (mgmt_junos).
```

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.8.2.dev1/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.8.2.dev1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt/vsrx.txt` & `networklab-1.8.2.dev1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/libvirt.sh` & `networklab-1.8.2.dev1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/install/ubuntu.sh` & `networklab-1.8.2.dev1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/__init__.py` & `networklab-1.8.2.dev1/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/_dataplane.py` & `networklab-1.8.2.dev1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/_routing.py` & `networklab-1.8.2.dev1/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/bfd.py` & `networklab-1.8.2.dev1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/bfd.yml` & `networklab-1.8.2.dev1/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/bgp.py` & `networklab-1.8.2.dev1/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/bgp.yml` & `networklab-1.8.2.dev1/netsim/modules/bgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/dhcp.py` & `networklab-1.8.2.dev1/netsim/modules/dhcp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/dhcp.yml` & `networklab-1.8.2.dev1/netsim/modules/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/eigrp.py` & `networklab-1.8.2.dev1/netsim/modules/eigrp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/evpn.py` & `networklab-1.8.2.dev1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/evpn.yml` & `networklab-1.8.2.dev1/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/gateway.py` & `networklab-1.8.2.dev1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/gateway.yml` & `networklab-1.8.2.dev1/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/isis.py` & `networklab-1.8.2.dev1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/isis.yml` & `networklab-1.8.2.dev1/netsim/modules/isis.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/mpls.py` & `networklab-1.8.2.dev1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/mpls.yml` & `networklab-1.8.2.dev1/netsim/modules/mpls.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/ospf.py` & `networklab-1.8.2.dev1/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/ospf.yml` & `networklab-1.8.2.dev1/netsim/modules/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/srv6.py` & `networklab-1.8.2.dev1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/vlan.py` & `networklab-1.8.2.dev1/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/vlan.yml` & `networklab-1.8.2.dev1/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/vrf.py` & `networklab-1.8.2.dev1/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/vrf.yml` & `networklab-1.8.2.dev1/netsim/modules/vrf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/vxlan.py` & `networklab-1.8.2.dev1/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/modules/vxlan.yml` & `networklab-1.8.2.dev1/netsim/modules/vxlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/__init__.py` & `networklab-1.8.2.dev1/netsim/outputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,13 +61,13 @@
     return 'templates/outputs/' + self.output + "/" + fmtname + ".j2"
 
   def get_output_name(self, fname: str, topology: Box) -> typing.Optional[str]:
     if fname:
       return fname
 
     if self.settings:
-      return self.settings.filename
+      return self.settings.get('filename',None)
 
     return None
 
   def write(self, topology: Box) -> None:
     log.fatal('someone called the "write" method of TopologyOutput abstract class')
```

### Comparing `networklab-1.8.1.post1/netsim/outputs/ansible.py` & `networklab-1.8.2.dev1/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/common.py` & `networklab-1.8.2.dev1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/d2.py` & `networklab-1.8.2.dev1/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/d2.yml` & `networklab-1.8.2.dev1/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/devices.py` & `networklab-1.8.2.dev1/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/graph.py` & `networklab-1.8.2.dev1/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/graphite.py` & `networklab-1.8.2.dev1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/provider.py` & `networklab-1.8.2.dev1/netsim/outputs/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 from box import Box
 
 from . import _TopologyOutput,check_writeable
 from .. import providers
 from ..augment import nodes
 from ..utils import log,strings
 
-def get_provider_module(topology: Box, provider: str) -> providers._Provider:
-  return providers._Provider.load(provider,topology.defaults.providers[provider])
-
 def write_provider_file(topology: Box, provider: str, filename: typing.Optional[str]) -> None:
-  p_module = get_provider_module(topology,provider)
+  p_module = providers.get_provider_module(topology,provider)
   p_module.create(topology,filename)
 
 class ProviderConfiguration(_TopologyOutput):
 
   DESCRIPTION :str = 'Create virtualization provider configuration file(s)'
 
   def write(self, topology: Box) -> None:
@@ -30,15 +27,15 @@
 
     if self.format:
       log.error('Specified output format(s) %s ignored' % self.format,log.IncorrectValue,'provider')
 
     # Creates a "ghost clean" topology after transformation
     # (AKA, remove unmanaged devices)
     topology = nodes.ghost_buster(topology)
-    p_module = get_provider_module(topology,topology.provider)
+    p_module = providers.get_provider_module(topology,topology.provider)
     providers.mark_providers(topology)
     p_module.call('pre_output_transform',topology)
     write_provider_file(providers.select_topology(topology,topology.provider),topology.provider,filename)
 
     for subprovider in topology[topology.provider].providers.keys():  # Iterate over subproviders
       strings.print_colored_text('[INFO]    ','bright_cyan',alt_txt=None)
       print(f"Creating configuration file for secondary provider {subprovider}")
```

### Comparing `networklab-1.8.1.post1/netsim/outputs/report.py` & `networklab-1.8.2.dev1/netsim/outputs/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/tools.py` & `networklab-1.8.2.dev1/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/outputs/yaml.py` & `networklab-1.8.2.dev1/netsim/outputs/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from . import _TopologyOutput,check_writeable
 
 class YAML(_TopologyOutput):
 
   DESCRIPTION :str = 'Inspect transformed data in YAML format'
 
   def write(self, topo: Box) -> None:
-    outfile = self.settings.filename or '-'
+    outfile = self.settings.get('filename',None) or '-'
     modname = type(self).__name__
 
     if hasattr(self,'filenames'):
       outfile = self.filenames[0]
       if len(self.filenames) > 1:
         log.error('Extra output filename(s) ignored: %s' % str(self.filenames[1:]),log.IncorrectValue,modname)
```

### Comparing `networklab-1.8.1.post1/netsim/providers/__init__.py` & `networklab-1.8.2.dev1/netsim/providers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,17 @@
         n.box = image_spec[0]
         if len(image_spec) > 1:
           n.box_version = image_spec[1]
 
   def transform_node_images(self, topology: Box) -> None:
     pass
 
+  def validate_node_image(self, node: Box, topology: Box) -> None:
+    pass
+
   def transform(self, topology: Box) -> None:
     self.transform_node_images(topology)
     if "processor" in topology.defaults:
       return
     else:
       processor_name = ""
       if platform.system() == "Windows":
@@ -318,7 +321,19 @@
 
   for fp,fstart in fmap.items():                                # Iterate over forwarded ports
     if not fp in pmap:                                          # Is the port we're trying to forward known to netlab?
       continue                                                  # ... nope, bad luck, move on
     node_fp.append([ fstart + node.id, pmap[fp]])               # Append [host,device] port mapping
 
   return node_fp
+
+"""
+validate_images -- check the images used by individual nodes against provider image repo
+"""
+
+def validate_images(topology: Box) -> None:
+  p_cache: dict = {}
+
+  for n_data in topology.nodes.values():
+    execute_node('validate_node_image',n_data,topology)
+
+  log.exit_on_error()
```

### Comparing `networklab-1.8.1.post1/netsim/providers/clab.py` & `networklab-1.8.2.dev1/netsim/providers/clab.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 from box import Box
 
 from . import _Provider,get_forwarded_ports
 from ..utils import log
 from ..data import filemaps, get_empty_box
 from ..cli import is_dry_run,external_commands
+from ..augment import devices
 
 def list_bridges( topology: Box ) -> typing.Set[str]:
   return { l.bridge for l in topology.links if l.bridge and l.node_count != 2 and not 'external_bridge' in l.clab }
 
 def use_ovs_bridge( topology: Box ) -> bool:
     return topology.defaults.providers.clab.bridge_type == "ovs-bridge"
 
@@ -158,7 +159,38 @@
       return stat_box
     except:
       log.error('Cannot execute "docker ps": {ex}',category=log.FatalError,module='clab')
       return get_empty_box()
 
   def get_node_name(self, node: str, topology: Box) -> str:
     return f'clab-{ topology.name }-{ node }'
+
+  def validate_node_image(self, node: Box, topology: Box) -> None:
+    if not getattr(self,'image_cache',None):                # Create an image cache on first call
+      self.image_cache: dict = {}
+
+    log.print_verbose(f'clab: validating node {node.name} image {node.box}')
+    if node.box in self.image_cache:                        # We already checked this image, move on
+      return
+    
+    docker_image = external_commands.run_command(           # Get image status from Docker
+                      ['docker', 'image', 'ls', '--format', 'json', node.box],
+                      check_result=True, ignore_errors=True, return_stdout=True)
+    self.image_cache[node.box] = docker_image
+
+    if docker_image:                                        # If we got something back, the image is installed
+      return
+    
+    log.print_verbose(f'clab: image {node.box} is not installed: {docker_image}')
+    dp_data = devices.get_provider_data(node,topology.defaults)
+    if 'build' not in dp_data:                              # We have no build recipe, let's hope it's downloadable
+      return
+
+    log.error(
+      f'Container {node.box} used by node {node.name} is not installed',
+      category=log.IncorrectValue,
+      module='clab',
+      more_hints=[ 
+        f"This container image is not available on Docker Hub and has to be installed locally.",
+        f"If you're using a private Docker repository, use the 'docker image pull {node.box}'",
+        f"command to pull the image from it or build/install it using this recipe:",
+        dp_data.build ])
```

### Comparing `networklab-1.8.1.post1/netsim/providers/clab.yml` & `networklab-1.8.2.dev1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/providers/external.py` & `networklab-1.8.2.dev1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/providers/libvirt.py` & `networklab-1.8.2.dev1/netsim/providers/libvirt.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing
 from box import Box
 import pathlib
 import tempfile
 import netaddr
 
 from ..data import types,get_empty_box
-from ..utils import log
+from ..utils import log,strings
 from ..utils import files as _files
 from . import _Provider
 from ..augment import devices
 from ..augment.links import get_link_by_index
 from ..cli import is_dry_run,external_commands
 
 LIBVIRT_MANAGEMENT_NETWORK_NAME  = "vagrant-libvirt"
@@ -121,23 +121,26 @@
     net_list = external_commands.run_command(
       ['virsh','net-list'],check_result=True,return_stdout=True)
     if isinstance(net_list,str):
       create_net = not mgmt_net in net_list
   else:
     if log.debug_active('libvirt'):
       print(f"Deleting libvirt management network {mgmt_net}")
+    
+    # Remove management network if it exists
     external_commands.run_command(
-      ['virsh','net-destroy',mgmt_net],check_result=True,ignore_errors=True)    # Remove management network
+      ['virsh','net-destroy',mgmt_net],check_result=True,ignore_errors=True,return_stdout=True)
     external_commands.run_command(
-      ['virsh','net-undefine',mgmt_net],check_result=True,ignore_errors=True)   # ... if it exists
+      ['virsh','net-undefine',mgmt_net],check_result=True,ignore_errors=True,return_stdout=True)
 
   if not create_net:
     return
 
   if not log.QUIET:
+    strings.print_colored_text('[CREATED] ','green',None)
     print(f'creating libvirt management network {mgmt_net}')
 
   if topology is None:
     net_template = get_libvirt_mgmt_template()                    # When called without topology data use the default template
   else:
     net_template = create_network_template(topology)              # Otherwise create a temporary XML file
 
@@ -351,7 +354,42 @@
       return stat_box
     except:
       log.error('Cannot execute "vagrant status --machine-readable": {ex}',category=log.FatalError,module='libvirt')
       return get_empty_box()
 
   def get_node_name(self, node: str, topology: Box) -> str:
     return f'{ topology.name.split(".")[0] }_{ node }'
+
+  def validate_node_image(self, node: Box, topology: Box) -> None:
+    box_list = getattr(self,'box_list',None)
+    if not box_list:                                        # Create an box cache on first call
+      box_list = external_commands.run_command(             # Get the list of Vagrant boxes
+                      ['vagrant', 'box', 'list'],
+                      check_result=True, ignore_errors=True, return_stdout=True)
+      box_list = box_list if isinstance(box_list,str) else ''
+      self.box_list = box_list.split('\n')
+
+    log.print_verbose(f'libvirt: validating node {node.name} image {node.box}')
+    box_specs = node.box.split(':')
+    box_name = box_specs[0]
+    box_version = box_specs[1] if len(box_specs) > 1 else ''
+
+    for box_line in self.box_list:                          # Iterate over Vagrant boxes
+      if '(libvirt' not in box_line:                        # Ignore non-libvirt boxes
+        continue
+      if box_name + ' ' in box_line and box_version + ')' in box_line:
+        return                                              # Matching box name and version
+
+    log.print_verbose(f'libvirt: image {node.box} is not installed')
+    dp_data = devices.get_provider_data(node,topology.defaults)
+    if 'build' not in dp_data:                              # We have no build recipe, let's hope it's downloadable
+      return
+
+    log.error(
+      f'Vagrant box {node.box} used by node {node.name} is not installed',
+      category=log.IncorrectValue,
+      module='libvirt',
+      more_hints=[ 
+        f"This box is not available on Vagrant Cloud and has to be installed locally.",
+        f"If you have the Vagrant box available in a private repository, use the",
+        f"'vagrant box add <url>' command to add it, or use this recipe to build it:",
+        dp_data.build ])
```

### Comparing `networklab-1.8.1.post1/netsim/providers/libvirt.yml` & `networklab-1.8.2.dev1/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/clab/clab.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/hosts.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/cumulus/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/clab/frr/hosts.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/frr/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/external/external.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.8.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/tools/__init__.py` & `networklab-1.8.2.dev1/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/tools/graphite.py` & `networklab-1.8.2.dev1/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/tools/graphite.yml` & `networklab-1.8.2.dev1/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/tools/suzieq.yml` & `networklab-1.8.2.dev1/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/topology-defaults.yml` & `networklab-1.8.2.dev1/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/bgp.py` & `networklab-1.8.2.dev1/netsim/utils/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/callback.py` & `networklab-1.8.2.dev1/netsim/utils/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/files.py` & `networklab-1.8.2.dev1/netsim/utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 * add topology directory to any other path
 """
 def expand_package(path: str) -> pathlib.Path:
   return get_moddir () / path.replace('package:','')
 
 def absolute_search_path(
       path: typing.List[str],
-      curdir: str = '.') -> typing.List[str]:
+      curdir: str = '.',
+      skip_missing: bool = False) -> typing.List[str]:
   a_path = []
   for p_entry in path:
     if 'package:' in p_entry:
       p_abs = expand_package(p_entry)
     elif 'topology:' in p_entry:
       topology = global_vars.get_topology()
       if topology:
@@ -104,15 +105,16 @@
     elif p_entry[0] in ['.','/']:
       p_abs = pathlib.Path(p_entry)    
     else:
       p_abs = pathlib.Path(curdir) / p_entry
 
     p_final = str(p_abs.resolve())
     if not p_final in a_path:
-      a_path.append(p_final)
+      if p_abs.is_dir() or not skip_missing:
+        a_path.append(p_final)
 
   return a_path
 
 # 
 # Find a file in a search path
 #
 def find_file(path: str, search_path: typing.List[str]) -> typing.Optional[str]:
```

### Comparing `networklab-1.8.1.post1/netsim/utils/log.py` & `networklab-1.8.2.dev1/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/read.py` & `networklab-1.8.2.dev1/netsim/utils/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/sort.py` & `networklab-1.8.2.dev1/netsim/utils/sort.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/status.py` & `networklab-1.8.2.dev1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/strings.py` & `networklab-1.8.2.dev1/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/templates.py` & `networklab-1.8.2.dev1/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/utils/versioning.py` & `networklab-1.8.2.dev1/netsim/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/netsim/validate/linux.py` & `networklab-1.8.2.dev1/netsim/validate/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/networklab.egg-info/PKG-INFO` & `networklab-1.8.2.dev1/networklab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.1.post1
+Version: 1.8.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.8.1.post1/networklab.egg-info/SOURCES.txt` & `networklab-1.8.2.dev1/networklab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 netsim/ansible/tasks/deploy-config/linux-clab.yml
 netsim/ansible/tasks/deploy-config/linux.yml
 netsim/ansible/tasks/deploy-config/missing.yml
 netsim/ansible/tasks/deploy-config/none.yml
 netsim/ansible/tasks/deploy-config/nxos.yml
 netsim/ansible/tasks/deploy-config/routeros.yml
 netsim/ansible/tasks/deploy-config/routeros7.yml
+netsim/ansible/tasks/deploy-config/sonic.yml
 netsim/ansible/tasks/deploy-config/srlinux.yml
 netsim/ansible/tasks/deploy-config/sros.yml
 netsim/ansible/tasks/deploy-config/vyos.yml
 netsim/ansible/tasks/fetch-config/arcos.yml
 netsim/ansible/tasks/fetch-config/arubacx.yml
 netsim/ansible/tasks/fetch-config/asa.yml
 netsim/ansible/tasks/fetch-config/cumulus.yml
@@ -104,14 +105,15 @@
 netsim/ansible/templates/bgp/junos.j2
 netsim/ansible/templates/bgp/none.j2
 netsim/ansible/templates/bgp/nxos.j2
 netsim/ansible/templates/bgp/routeros.j2
 netsim/ansible/templates/bgp/routeros.macro.j2
 netsim/ansible/templates/bgp/routeros7.j2
 netsim/ansible/templates/bgp/routeros7.macro.j2
+netsim/ansible/templates/bgp/sonic.j2
 netsim/ansible/templates/bgp/srlinux.cli.j2
 netsim/ansible/templates/bgp/srlinux.j2
 netsim/ansible/templates/bgp/srlinux.macro.j2
 netsim/ansible/templates/bgp/sros.gnmi.macro.j2
 netsim/ansible/templates/bgp/sros.j2
 netsim/ansible/templates/bgp/sros.md-cli.j2
 netsim/ansible/templates/bgp/sros.openconfig.j2
@@ -172,22 +174,25 @@
 netsim/ansible/templates/initial/nxos.vrf.j2
 netsim/ansible/templates/initial/routeros.j2
 netsim/ansible/templates/initial/routeros.vlan.j2
 netsim/ansible/templates/initial/routeros.vrf.j2
 netsim/ansible/templates/initial/routeros7.j2
 netsim/ansible/templates/initial/routeros7.vlan.j2
 netsim/ansible/templates/initial/routeros7.vrf.j2
+netsim/ansible/templates/initial/sonic.j2
 netsim/ansible/templates/initial/srlinux.cli.j2
 netsim/ansible/templates/initial/srlinux.j2
 netsim/ansible/templates/initial/sros.j2
 netsim/ansible/templates/initial/sros.md-cli.j2
 netsim/ansible/templates/initial/sros.openconfig.j2
 netsim/ansible/templates/initial/vyos.j2
 netsim/ansible/templates/initial/vyos.vlan.j2
 netsim/ansible/templates/initial/vyos.vrf.j2
+netsim/ansible/templates/initial/frr/daemons.j2
+netsim/ansible/templates/initial/linux/bash_profile.j2
 netsim/ansible/templates/initial/linux/hosts.j2
 netsim/ansible/templates/initial/linux/ubuntu.j2
 netsim/ansible/templates/initial/linux/vanilla.j2
 netsim/ansible/templates/isis/asa.j2
 netsim/ansible/templates/isis/eos.j2
 netsim/ansible/templates/isis/frr.j2
 netsim/ansible/templates/isis/ios.j2
@@ -365,14 +370,15 @@
 netsim/augment/main.py
 netsim/augment/nodes.py
 netsim/augment/plugin.py
 netsim/augment/tools.py
 netsim/augment/topology.py
 netsim/augment/validate.py
 netsim/cli/__init__.py
+netsim/cli/_nodeset.py
 netsim/cli/alias.txt
 netsim/cli/ansible.py
 netsim/cli/clab.py
 netsim/cli/collect.py
 netsim/cli/config.py
 netsim/cli/connect.py
 netsim/cli/create.py
@@ -395,14 +401,17 @@
 netsim/cli/usage.py
 netsim/cli/usage.txt
 netsim/cli/validate.py
 netsim/cli/version.py
 netsim/cli/clab_actions/__init__.py
 netsim/cli/clab_actions/build.py
 netsim/cli/clab_actions/tarball.py
+netsim/cli/libvirt_actions/__init__.py
+netsim/cli/libvirt_actions/config.py
+netsim/cli/libvirt_actions/package.py
 netsim/cli/show_commands/__init__.py
 netsim/cli/show_commands/attributes.py
 netsim/cli/show_commands/defaults.py
 netsim/cli/show_commands/devices.py
 netsim/cli/show_commands/images.py
 netsim/cli/show_commands/module_support.py
 netsim/cli/show_commands/modules.py
@@ -443,14 +452,15 @@
 netsim/devices/junos.yml
 netsim/devices/linux.py
 netsim/devices/linux.yml
 netsim/devices/none.yml
 netsim/devices/nxos.yml
 netsim/devices/routeros.yml
 netsim/devices/routeros7.yml
+netsim/devices/sonic.yml
 netsim/devices/srlinux.yml
 netsim/devices/sros.yml
 netsim/devices/unknown.py
 netsim/devices/unknown.yml
 netsim/devices/vmx.py
 netsim/devices/vmx.yml
 netsim/devices/vptx.py
@@ -512,28 +522,32 @@
 netsim/install/ansible.sh
 netsim/install/containerlab.sh
 netsim/install/grpc.sh
 netsim/install/libvirt.sh
 netsim/install/ubuntu.sh
 netsim/install/libvirt/arubacx.txt
 netsim/install/libvirt/asav.txt
+netsim/install/libvirt/asav.xml.j2
 netsim/install/libvirt/csr.txt
 netsim/install/libvirt/dellos10.txt
 netsim/install/libvirt/eos.txt
 netsim/install/libvirt/eos.xml.j2
 netsim/install/libvirt/iosv.txt
 netsim/install/libvirt/iosv.xml.j2
 netsim/install/libvirt/iosxr.txt
 netsim/install/libvirt/nxos.txt
 netsim/install/libvirt/nxos.xml.j2
 netsim/install/libvirt/routeros7.txt
+netsim/install/libvirt/sonic.txt
+netsim/install/libvirt/sonic.xml.j2
 netsim/install/libvirt/vptx.txt
 netsim/install/libvirt/vptx.xml.j2
 netsim/install/libvirt/vsrx.txt
 netsim/install/libvirt/asav/day0-config
+netsim/install/libvirt/dellos10/run.sh
 netsim/install/libvirt/vptx/juniper.conf
 netsim/install/libvirt/vptx/make-config.sh
 netsim/install/libvirt/vptx/run.sh
 netsim/install/libvirt/vsrx/juniper.conf
 netsim/modules/__init__.py
 netsim/modules/_dataplane.py
 netsim/modules/_routing.py
@@ -617,14 +631,15 @@
 netsim/templates/provider/libvirt/libvirt-bridge.j2
 netsim/templates/provider/libvirt/libvirt-tunnel.j2
 netsim/templates/provider/libvirt/linux-domain.j2
 netsim/templates/provider/libvirt/none-domain.j2
 netsim/templates/provider/libvirt/nxos-domain.j2
 netsim/templates/provider/libvirt/routeros-domain.j2
 netsim/templates/provider/libvirt/routeros7-domain.j2
+netsim/templates/provider/libvirt/sonic-domain.j2
 netsim/templates/provider/libvirt/vagrant-libvirt.xml
 netsim/templates/provider/libvirt/vptx-domain.j2
 netsim/templates/provider/libvirt/vsrx-domain.j2
 netsim/templates/provider/libvirt/vyos-domain.j2
 netsim/templates/provider/virtualbox/Vagrantfile.j2
 netsim/templates/provider/virtualbox/arcos-domain.j2
 netsim/templates/provider/virtualbox/cumulus-domain.j2
```

### Comparing `networklab-1.8.1.post1/setup.py` & `networklab-1.8.2.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1.post1/tests/test_transformation.py` & `networklab-1.8.2.dev1/tests/test_transformation.py`

 * *Files identical despite different names*

