# Comparing `tmp/brynq_sdk_functions-1.0.0.tar.gz` & `tmp/brynq_sdk_functions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_functions-1.0.0.tar", last modified: Wed Apr 17 12:36:52 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_functions-1.0.1.tar", last modified: Tue Apr 30 07:52:04 2024, max compression
```

## Comparing `brynq_sdk_functions-1.0.0.tar` & `brynq_sdk_functions-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk/functions/
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-17 12:36:35.000000 brynq_sdk_functions-1.0.0/brynq_sdk/functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36635 2024-04-17 12:36:35.000000 brynq_sdk_functions-1.0.0/brynq_sdk/functions/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/brynq_sdk_functions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 12:36:52.000000 brynq_sdk_functions-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-17 12:36:35.000000 brynq_sdk_functions-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:52:04.000000 brynq_sdk_functions-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-30 07:52:04.000000 brynq_sdk_functions-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:52:04.000000 brynq_sdk_functions-1.0.1/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:52:04.000000 brynq_sdk_functions-1.0.1/brynq_sdk/functions/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-30 07:51:47.000000 brynq_sdk_functions-1.0.1/brynq_sdk/functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36635 2024-04-30 07:51:47.000000 brynq_sdk_functions-1.0.1/brynq_sdk/functions/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:52:04.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-30 07:52:03.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-30 07:52:03.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:52:03.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:52:03.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-30 07:52:03.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 07:52:03.000000 brynq_sdk_functions-1.0.1/brynq_sdk_functions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 07:52:04.000000 brynq_sdk_functions-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-30 07:51:47.000000 brynq_sdk_functions-1.0.1/setup.py
```

### Comparing `brynq_sdk_functions-1.0.0/brynq_sdk/functions/functions.py` & `brynq_sdk_functions-1.0.1/brynq_sdk/functions/functions.py`

 * *Files identical despite different names*

