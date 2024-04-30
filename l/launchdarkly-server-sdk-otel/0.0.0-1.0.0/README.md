# Comparing `tmp/launchdarkly_server_sdk_otel-0.0.0.tar.gz` & `tmp/launchdarkly_server_sdk_otel-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchdarkly_server_sdk_otel-0.0.0.tar", last modified: Wed Apr 24 15:42:16 2024, max compression
+gzip compressed data, was "launchdarkly_server_sdk_otel-1.0.0.tar", max compression
```

## Comparing `launchdarkly_server_sdk_otel-0.0.0.tar` & `launchdarkly_server_sdk_otel-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,8 @@
-drwxr-xr-x   0 mkeeler   (1000) mkeeler   (1000)        0 2024-04-24 15:42:16.296593 launchdarkly_server_sdk_otel-0.0.0/
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)      143 2024-04-24 15:42:16.296593 launchdarkly_server_sdk_otel-0.0.0/PKG-INFO
-drwxr-xr-x   0 mkeeler   (1000) mkeeler   (1000)        0 2024-04-24 15:42:16.296593 launchdarkly_server_sdk_otel-0.0.0/launchdarkly_server_sdk_otel.egg-info/
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)      143 2024-04-24 15:42:16.000000 launchdarkly_server_sdk_otel-0.0.0/launchdarkly_server_sdk_otel.egg-info/PKG-INFO
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)      241 2024-04-24 15:42:16.000000 launchdarkly_server_sdk_otel-0.0.0/launchdarkly_server_sdk_otel.egg-info/SOURCES.txt
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)        1 2024-04-24 15:42:16.000000 launchdarkly_server_sdk_otel-0.0.0/launchdarkly_server_sdk_otel.egg-info/dependency_links.txt
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)        7 2024-04-24 15:42:16.000000 launchdarkly_server_sdk_otel-0.0.0/launchdarkly_server_sdk_otel.egg-info/top_level.txt
-drwxr-xr-x   0 mkeeler   (1000) mkeeler   (1000)        0 2024-04-24 15:42:16.296593 launchdarkly_server_sdk_otel-0.0.0/ldotel/
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)        0 2024-04-24 15:40:23.000000 launchdarkly_server_sdk_otel-0.0.0/ldotel/__init__.py
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)      169 2024-04-24 15:42:12.000000 launchdarkly_server_sdk_otel-0.0.0/pyproject.toml
--rw-r--r--   0 mkeeler   (1000) mkeeler   (1000)       38 2024-04-24 15:42:16.296593 launchdarkly_server_sdk_otel-0.0.0/setup.cfg
+-rw-r--r--   0        0        0      557 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4592 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/README.md
+-rw-r--r--   0        0        0       50 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/ldotel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/ldotel/testing/__init__.py
+-rw-r--r--   0        0        0     6334 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/ldotel/testing/test_tracing.py
+-rw-r--r--   0        0        0     3786 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/ldotel/tracing.py
+-rw-r--r--   0        0        0     1812 2024-04-30 19:48:09.377712 launchdarkly_server_sdk_otel-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 launchdarkly_server_sdk_otel-1.0.0/PKG-INFO
```

