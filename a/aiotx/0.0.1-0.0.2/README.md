# Comparing `tmp/aiotx-0.0.1.tar.gz` & `tmp/aiotx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.0.1.tar", last modified: Tue Apr 30 05:38:45 2024, max compression
+gzip compressed data, was "aiotx-0.0.2.tar", last modified: Tue Apr 30 05:51:29 2024, max compression
```

## Comparing `aiotx-0.0.1.tar` & `aiotx-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:38:45.363676 aiotx-0.0.1/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     3078 2024-04-30 05:29:10.000000 aiotx-0.0.1/.gitignore
--rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)      490 2024-04-30 05:38:45.363676 aiotx-0.0.1/PKG-INFO
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       42 2024-04-30 05:36:02.000000 aiotx-0.0.1/README.md
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:38:45.359676 aiotx-0.0.1/aiotx/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:34:42.000000 aiotx-0.0.1/aiotx/__init__.py
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:38:45.359676 aiotx-0.0.1/aiotx.egg-info/
--rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)      490 2024-04-30 05:38:45.000000 aiotx-0.0.1/aiotx.egg-info/PKG-INFO
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      216 2024-04-30 05:38:45.000000 aiotx-0.0.1/aiotx.egg-info/SOURCES.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        1 2024-04-30 05:38:45.000000 aiotx-0.0.1/aiotx.egg-info/dependency_links.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       93 2024-04-30 05:38:45.000000 aiotx-0.0.1/aiotx.egg-info/requires.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        6 2024-04-30 05:38:45.000000 aiotx-0.0.1/aiotx.egg-info/top_level.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      419 2024-04-30 05:38:25.000000 aiotx-0.0.1/pyproject.toml
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      114 2024-04-30 05:38:45.363676 aiotx-0.0.1/setup.cfg
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      601 2024-04-30 05:38:42.000000 aiotx-0.0.1/setup.py
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:51:29.774702 aiotx-0.0.2/
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     3078 2024-04-30 05:29:10.000000 aiotx-0.0.2/.gitignore
+-rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3070 2024-04-30 05:51:29.774702 aiotx-0.0.2/PKG-INFO
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1636 2024-04-30 05:49:52.000000 aiotx-0.0.2/README.md
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:51:29.774702 aiotx-0.0.2/aiotx/
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:34:42.000000 aiotx-0.0.2/aiotx/__init__.py
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:51:29.774702 aiotx-0.0.2/aiotx.egg-info/
+-rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3070 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/PKG-INFO
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      216 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        1 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       93 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/requires.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        6 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/top_level.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      419 2024-04-30 05:38:25.000000 aiotx-0.0.2/pyproject.toml
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      114 2024-04-30 05:51:29.778702 aiotx-0.0.2/setup.cfg
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1769 2024-04-30 05:51:10.000000 aiotx-0.0.2/setup.py
```

### Comparing `aiotx-0.0.1/.gitignore` & `aiotx-0.0.2/.gitignore`

 * *Files identical despite different names*

