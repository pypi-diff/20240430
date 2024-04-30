# Comparing `tmp/dask-kubernetes-2024.4.2.tar.gz` & `tmp/dask_kubernetes-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2024.4.2.tar", last modified: Wed Apr 24 14:36:05 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dask-kubernetes-2024.4.2.tar` & `dask_kubernetes-2024.5.0.tar`

### file list

```diff
@@ -1,110 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.074747 dask-kubernetes-2024.4.2/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-24 14:36:05.090747 dask-kubernetes-2024.4.2/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30973 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.070747 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.074747 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/versioneer.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/__init__.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/_version.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/config.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/conftest.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/constants.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/exceptions.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/kubernetes.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/cli/cli.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/_objects.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/networking.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/validation.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0        0        0    30122 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/controller.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/plugins/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/plugins/noop/noop.py
+-rw-r--r--   0        0        0    30973 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/test_controller.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/templates.yaml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/Dockerfile
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/README.md -> dask-kubernetes-operator/README.md
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/.helmignore
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/README.md
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0        0        0   283847 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0        0        0   471240 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0        0        0   140704 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/NOTES.txt
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/manifests/README.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/hack/Dockerfile
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/hack/lint.sh
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/hack/regenerate-code.sh
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/apis/register.go
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/apis/kubernetes.dask.org/v1/doc.go
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/apis/kubernetes.dask.org/v1/register.go
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/apis/kubernetes.dask.org/v1/types.go
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/apis/kubernetes.dask.org/v1/zz_generated.deepcopy.go
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/utils.go
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/internal/internal.go
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskautoscaler.go
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskautoscalerspec.go
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskcluster.go
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskclusterspec.go
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskclusterstatus.go
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskjob.go
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskjobspec.go
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskjobstatus.go
+-rw-r--r--   0        0        0     9474 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskworkergroup.go
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/daskworkergroupspec.go
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/jobspec.go
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/schedulerspec.go
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/applyconfiguration/kubernetes.dask.org/v1/workerspec.go
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/clientset.go
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/doc.go
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/fake/clientset_generated.go
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/fake/doc.go
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/fake/register.go
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/scheme/doc.go
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/scheme/register.go
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/daskautoscaler.go
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/daskcluster.go
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/daskjob.go
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/daskworkergroup.go
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/doc.go
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/generated_expansion.go
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/kubernetes.dask.org_client.go
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/fake/doc.go
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/fake/fake_daskautoscaler.go
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/fake/fake_daskcluster.go
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/fake/fake_daskjob.go
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/fake/fake_daskworkergroup.go
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/clientset/versioned/typed/kubernetes.dask.org/v1/fake/fake_kubernetes.dask.org_client.go
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/factory.go
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/generic.go
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/internalinterfaces/factory_interfaces.go
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/kubernetes.dask.org/interface.go
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/kubernetes.dask.org/v1/daskautoscaler.go
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/kubernetes.dask.org/v1/daskcluster.go
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/kubernetes.dask.org/v1/daskjob.go
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/kubernetes.dask.org/v1/daskworkergroup.go
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/informers/externalversions/kubernetes.dask.org/v1/interface.go
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/listers/kubernetes.dask.org/v1/daskautoscaler.go
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/listers/kubernetes.dask.org/v1/daskcluster.go
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/listers/kubernetes.dask.org/v1/daskjob.go
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/listers/kubernetes.dask.org/v1/daskworkergroup.go
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/go_client/pkg/client/listers/kubernetes.dask.org/v1/expansion_generated.go
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0        0        0    37807 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/kubecluster.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/.gitignore
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/README.rst
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 dask_kubernetes-2024.5.0/PKG-INFO
```

### Comparing `dask-kubernetes-2024.4.2/LICENSE` & `dask_kubernetes-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/PKG-INFO` & `dask_kubernetes-2024.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dask-kubernetes
-Version: 2024.4.2
-Summary: Native Kubernetes integration for Dask
-Home-page: https://github.com/dask/dask-kubernetes
-Maintainer: Jacob Tomlinson
-License: BSD
-Keywords: dask,kubernetes,distributed
-Requires-Python: >=3.9
-License-File: LICENSE
-
 Dask Kubernetes
 ===============
 
 
 .. image:: https://github.com/dask/dask-kubernetes/actions/workflows/lint.yaml/badge.svg
    :target: https://github.com/dask/dask-kubernetes/actions/workflows/lint.yaml
    :alt: Linting GitHub Actions CI Status
```

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_async.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,886 +1,807 @@
 import asyncio
-import base64
-import getpass
-import os
-import random
-import sys
-from time import time
+import json
+import os.path
+import pathlib
+from contextlib import asynccontextmanager
+from datetime import datetime, timedelta
 
-import dask
-import kubernetes_asyncio as kubernetes
+import dask.config
 import pytest
 import yaml
-from dask.distributed import Client, wait
-from dask.utils import tmpfile
-from distributed.utils_test import captured_logger
-
-import dask_kubernetes
-from dask_kubernetes import (
-    ClusterAuth,
-    KubeAuth,
-    KubeCluster,
-    KubeConfig,
-    clean_pod_template,
-    make_pod_spec,
-)
-from dask_kubernetes.common.utils import get_current_namespace
-from dask_kubernetes.constants import KUBECLUSTER_CONTAINER_NAME
-
-TEST_DIR = os.path.abspath(os.path.join(__file__, ".."))
-CONFIG_DEMO = os.path.join(TEST_DIR, "config-demo.yaml")
-FAKE_CERT = os.path.join(TEST_DIR, "fake-cert-file")
-FAKE_KEY = os.path.join(TEST_DIR, "fake-key-file")
-FAKE_CA = os.path.join(TEST_DIR, "fake-ca-file")
-
-
-@pytest.fixture
-def pod_spec(docker_image):
-    yield clean_pod_template(
-        make_pod_spec(
-            image=docker_image,
-            extra_container_config={"imagePullPolicy": "IfNotPresent"},
-        )
-    )
-
-
-@pytest.fixture
-def user_env():
-    """The env var USER is not always set on non-linux systems."""
-    if "USER" not in os.environ:
-        os.environ["USER"] = getpass.getuser()
-        yield
-        del os.environ["USER"]
-    else:
-        yield
-
-
-cluster_kwargs = {"asynchronous": True}
-
+from dask.distributed import Client
+from kr8s.asyncio.objects import Deployment, Pod, Service
 
-@pytest.fixture
-async def cluster(k8s_cluster, pod_spec):
-    async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
-        yield cluster
+from dask_kubernetes.constants import MAX_CLUSTER_NAME_LEN
+from dask_kubernetes.operator._objects import DaskCluster, DaskJob, DaskWorkerGroup
+from dask_kubernetes.operator.controller import (
+    KUBERNETES_DATETIME_FORMAT,
+    get_job_runner_pod_name,
+)
 
+DIR = pathlib.Path(__file__).parent.absolute()
 
-@pytest.fixture
-async def remote_cluster(k8s_cluster, pod_spec):
-    async with KubeCluster(pod_spec, deploy_mode="remote", **cluster_kwargs) as cluster:
-        yield cluster
+_EXPECTED_ANNOTATIONS = {"test-annotation": "annotation-value"}
+_EXPECTED_LABELS = {"test-label": "label-value"}
+DEFAULT_CLUSTER_NAME = "simple"
+
+
+@pytest.fixture()
+def gen_cluster_manifest(tmp_path):
+    def factory(cluster_name=DEFAULT_CLUSTER_NAME):
+        original_manifest_path = os.path.join(DIR, "resources", "simplecluster.yaml")
+        with open(original_manifest_path, "r") as original_manifest_file:
+            manifest = yaml.safe_load(original_manifest_file)
+
+        manifest["metadata"]["name"] = cluster_name
+        new_manifest_path = tmp_path / "cluster.yaml"
+        new_manifest_path.write_text(yaml.safe_dump(manifest))
+        return tmp_path
+
+    return factory
+
+
+@pytest.fixture()
+def gen_cluster(k8s_cluster, ns, gen_cluster_manifest):
+    """Yields an instantiated context manager for creating/deleting a simple cluster."""
+
+    @asynccontextmanager
+    async def cm(cluster_name=DEFAULT_CLUSTER_NAME):
+        cluster_path = gen_cluster_manifest(cluster_name)
+        # Create cluster resource
+        k8s_cluster.kubectl("apply", "-n", ns, "-f", cluster_path)
+        while cluster_name not in k8s_cluster.kubectl(
+            "get", "daskclusters.kubernetes.dask.org", "-n", ns
+        ):
+            await asyncio.sleep(0.1)
+
+        try:
+            yield cluster_name, ns
+        finally:
+            # Test: remove the wait=True, because I think this is blocking the operator
+            k8s_cluster.kubectl("delete", "-n", ns, "-f", cluster_path)
+
+    yield cm
+
+
+@pytest.fixture()
+def gen_job(k8s_cluster, ns):
+    """Yields an instantiated context manager for creating/deleting a simple job."""
+
+    @asynccontextmanager
+    async def cm(job_file):
+        job_path = os.path.join(DIR, "resources", job_file)
+        with open(job_path) as f:
+            job_name = yaml.load(f, yaml.Loader)["metadata"]["name"]
+
+        # Create cluster resource
+        k8s_cluster.kubectl("apply", "-n", ns, "-f", job_path)
+        while job_name not in k8s_cluster.kubectl(
+            "get", "daskjobs.kubernetes.dask.org", "-n", ns
+        ):
+            await asyncio.sleep(0.1)
+
+        try:
+            yield job_name, ns
+        finally:
+            # Test: remove the wait=True, because I think this is blocking the operator
+            k8s_cluster.kubectl("delete", "-n", ns, "-f", job_path)
+            while job_name in k8s_cluster.kubectl(
+                "get", "daskjobs.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
 
+    yield cm
 
-@pytest.fixture
-async def client(cluster):
-    async with Client(cluster, asynchronous=True) as client:
-        yield client
 
+@pytest.fixture()
+def gen_worker_group(k8s_cluster, ns):
+    """Yields an instantiated context manager for creating/deleting a worker group."""
+
+    @asynccontextmanager
+    async def cm(worker_group_file):
+        worker_group_path = os.path.join(DIR, "resources", worker_group_file)
+        with open(worker_group_path) as f:
+            worker_group_name = yaml.load(f, yaml.Loader)["metadata"]["name"]
+
+        # Create cluster resource
+        k8s_cluster.kubectl("apply", "-n", ns, "-f", worker_group_path)
+        while worker_group_name not in k8s_cluster.kubectl(
+            "get", "daskworkergroups.kubernetes.dask.org", "-n", ns
+        ):
+            await asyncio.sleep(0.1)
+
+        try:
+            yield worker_group_name, ns
+        finally:
+            # Test: remove the wait=True, because I think this is blocking the operator
+            k8s_cluster.kubectl("delete", "-n", ns, "-f", worker_group_path)
+            while worker_group_name in k8s_cluster.kubectl(
+                "get", "daskworkergroups.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
 
-@pytest.mark.anyio
-async def test_fixtures(client):
-    """An initial test to get all the fixtures to run and check the cluster is usable."""
-    assert client
+    yield cm
 
 
-@pytest.mark.anyio
-async def test_versions(client):
-    await client.get_versions(check=True)
+def test_customresources(k8s_cluster):
+    assert "daskclusters.kubernetes.dask.org" in k8s_cluster.kubectl("get", "crd")
+    assert "daskworkergroups.kubernetes.dask.org" in k8s_cluster.kubectl("get", "crd")
+    assert "daskjobs.kubernetes.dask.org" in k8s_cluster.kubectl("get", "crd")
 
 
-@pytest.mark.anyio
-async def test_cluster_create(cluster):
-    cluster.scale(1)
-    await cluster
-    async with Client(cluster, asynchronous=True) as client:
-        result = await client.submit(lambda x: x + 1, 10)
-        assert result == 11
+def test_operator_runs(kopf_runner):
+    with kopf_runner as runner:
+        pass
 
+    assert runner.exit_code == 0
+    assert runner.exception is None
 
-@pytest.mark.anyio
-async def test_basic(cluster, client):
-    cluster.scale(2)
-    future = client.submit(lambda x: x + 1, 10)
-    result = await future
-    assert result == 11
 
-    await client.wait_for_workers(2)
+def test_operator_plugins(kopf_runner):
+    with kopf_runner as runner:
+        pass
 
-    # Ensure that inter-worker communication works well
-    futures = client.map(lambda x: x + 1, range(10))
-    total = client.submit(sum, futures)
-    assert (await total) == sum(map(lambda x: x + 1, range(10)))
-    assert all((await client.has_what()).values())
+    assert runner.exit_code == 0
+    assert runner.exception is None
+    assert "Plugin 'noop' running." in runner.stdout
 
 
+@pytest.mark.timeout(180)
 @pytest.mark.anyio
-async def test_logs(remote_cluster):
-    cluster = remote_cluster
-    cluster.scale(2)
-    await cluster
-
-    async with Client(cluster, asynchronous=True) as client:
-        await client.wait_for_workers(2)
+async def test_simplecluster(k8s_cluster, kopf_runner, gen_cluster):
+    with kopf_runner:
+        async with gen_cluster() as (cluster_name, ns):
+            scheduler_deployment_name = "simple-scheduler"
+            worker_pod_name = "simple-default-worker"
+            service_name = "simple-scheduler"
 
-    logs = await cluster.get_logs()
-    assert len(logs) == 4
-    for _, log in logs.items():
-        assert (
-            "distributed.scheduler" in log
-            or "distributed.worker" in log
-            or "Creating scheduler pod" in log
-        )
+            while scheduler_deployment_name not in k8s_cluster.kubectl(
+                "get", "deployments", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
+            while service_name not in k8s_cluster.kubectl("get", "svc", "-n", ns):
+                await asyncio.sleep(0.1)
+            while worker_pod_name not in k8s_cluster.kubectl("get", "pods", "-n", ns):
+                await asyncio.sleep(0.1)
 
+            with k8s_cluster.port_forward(
+                f"service/{service_name}", 8786, "-n", ns
+            ) as port:
+                async with Client(
+                    f"tcp://localhost:{port}", asynchronous=True
+                ) as client:
+                    await client.wait_for_workers(2)
+                    # Ensure that inter-worker communication works well
+                    futures = client.map(lambda x: x + 1, range(10))
+                    total = client.submit(sum, futures)
+                    assert (await total) == sum(map(lambda x: x + 1, range(10)))
+
+            # Get the first env value (the only one) of the scheduler
+            scheduler_env = k8s_cluster.kubectl(
+                "get",
+                "pods",
+                "-n",
+                ns,
+                "--selector=dask.org/component=scheduler",
+                "-o",
+                "jsonpath='{.items[0].spec.containers[0].env[0]}'",
+            )
+            # Just check if it's in the string, no need to parse the json
+            assert "SCHEDULER_ENV" in scheduler_env
 
-@pytest.mark.anyio
-async def test_dask_worker_name_env_variable(k8s_cluster, pod_spec, user_env):
-    with dask.config.set({"kubernetes.name": "foo-{USER}-{uuid}"}):
-        async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
-            assert "foo-" + getpass.getuser() in cluster.name
+            # Get the first annotation (the only one) of the scheduler
+            scheduler_annotations = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "pods",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/component=scheduler",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.annotations}'",
+                )[1:-1]
+            )  # First and last char is a quote
+            assert _EXPECTED_ANNOTATIONS.items() <= scheduler_annotations.items()
+
+            # Get the first annotation (the only one) of the scheduler
+            service_annotations = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "svc",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/cluster-name=simple",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.annotations}'",
+                )[1:-1]
+            )  # First and last char is a quote
+            assert _EXPECTED_ANNOTATIONS.items() <= service_annotations.items()
+
+            # Get the first env value (the only one) of the first worker
+            worker_env = k8s_cluster.kubectl(
+                "get",
+                "pods",
+                "-n",
+                ns,
+                "--selector=dask.org/component=worker",
+                "-o",
+                "jsonpath='{.items[0].spec.containers[0].env[0]}'",
+            )
+            # Just check if it's in the string, no need to parse the json
+            assert "WORKER_ENV" in worker_env
+            assert cluster_name
+
+            # Get the first annotation (the only one) of a worker
+            worker_annotations = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "pods",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/component=worker",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.annotations}'",
+                )[1:-1]
+            )
+            assert _EXPECTED_ANNOTATIONS.items() <= worker_annotations.items()
 
+            # Assert labels from the dask cluster are propagated into the dask worker group
+            workergroup_labels = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "daskworkergroups",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/component=workergroup",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.labels}'",
+                )[1:-1]
+            )
+            assert _EXPECTED_LABELS.items() <= workergroup_labels.items()
+            assert "worker-sublabel" in workergroup_labels
 
-@pytest.mark.anyio
-async def test_diagnostics_link_env_variable(k8s_cluster, pod_spec, user_env):
-    pytest.importorskip("bokeh")
-    with dask.config.set({"distributed.dashboard.link": "foo-{USER}-{port}"}):
-        async with KubeCluster(pod_spec, asynchronous=True) as cluster:
-            port = cluster.forwarded_dashboard_port
+            # Assert labels from the dask cluster are propagated into the dask scheduler
+            scheduler_labels = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "pods",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/component=scheduler",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.labels}'",
+                )[1:-1]
+            )
+            assert _EXPECTED_LABELS.items() <= scheduler_labels.items()
+            assert "scheduler-sublabel" in scheduler_labels
 
-            assert (
-                "foo-" + getpass.getuser() + "-" + str(port) in cluster.dashboard_link
+            # Assert labels from the dask cluster are propagated into the dask worker pod
+            worker_labels = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "pods",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/component=worker",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.labels}'",
+                )[1:-1]
             )
+            assert _EXPECTED_LABELS.items() <= worker_labels.items()
+            assert "worker-sublabel" in workergroup_labels
 
 
-@pytest.mark.skip(reason="Cannot run two closers locally as loadbalancer ports collide")
 @pytest.mark.anyio
-async def test_namespace(k8s_cluster, pod_spec):
-    async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
-        assert "dask" in cluster.name
-        assert getpass.getuser() in cluster.name
-        async with KubeCluster(pod_spec, **cluster_kwargs) as cluster2:
-            assert cluster.name != cluster2.name
-
-            cluster2.scale(1)
-            while len(await cluster2.pods()) != 1:
+async def test_scalesimplecluster(k8s_cluster, kopf_runner, gen_cluster):
+    with kopf_runner:
+        async with gen_cluster() as (cluster_name, ns):
+            scheduler_deployment_name = "simple-scheduler"
+            worker_pod_name = "simple-default-worker"
+            service_name = "simple-scheduler"
+            while scheduler_deployment_name not in k8s_cluster.kubectl(
+                "get", "deployments", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
+            while service_name not in k8s_cluster.kubectl("get", "svc", "-n", ns):
+                await asyncio.sleep(0.1)
+            while worker_pod_name not in k8s_cluster.kubectl("get", "pods", "-n", ns):
                 await asyncio.sleep(0.1)
 
-
-@pytest.mark.anyio
-async def test_adapt(cluster):
-    cluster.adapt()
-    async with Client(cluster, asynchronous=True) as client:
-        future = client.submit(lambda x: x + 1, 10)
-        result = await future
-        assert result == 11
-
-
-@pytest.mark.xfail(reason="The widget has changed upstream")
-@pytest.mark.anyio
-async def test_ipython_display(cluster):
-    ipywidgets = pytest.importorskip("ipywidgets")
-    cluster.scale(1)
-    await cluster
-    cluster._ipython_display_()
-    box = cluster._cached_widget
-    assert isinstance(box, ipywidgets.Widget)
-    cluster._ipython_display_()
-    assert cluster._cached_widget is box
-
-    start = time()
-    while "<td>1</td>" not in str(box):  # one worker in a table
-        assert time() < start + 20
-        await asyncio.sleep(0.5)
-
-
-@pytest.mark.anyio
-async def test_env(k8s_cluster, pod_spec):
-    async with KubeCluster(pod_spec, env={"ABC": "DEF"}, **cluster_kwargs) as cluster:
-        cluster.scale(1)
-        await cluster
-        async with Client(cluster, asynchronous=True) as client:
-            await client.wait_for_workers(1)
-            env = await client.run(lambda: dict(os.environ))
-            assert all(v["ABC"] == "DEF" for v in env.values())
+            with k8s_cluster.port_forward(
+                f"service/{service_name}", 8786, "-n", ns
+            ) as port:
+                async with Client(
+                    f"tcp://localhost:{port}", asynchronous=True
+                ) as client:
+                    k8s_cluster.kubectl(
+                        "scale",
+                        "-n",
+                        ns,
+                        "--replicas=5",
+                        "daskworkergroup.kubernetes.dask.org",
+                        "simple-default",
+                    )
+                    await client.wait_for_workers(5)
+                    k8s_cluster.kubectl(
+                        "scale",
+                        "-n",
+                        ns,
+                        "--replicas=3",
+                        "daskworkergroup.kubernetes.dask.org",
+                        "simple-default",
+                    )
+                    # TODO: Currently, doesn't test anything. Need to add optional
+                    #       argument to wait when removing workers once distributed
+                    #       PR github.com/dask/distributed/pull/6377 is merged.
+                    await client.wait_for_workers(3)
 
 
 @pytest.mark.anyio
-async def test_pod_from_yaml(k8s_cluster, docker_image):
-    test_yaml = {
-        "kind": "Pod",
-        "metadata": {"labels": {"app": "dask", "component": "dask-worker"}},
-        "spec": {
-            "containers": [
-                {
-                    "args": [
-                        "dask-worker",
-                        "$(DASK_SCHEDULER_ADDRESS)",
-                        "--nthreads",
-                        "1",
-                    ],
-                    "image": docker_image,
-                    "imagePullPolicy": "IfNotPresent",
-                    "name": KUBECLUSTER_CONTAINER_NAME,
-                }
-            ]
-        },
-    }
-
-    with tmpfile(extension="yaml") as fn:
-        with open(fn, mode="w") as f:
-            yaml.dump(test_yaml, f)
-        async with KubeCluster(f.name, **cluster_kwargs) as cluster:
-            cluster.scale(2)
-            await cluster
-            async with Client(cluster, asynchronous=True) as client:
-                future = client.submit(lambda x: x + 1, 10)
-                result = await future.result(timeout=30)
-                assert result == 11
-
-                await client.wait_for_workers(2)
-
-                # Ensure that inter-worker communication works well
-                futures = client.map(lambda x: x + 1, range(10))
-                total = client.submit(sum, futures)
-                assert (await total) == sum(map(lambda x: x + 1, range(10)))
-                assert all((await client.has_what()).values())
-
-
-@pytest.mark.anyio
-async def test_pod_expand_env_vars(k8s_cluster, docker_image):
-    try:
-        os.environ["FOO_IMAGE"] = docker_image
-
-        test_yaml = {
-            "kind": "Pod",
-            "metadata": {"labels": {"app": "dask", "component": "dask-worker"}},
-            "spec": {
-                "containers": [
-                    {
-                        "args": [
-                            "dask-worker",
-                            "$(DASK_SCHEDULER_ADDRESS)",
-                            "--nthreads",
-                            "1",
-                        ],
-                        "image": "${FOO_IMAGE}",
-                        "imagePullPolicy": "IfNotPresent",
-                        "name": KUBECLUSTER_CONTAINER_NAME,
-                    }
-                ]
-            },
-        }
-
-        with tmpfile(extension="yaml") as fn:
-            with open(fn, mode="w") as f:
-                yaml.dump(test_yaml, f)
-            async with KubeCluster(f.name, **cluster_kwargs) as cluster:
-                assert cluster.pod_template.spec.containers[0].image == docker_image
-    finally:
-        del os.environ["FOO_IMAGE"]
-
-
-@pytest.mark.anyio
-async def test_pod_template_dict(docker_image):
-    spec = {
-        "metadata": {},
-        "restartPolicy": "Never",
-        "spec": {
-            "containers": [
-                {
-                    "args": [
-                        "dask-worker",
-                        "$(DASK_SCHEDULER_ADDRESS)",
-                        "--nthreads",
-                        "1",
-                        "--death-timeout",
-                        "60",
-                    ],
-                    "command": None,
-                    "image": docker_image,
-                    "imagePullPolicy": "IfNotPresent",
-                    "name": KUBECLUSTER_CONTAINER_NAME,
-                }
-            ]
-        },
-    }
+async def test_scalesimplecluster_from_cluster_spec(
+    k8s_cluster, kopf_runner, gen_cluster
+):
+    with kopf_runner:
+        async with gen_cluster() as (cluster_name, ns):
+            scheduler_deployment_name = "simple-scheduler"
+            worker_pod_name = "simple-default-worker"
+            service_name = "simple-scheduler"
+            while scheduler_deployment_name not in k8s_cluster.kubectl(
+                "get", "pods", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
+            while service_name not in k8s_cluster.kubectl("get", "svc", "-n", ns):
+                await asyncio.sleep(0.1)
+            while worker_pod_name not in k8s_cluster.kubectl("get", "pods", "-n", ns):
+                await asyncio.sleep(0.1)
 
-    async with KubeCluster(spec, port=32000, **cluster_kwargs) as cluster:
-        cluster.scale(2)
-        await cluster
-        async with Client(cluster, asynchronous=True) as client:
-            future = client.submit(lambda x: x + 1, 10)
-            result = await future
-            assert result == 11
-
-            await client.wait_for_workers(2)
-
-            # Ensure that inter-worker communication works well
-            futures = client.map(lambda x: x + 1, range(10))
-            total = client.submit(sum, futures)
-            assert (await total) == sum(map(lambda x: x + 1, range(10)))
-            assert all((await client.has_what()).values())
+            with k8s_cluster.port_forward(
+                f"service/{service_name}", 8786, "-n", ns
+            ) as port:
+                async with Client(
+                    f"tcp://localhost:{port}", asynchronous=True
+                ) as client:
+                    k8s_cluster.kubectl(
+                        "scale",
+                        "-n",
+                        ns,
+                        "--replicas=5",
+                        "daskcluster.kubernetes.dask.org",
+                        cluster_name,
+                    )
+                    await client.wait_for_workers(5)
+                    k8s_cluster.kubectl(
+                        "scale",
+                        "-n",
+                        ns,
+                        "--replicas=3",
+                        "daskcluster.kubernetes.dask.org",
+                        cluster_name,
+                    )
+                    # TODO: Currently, doesn't test anything. Need to add optional
+                    #       argument to wait when removing workers once distributed
+                    #       PR github.com/dask/distributed/pull/6377 is merged.
+                    await client.wait_for_workers(3)
 
 
 @pytest.mark.anyio
-async def test_pod_template_minimal_dict(k8s_cluster, docker_image):
-    spec = {
-        "spec": {
-            "containers": [
-                {
-                    "args": [
-                        "dask-worker",
-                        "$(DASK_SCHEDULER_ADDRESS)",
-                        "--nthreads",
-                        "1",
-                        "--death-timeout",
-                        "60",
-                    ],
-                    "command": None,
-                    "image": docker_image,
-                    "imagePullPolicy": "IfNotPresent",
-                    "name": KUBECLUSTER_CONTAINER_NAME,
-                }
-            ]
-        }
-    }
-
-    async with KubeCluster(spec, **cluster_kwargs) as cluster:
-        cluster.adapt()
-        async with Client(cluster, asynchronous=True) as client:
-            future = client.submit(lambda x: x + 1, 10)
-            result = await future
-            assert result == 11
+async def test_recreate_scheduler_pod(k8s_cluster, kopf_runner, gen_cluster):
+    with kopf_runner:
+        async with gen_cluster() as (cluster_name, ns):
+            scheduler_deployment_name = "simple-scheduler"
+            worker_pod_name = "simple-default-worker"
+            service_name = "simple-scheduler"
+            while scheduler_deployment_name not in k8s_cluster.kubectl(
+                "get", "pods", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
+            while service_name not in k8s_cluster.kubectl("get", "svc", "-n", ns):
+                await asyncio.sleep(0.1)
+            while worker_pod_name not in k8s_cluster.kubectl("get", "pods", "-n", ns):
+                await asyncio.sleep(0.1)
+            k8s_cluster.kubectl(
+                "delete",
+                "pods",
+                "-l",
+                "dask.org/cluster-name=simple,dask.org/component=scheduler",
+                "-n",
+                ns,
+            )
+            k8s_cluster.kubectl(
+                "wait",
+                "--for=condition=Ready",
+                "-l",
+                "dask.org/cluster-name=simple,dask.org/component=scheduler",
+                "pod",
+                "-n",
+                ns,
+                "--timeout=60s",
+            )
+            assert scheduler_deployment_name in k8s_cluster.kubectl(
+                "get", "pods", "-n", ns
+            )
 
 
 @pytest.mark.anyio
-async def test_pod_template_from_conf(docker_image):
-    spec = {
-        "spec": {
-            "containers": [{"name": KUBECLUSTER_CONTAINER_NAME, "image": docker_image}]
-        }
-    }
-
-    with dask.config.set({"kubernetes.worker-template": spec}):
-        async with KubeCluster(**cluster_kwargs) as cluster:
-            assert (
-                cluster.pod_template.spec.containers[0].name
-                == KUBECLUSTER_CONTAINER_NAME
+@pytest.mark.skip(reason="Flaky in CI")
+async def test_recreate_worker_pods(k8s_cluster, kopf_runner, gen_cluster):
+    with kopf_runner:
+        async with gen_cluster() as (cluster_name, ns):
+            cluster = await DaskCluster.get(cluster_name, namespace=ns)
+            # Get the default worker group
+            while not (wgs := await cluster.worker_groups()):
+                await asyncio.sleep(0.1)
+            [wg] = wgs
+            # Wait for worker Pods to be created
+            while not (pods := await wg.pods()):
+                await asyncio.sleep(0.1)
+            # Store number of workers
+            n_pods = len(pods)
+            # Wait for worker Pods to be ready
+            await asyncio.gather(
+                *[pod.wait(conditions="condition=Ready", timeout=60) for pod in pods]
+            )
+            # Delete a worker Pod
+            await pods[0].delete()
+            # Wait for Pods to be recreated
+            while len((pods := await wg.pods())) < n_pods:
+                await asyncio.sleep(0.1)
+            # Wait for worker Pods to be ready
+            await asyncio.gather(
+                *[pod.wait(conditions="condition=Ready", timeout=60) for pod in pods]
             )
 
 
 @pytest.mark.anyio
-async def test_pod_template_with_custom_container_name(docker_image):
-    container_name = "my-custom-container"
-    spec = {"spec": {"containers": [{"name": container_name, "image": docker_image}]}}
-
-    with dask.config.set({"kubernetes.worker-template": spec}):
-        async with KubeCluster(**cluster_kwargs) as cluster:
-            assert cluster.pod_template.spec.containers[0].name == container_name
+async def test_simplecluster_batched_worker_deployments(
+    k8s_cluster, kopf_runner, gen_cluster
+):
+    with kopf_runner:
+        with dask.config.set(
+            {
+                "kubernetes.controller.worker-allocation.batch-size": 1,
+                "kubernetes.controller.worker-allocation.delay": 5,
+            }
+        ):
+            async with gen_cluster() as (cluster_name, ns):
+                scheduler_deployment_name = "simple-scheduler"
+                worker_pod_name = "simple-default-worker"
+                service_name = "simple-scheduler"
+                while scheduler_deployment_name not in k8s_cluster.kubectl(
+                    "get", "deployments", "-n", ns
+                ):
+                    await asyncio.sleep(0.1)
+                while service_name not in k8s_cluster.kubectl("get", "svc", "-n", ns):
+                    await asyncio.sleep(0.1)
+                while worker_pod_name not in k8s_cluster.kubectl(
+                    "get", "pods", "-n", ns
+                ):
+                    await asyncio.sleep(0.1)
+
+                with k8s_cluster.port_forward(
+                    f"service/{service_name}", 8786, "-n", ns
+                ) as port:
+                    async with Client(
+                        f"tcp://localhost:{port}", asynchronous=True
+                    ) as client:
+                        await client.wait_for_workers(2)
+                        futures = client.map(lambda x: x + 1, range(10))
+                        total = client.submit(sum, futures)
+                        assert (await total) == sum(map(lambda x: x + 1, range(10)))
+
+
+def _get_job_status(k8s_cluster, ns):
+    return json.loads(
+        k8s_cluster.kubectl(
+            "get",
+            "-n",
+            ns,
+            "daskjobs.kubernetes.dask.org",
+            "-o",
+            "jsonpath='{.items[0].status}'",
+        )[1:-1]
+    )
 
 
-@pytest.mark.anyio
-async def test_constructor_parameters(k8s_cluster, pod_spec):
-    env = {"FOO": "BAR", "A": 1}
-    async with KubeCluster(
-        pod_spec, name="myname", env=env, **cluster_kwargs
-    ) as cluster:
-        pod = cluster.pod_template
-        assert pod.metadata.namespace == get_current_namespace()
+def _assert_job_status_created(job_status):
+    assert "jobStatus" in job_status
 
-        var = [v for v in pod.spec.containers[0].env if v.name == "FOO"]
-        assert var and var[0].value == "BAR"
 
-        var = [v for v in pod.spec.containers[0].env if v.name == "A"]
-        assert var and var[0].value == "1"
-
-        assert pod.metadata.generate_name == "myname"
+def _assert_job_status_cluster_created(job, job_status):
+    assert "jobStatus" in job_status
+    assert job_status["clusterName"] == job
+    assert job_status["jobRunnerPodName"] == get_job_runner_pod_name(job)
+
+
+def _assert_job_status_running(job, job_status):
+    assert "jobStatus" in job_status
+    assert job_status["clusterName"] == job
+    assert job_status["jobRunnerPodName"] == get_job_runner_pod_name(job)
+    start_time = datetime.strptime(job_status["startTime"], KUBERNETES_DATETIME_FORMAT)
+    assert datetime.utcnow() > start_time > (datetime.utcnow() - timedelta(seconds=10))
+
+
+def _assert_final_job_status(job, job_status, expected_status):
+    assert job_status["jobStatus"] == expected_status
+    assert job_status["clusterName"] == job
+    assert job_status["jobRunnerPodName"] == get_job_runner_pod_name(job)
+    start_time = datetime.strptime(job_status["startTime"], KUBERNETES_DATETIME_FORMAT)
+    assert datetime.utcnow() > start_time > (datetime.utcnow() - timedelta(minutes=1))
+    end_time = datetime.strptime(job_status["endTime"], KUBERNETES_DATETIME_FORMAT)
+    assert datetime.utcnow() > end_time > (datetime.utcnow() - timedelta(minutes=1))
+    assert set(job_status.keys()) == {
+        "clusterName",
+        "jobRunnerPodName",
+        "jobStatus",
+        "startTime",
+        "endTime",
+    }
 
 
 @pytest.mark.anyio
-async def test_reject_evicted_workers(cluster):
-    cluster.scale(1)
-    await cluster
-
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 1:
-        await asyncio.sleep(0.1)
-        assert time() < start + 60
-
-    # Evict worker
-    [worker] = cluster.workers.values()
-    await cluster.core_api.create_namespaced_pod_eviction(
-        (await worker.describe_pod()).metadata.name,
-        (await worker.describe_pod()).metadata.namespace,
-        kubernetes.client.V1Eviction(
-            delete_options=kubernetes.client.V1DeleteOptions(grace_period_seconds=300),
-            metadata=(await worker.describe_pod()).metadata,
-        ),
-    )
+async def test_job(k8s_cluster, kopf_runner, gen_job):
+    with kopf_runner as runner:
+        async with gen_job("simplejob.yaml") as (job, ns):
+            assert job
+
+            runner_name = f"{job}-runner"
+
+            # Assert that job was created
+            while job not in k8s_cluster.kubectl(
+                "get", "daskjobs.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
 
-    # Wait until worker removal has been picked up by scheduler
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 0:
-        delta = time() - start
-        assert delta < 60, f"Scheduler failed to remove worker in {delta:.0f}s"
-        await asyncio.sleep(0.1)
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_job_status_created(job_status)
 
-    # Wait until worker removal has been handled by cluster
-    while len(cluster.workers) != 0:
-        delta = time() - start
-        assert delta < 60, f"Cluster failed to remove worker in {delta:.0f}s"
-        await asyncio.sleep(0.1)
+            # Assert that cluster is created
+            while job not in k8s_cluster.kubectl(
+                "get", "daskclusters.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
 
+            await asyncio.sleep(0.1)  # Wait for a short time, to avoid race condition
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_job_status_cluster_created(job, job_status)
 
-@pytest.mark.anyio
-async def test_scale_up_down(cluster, client):
-    np = pytest.importorskip("numpy")
-    cluster.scale(2)
-    await cluster
+            # Assert job pod is created
+            while job not in k8s_cluster.kubectl("get", "po", "-n", ns):
+                await asyncio.sleep(0.1)
 
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 2:
-        await asyncio.sleep(0.1)
-        assert time() < start + 60
+            # Assert that pod started Running
+            while "Running" not in k8s_cluster.kubectl("get", "po", "-n", ns):
+                await asyncio.sleep(0.1)
 
-    a, b = list(cluster.scheduler_info["workers"])
-    x = client.submit(np.ones, 1, workers=a)
-    y = client.submit(np.ones, 50_000, workers=b)
+            await asyncio.sleep(5)  # Wait for a short time, to avoid race condition
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_job_status_running(job, job_status)
+
+            job_annotations = json.loads(
+                k8s_cluster.kubectl(
+                    "get",
+                    "pods",
+                    "-n",
+                    ns,
+                    "--selector=dask.org/component=job-runner",
+                    "-o",
+                    "jsonpath='{.items[0].metadata.annotations}'",
+                )[1:-1]
+            )
+            assert _EXPECTED_ANNOTATIONS.items() <= job_annotations.items()
 
-    await wait([x, y])
+            # Assert job pod runs to completion (will fail if doesn't connect to cluster)
+            while "Completed" not in k8s_cluster.kubectl(
+                "get", "-n", ns, "po", runner_name
+            ):
+                await asyncio.sleep(0.1)
 
-    cluster.scale(1)
-    await cluster
+            # Assert cluster is removed on completion
+            while job in k8s_cluster.kubectl(
+                "get", "-n", ns, "daskclusters.kubernetes.dask.org"
+            ):
+                await asyncio.sleep(0.1)
 
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 1:
-        await asyncio.sleep(0.1)
-        assert time() < start + 60
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_final_job_status(job, job_status, "Successful")
 
-    # assert set(cluster.scheduler_info["workers"]) == {b}
+    assert "A DaskJob has been created" in runner.stdout
+    assert "Job succeeded, deleting Dask cluster." in runner.stdout
 
 
-@pytest.mark.xfail(
-    reason="The delay between scaling up, starting a worker, and then scale down causes issues"
-)
 @pytest.mark.anyio
-async def test_scale_up_down_fast(cluster, client):
-    cluster.scale(1)
-    await cluster
-
-    start = time()
-    await client.wait_for_workers(1)
-
-    worker = next(iter(cluster.scheduler_info["workers"].values()))
-
-    # Put some data on this worker
-    future = client.submit(lambda: b"\x00" * int(1e6))
-    await wait(future)
-    assert worker in cluster.scheduler.tasks[future.key].who_has
-
-    # Rescale the cluster many times without waiting: this should put some
-    # pressure on kubernetes but this should never fail nor delete our worker
-    # with the temporary result.
-    for i in range(10):
-        await cluster._scale_up(4)
-        await asyncio.sleep(random.random() / 2)
-        cluster.scale(1)
-        await asyncio.sleep(random.random() / 2)
+async def test_failed_job(k8s_cluster, kopf_runner, gen_job):
+    with kopf_runner as runner:
+        async with gen_job("failedjob.yaml") as (job, ns):
+            assert job
 
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 1:
-        await asyncio.sleep(0.1)
-        assert time() < start + 20
+            runner_name = f"{job}-runner"
 
-    # The original task result is still stored on the original worker: this pod
-    # has never been deleted when rescaling the cluster and the result can
-    # still be fetched back.
-    assert worker in cluster.scheduler.tasks[future.key].who_has
-    assert len(await future) == int(1e6)
-
-
-@pytest.mark.xfail(reason="scaling has some unfortunate state")
-@pytest.mark.anyio
-async def test_scale_down_pending(cluster, client, cleanup_namespaces):
-    # Try to scale the cluster to use more pods than available
-    nodes = (await cluster.core_api.list_node()).items
-    max_pods = sum(int(node.status.allocatable["pods"]) for node in nodes)
-    if max_pods > 50:
-        # It's probably not reasonable to run this test against a large
-        # kubernetes cluster.
-        pytest.skip("Require a small test kubernetes cluster (maxpod <= 50)")
-    extra_pods = 5
-    requested_pods = max_pods + extra_pods
-    cluster.scale(requested_pods)
+            # Assert that job was created
+            while job not in k8s_cluster.kubectl(
+                "get", "daskjobs.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
 
-    start = time()
-    while len(cluster.scheduler_info["workers"]) < 2:
-        await asyncio.sleep(0.1)
-        # Wait a bit because the kubernetes cluster can take time to provision
-        # the requested pods as we requested a large number of pods.
-        assert time() < start + 60
-
-    pending_pods = [p for p in (await cluster.pods()) if p.status.phase == "Pending"]
-    assert len(pending_pods) >= extra_pods
-
-    running_workers = list(cluster.scheduler_info["workers"].keys())
-    assert len(running_workers) >= 2
-
-    # Put some data on those workers to make them important to keep as long
-    # as possible.
-    def load_data(i):
-        return b"\x00" * (i * int(1e6))
-
-    futures = [
-        client.submit(load_data, i, workers=w) for i, w in enumerate(running_workers)
-    ]
-    await wait(futures)
-
-    # Reduce the cluster size down to the actually useful nodes: pending pods
-    # and running pods without results should be shutdown and removed first:
-    cluster.scale(len(running_workers))
-
-    start = time()
-    pod_statuses = [p.status.phase for p in await cluster.pods()]
-    while len(pod_statuses) != len(running_workers):
-        if time() - start > 60:
-            raise AssertionError(
-                "Expected %d running pods but got %r"
-                % (len(running_workers), pod_statuses)
-            )
-        await asyncio.sleep(0.1)
-        pod_statuses = [p.status.phase for p in await cluster.pods()]
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_job_status_created(job_status)
 
-    assert pod_statuses == ["Running"] * len(running_workers)
-    assert list(cluster.scheduler_info["workers"].keys()) == running_workers
+            # Assert that cluster is created
+            while job not in k8s_cluster.kubectl(
+                "get", "daskclusters.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
 
-    # Terminate everything
-    cluster.scale(0)
+            await asyncio.sleep(0.1)  # Wait for a short time, to avoid race condition
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_job_status_cluster_created(job, job_status)
 
-    start = time()
-    while len(cluster.scheduler_info["workers"]) > 0:
-        await asyncio.sleep(0.1)
-        assert time() < start + 60
+            # Assert job pod is created
+            while job not in k8s_cluster.kubectl("get", "po", "-n", ns):
+                await asyncio.sleep(0.1)
 
+            # Assert that pod started Running
+            while "Running" not in k8s_cluster.kubectl("get", "po", "-n", ns):
+                await asyncio.sleep(0.1)
 
-@pytest.mark.anyio
-async def test_automatic_startup(k8s_cluster, docker_image):
-    test_yaml = {
-        "kind": "Pod",
-        "metadata": {"labels": {"foo": "bar"}},
-        "spec": {
-            "containers": [
-                {
-                    "args": [
-                        "dask-worker",
-                        "$(DASK_SCHEDULER_ADDRESS)",
-                        "--nthreads",
-                        "1",
-                    ],
-                    "image": docker_image,
-                    "name": KUBECLUSTER_CONTAINER_NAME,
-                }
-            ]
-        },
-    }
+            await asyncio.sleep(5)  # Wait for a short time, to avoid race condition
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_job_status_running(job, job_status)
+
+            # Assert job pod runs to failure
+            while "Error" not in k8s_cluster.kubectl(
+                "get", "po", "-n", ns, runner_name
+            ):
+                await asyncio.sleep(0.1)
 
-    with tmpfile(extension="yaml") as fn:
-        with open(fn, mode="w") as f:
-            yaml.dump(test_yaml, f)
-        with dask.config.set({"kubernetes.worker-template-path": fn}):
-            async with KubeCluster(**cluster_kwargs) as cluster:
-                assert cluster.pod_template.metadata.labels["foo"] == "bar"
-
-
-@pytest.mark.anyio
-async def test_repr(cluster):
-    for text in [repr(cluster), str(cluster)]:
-        assert "Box" not in text
-        assert (
-            cluster.scheduler.address in text
-            or cluster.scheduler.external_address in text
-        )
-
-
-@pytest.mark.anyio
-async def test_escape_username(k8s_cluster, pod_spec, monkeypatch):
-    monkeypatch.setenv("LOGNAME", "Foo!._")
-
-    async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
-        assert "foo" in cluster.name
-        assert "!" not in cluster.name
-        assert "." not in cluster.name
-        assert "_" not in cluster.name
-        assert "foo" in cluster.pod_template.metadata.labels["user"]
-
-
-@pytest.mark.anyio
-async def test_escape_name(k8s_cluster, pod_spec):
-    async with KubeCluster(pod_spec, name="foo@bar", **cluster_kwargs) as cluster:
-        assert "@" not in str(cluster.pod_template)
-
-
-@pytest.mark.anyio
-async def test_maximum(cluster):
-    with dask.config.set({"kubernetes.count.max": 1}):
-        with captured_logger("dask_kubernetes") as logger:
-            cluster.scale(10)
-            await cluster
-
-            start = time()
-            while len(cluster.scheduler_info["workers"]) <= 0:
-                await asyncio.sleep(0.1)
-                assert time() < start + 60
-            await asyncio.sleep(0.5)
-            while len(cluster.scheduler_info["workers"]) != 1:
-                await asyncio.sleep(0.1)
-                assert time() < start + 60
-
-        result = logger.getvalue()
-        assert "scale beyond maximum number of workers" in result.lower()
-
-
-def test_default_toleration(pod_spec):
-    tolerations = pod_spec.to_dict()["spec"]["tolerations"]
-    assert {
-        "key": "k8s.dask.org/dedicated",
-        "operator": "Equal",
-        "value": "worker",
-        "effect": "NoSchedule",
-        "toleration_seconds": None,
-    } in tolerations
-    assert {
-        "key": "k8s.dask.org_dedicated",
-        "operator": "Equal",
-        "value": "worker",
-        "effect": "NoSchedule",
-        "toleration_seconds": None,
-    } in tolerations
-
-
-def test_default_toleration_preserved(docker_image):
-    pod_spec = clean_pod_template(
-        make_pod_spec(
-            image=docker_image,
-            extra_pod_config={
-                "tolerations": [
-                    {
-                        "key": "example.org/toleration",
-                        "operator": "Exists",
-                        "effect": "NoSchedule",
-                    }
-                ]
-            },
-        )
-    )
-    tolerations = pod_spec.to_dict()["spec"]["tolerations"]
-    assert {
-        "key": "k8s.dask.org/dedicated",
-        "operator": "Equal",
-        "value": "worker",
-        "effect": "NoSchedule",
-        "toleration_seconds": None,
-    } in tolerations
-    assert {
-        "key": "k8s.dask.org_dedicated",
-        "operator": "Equal",
-        "value": "worker",
-        "effect": "NoSchedule",
-        "toleration_seconds": None,
-    } in tolerations
-    assert {
-        "key": "example.org/toleration",
-        "operator": "Exists",
-        "effect": "NoSchedule",
-    } in tolerations
+            # Assert cluster is removed on completion
+            while job in k8s_cluster.kubectl(
+                "get", "-n", ns, "daskclusters.kubernetes.dask.org"
+            ):
+                await asyncio.sleep(0.1)
 
+            job_status = _get_job_status(k8s_cluster, ns)
+            _assert_final_job_status(job, job_status, "Failed")
 
-@pytest.mark.anyio
-async def test_auth_missing(k8s_cluster, pod_spec):
-    with pytest.raises(kubernetes.config.ConfigException) as info:
-        await KubeCluster(pod_spec, auth=[], **cluster_kwargs)
-
-    assert "No authorization methods were provided" in str(info.value)
+    assert "A DaskJob has been created" in runner.stdout
+    assert "Job failed, deleting Dask cluster." in runner.stdout
 
 
 @pytest.mark.anyio
-async def test_auth_tries_all_methods(k8s_cluster, pod_spec):
-    fails = {"count": 0}
-
-    class FailAuth(ClusterAuth):
-        def load(self):
-            fails["count"] += 1
-            raise kubernetes.config.ConfigException("Fail #{count}".format(**fails))
-
-    with pytest.raises(kubernetes.config.ConfigException) as info:
-        await KubeCluster(pod_spec, auth=[FailAuth()] * 3, **cluster_kwargs)
+async def test_object_dask_cluster(k8s_cluster, kopf_runner, gen_cluster):
+    with kopf_runner:
+        async with gen_cluster() as (cluster_name, ns):
+            cluster = await DaskCluster.get(cluster_name, namespace=ns)
 
-    assert "Fail #3" in str(info.value)
-    assert fails["count"] == 3
+            worker_groups = []
+            while not worker_groups:
+                worker_groups = await cluster.worker_groups()
+                await asyncio.sleep(0.1)
+            assert len(worker_groups) == 1  # Just the default worker group
+            wg = worker_groups[0]
+            assert isinstance(wg, DaskWorkerGroup)
+
+            # Test for non-replicated environment variables; Fix for https://github.com/dask/dask-kubernetes/issues/841
+            for deployment in await wg.deployments():
+                env_vars = deployment.spec["template"]["spec"]["containers"]["env"]
+                env_var_names = [env_var["name"] for env_var in env_vars]
+                assert len(env_var_names) == len(set(env_var_names))
+                assert "DASK_WORKER_NAME" in env_var_names
+                assert "DASK_SCHEDULER_ADDRESS" in env_var_names
+
+            scheduler_pod = await cluster.scheduler_pod()
+            assert isinstance(scheduler_pod, Pod)
+
+            scheduler_deployment = await cluster.scheduler_deployment()
+            assert isinstance(scheduler_deployment, Deployment)
+
+            scheduler_service = await cluster.scheduler_service()
+            assert isinstance(scheduler_service, Service)
 
 
-@pytest.mark.xfail(
-    reason="Updating the default client configuration is broken in kubernetes"
-)
 @pytest.mark.anyio
-async def test_auth_kubeconfig_with_filename():
-    await KubeConfig(config_file=CONFIG_DEMO).load()
-
-    # we've set the default configuration, so check that it is default
-    config = kubernetes.client.Configuration()
-    assert config.host == "https://1.2.3.4"
-    assert config.cert_file == FAKE_CERT
-    assert config.key_file == FAKE_KEY
-    assert config.ssl_ca_cert == FAKE_CA
+async def test_object_dask_worker_group(
+    k8s_cluster, kopf_runner, gen_cluster, gen_worker_group
+):
+    with kopf_runner:
+        async with (
+            gen_cluster() as (cluster_name, ns),
+            gen_worker_group("simpleworkergroup.yaml") as (
+                additional_workergroup_name,
+                _,
+            ),
+        ):
+            cluster = await DaskCluster.get(cluster_name, namespace=ns)
+            additional_workergroup = await DaskWorkerGroup.get(
+                additional_workergroup_name, namespace=ns
+            )
 
+            worker_groups = []
+            while not worker_groups:
+                worker_groups = await cluster.worker_groups()
+                await asyncio.sleep(0.1)
+            assert len(worker_groups) == 1  # Just the default worker group
+            worker_groups = worker_groups + [additional_workergroup]
 
-@pytest.mark.xfail(
-    reason="Updating the default client configuration is broken in kubernetes"
-)
-@pytest.mark.anyio
-async def test_auth_kubeconfig_with_context():
-    await KubeConfig(config_file=CONFIG_DEMO, context="exp-scratch").load()
+            for wg in worker_groups:
+                assert isinstance(wg, DaskWorkerGroup)
 
-    # we've set the default configuration, so check that it is default
-    config = kubernetes.client.Configuration()
-    assert config.host == "https://5.6.7.8"
-    assert config.api_key["authorization"] == "Basic {}".format(
-        base64.b64encode(b"exp:some-password").decode("ascii")
-    )
+                deployments = []
+                while not deployments:
+                    deployments = await wg.deployments()
+                    await asyncio.sleep(0.1)
+                assert all([isinstance(d, Deployment) for d in deployments])
+
+                pods = []
+                while not pods:
+                    pods = await wg.pods()
+                    await asyncio.sleep(0.1)
+                assert all([isinstance(p, Pod) for p in pods])
+
+                assert (await wg.cluster()).name == cluster.name
+
+                for deployment in deployments:
+                    assert deployment.labels["dask.org/cluster-name"] == cluster.name
+                    for env in deployment.spec["template"]["spec"]["containers"][0][
+                        "env"
+                    ]:
+                        if env["name"] == "DASK_WORKER_NAME":
+                            if wg.name == additional_workergroup_name:
+                                assert env["value"] == "test-worker"
+                            else:
+                                assert env["value"] == deployment.name
+                        if env["name"] == "DASK_SCHEDULER_ADDRESS":
+                            scheduler_service = await cluster.scheduler_service()
+                            assert f"{scheduler_service.name}.{ns}" in env["value"]
 
 
-@pytest.mark.xfail(
-    reason="Updating the default client configuration is broken in async kubernetes"
-)
 @pytest.mark.anyio
-async def test_auth_explicit():
-    await KubeAuth(
-        host="https://9.8.7.6", username="abc", password="some-password"
-    ).load()
-
-    config = kubernetes.client.Configuration()
-    assert config.host == "https://9.8.7.6"
-    assert config.username == "abc"
-    assert config.password == "some-password"
-    assert config.get_basic_auth_token() == "Basic {}".format(
-        base64.b64encode(b"abc:some-password").decode("ascii")
-    )
+@pytest.mark.skip(reason="Flaky in CI")
+async def test_object_dask_job(k8s_cluster, kopf_runner, gen_job):
+    with kopf_runner:
+        async with gen_job("simplejob.yaml") as (job_name, ns):
+            job = await DaskJob.get(job_name, namespace=ns)
 
+            job_pod = await job.pod()
+            assert isinstance(job_pod, Pod)
 
-@pytest.mark.anyio
-async def test_start_with_workers(k8s_cluster, pod_spec):
-    async with KubeCluster(pod_spec, n_workers=2, **cluster_kwargs) as cluster:
-        async with Client(cluster, asynchronous=True) as client:
-            await client.wait_for_workers(2)
+            cluster = await job.cluster()
+            assert isinstance(cluster, DaskCluster)
 
 
-@pytest.mark.anyio
-@pytest.mark.xfail(reason="Flaky in CI and classic is deprecated anyway")
-async def test_adapt_delete(cluster, ns):
+async def _get_cluster_status(k8s_cluster, ns, cluster_name):
     """
-    testing whether KubeCluster.adapt will bring
-    back deleted worker pod (issue #244)
+    Will loop infinitely in search of non-falsey cluster status.
+    Make sure there is a timeout on any test which calls this.
     """
-    core_api = cluster.core_api
-
-    async def get_worker_pods():
-        pods_list = await core_api.list_namespaced_pod(
-            namespace=ns,
-            label_selector=f"dask.org/component=worker,dask.org/cluster-name={cluster.name}",
-        )
-        return [x.metadata.name for x in pods_list.items]
-
-    cluster.adapt(maximum=2, minimum=2)
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 2:
-        await asyncio.sleep(0.1)
-        assert time() < start + 60
-
-    worker_pods = await get_worker_pods()
-    assert len(worker_pods) == 2
-    # delete one worker pod
-    to_delete = worker_pods[0]
-    await core_api.delete_namespaced_pod(name=to_delete, namespace=ns)
-    # wait until it is deleted
-    start = time()
     while True:
-        worker_pods = await get_worker_pods()
-        if to_delete not in worker_pods:
-            break
+        cluster_status = k8s_cluster.kubectl(
+            "get",
+            "-n",
+            ns,
+            "daskcluster.kubernetes.dask.org",
+            cluster_name,
+            "-o",
+            "jsonpath='{.status.phase}'",
+        ).strip("'")
+        if cluster_status:
+            return cluster_status
         await asyncio.sleep(0.1)
-        assert time() < start + 60
-    # test whether adapt will bring it back
-    start = time()
-    while len(cluster.scheduler_info["workers"]) != 2:
-        await asyncio.sleep(0.1)
-        assert time() < start + 60
-    assert len(cluster.scheduler_info["workers"]) == 2
 
 
-@pytest.mark.anyio
-@pytest.mark.xfail(reason="Failing in CI with FileNotFoundError")
-async def test_auto_refresh(cluster):
-    config = {
-        "apiVersion": "v1",
-        "clusters": [
-            {
-                "cluster": {"certificate-authority-data": "", "server": ""},
-                "name": "mock_gcp_config",
-            }
-        ],
-        "contexts": [
-            {
-                "context": {
-                    "cluster": "mock_gcp_config",
-                    "user": "mock_gcp_config",
-                },
-                "name": "mock_gcp_config",
-            }
-        ],
-        "current-context": "mock_gcp_config",
-        "kind": "config",
-        "preferences": {},
-        "users": [
-            {
-                "name": "mock_gcp_config",
-                "user": {
-                    "auth-provider": {
-                        "config": {
-                            "access-token": "",
-                            "cmd-args": "--fake-arg arg",
-                            "cmd-path": f"{sys.executable} {TEST_DIR}/fake_gcp_auth.py",
-                            "expiry": "",
-                            "expiry-key": "{.credential.token_expiry}",
-                            "toekn-key": "{.credential.access_token}",
-                        },
-                        "name": "gcp",
-                    }
-                },
-            }
-        ],
-    }
-    config_persister = False
-
-    loader = dask_kubernetes.AutoRefreshKubeConfigLoader(
-        config_dict=config,
-        config_base_path=None,
-        config_persister=config_persister,
-    )
-
-    await loader.load_gcp_token()
-    # Check that we get back a token
-    assert loader.token == f"Bearer {'0' * 137}"
-
-    next_expire = loader.token_expire_ts
-    for task in asyncio.all_tasks():
-        if task.get_name() == "dask_auth_auto_refresh":
-            await asyncio.wait_for(task, 10)
-
-    # Ensure that our token expiration timer was refreshed
-    assert loader.token_expire_ts > next_expire
-
-    # Ensure refresh task was re-created
-    for task in asyncio.all_tasks():
-        if task.get_name() == "dask_auth_auto_refresh":
-            loader.auto_refresh = False
-            await asyncio.wait_for(task, 60)
-            break
-    else:
-        assert False
+@pytest.mark.timeout(180)
+@pytest.mark.anyio
+@pytest.mark.parametrize(
+    "cluster_name,expected_status",
+    [
+        ("valid-name", "Created"),
+        ((MAX_CLUSTER_NAME_LEN + 1) * "a", "Error"),
+        ("invalid.chars.in.name", "Error"),
+    ],
+)
+async def test_create_cluster_validates_name(
+    cluster_name, expected_status, k8s_cluster, kopf_runner, gen_cluster
+):
+    with kopf_runner:
+        async with gen_cluster(cluster_name=cluster_name) as (_, ns):
+            actual_status = await _get_cluster_status(k8s_cluster, ns, cluster_name)
+            assert expected_status == actual_status
```

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/cli/cli.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/common/networking.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/networking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import asyncio
 import random
 import socket
-import subprocess
+import threading
 import time
 from contextlib import suppress
-from weakref import finalize
 
 import kr8s
-import kubernetes_asyncio as kubernetes
 from distributed.core import rpc
-from kr8s.asyncio.objects import Pod
+from kr8s.asyncio.objects import Pod, Service
 from tornado.iostream import StreamClosedError
 
-from dask_kubernetes.common.utils import check_dependency
 from dask_kubernetes.exceptions import CrashLoopBackOffError
 
 
 async def get_internal_address_for_scheduler_service(
     service,
     port_forward_cluster_ip=None,
     service_name_resolution_retries=20,
@@ -40,30 +37,29 @@
     port = await port_forward_service(
         service.metadata.name, service.metadata.namespace, port, local_port
     )
     return f"tcp://{host}:{port}"
 
 
 async def get_external_address_for_scheduler_service(
-    core_api,
     service,
     port_forward_cluster_ip=None,
     service_name_resolution_retries=20,
     port_name="tcp-comm",
     local_port=None,
 ):
     """Take a service object and return the scheduler address."""
     if service.spec.type == "LoadBalancer":
         port = _get_port(service, port_name)
         lb = service.status.load_balancer.ingress[0]
         host = lb.hostname or lb.ip
     elif service.spec.type == "NodePort":
         port = _get_port(service, port_name, is_node_port=True)
-        nodes = await core_api.list_node()
-        host = nodes.items[0].status.addresses[0].address
+        nodes = await kr8s.asyncio.get("nodes")
+        host = nodes[0].status.addresses[0].address
     elif service.spec.type == "ClusterIP":
         port = _get_port(service, port_name)
         if not port_forward_cluster_ip:
             with suppress(socket.gaierror):
                 # Try to resolve the service name. If we are inside the cluster this should succeed.
                 host = f"{service.metadata.name}.{service.metadata.namespace}"
                 if await _is_service_available(
@@ -122,38 +118,44 @@
             return guess
         except OSError:
             retries -= 1
     raise ConnectionError("Not able to find a free port.")
 
 
 async def port_forward_service(service_name, namespace, remote_port, local_port=None):
-    check_dependency("kubectl")
     if not local_port:
         local_port = _random_free_port(49152, 65535)  # IANA suggested range
     elif _port_in_use(local_port):
         raise ConnectionError("Specified Port already in use.")
-    kproc = subprocess.Popen(
-        [
-            "kubectl",
-            "port-forward",
-            "--address",
-            "0.0.0.0",
-            "--namespace",
-            f"{namespace}",
-            f"service/{service_name}",
-            f"{local_port}:{remote_port}",
-        ],
-        stdout=subprocess.DEVNULL,
-        stderr=subprocess.DEVNULL,
+    pf = threading.Thread(
+        name=f"DaskKubernetesPortForward ({namespace}/{service_name} {local_port}->{remote_port})",
+        target=run_port_forward,
+        args=(
+            service_name,
+            namespace,
+            remote_port,
+            local_port,
+        ),
+        daemon=True,
     )
-    finalize(kproc, kproc.kill)
+    pf.start()
 
     if await is_comm_open("localhost", local_port, retries=2000):
         return local_port
-    raise ConnectionError("kubectl port forward failed")
+    raise ConnectionError("port forward failed")
+
+
+def run_port_forward(service_name, namespace, remote_port, local_port):
+    async def _run():
+        svc = await Service.get(service_name, namespace=namespace)
+        async with svc.portforward(remote_port, local_port):
+            while True:
+                await asyncio.sleep(0.1)
+
+    asyncio.run(_run())
 
 
 async def is_comm_open(ip, port, retries=200):
     while retries > 0:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             result = sock.connect_ex((ip, port))
         if result == 0:
@@ -173,33 +175,30 @@
     service_name,
     namespace,
     port_name="tcp-comm",
     port_forward_cluster_ip=None,
     local_port=None,
     allow_external=True,
 ):
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        api = kubernetes.client.CoreV1Api(api_client)
-        service = await api.read_namespaced_service(service_name, namespace)
-        if allow_external:
-            address = await get_external_address_for_scheduler_service(
-                api,
-                service,
-                port_forward_cluster_ip=port_forward_cluster_ip,
-                port_name=port_name,
-                local_port=local_port,
-            )
-        else:
-            address = await get_internal_address_for_scheduler_service(
-                service,
-                port_forward_cluster_ip=port_forward_cluster_ip,
-                port_name=port_name,
-                local_port=local_port,
-            )
-        return address
+    service = await Service.get(service_name, namespace=namespace)
+    if allow_external:
+        address = await get_external_address_for_scheduler_service(
+            service,
+            port_forward_cluster_ip=port_forward_cluster_ip,
+            port_name=port_name,
+            local_port=local_port,
+        )
+    else:
+        address = await get_internal_address_for_scheduler_service(
+            service,
+            port_forward_cluster_ip=port_forward_cluster_ip,
+            port_name=port_name,
+            local_port=local_port,
+        )
+    return address
 
 
 async def wait_for_scheduler(cluster_name, namespace, timeout=None):
     pod_start_time = None
     while True:
         try:
             pod = await Pod.get(
```

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/conftest.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import logging
 import os
 import pathlib
+import shutil
 import subprocess
 import sys
 import tempfile
 import uuid
 
 import pytest
 from kopf.testing import KopfRunner
 from pytest_kind.cluster import KindCluster
 
-from dask_kubernetes.common.utils import check_dependency
-
 DIR = pathlib.Path(__file__).parent.absolute()
 
+
+def check_dependency(dependency):
+    if shutil.which(dependency) is None:
+        raise RuntimeError(
+            f"Missing dependency {dependency}. "
+            f"Please install {dependency} following the instructions for your OS. "
+        )
+
+
 check_dependency("helm")
 check_dependency("kubectl")
 check_dependency("docker")
 
 DISABLE_LOGGERS = ["httpcore", "httpx"]
```

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/kubernetes.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/_objects.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/controller.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 import kopf
 import kr8s
 import pkg_resources
 from distributed.core import clean_exception, rpc
 from distributed.protocol.pickle import dumps
 from kr8s.asyncio.objects import Deployment, Pod, Service
 
-from dask_kubernetes.common.objects import validate_cluster_name
 from dask_kubernetes.constants import SCHEDULER_NAME_TEMPLATE
 from dask_kubernetes.exceptions import ValidationError
 from dask_kubernetes.operator._objects import (
     DaskAutoscaler,
     DaskCluster,
     DaskJob,
     DaskWorkerGroup,
 )
 from dask_kubernetes.operator.networking import get_scheduler_address
+from dask_kubernetes.operator.validation import validate_cluster_name
 
 _ANNOTATION_NAMESPACES_TO_IGNORE = (
     "kopf.zalando.org",
     "kubectl.kubernetes.io",
 )
 _LABEL_NAMESPACES_TO_IGNORE = ()
```

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/templates.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 from rich.console import Group
 from rich.live import Live
 from rich.panel import Panel
 from rich.spinner import Spinner
 from rich.table import Table
 from tornado.ioloop import IOLoop
 
-from dask_kubernetes.common.objects import validate_cluster_name
 from dask_kubernetes.exceptions import CrashLoopBackOffError, SchedulerStartupError
 from dask_kubernetes.operator._objects import (
     DaskAutoscaler,
     DaskCluster,
     DaskWorkerGroup,
 )
 from dask_kubernetes.operator.networking import (
     get_scheduler_address,
     wait_for_scheduler,
     wait_for_scheduler_comm,
 )
+from dask_kubernetes.operator.validation import validate_cluster_name
 
 logger = logging.getLogger(__name__)
 
 
 class CreateMode(Enum):
     CREATE_ONLY = "CREATE_ONLY"
     CREATE_OR_CONNECT = "CREATE_OR_CONNECT"
```

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask_kubernetes-2024.5.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,14 @@
 from distributed.utils import TimeoutError
 
 from dask_kubernetes.constants import MAX_CLUSTER_NAME_LEN
 from dask_kubernetes.exceptions import SchedulerStartupError, ValidationError
 from dask_kubernetes.operator import KubeCluster, make_cluster_spec
 
 
-def test_experimental_shim():
-    with pytest.deprecated_call():
-        from dask_kubernetes.experimental import KubeCluster as ExperimentalKubeCluster
-
-    assert ExperimentalKubeCluster is KubeCluster
-
-
 def test_kubecluster(kopf_runner, docker_image, ns):
     with kopf_runner:
         with KubeCluster(
             name="cluster", namespace=ns, image=docker_image, n_workers=1
         ) as cluster:
             with Client(cluster) as client:
                 client.scheduler_info()
@@ -77,35 +70,41 @@
             assert cluster1.forwarded_dashboard_port == "8888"
             with Client(cluster1) as client1:
                 assert client1.submit(lambda x: x + 1, 10).result() == 11
 
 
 def test_multiple_clusters_simultaneously(kopf_runner, docker_image, ns):
     with kopf_runner:
-        with KubeCluster(
-            name="fizz", image=docker_image, n_workers=1, namespace=ns
-        ) as cluster1, KubeCluster(
-            name="buzz", image=docker_image, n_workers=1, namespace=ns
-        ) as cluster2:
+        with (
+            KubeCluster(
+                name="fizz", image=docker_image, n_workers=1, namespace=ns
+            ) as cluster1,
+            KubeCluster(
+                name="buzz", image=docker_image, n_workers=1, namespace=ns
+            ) as cluster2,
+        ):
             with Client(cluster1) as client1, Client(cluster2) as client2:
                 assert client1.submit(lambda x: x + 1, 10).result() == 11
                 assert client2.submit(lambda x: x + 1, 10).result() == 11
 
 
 def test_multiple_clusters_simultaneously_same_loop(kopf_runner, docker_image, ns):
     with kopf_runner:
-        with KubeCluster(
-            name="fizz", image=docker_image, n_workers=1, namespace=ns
-        ) as cluster1, KubeCluster(
-            name="buzz",
-            image=docker_image,
-            loop=cluster1.loop,
-            n_workers=1,
-            namespace=ns,
-        ) as cluster2:
+        with (
+            KubeCluster(
+                name="fizz", image=docker_image, n_workers=1, namespace=ns
+            ) as cluster1,
+            KubeCluster(
+                name="buzz",
+                image=docker_image,
+                loop=cluster1.loop,
+                n_workers=1,
+                namespace=ns,
+            ) as cluster2,
+        ):
             with Client(cluster1) as client1, Client(cluster2) as client2:
                 assert cluster1.loop is cluster2.loop is client1.loop is client2.loop
                 assert client1.submit(lambda x: x + 1, 10).result() == 11
                 assert client2.submit(lambda x: x + 1, 10).result() == 11
 
 
 @pytest.mark.anyio
```

