# Comparing `tmp/firebolt_sdk-1.4.1.tar.gz` & `tmp/firebolt_sdk-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firebolt-python-sdk/firebolt-python-sdk/dist/.tmp-lg12hel_/firebolt_sdk-1.4.1.tar", last modified: Wed Apr 17 09:22:21 2024, max compression
+gzip compressed data, was "/home/runner/work/firebolt-python-sdk/firebolt-python-sdk/dist/.tmp-vyd95s1r/firebolt_sdk-1.4.2.tar", last modified: Tue Apr 30 12:33:30 2024, max compression
```

## Comparing `firebolt_sdk-1.4.1.tar` & `firebolt_sdk-1.4.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2221 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 09:22:15.000000 firebolt_sdk-1.4.1/src/firebolt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/async_db/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/client/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/request_auth_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/auth/username_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/client/resource_manager_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/common/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/base_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/token_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/db/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/db/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/model/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/engine_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V1/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/V2/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/model/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/service/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V1/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/V2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/service/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/token_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/usage_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-17 09:22:05.000000 firebolt_sdk-1.4.1/src/firebolt/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 09:22:20.000000 firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2229 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 12:33:26.000000 firebolt_sdk-1.4.2/src/firebolt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/async_db/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/async_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/async_db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/async_db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/async_db/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/request_auth_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/auth/username_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/client/resource_manager_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/base_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/token_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/db/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/model/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/engine_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V1/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/model/V2/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V2/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/V2/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/model/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/service/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V1/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/V2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/service/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/utils/token_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/utils/usage_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-30 12:33:15.000000 firebolt_sdk-1.4.2/src/firebolt/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 12:33:30.000000 firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/top_level.txt
```

### Comparing `firebolt_sdk-1.4.1/LICENSE` & `firebolt_sdk-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/PKG-INFO` & `firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firebolt_sdk
-Version: 1.4.1
+Name: firebolt-sdk
+Version: 1.4.2
 Summary: Python SDK for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sdk
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sdk/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `firebolt_sdk-1.4.1/README.md` & `firebolt_sdk-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/setup.cfg` & `firebolt_sdk-1.4.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 [options.extras_require]
 ciso8601 = 
 	ciso8601==2.2.0
 dev = 
 	allure-pytest==2.*
 	devtools==0.7.0
-	mypy==1.*
+	mypy==1.*,<1.10.0
 	pre-commit==2.15.0
 	pyfakefs>=4.5.3
 	pytest==7.2.0
 	pytest-cov==3.0.0
 	pytest-httpx>=0.13.0
 	pytest-mock==3.6.1
 	pytest-timeout==2.1.0
```

### Comparing `firebolt_sdk-1.4.1/src/firebolt/async_db/__init__.py` & `firebolt_sdk-1.4.2/src/firebolt/async_db/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/async_db/connection.py` & `firebolt_sdk-1.4.2/src/firebolt/async_db/connection.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/async_db/cursor.py` & `firebolt_sdk-1.4.2/src/firebolt/async_db/cursor.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/async_db/util.py` & `firebolt_sdk-1.4.2/src/firebolt/async_db/util.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/auth/base.py` & `firebolt_sdk-1.4.2/src/firebolt/client/auth/base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/auth/client_credentials.py` & `firebolt_sdk-1.4.2/src/firebolt/client/auth/client_credentials.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/auth/request_auth_base.py` & `firebolt_sdk-1.4.2/src/firebolt/client/auth/request_auth_base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/auth/service_account.py` & `firebolt_sdk-1.4.2/src/firebolt/client/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/auth/token.py` & `firebolt_sdk-1.4.2/src/firebolt/client/auth/token.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/auth/username_password.py` & `firebolt_sdk-1.4.2/src/firebolt/client/auth/username_password.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/client.py` & `firebolt_sdk-1.4.2/src/firebolt/client/client.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/http_backend.py` & `firebolt_sdk-1.4.2/src/firebolt/client/http_backend.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/client/resource_manager_hooks.py` & `firebolt_sdk-1.4.2/src/firebolt/client/resource_manager_hooks.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/common/_types.py` & `firebolt_sdk-1.4.2/src/firebolt/common/_types.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/common/base_connection.py` & `firebolt_sdk-1.4.2/src/firebolt/common/base_connection.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/common/base_cursor.py` & `firebolt_sdk-1.4.2/src/firebolt/common/base_cursor.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/common/settings.py` & `firebolt_sdk-1.4.2/src/firebolt/common/settings.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/db/__init__.py` & `firebolt_sdk-1.4.2/src/firebolt/db/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/db/connection.py` & `firebolt_sdk-1.4.2/src/firebolt/db/connection.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/db/cursor.py` & `firebolt_sdk-1.4.2/src/firebolt/db/cursor.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/db/util.py` & `firebolt_sdk-1.4.2/src/firebolt/db/util.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V1/__init__.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V1/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V1/binding.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V1/binding.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V1/database.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V1/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V1/engine.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V1/engine.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V2/__init__.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V2/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V2/database.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V2/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V2/engine.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V2/engine.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/model/V2/instance_type.py` & `firebolt_sdk-1.4.2/src/firebolt/model/V2/instance_type.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V1/base.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V1/base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V1/binding.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V1/binding.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V1/database.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V1/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V1/region.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V1/region.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V1/types.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V1/types.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V2/base.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V2/base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V2/database.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V2/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,21 +83,21 @@
             condition = []
             if name_contains:
                 condition.append("database_name like ?")
                 parameters.append(f"%{name_contains}%")
             if attached_engine_name_eq:
                 condition.append(
                     "any_match(eng -> split_part(eng, ' ', 1) = ?,"
-                    " split(',', attached_engines))"
+                    " string_to_array(attached_engines, ','))"
                 )
                 parameters.append(attached_engine_name_eq)
             if attached_engine_name_contains:
                 condition.append(
                     "any_match(eng -> split_part(eng, ' ', 1) like ?,"
-                    " split(',', attached_engines))"
+                    " string_to_array(attached_engines, ','))"
                 )
                 parameters.append(f"%{attached_engine_name_contains}%")
             if region_eq:
                 condition.append("region = ?")
                 parameters.append(str(region_eq))
             sql += self.GET_WHERE_SQL + " AND ".join(condition)
```

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V2/engine.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V2/engine.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V2/instance_type.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V2/instance_type.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/V2/types.py` & `firebolt_sdk-1.4.2/src/firebolt/service/V2/types.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/service/manager.py` & `firebolt_sdk-1.4.2/src/firebolt/service/manager.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/utils/exception.py` & `firebolt_sdk-1.4.2/src/firebolt/utils/exception.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/utils/token_storage.py` & `firebolt_sdk-1.4.2/src/firebolt/utils/token_storage.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/utils/urls.py` & `firebolt_sdk-1.4.2/src/firebolt/utils/urls.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/utils/usage_tracker.py` & `firebolt_sdk-1.4.2/src/firebolt/utils/usage_tracker.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt/utils/util.py` & `firebolt_sdk-1.4.2/src/firebolt/utils/util.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/PKG-INFO` & `firebolt_sdk-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firebolt-sdk
-Version: 1.4.1
+Name: firebolt_sdk
+Version: 1.4.2
 Summary: Python SDK for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sdk
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sdk/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/SOURCES.txt` & `firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-1.4.1/src/firebolt_sdk.egg-info/requires.txt` & `firebolt_sdk-1.4.2/src/firebolt_sdk.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [ciso8601]
 ciso8601==2.2.0
 
 [dev]
 allure-pytest==2.*
 devtools==0.7.0
-mypy==1.*
+mypy<1.10.0,==1.*
 pre-commit==2.15.0
 pyfakefs>=4.5.3
 pytest==7.2.0
 pytest-cov==3.0.0
 pytest-httpx>=0.13.0
 pytest-mock==3.6.1
 pytest-timeout==2.1.0
```

