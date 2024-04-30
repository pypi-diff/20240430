# Comparing `tmp/enhomie-0.2.2.tar.gz` & `tmp/enhomie-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhomie-0.2.2.tar", last modified: Thu Apr 25 02:32:13 2024, max compression
+gzip compressed data, was "enhomie-0.3.0.tar", last modified: Tue Apr 30 01:52:19 2024, max compression
```

## Comparing `enhomie-0.2.2.tar` & `enhomie-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.906729 enhomie-0.2.2/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-14 23:33:41.000000 enhomie-0.2.2/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       31 2024-03-14 23:35:40.000000 enhomie-0.2.2/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3454 2024-04-25 02:32:13.906729 enhomie-0.2.2/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3065 2024-04-25 02:26:08.000000 enhomie-0.2.2/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.904729 enhomie-0.2.2/enhomie/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.904729 enhomie-0.2.2/enhomie/builtins/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      423 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/builtins/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1644 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/builtins/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.904729 enhomie-0.2.2/enhomie/builtins/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/builtins/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      948 2024-04-25 01:47:19.000000 enhomie-0.2.2/enhomie/builtins/test/test_params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1277 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/builtins/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1778 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/builtins/when.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.904729 enhomie-0.2.2/enhomie/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2024 2024-04-08 05:15:33.000000 enhomie-0.2.2/enhomie/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2183 2024-04-23 07:21:16.000000 enhomie-0.2.2/enhomie/config/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.904729 enhomie-0.2.2/enhomie/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1205 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6000 2024-04-23 07:21:16.000000 enhomie-0.2.2/enhomie/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.905729 enhomie-0.2.2/enhomie/homie/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/homie/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6728 2024-04-25 02:26:08.000000 enhomie-0.2.2/enhomie/homie/desire.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5409 2024-04-25 02:26:08.000000 enhomie-0.2.2/enhomie/homie/group.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    15456 2024-04-24 23:58:04.000000 enhomie-0.2.2/enhomie/homie/homie.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3425 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/homie/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6075 2024-04-25 02:26:08.000000 enhomie-0.2.2/enhomie/homie/scene.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.905729 enhomie-0.2.2/enhomie/homie/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/homie/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2633 2024-04-15 08:22:12.000000 enhomie-0.2.2/enhomie/homie/test/test_desire.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2184 2024-04-15 08:22:39.000000 enhomie-0.2.2/enhomie/homie/test/test_group.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4354 2024-04-15 08:23:16.000000 enhomie-0.2.2/enhomie/homie/test/test_homie.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2587 2024-04-15 08:23:41.000000 enhomie-0.2.2/enhomie/homie/test/test_scene.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1303 2024-04-15 08:24:01.000000 enhomie-0.2.2/enhomie/homie/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3251 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/homie/when.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.905729 enhomie-0.2.2/enhomie/philipshue/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:09.000000 enhomie-0.2.2/enhomie/philipshue/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10528 2024-04-25 01:47:19.000000 enhomie-0.2.2/enhomie/philipshue/bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8007 2024-04-08 04:48:39.000000 enhomie-0.2.2/enhomie/philipshue/device.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1826 2024-04-14 14:22:48.000000 enhomie-0.2.2/enhomie/philipshue/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.906729 enhomie-0.2.2/enhomie/philipshue/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      635 2024-04-08 05:44:56.000000 enhomie-0.2.2/enhomie/philipshue/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5062 2024-04-25 01:47:19.000000 enhomie-0.2.2/enhomie/philipshue/test/test_bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3131 2024-04-15 08:24:45.000000 enhomie-0.2.2/enhomie/philipshue/test/test_device.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3263 2024-04-08 04:36:12.000000 enhomie-0.2.2/enhomie/philipshue/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2126 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/philipshue/when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-24 11:17:04.000000 enhomie-0.2.2/enhomie/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.906729 enhomie-0.2.2/enhomie/ubiquiti/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:29.000000 enhomie-0.2.2/enhomie/ubiquiti/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7558 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/ubiquiti/client.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1991 2024-04-14 14:21:10.000000 enhomie-0.2.2/enhomie/ubiquiti/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9316 2024-04-25 01:47:19.000000 enhomie-0.2.2/enhomie/ubiquiti/router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.906729 enhomie-0.2.2/enhomie/ubiquiti/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/ubiquiti/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4146 2024-04-15 08:25:06.000000 enhomie-0.2.2/enhomie/ubiquiti/test/test_client.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3494 2024-04-25 01:47:19.000000 enhomie-0.2.2/enhomie/ubiquiti/test/test_router.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2643 2024-04-08 04:36:08.000000 enhomie-0.2.2/enhomie/ubiquiti/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2148 2024-04-08 04:21:22.000000 enhomie-0.2.2/enhomie/ubiquiti/when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-25 02:28:56.000000 enhomie-0.2.2/enhomie/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:13.906729 enhomie-0.2.2/enhomie.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3454 2024-04-25 02:32:13.000000 enhomie-0.2.2/enhomie.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1568 2024-04-25 02:32:13.000000 enhomie-0.2.2/enhomie.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-25 02:32:13.000000 enhomie-0.2.2/enhomie.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-25 02:32:13.000000 enhomie-0.2.2/enhomie.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        8 2024-04-25 02:32:13.000000 enhomie-0.2.2/enhomie.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      521 2024-04-08 04:22:21.000000 enhomie-0.2.2/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-14 14:15:36.000000 enhomie-0.2.2/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-25 02:32:13.906729 enhomie-0.2.2/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.070260 enhomie-0.3.0/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-14 23:33:41.000000 enhomie-0.3.0/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       31 2024-03-14 23:35:40.000000 enhomie-0.3.0/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3454 2024-04-30 01:52:19.070260 enhomie-0.3.0/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3065 2024-04-25 02:26:08.000000 enhomie-0.3.0/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.068260 enhomie-0.3.0/enhomie/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.068260 enhomie-0.3.0/enhomie/builtins/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      423 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/builtins/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1644 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/builtins/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.068260 enhomie-0.3.0/enhomie/builtins/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/builtins/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      948 2024-04-25 01:47:19.000000 enhomie-0.3.0/enhomie/builtins/test/test_params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1277 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/builtins/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1778 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/builtins/when.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.068260 enhomie-0.3.0/enhomie/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2024 2024-04-08 05:15:33.000000 enhomie-0.3.0/enhomie/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2174 2024-04-30 01:49:23.000000 enhomie-0.3.0/enhomie/config/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.068260 enhomie-0.3.0/enhomie/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1205 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5966 2024-04-30 01:49:23.000000 enhomie-0.3.0/enhomie/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.068260 enhomie-0.3.0/enhomie/homie/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/homie/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6708 2024-04-30 01:49:23.000000 enhomie-0.3.0/enhomie/homie/desire.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5409 2024-04-25 02:26:08.000000 enhomie-0.3.0/enhomie/homie/group.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    15266 2024-04-30 01:49:23.000000 enhomie-0.3.0/enhomie/homie/homie.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3425 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/homie/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6075 2024-04-25 02:26:08.000000 enhomie-0.3.0/enhomie/homie/scene.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.069260 enhomie-0.3.0/enhomie/homie/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/homie/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2633 2024-04-15 08:22:12.000000 enhomie-0.3.0/enhomie/homie/test/test_desire.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2184 2024-04-15 08:22:39.000000 enhomie-0.3.0/enhomie/homie/test/test_group.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4354 2024-04-15 08:23:16.000000 enhomie-0.3.0/enhomie/homie/test/test_homie.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2587 2024-04-15 08:23:41.000000 enhomie-0.3.0/enhomie/homie/test/test_scene.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1303 2024-04-15 08:24:01.000000 enhomie-0.3.0/enhomie/homie/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3251 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/homie/when.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.069260 enhomie-0.3.0/enhomie/philipshue/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:09.000000 enhomie-0.3.0/enhomie/philipshue/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10510 2024-04-30 01:49:23.000000 enhomie-0.3.0/enhomie/philipshue/bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8007 2024-04-08 04:48:39.000000 enhomie-0.3.0/enhomie/philipshue/device.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1826 2024-04-14 14:22:48.000000 enhomie-0.3.0/enhomie/philipshue/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.069260 enhomie-0.3.0/enhomie/philipshue/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      635 2024-04-08 05:44:56.000000 enhomie-0.3.0/enhomie/philipshue/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5062 2024-04-25 01:47:19.000000 enhomie-0.3.0/enhomie/philipshue/test/test_bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3131 2024-04-15 08:24:45.000000 enhomie-0.3.0/enhomie/philipshue/test/test_device.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3263 2024-04-08 04:36:12.000000 enhomie-0.3.0/enhomie/philipshue/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2126 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/philipshue/when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-24 11:17:04.000000 enhomie-0.3.0/enhomie/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.069260 enhomie-0.3.0/enhomie/ubiquiti/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:29.000000 enhomie-0.3.0/enhomie/ubiquiti/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7558 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/ubiquiti/client.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1991 2024-04-14 14:21:10.000000 enhomie-0.3.0/enhomie/ubiquiti/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9298 2024-04-30 01:49:23.000000 enhomie-0.3.0/enhomie/ubiquiti/router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.069260 enhomie-0.3.0/enhomie/ubiquiti/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/ubiquiti/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4146 2024-04-15 08:25:06.000000 enhomie-0.3.0/enhomie/ubiquiti/test/test_client.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3494 2024-04-25 01:47:19.000000 enhomie-0.3.0/enhomie/ubiquiti/test/test_router.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2643 2024-04-08 04:36:08.000000 enhomie-0.3.0/enhomie/ubiquiti/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2148 2024-04-08 04:21:22.000000 enhomie-0.3.0/enhomie/ubiquiti/when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-30 01:49:47.000000 enhomie-0.3.0/enhomie/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-30 01:52:19.070260 enhomie-0.3.0/enhomie.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3454 2024-04-30 01:52:19.000000 enhomie-0.3.0/enhomie.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1568 2024-04-30 01:52:19.000000 enhomie-0.3.0/enhomie.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-30 01:52:19.000000 enhomie-0.3.0/enhomie.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-30 01:52:19.000000 enhomie-0.3.0/enhomie.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        8 2024-04-30 01:52:19.000000 enhomie-0.3.0/enhomie.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      521 2024-04-08 04:22:21.000000 enhomie-0.3.0/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-14 14:15:36.000000 enhomie-0.3.0/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-30 01:52:19.070260 enhomie-0.3.0/setup.cfg
```

### Comparing `enhomie-0.2.2/LICENSE` & `enhomie-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/PKG-INFO` & `enhomie-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhomie
-Version: 0.2.2
+Version: 0.3.0
 Summary: Enasis Network Homie Automate
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `enhomie-0.2.2/README.md` & `enhomie-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/__init__.py` & `enhomie-0.3.0/enhomie/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/builtins/params.py` & `enhomie-0.3.0/enhomie/builtins/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/builtins/test/test_params.py` & `enhomie-0.3.0/enhomie/builtins/test/test_params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/builtins/test/test_when.py` & `enhomie-0.3.0/enhomie/builtins/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/builtins/when.py` & `enhomie-0.3.0/enhomie/builtins/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/config/config.py` & `enhomie-0.3.0/enhomie/config/config.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/config/params.py` & `enhomie-0.3.0/enhomie/config/params.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,27 +42,27 @@
     .. note::
        These parameters are in addition to those found in
        :class:`encommon.config.Params`.
 
     :param groups: Dictionary of parameters for the groups.
     :param scenes: Dictionary of parameters for the scenes.
     :param desires: List of desired states and conditionals.
-    :param cache: Optional cache file but required if using
-        any delay within your desired condition conditonals.
+    :param cache: Optional cache file but required if state
+        between executions is required; when in production.
     :param phue_bridges: Paramters for the product bridges.
     :param phue_devices: Paramters for the product devices.
     :param ubiq_routers: Paramters for the product routers.
     :param ubiq_clients: Paramters for the product clients.
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
     groups: Optional[_GROUPS] = None
     scenes: Optional[_SCENES] = None
     desires: Optional[_DESIRES] = None
 
-    cache: str = 'file::memory:?cache=shared'
+    cache: str = 'sqlite:///:memory:'
 
     phue_bridges: Optional[_PHUE_BRIDGES] = None
     phue_devices: Optional[_PHUE_DEVICES] = None
     ubiq_routers: Optional[_UBIQ_ROUTERS] = None
     ubiq_clients: Optional[_UBIQ_CLIENTS] = None
```

### Comparing `enhomie-0.2.2/enhomie/config/test/test_config.py` & `enhomie-0.3.0/enhomie/config/test/test_config.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/conftest.py` & `enhomie-0.3.0/enhomie/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
     :param tmp_path: pytest object for temporal filesystem.
     :returns: Newly constructed instance of related class.
     """
 
     save_text(
         f'{tmp_path}/config.yml',
         content=(
-            "cache: ':memory:'\n"
             'enconfig:\n'
             '  paths:\n'
             f'    - {tmp_path}\n'
             f'    - {CORE_SAMPLES}\n'
             f'    - {PHUE_SAMPLES}\n'
             f'    - {UBIQ_SAMPLES}\n'
             'enlogger:\n'
```

### Comparing `enhomie-0.2.2/enhomie/homie/__init__.py` & `enhomie-0.3.0/enhomie/homie/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/desire.py` & `enhomie-0.3.0/enhomie/homie/desire.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         """
         Return the boolean indicating whether desire is delayed.
 
         :returns: Boolean indicating whether desire is delayed.
         """
 
         homie = self.homie
-        timers = homie.timers['desire']
+        timers = homie.timers
 
         children = timers.children
 
         unique = self.name
         delay = self.delay
 
         if unique not in children:
@@ -258,15 +258,15 @@
         self,
     ) -> None:
         """
         Update the existing timer from mapping within the cache.
         """
 
         homie = self.homie
-        timers = homie.timers['desire']
+        timers = homie.timers
 
         timers.update(self.name, 'now')
 
 
     @property
     def outcomes(
         self,
```

### Comparing `enhomie-0.2.2/enhomie/homie/group.py` & `enhomie-0.3.0/enhomie/homie/group.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/homie.py` & `enhomie-0.3.0/enhomie/homie/homie.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from typing import Any
-from typing import Literal
 from typing import Optional
 from typing import TYPE_CHECKING
 
 from encommon.times import Timers
 from encommon.types import sort_dict
 
 from .desire import HomieDesire
@@ -25,29 +24,28 @@
 
 if TYPE_CHECKING:
     from ..config import Config
     from ..config import Params
 
 
 
-_TIMERS = Literal['desire']
 _DESCENES = dict[str, list[HomieDesire]]
 _DESIRED = dict[str, HomieDesire]
 
 
 
 class Homie:
     """
     Interact with supported devices to ensure desired state.
 
     :param config: Primary class instance for configuration.
     """
 
     __config: 'Config'
-    __timers: dict[_TIMERS, Timers]
+    __timers: Timers
 
     __phue_bridges: dict[str, PhueBridge]
     __phue_devices: dict[str, PhueDevice]
     __ubiq_routers: dict[str, UbiqRouter]
     __ubiq_clients: dict[str, UbiqClient]
 
     __groups: dict[str, HomieGroup]
@@ -60,15 +58,16 @@
         config: 'Config',
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         self.__config = config
-        self.__timers = {}
+
+        self.__make_timers()
 
         self.__phue_bridges = {}
         self.__phue_devices = {}
         self.__ubiq_routers = {}
         self.__ubiq_clients = {}
 
         self.__groups = {}
@@ -77,16 +76,14 @@
 
         self.log_d(
             base='homie',
             item='Homie',
             status='initial')
 
 
-        self.__make_timers()
-
         self.__make_phue_bridges()
         self.__make_phue_devices()
         self.__make_ubiq_routers()
         self.__make_ubiq_clients()
 
         self.__make_groups()
         self.__make_scenes()
@@ -134,20 +131,17 @@
     ) -> None:
         """
         Construct instances using the configuration parameters.
         """
 
         cache = self.params.cache
 
-        desire = Timers(
-            file=cache,
-            table='timers_desire')
+        timers = Timers(store=cache)
 
-        self.__timers = {
-            'desire': desire}
+        self.__timers = timers
 
 
     def __make_groups(
         self,
     ) -> None:
         """
         Construct instances using the configuration parameters.
@@ -416,22 +410,22 @@
 
         return self.config.params
 
 
     @property
     def timers(
         self,
-    ) -> dict[_TIMERS, Timers]:
+    ) -> Timers:
         """
         Return the timers instances defined within this instance.
 
         :returns: Timers instances defined within this instance.
         """
 
-        return dict(self.__timers)
+        return self.__timers
 
 
     @property
     def groups(
         self,
     ) -> dict[str, HomieGroup]:
         """
```

### Comparing `enhomie-0.2.2/enhomie/homie/params.py` & `enhomie-0.3.0/enhomie/homie/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/scene.py` & `enhomie-0.3.0/enhomie/homie/scene.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/test/test_desire.py` & `enhomie-0.3.0/enhomie/homie/test/test_desire.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/test/test_group.py` & `enhomie-0.3.0/enhomie/homie/test/test_group.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/test/test_homie.py` & `enhomie-0.3.0/enhomie/homie/test/test_homie.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/test/test_scene.py` & `enhomie-0.3.0/enhomie/homie/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/test/test_when.py` & `enhomie-0.3.0/enhomie/homie/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/homie/when.py` & `enhomie-0.3.0/enhomie/homie/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/__init__.py` & `enhomie-0.3.0/enhomie/philipshue/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/bridge.py` & `enhomie-0.3.0/enhomie/philipshue/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,15 @@
         self.__bridge = Bridge(params)
         self.__name = name
         self.__fetched = None
         self.__merged = None
 
 
         self.__timer = Timer(
-            timer=60,
-            start='-60s')
+            60, start='-60s')
 
 
         homie.log_d(
             base='philipshue',
             item='PhueBridge',
             name=name,
             status='created')
```

### Comparing `enhomie-0.2.2/enhomie/philipshue/device.py` & `enhomie-0.3.0/enhomie/philipshue/device.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/params.py` & `enhomie-0.3.0/enhomie/philipshue/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/test/__init__.py` & `enhomie-0.3.0/enhomie/philipshue/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/test/test_bridge.py` & `enhomie-0.3.0/enhomie/philipshue/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/test/test_device.py` & `enhomie-0.3.0/enhomie/philipshue/test/test_device.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/test/test_when.py` & `enhomie-0.3.0/enhomie/philipshue/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/philipshue/when.py` & `enhomie-0.3.0/enhomie/philipshue/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/__init__.py` & `enhomie-0.3.0/enhomie/ubiquiti/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/client.py` & `enhomie-0.3.0/enhomie/ubiquiti/client.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/params.py` & `enhomie-0.3.0/enhomie/ubiquiti/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/router.py` & `enhomie-0.3.0/enhomie/ubiquiti/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
         self.__router = Router(params)
         self.__name = name
         self.__fetched = None
         self.__merged = None
 
 
         self.__timer = Timer(
-            timer=60,
-            start='-60s')
+            60, start='-60s')
 
 
         homie.log_d(
             base='ubiquiti',
             item='UbiqRouter',
             name=name,
             status='created')
```

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/test/test_client.py` & `enhomie-0.3.0/enhomie/ubiquiti/test/test_client.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/test/test_router.py` & `enhomie-0.3.0/enhomie/ubiquiti/test/test_router.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/test/test_when.py` & `enhomie-0.3.0/enhomie/ubiquiti/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie/ubiquiti/when.py` & `enhomie-0.3.0/enhomie/ubiquiti/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/enhomie.egg-info/PKG-INFO` & `enhomie-0.3.0/enhomie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhomie
-Version: 0.2.2
+Version: 0.3.0
 Summary: Enasis Network Homie Automate
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `enhomie-0.2.2/enhomie.egg-info/SOURCES.txt` & `enhomie-0.3.0/enhomie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.2/pyproject.toml` & `enhomie-0.3.0/pyproject.toml`

 * *Files identical despite different names*

