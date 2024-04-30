# Comparing `tmp/assertai_alpha_deployer-0.2.tar.gz` & `tmp/assertai_alpha_deployer-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai_alpha_deployer-0.2.tar", last modified: Tue Apr 30 19:48:59 2024, max compression
+gzip compressed data, was "assertai_alpha_deployer-2.0.tar", last modified: Tue Apr 30 19:59:06 2024, max compression
```

## Comparing `assertai_alpha_deployer-0.2.tar` & `assertai_alpha_deployer-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:48:59.469376 assertai_alpha_deployer-0.2/
--rw-r--r--   0 devl      (1000) devl      (1000)       87 2024-04-30 19:48:59.469376 assertai_alpha_deployer-0.2/PKG-INFO
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:48:59.469376 assertai_alpha_deployer-0.2/assertai_alpha_deployer/
--rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer/__init__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer/__main__.py
--rw-rw-r--   0 devl      (1000) devl      (1000)     6486 2024-04-29 12:53:32.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer/script_manager.py
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:48:59.469376 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/
--rw-r--r--   0 devl      (1000) devl      (1000)       87 2024-04-30 19:48:59.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/PKG-INFO
--rw-rw-r--   0 devl      (1000) devl      (1000)      406 2024-04-30 19:48:59.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/SOURCES.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 19:48:59.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/dependency_links.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 19:48:59.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/entry_points.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 19:48:59.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/requires.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 19:48:59.000000 assertai_alpha_deployer-0.2/assertai_alpha_deployer.egg-info/top_level.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 19:48:59.469376 assertai_alpha_deployer-0.2/setup.cfg
--rw-rw-r--   0 devl      (1000) devl      (1000)      327 2024-04-30 19:47:18.000000 assertai_alpha_deployer-0.2/setup.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/PKG-INFO
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/assertai_alpha_deployer/
+-rw-rw-r--   0 devl      (1000) devl      (1000)        0 2024-04-30 08:56:14.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer/__init__.py
+-rw-rw-r--   0 devl      (1000) devl      (1000)       72 2024-04-30 19:45:43.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer/__main__.py
+-rw-rw-r--   0 devl      (1000) devl      (1000)     6486 2024-04-29 12:53:32.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer/script_manager.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/PKG-INFO
+-rw-rw-r--   0 devl      (1000) devl      (1000)      406 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/SOURCES.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/dependency_links.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/entry_points.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/requires.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 19:59:06.000000 assertai_alpha_deployer-2.0/assertai_alpha_deployer.egg-info/top_level.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 19:59:06.435482 assertai_alpha_deployer-2.0/setup.cfg
+-rw-rw-r--   0 devl      (1000) devl      (1000)     1037 2024-04-30 19:58:40.000000 assertai_alpha_deployer-2.0/setup.py
```

### Comparing `assertai_alpha_deployer-0.2/assertai_alpha_deployer/script_manager.py` & `assertai_alpha_deployer-2.0/assertai_alpha_deployer/script_manager.py`

 * *Files identical despite different names*

