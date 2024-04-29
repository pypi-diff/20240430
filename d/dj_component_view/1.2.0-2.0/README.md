# Comparing `tmp/dj_component_view-1.2.0.tar.gz` & `tmp/dj_component_view-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-1.2.0.tar` & `dj_component_view-2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-1.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-1.2.0/LICENSE
--rw-r--r--   0        0        0      432 2024-04-29 05:31:39.694978 dj_component_view-1.2.0/README.md
--rw-r--r--   0        0        0     1346 2024-04-29 05:42:00.228350 dj_component_view-1.2.0/dj_component_view.py
--rw-r--r--   0        0        0      423 2024-04-29 05:42:10.678561 dj_component_view-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 dj_component_view-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-2.0/LICENSE
+-rw-r--r--   0        0        0     2395 2024-04-29 22:03:34.762510 dj_component_view-2.0/README.md
+-rw-r--r--   0        0        0     1880 2024-04-29 21:53:33.082254 dj_component_view-2.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-04-29 19:36:09.877362 dj_component_view-2.0/pyproject.toml
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 dj_component_view-2.0/PKG-INFO
```

### Comparing `dj_component_view-1.2.0/.gitignore` & `dj_component_view-2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-1.2.0/LICENSE` & `dj_component_view-2.0/LICENSE`

 * *Files identical despite different names*

