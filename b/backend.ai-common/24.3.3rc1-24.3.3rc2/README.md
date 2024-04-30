# Comparing `tmp/backend.ai-common-24.3.3rc1.tar.gz` & `tmp/backend.ai-common-24.3.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-24.3.3rc1.tar", last modified: Mon Apr 29 16:32:29 2024, max compression
+gzip compressed data, was "backend.ai-common-24.3.3rc2.tar", last modified: Tue Apr 30 06:26:17 2024, max compression
```

## Comparing `backend.ai-common-24.3.3rc1.tar` & `backend.ai-common-24.3.3rc2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.412608 backend.ai-common-24.3.3rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-29 16:32:29.412608 backend.ai-common-24.3.3rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.384607 backend.ai-common-24.3.3rc1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.384607 backend.ai-common-24.3.3rc1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.408608 backend.ai-common-24.3.3rc1/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.408608 backend.ai-common-24.3.3rc1/ai/backend/common/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21031 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19400 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/etcd_etcetra.py
--rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    23163 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.384607 backend.ai-common-24.3.3rc1/ai/backend/common/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.408608 backend.ai-common-24.3.3rc1/ai/backend/common/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/ai/backend/common/models/minilang/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/netns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.408608 backend.ai-common-24.3.3rc1/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/typed_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    37609 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25051 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.384607 backend.ai-common-24.3.3rc1/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.408608 backend.ai-common-24.3.3rc1/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:29.412608 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-29 16:32:29.000000 backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:32:29.412608 backend.ai-common-24.3.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-29 16:32:28.000000 backend.ai-common-24.3.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.919759 backend.ai-common-24.3.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-30 06:26:17.919759 backend.ai-common-24.3.3rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.887759 backend.ai-common-24.3.3rc2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.887759 backend.ai-common-24.3.3rc2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.915759 backend.ai-common-24.3.3rc2/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.915759 backend.ai-common-24.3.3rc2/ai/backend/common/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21031 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19400 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/etcd_etcetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23163 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.887759 backend.ai-common-24.3.3rc2/ai/backend/common/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.915759 backend.ai-common-24.3.3rc2/ai/backend/common/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/models/minilang/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.915759 backend.ai-common-24.3.3rc2/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/typed_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37609 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25051 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.887759 backend.ai-common-24.3.3rc2/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.915759 backend.ai-common-24.3.3rc2/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.915759 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:26:17.919759 backend.ai-common-24.3.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-30 06:26:17.000000 backend.ai-common-24.3.3rc2/setup.py
```

### Comparing `backend.ai-common-24.3.3rc1/PKG-INFO` & `backend.ai-common-24.3.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 24.3.3rc1
+Version: 24.3.3rc2
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: asynctest>=0.13.0
 Requires-Dist: asyncudp>=0.4
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-plugin==24.03.3rc1
+Requires-Dist: backend.ai-plugin==24.03.3rc2
 Requires-Dist: callosum~=1.0.3
 Requires-Dist: click~=8.1.7
 Requires-Dist: coloredlogs~=15.0
 Requires-Dist: etcd-client-py==0.3.0
 Requires-Dist: etcetra~=0.1.19
 Requires-Dist: graypy==2.1.0
 Requires-Dist: ifaddr~=0.2
```

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/argparse.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/asyncio.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/auth/__init__.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/bgtask.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/cgroup.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/cgroup.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/cli.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/config.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/distributed.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/docker.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/enum_extension.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/enum_extension.pyi` & `backend.ai-common-24.3.3rc2/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/etcd.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/etcd_etcetra.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/etcd_etcetra.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/events.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/exception.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/files.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/identity.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/lock.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/lock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/logging.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/logging_utils.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/models/minilang/mount.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/models/minilang/mount.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/msgpack.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/netns.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/netns.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/networking.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/plugin/__init__.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/plugin/hook.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/plugin/monitor.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/redis_helper.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/redis_helper.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/sd_notify.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/service_ports.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/service_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/testutils.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/typed_validators.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/typed_validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/types.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/utils.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/validators.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/web/session/__init__.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/web/session/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-24.3.3rc2/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/PKG-INFO` & `backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 24.3.3rc1
+Version: 24.3.3rc2
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: asynctest>=0.13.0
 Requires-Dist: asyncudp>=0.4
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-plugin==24.03.3rc1
+Requires-Dist: backend.ai-plugin==24.03.3rc2
 Requires-Dist: callosum~=1.0.3
 Requires-Dist: click~=8.1.7
 Requires-Dist: coloredlogs~=15.0
 Requires-Dist: etcd-client-py==0.3.0
 Requires-Dist: etcetra~=0.1.19
 Requires-Dist: graypy==2.1.0
 Requires-Dist: ifaddr~=0.2
```

### Comparing `backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/backend.ai_common.egg-info/requires.txt` & `backend.ai-common-24.3.3rc2/backend.ai_common.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 aiohttp~=3.9.1
 aiomonitor~=0.7.0
 aiotools~=1.7.0
 async_timeout~=4.0
 asynctest>=0.13.0
 asyncudp>=0.4
 attrs>=20.3
-backend.ai-plugin==24.03.3rc1
+backend.ai-plugin==24.03.3rc2
 callosum~=1.0.3
 click~=8.1.7
 coloredlogs~=15.0
 etcd-client-py==0.3.0
 etcetra~=0.1.19
 graypy==2.1.0
 ifaddr~=0.2
```

### Comparing `backend.ai-common-24.3.3rc1/backend_shim.py` & `backend.ai-common-24.3.3rc2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.3rc1/setup.py` & `backend.ai-common-24.3.3rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==24.03.3rc1
+        """backend.ai-plugin==24.03.3rc2
 """,
         'callosum~=1.0.3',
         'click~=8.1.7',
         'coloredlogs~=15.0',
         'etcd-client-py==0.3.0',
         'etcetra~=0.1.19',
         'graypy==2.1.0',
@@ -127,11 +127,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.3rc1
+    'version': """24.03.3rc2
 """,
     'zip_safe': False,
 })
```

