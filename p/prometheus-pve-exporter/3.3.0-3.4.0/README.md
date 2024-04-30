# Comparing `tmp/prometheus_pve_exporter-3.3.0.tar.gz` & `tmp/prometheus_pve_exporter-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_pve_exporter-3.3.0.tar", last modified: Sat Apr 27 10:08:03 2024, max compression
+gzip compressed data, was "prometheus_pve_exporter-3.4.0.tar", last modified: Tue Apr 30 16:38:27 2024, max compression
```

## Comparing `prometheus_pve_exporter-3.3.0.tar` & `prometheus_pve_exporter-3.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/container-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/container-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/pve.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/pylintrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.932236 prometheus_pve_exporter-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4115 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.437092 prometheus_pve_exporter-3.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.433092 prometheus_pve_exporter-3.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.433092 prometheus_pve_exporter-3.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/.github/workflows/container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/.github/workflows/container-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-04-30 16:38:27.437092 prometheus_pve_exporter-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/pve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/pylintrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:38:27.437092 prometheus_pve_exporter-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.429092 prometheus_pve_exporter-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.437092 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-04-30 16:38:27.000000 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 16:38:27.000000 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:38:27.000000 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 16:38:27.000000 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 16:38:27.000000 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 16:38:27.000000 prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.437092 prometheus_pve_exporter-3.4.0/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4115 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:38:27.437092 prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-30 16:38:23.000000 prometheus_pve_exporter-3.4.0/src/pve_exporter/http.py
```

### Comparing `prometheus_pve_exporter-3.3.0/.github/workflows/ci.yml` & `prometheus_pve_exporter-3.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/.github/workflows/container-image.yml` & `prometheus_pve_exporter-3.4.0/.github/workflows/container-image.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/.github/workflows/container-test.yml` & `prometheus_pve_exporter-3.4.0/.github/workflows/container-test.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/.github/workflows/pypi.yml` & `prometheus_pve_exporter-3.4.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/CHANGELOG.rst` & `prometheus_pve_exporter-3.4.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
 `Unreleased`_
 -------------
 
 
+`3.4.0`_ - 2024-04-30
+---------------------
+
+Added
+~~~~~
+
+- Add tags label to pve_guest_info metric (#246)
+
+
 `3.3.0`_ - 2024-04-27
 ---------------------
 
 Added
 ~~~~~
 
 - Add ZFS replication metrics (#243)
@@ -394,15 +403,16 @@
 ~~~~~
 
 -  IPv6 support
 
 
 .. _Keep a Changelog: http://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: http://semver.org/spec/v2.0.0.html
-.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.3.0...HEAD
+.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.4.0...HEAD
+.. _3.4.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.3.0...v3.4.0
 .. _3.3.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...v3.3.0
 .. _3.2.5: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...v3.2.5
 .. _3.2.4: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.3...v3.2.4
 .. _3.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.2...v3.2.3
 .. _3.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...v3.2.2
 .. _3.2.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.0...v3.2.1
 .. _3.2.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.1.0...v3.2.0
```

### Comparing `prometheus_pve_exporter-3.3.0/Dockerfile` & `prometheus_pve_exporter-3.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/LICENSE` & `prometheus_pve_exporter-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/PKG-INFO` & `prometheus_pve_exporter-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.3.0
+Version: 3.4.0
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -203,15 +203,15 @@
     # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
     # TYPE pve_storage_shared gauge
     pve_storage_shared{id="storage/proxmox/local"} 0.0
     pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
     pve_storage_shared{id="storage/proxmox/vms"} 0.0
     # HELP pve_guest_info VM/CT info
     # TYPE pve_guest_info gauge
-    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
+    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu",tags="tag1;tag2"} 1.0
     # HELP pve_storage_info Storage info
     # TYPE pve_storage_info gauge
     pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
     pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
     pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
     # HELP pve_node_info Node info
     # TYPE pve_node_info gauge
@@ -349,14 +349,23 @@
           - source_labels: [__address__]
             target_label: __param_target
           - source_labels: [__param_target]
             target_label: instance
           - target_label: __address__
             replacement: 127.0.0.1:9221  # PVE exporter.
 
+**Note on alerting:**
+
+You can do VM tag based alerting, by using joins on ``pve_guest_info`` metric. For
+example, alerting only when VM with `critical` tag is down:
+
+.. code:: promql
+
+   (pve_guest_info{tags=~".*critical.*"} * on(id) group_left(name) pve_up{}) == 0
+
 **Note on scraping large clusters:**
 
 It is adviced to setup separate jobs to collect ``cluster`` metrics and
 ``node`` metrics in larger deployments. Scraping any node in a cluster with the
 url params set to ``cluster=1&node=0`` results in the same set of metrics. Hence
 cluster metrics can be scraped efficiently from a single node or from a subset
 of cluster nodes (e.g., a different node selected on every scrape via
```

### Comparing `prometheus_pve_exporter-3.3.0/README.rst` & `prometheus_pve_exporter-3.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
     # TYPE pve_storage_shared gauge
     pve_storage_shared{id="storage/proxmox/local"} 0.0
     pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
     pve_storage_shared{id="storage/proxmox/vms"} 0.0
     # HELP pve_guest_info VM/CT info
     # TYPE pve_guest_info gauge
-    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
+    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu",tags="tag1;tag2"} 1.0
     # HELP pve_storage_info Storage info
     # TYPE pve_storage_info gauge
     pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
     pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
     pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
     # HELP pve_node_info Node info
     # TYPE pve_node_info gauge
@@ -321,14 +321,23 @@
           - source_labels: [__address__]
             target_label: __param_target
           - source_labels: [__param_target]
             target_label: instance
           - target_label: __address__
             replacement: 127.0.0.1:9221  # PVE exporter.
 
+**Note on alerting:**
+
+You can do VM tag based alerting, by using joins on ``pve_guest_info`` metric. For
+example, alerting only when VM with `critical` tag is down:
+
+.. code:: promql
+
+   (pve_guest_info{tags=~".*critical.*"} * on(id) group_left(name) pve_up{}) == 0
+
 **Note on scraping large clusters:**
 
 It is adviced to setup separate jobs to collect ``cluster`` metrics and
 ``node`` metrics in larger deployments. Scraping any node in a cluster with the
 url params set to ``cluster=1&node=0`` results in the same set of metrics. Hence
 cluster metrics can be scraped efficiently from a single node or from a subset
 of cluster nodes (e.g., a different node selected on every scrape via
```

### Comparing `prometheus_pve_exporter-3.3.0/pylintrc.toml` & `prometheus_pve_exporter-3.4.0/pylintrc.toml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/pyproject.toml` & `prometheus_pve_exporter-3.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prometheus-pve-exporter"
-version = "3.3.0"
+version = "3.4.0"
 authors = [{ name = "Lorenz Schori", email = "lo@znerol.ch" }]
 description = "Proxmox VE exporter for the Prometheus monitoring system."
 requires-python = ">=3.9"
 keywords = ["prometheus", "exporter", "network", "monitoring", "proxmox"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `prometheus_pve_exporter-3.3.0/requirements.txt` & `prometheus_pve_exporter-3.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.3.0
+Version: 3.4.0
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -203,15 +203,15 @@
     # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
     # TYPE pve_storage_shared gauge
     pve_storage_shared{id="storage/proxmox/local"} 0.0
     pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
     pve_storage_shared{id="storage/proxmox/vms"} 0.0
     # HELP pve_guest_info VM/CT info
     # TYPE pve_guest_info gauge
-    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
+    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu",tags="tag1;tag2"} 1.0
     # HELP pve_storage_info Storage info
     # TYPE pve_storage_info gauge
     pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
     pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
     pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
     # HELP pve_node_info Node info
     # TYPE pve_node_info gauge
@@ -349,14 +349,23 @@
           - source_labels: [__address__]
             target_label: __param_target
           - source_labels: [__param_target]
             target_label: instance
           - target_label: __address__
             replacement: 127.0.0.1:9221  # PVE exporter.
 
+**Note on alerting:**
+
+You can do VM tag based alerting, by using joins on ``pve_guest_info`` metric. For
+example, alerting only when VM with `critical` tag is down:
+
+.. code:: promql
+
+   (pve_guest_info{tags=~".*critical.*"} * on(id) group_left(name) pve_up{}) == 0
+
 **Note on scraping large clusters:**
 
 It is adviced to setup separate jobs to collect ``cluster`` metrics and
 ``node`` metrics in larger deployments. Scraping any node in a cluster with the
 url params set to ``cluster=1&node=0`` results in the same set of metrics. Hence
 cluster metrics can be scraped efficiently from a single node or from a subset
 of cluster nodes (e.g., a different node selected on every scrape via
```

### Comparing `prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt` & `prometheus_pve_exporter-3.4.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/src/pve_exporter/cli.py` & `prometheus_pve_exporter-3.4.0/src/pve_exporter/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/__init__.py` & `prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/cluster.py` & `prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,28 +205,28 @@
                 labels=['id']),
         }
 
         info_metrics = {
             'guest': GaugeMetricFamily(
                 'pve_guest_info',
                 'VM/CT info',
-                labels=['id', 'node', 'name', 'type', 'template']),
+                labels=['id', 'node', 'name', 'type', 'template', 'tags']),
             'storage': GaugeMetricFamily(
                 'pve_storage_info',
                 'Storage info',
                 labels=['id', 'node', 'storage']),
         }
 
         info_lookup = {
             'lxc': {
-                'labels': ['id', 'node', 'name', 'type', 'template'],
+                'labels': ['id', 'node', 'name', 'type', 'template', 'tags'],
                 'gauge': info_metrics['guest'],
             },
             'qemu': {
-                'labels': ['id', 'node', 'name', 'type', 'template'],
+                'labels': ['id', 'node', 'name', 'type', 'template', 'tags'],
                 'gauge': info_metrics['guest'],
             },
             'storage': {
                 'labels': ['id', 'node', 'storage'],
                 'gauge': info_metrics['storage'],
             },
         }
```

### Comparing `prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/node.py` & `prometheus_pve_exporter-3.4.0/src/pve_exporter/collector/node.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/src/pve_exporter/config.py` & `prometheus_pve_exporter-3.4.0/src/pve_exporter/config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.3.0/src/pve_exporter/http.py` & `prometheus_pve_exporter-3.4.0/src/pve_exporter/http.py`

 * *Files identical despite different names*

