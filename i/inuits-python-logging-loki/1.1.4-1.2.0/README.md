# Comparing `tmp/inuits_python_logging_loki-1.1.4.tar.gz` & `tmp/inuits_python_logging_loki-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_python_logging_loki-1.1.4.tar", last modified: Mon Apr 15 15:13:14 2024, max compression
+gzip compressed data, was "inuits_python_logging_loki-1.2.0.tar", last modified: Tue Apr 30 14:49:50 2024, max compression
```

## Comparing `inuits_python_logging_loki-1.1.4.tar` & `inuits_python_logging_loki-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/logging_loki/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/tests/test_emitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/logging_loki/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/json_loki_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/log_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/loki_context_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/loki_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/tests/test_emitter_v1.py
```

### Comparing `inuits_python_logging_loki-1.1.4/LICENSE` & `inuits_python_logging_loki-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.1.4/PKG-INFO` & `inuits_python_logging_loki-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits_python_logging_loki-1.1.4/README.md` & `inuits_python_logging_loki-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/PKG-INFO` & `inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits_python_logging_loki-1.1.4/logging_loki/const.py` & `inuits_python_logging_loki-1.2.0/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.1.4/logging_loki/emitter.py` & `inuits_python_logging_loki-1.2.0/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.1.4/logging_loki/handlers.py` & `inuits_python_logging_loki-1.2.0/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.1.4/pyproject.toml` & `inuits_python_logging_loki-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inuits-python-logging-loki"
-version = "1.1.4"
+version = "1.2.0"
 description = "Python logging handler for Grafana Loki."
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }, {name="Andrey Maslov", email="greyzmeem@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `inuits_python_logging_loki-1.1.4/tests/test_emitter_v1.py` & `inuits_python_logging_loki-1.2.0/tests/test_emitter_v1.py`

 * *Files identical despite different names*

